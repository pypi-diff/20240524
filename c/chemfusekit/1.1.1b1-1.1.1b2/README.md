# Comparing `tmp/chemfusekit-1.1.1b1.tar.gz` & `tmp/chemfusekit-1.1.1b2.tar.gz`

## Comparing `chemfusekit-1.1.1b1.tar` & `chemfusekit-1.1.1b2.tar`

### file list

```diff
@@ -1,133 +1,144 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.python-version
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.releaserc.yml
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/CHANGELOG.md
--rw-r--r--   0        0        0     5231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/cda_example_notebook.ipynb
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/requirements-dev.lock
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/requirements.lock
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/gh_pages.yml
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/thesis.yml
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/__init__.py
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/__utils.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/knn.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lda.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lldf.py
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/lr.py
--rw-r--r--   0        0        0     8825 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/pca.py
--rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/plsda.py
--rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/chemfusekit/svm.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/README.md
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/babel.config.js
--rw-r--r--   0        0        0     4025 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docusaurus.config.js
--rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/package-lock.json
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/package.json
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/sidebars.js
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/complete-workflow.md
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/tutorial.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/_category_.json
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/knn.md
--rw-r--r--   0        0        0     2311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/knn/knnsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/_category_.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/lda.md
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lda/ldasettings.md
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/_category_.json
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldf.md
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldfmodel.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lldf/lldfsettings.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/_category_.json
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/lr.md
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/lr/lrsettings.md
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/_category_.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/pca.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/pca/pcasettings.md
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/_category_.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/plsda.md
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/plsda/plsdasettings.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/_category_.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/svm.md
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/docs/svm/svmsettings.md
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/index.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/styles.module.css
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/css/custom.css
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/index.js
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/index.module.css
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project.md
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/continuous-integration.md
--rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/process-model.md
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/project-philosophy.md
--rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/project-plan.md
--rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/requirements-specification.md
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/src/pages/project/use-cases.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/.nojekyll
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/colab-logo.svg
--rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/docusaurus-social-card.jpg
--rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/docusaurus.png
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/favicon.ico
--rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/happy-woman.svg
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/logo.svg
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/docs/static/img/magnifying-glass.svg
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Beartype.md
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Constructors.md
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Conventional Commits.md
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Kanban.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Logistic Regression.md
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PCA-LR.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PCA.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/PEP coding standards.md
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/SVM.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/To do.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Use Case Diagram.md
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/kNN.md
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/app.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/appearance.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/community-plugins.json
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/core-plugins-migration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/core-plugins.json
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/daily-notes.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/templates.json
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/workspace.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/data.json
--rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/main.js
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/manifest.json
--rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/main.js
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/manifest.json
--rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/styles.css
--rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/main.js
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-19.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-20.md
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-22.md
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-04-23.md
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-06.md
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-07.md
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-08.md
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-09.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-17.md
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Devlog/2024-05-18.md
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/Templates/Daily devlog.md
--rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Components.md
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Process state machine.md
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Sequence.md
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/notes/UML/Use cases.md
--rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/qepas.xlsx
--rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/rt.xlsx
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_knn.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lda.py
--rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lldf.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_lr.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_pca.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_plsda.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/tests/test_svm.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/0-header.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/1-abstract.md
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/2-index.md.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/3-intro.md
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/999-ringraziamenti.md
--rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/thesis/logo-unibg.png
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/.gitignore
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/pyproject.toml
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/readme.md
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.python-version
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.releaserc.yml
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/CHANGELOG.md
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/requirements-dev.lock
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/requirements.lock
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/gh_pages.yml
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/thesis.yml
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/__init__.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/__utils.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/knn.py
+-rw-r--r--   0        0        0     4418 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lda.py
+-rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lldf.py
+-rw-r--r--   0        0        0     4685 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/lr.py
+-rw-r--r--   0        0        0     9783 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/pca.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/plsda.py
+-rw-r--r--   0        0        0     2815 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/chemfusekit/svm.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/README.md
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/babel.config.js
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docusaurus.config.js
+-rw-r--r--   0        0        0  1020872 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/package-lock.json
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/package.json
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/sidebars.js
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/complete-workflow.md
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/tutorial.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/_category_.json
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/knn.md
+-rw-r--r--   0        0        0     2376 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/knn/knnsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/_category_.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/lda.md
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lda/ldasettings.md
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/_category_.json
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldf.md
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldfmodel.md
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lldf/lldfsettings.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/_category_.json
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/lr.md
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/lr/lrsettings.md
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/_category_.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/pca.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/pca/pcasettings.md
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/_category_.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/plsda.md
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/plsda/plsdasettings.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/_category_.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/svm.md
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/svm/svmsettings.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/_category_.json
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/graphmode.md
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/graphoutput.md
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/printconfusionmatrix.md
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/printtable.md
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/docs/utils/runsplittests.md
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/index.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/styles.module.css
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/css/custom.css
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/index.js
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/index.module.css
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/_category_.json
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/continuous-integration.md
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/index.md
+-rw-r--r--   0        0        0     2595 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/process-model.md
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/project-philosophy.md
+-rw-r--r--   0        0        0    10945 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/project-plan.md
+-rw-r--r--   0        0        0     4767 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/requirements-specification.md
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/src/pages/project/use-cases.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/.nojekyll
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/colab-logo.svg
+-rw-r--r--   0        0        0    55746 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/docusaurus-social-card.jpg
+-rw-r--r--   0        0        0    10723 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/docusaurus.png
+-rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/favicon.ico
+-rw-r--r--   0        0        0    23978 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/happy-woman.svg
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/logo.svg
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/docs/static/img/magnifying-glass.svg
+-rw-r--r--   0        0        0   241829 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/knn_notebook.ipynb
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/pca_lda_notebook.ipynb
+-rw-r--r--   0        0        0  1664059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/pca_lr_notebook.ipynb
+-rw-r--r--   0        0        0   533536 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/plsda_notebook.ipynb
+-rw-r--r--   0        0        0   176230 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/examples/svm_notebook.ipynb
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Beartype.md
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Constructors.md
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Conventional Commits.md
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Kanban.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Logistic Regression.md
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PCA-LR.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PCA.md
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/PEP coding standards.md
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/SVM.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/To do.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Use Case Diagram.md
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/kNN.md
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/app.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/appearance.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/community-plugins.json
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/core-plugins-migration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/core-plugins.json
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/daily-notes.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/templates.json
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/workspace.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/data.json
+-rw-r--r--   0        0        0   141498 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/main.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/manifest.json
+-rw-r--r--   0        0        0   723669 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/main.js
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/manifest.json
+-rw-r--r--   0        0        0    53515 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/styles.css
+-rw-r--r--   0        0        0   294758 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/main.js
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/manifest.json
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-19.md
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-20.md
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-22.md
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-04-23.md
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-06.md
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-07.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-08.md
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-09.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-17.md
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Devlog/2024-05-18.md
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/Templates/Daily devlog.md
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Components.md
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Process state machine.md
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Sequence.md
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/notes/UML/Use cases.md
+-rw-r--r--   0        0        0   590311 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/qepas.xlsx
+-rw-r--r--   0        0        0    18770 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/rt.xlsx
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_knn.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lda.py
+-rw-r--r--   0        0        0     2631 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lldf.py
+-rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_lr.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_pca.py
+-rw-r--r--   0        0        0     4673 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_plsda.py
+-rw-r--r--   0        0        0     4294 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/tests/test_svm.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/0-header.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/1-abstract.md
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/2-index.md.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/3-intro.md
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/999-ringraziamenti.md
+-rw-r--r--   0        0        0    21285 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/thesis/logo-unibg.png
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/.gitignore
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/pyproject.toml
+-rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/readme.md
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 chemfusekit-1.1.1b2/PKG-INFO
```

### Comparing `chemfusekit-1.1.1b1/.releaserc.yml` & `chemfusekit-1.1.1b2/.releaserc.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/CHANGELOG.md` & `chemfusekit-1.1.1b2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## [1.1.1-beta.2](https://github.com/f-aguzzi/tesi/compare/v1.1.1-beta.1...v1.1.1-beta.2) (2024-05-24)
+
+
+### Bug Fixes
+
+* wrong training procedure in SVM ([#25](https://github.com/f-aguzzi/tesi/issues/25)) ([7f25487](https://github.com/f-aguzzi/tesi/commit/7f254876fcdbd2ba5c46278d31eb851a50659e8f))
+
 ## [1.1.1-beta.1](https://github.com/f-aguzzi/tesi/compare/v1.1.0...v1.1.1-beta.1) (2024-05-23)
 
 
 ### Bug Fixes
 
 * wrong training procedure in SVM ([74d1741](https://github.com/f-aguzzi/tesi/commit/74d1741743f53eea6cc2d9002005c6426bf4f0d0))
```

### Comparing `chemfusekit-1.1.1b1/cda_example_notebook.ipynb` & `chemfusekit-1.1.1b2/examples/pca_lda_notebook.ipynb`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9812478378103378%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(4, '!wget "*

 * *            "https://github.com/f-aguzzi/tesi/raw/main/tests/rt.xlsx\\n'), (5, '\\n'), (6, '# "*

 * *            "Automatically inline the graphs\\n'), (7, '%matplotlib inline')], delete: [4]}}, 3: "*

 * *            '{\'source\': {insert: [(0, \'%matplotlib inline \\n\'), (1, \'\\n\'), (6, "    '*

 * *            'qepas_path=\'tests/qepas.xlsx\',    # (or put the name of your files)\\n"), (8, "    '*

 * *            'rt_path=\'tests/rt.xlsx\',\\n")], delete: [6, 4]}}, 6: {\'s […]*

```diff
@@ -18,15 +18,18 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "%pip install chemfusekit\n",
                 "\n",
                 "# Optional: download the example data from the repository (you could upload your own files)\n",
                 "!wget https://github.com/f-aguzzi/tesi/raw/main/tests/qepas.xlsx\n",
-                "!wget https://github.com/f-aguzzi/tesi/raw/main/tests/rt.xlsx"
+                "!wget https://github.com/f-aguzzi/tesi/raw/main/tests/rt.xlsx\n",
+                "\n",
+                "# Automatically inline the graphs\n",
+                "%matplotlib inline"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## First step: Low-Level Data Fusion\n",
@@ -37,21 +40,23 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
+                "%matplotlib inline \n",
+                "\n",
                 "from chemfusekit.lldf import LLDFSettings, LLDF\n",
                 "\n",
                 "# Initialize the settings for low-level data fusion\n",
                 "lldf_settings = LLDFSettings(\n",
-                "    qepas_path='qepas.xlsx',    # (or put the name of your files)\n",
+                "    qepas_path='tests/qepas.xlsx',    # (or put the name of your files)\n",
                 "    qepas_sheet='Sheet1',\n",
-                "    rt_path='rt.xlsx',\n",
+                "    rt_path='tests/rt.xlsx',\n",
                 "    rt_sheet='Sheet1',\n",
                 "    preprocessing='snv'  # normalization preprocessing; other options: savgol or both\n",
                 ")\n",
                 "\n",
                 "# Initialize and run low-level data fusion\n",
                 "lldf = LLDF(lldf_settings)\n",
                 "lldf.lldf()"
@@ -82,30 +87,30 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from chemfusekit.pca import PCASettings, PCA\n",
+                "from chemfusekit.pca import PCASettings, PCA, GraphMode\n",
                 "\n",
                 "# Initialize the settings for Principal Component Analysis\n",
                 "pca_settings = PCASettings(\n",
                 "    target_variance=0.99,\n",
                 "    confidence_level=0.05,\n",
                 "    initial_components=10,\n",
-                "    output=True # graphs will be printed\n",
+                "    output=GraphMode.GRAPHIC # graphs will be printed as pictures\n",
                 ")\n",
                 "\n",
                 "# Initialize and run the PCA class\n",
                 "pca = PCA(lldf.fused_data, pca_settings)\n",
                 "pca.pca()\n",
                 "\n",
                 "# Print the number of components and the statistics\n",
-                "print(pca.components)\n",
+                "print(f\"\\nNumber of components: {pca.components}\\n\")\n",
                 "pca.pca_stats()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
@@ -117,19 +122,20 @@
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
-                "from chemfusekit.lda import LDASettings, LDA\n",
+                "from chemfusekit.lda import LDASettings, LDA, GraphMode\n",
                 "\n",
                 "settings = LDASettings(\n",
                 "    components=(pca.components - 1),    # one less component than the number determined by PCA\n",
-                "    output=True # graphs will be printed\n",
+                "    output=GraphMode.GRAPHIC,   # graphs will be printed as pictures\n",
+                "    test_split=True # Run split test\n",
                 ")\n",
                 "\n",
                 "# Initialize and run the LDA class\n",
                 "lda = LDA(lldf.fused_data, settings)\n",
                 "lda.lda()"
             ]
         },
@@ -150,21 +156,14 @@
                 "x_data_sample = lldf.fused_data.x_train.iloc[119] # should be DMMP\n",
                 "x_data_sample = x_data_sample.iloc[1:].to_frame().transpose()\n",
                 "\n",
                 "# Let's run the prediction:\n",
                 "predictions = lda.predict(x_data_sample)\n",
                 "print(predictions)"
             ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3 (ipykernel)",
             "language": "python",
             "name": "python3"
@@ -175,18 +174,18 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.5"
+            "version": "3.12.3"
         },
         "vscode": {
             "interpreter": {
-                "hash": "aee8b7b246df8f9039afb4144a1f6fd8d2ca17a180786b69acc140d282b71a49"
+                "hash": "0adf20f4cd3c09df9458869b76345de81eb21527fdd82bbecfd21ff585123f63"
             }
         }
     },
     "nbformat": 4,
     "nbformat_minor": 4
 }
```

### Comparing `chemfusekit-1.1.1b1/requirements-dev.lock` & `chemfusekit-1.1.1b2/requirements.lock`

 * *Files 11% similar despite different names*

```diff
@@ -4,39 +4,44 @@
 # last locked with the following flags:
 #   pre: false
 #   features: []
 #   all-features: false
 #   with-sources: false
 
 -e file:.
-astroid==3.1.0
-    # via pylint
+attrs==23.2.0
+    # via jsonschema
+    # via referencing
 beartype==0.18.5
     # via chemfusekit
 contourpy==1.2.1
     # via matplotlib
 cycler==0.12.1
     # via matplotlib
-dill==0.3.8
-    # via pylint
 et-xmlfile==1.1.0
     # via openpyxl
+fastjsonschema==2.19.1
+    # via nbformat
 fonttools==4.51.0
     # via matplotlib
-isort==5.13.2
-    # via pylint
 joblib==1.4.2
     # via scikit-learn
+jsonschema==4.22.0
+    # via nbformat
+jsonschema-specifications==2023.12.1
+    # via jsonschema
+jupyter-core==5.7.2
+    # via nbformat
 kiwisolver==1.4.5
     # via matplotlib
 matplotlib==3.8.4
     # via chemfusekit
     # via seaborn
-mccabe==0.7.0
-    # via pylint
+nbformat==5.10.4
+    # via chemfusekit
 numpy==1.26.4
     # via chemfusekit
     # via contourpy
     # via matplotlib
     # via pandas
     # via scikit-learn
     # via scipy
@@ -47,36 +52,44 @@
     # via matplotlib
     # via plotly
 pandas==2.2.2
     # via chemfusekit
     # via seaborn
 pillow==10.3.0
     # via matplotlib
-platformdirs==4.2.1
-    # via pylint
+platformdirs==4.2.2
+    # via jupyter-core
 plotly==5.22.0
     # via chemfusekit
-pylint==3.1.1
 pyparsing==3.1.2
     # via matplotlib
 python-dateutil==2.9.0.post0
     # via matplotlib
     # via pandas
 pytz==2024.1
     # via pandas
+referencing==0.35.1
+    # via jsonschema
+    # via jsonschema-specifications
+rpds-py==0.18.1
+    # via jsonschema
+    # via referencing
 scikit-learn==1.4.2
     # via chemfusekit
 scipy==1.13.0
     # via chemfusekit
     # via scikit-learn
 seaborn==0.13.2
     # via chemfusekit
 six==1.16.0
     # via python-dateutil
+tabulate==0.9.0
+    # via chemfusekit
 tenacity==8.3.0
     # via plotly
 threadpoolctl==3.5.0
     # via scikit-learn
-tomlkit==0.12.5
-    # via pylint
+traitlets==5.14.3
+    # via jupyter-core
+    # via nbformat
 tzdata==2024.1
     # via pandas
```

### Comparing `chemfusekit-1.1.1b1/.github/workflows/gh_pages.yml` & `chemfusekit-1.1.1b2/.github/workflows/gh_pages.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/.github/workflows/pylint.yml` & `chemfusekit-1.1.1b2/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/.github/workflows/release.yml` & `chemfusekit-1.1.1b2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/.github/workflows/thesis.yml` & `chemfusekit-1.1.1b2/.github/workflows/thesis.yml`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/.github/workflows/unittest.yml` & `chemfusekit-1.1.1b2/.github/workflows/unittest.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,19 +9,15 @@
 jobs:
   build:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v3 
       - name: Install the latest version of rye
-        uses: phi-friday/install-rye@v1.4
-        with:
-          rye_version: "latest"
-          python_version: 3.12
-          use_uv: true
+        uses: eifinger/setup-rye@v3
       - name: Install dependencies
         run: rye sync --no-lock
       - name: Run unit tests on the code
         run: rye run test
       - name: Check test results
         run: |
           test_result=$(rye run test |& grep "FAILED" | wc -w)
```

### Comparing `chemfusekit-1.1.1b1/chemfusekit/knn.py` & `chemfusekit-1.1.1b2/chemfusekit/knn.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,40 @@
 from beartype.typing import Callable
 
 from sklearn.neighbors import KNeighborsClassifier
 
 import pandas as pd
 
 from chemfusekit.lldf import LLDFModel
-from chemfusekit.__utils import run_split_test, print_confusion_matrix
+from chemfusekit.__utils import run_split_test, print_confusion_matrix, print_table, GraphMode
 
 class KNNSettings:
     '''Holds the settings for the kNN object.'''
     def __init__(
             self,
             n_neighbors: int = 15,
             metric: str | Callable = 'euclidean',
             weights: str | Callable = 'uniform',
             algorithm: str = 'auto',
-            output: bool = False,
+            output: GraphMode = GraphMode.NONE,
             test_split: bool = False
         ):
         if n_neighbors < 1:
             raise ValueError("Invalid n_neighbors number: should be a positive integer.")
         if metric not in ['minkwoski', 'precomputed', 'euclidean'] and not callable(metric):
             raise ValueError(
                 "Invalid metric: should be 'minkwoski', 'precomputed', 'euclidean' or a callable."
             )
         if weights not in ['uniform', 'distance'] and not callable(weights):
             raise ValueError("Invalid weight: should be 'uniform', 'distance' or a callable")
         if algorithm not in ['auto', 'ball_tree', 'kd_tree', 'brute']:
             raise  ValueError(
                 "Invalid algorithm: should be 'auto', 'ball_tree', 'kd_tree' or 'brute'."
             )
-        if test_split is True and output is False:
+        if test_split is True and output is GraphMode.NONE:
             raise Warning(
                 "You selected test_split but it won't run because you disabled the output."
             )
         self.n_neighbors = n_neighbors
         self.metric = metric
         self.weights = weights
         self.algorithm = algorithm
@@ -60,24 +60,29 @@
             algorithm=self.settings.algorithm
         )
         knn.fit(self.fused_data.x_data, self.fused_data.y)
 
         # Save the trained model
         self.model = knn
 
-        if self.settings.output:
-            # View the prediction on the test data
-            y_pred = knn.predict(self.fused_data.x_data)
-            print(y_pred)
-
-            print_confusion_matrix(
-                self.fused_data.y,
-                y_pred,
-                "Confusion Matrix based on the whole data set"
-            )
+        # View the prediction on the test data
+        y_pred = knn.predict(self.fused_data.x_data)
+        print_table(
+            ["Predictions"],
+            y_pred.reshape(1,len(y_pred)),
+            "Data and predictions",
+            self.settings.output
+        )
+
+        print_confusion_matrix(
+            self.fused_data.y,
+            y_pred,
+            "Confusion Matrix based on the whole data set",
+            self.settings.output
+        )
 
         if self.settings.test_split and self.settings.output:
             knn_split = KNeighborsClassifier(
                 n_neighbors=self.settings.n_neighbors,
                 metric=self.settings.metric,
                 weights=self.settings.weights,
                 algorithm=self.settings.algorithm
```

### Comparing `chemfusekit-1.1.1b1/chemfusekit/lda.py` & `chemfusekit-1.1.1b2/chemfusekit/svm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,83 +1,81 @@
-'''Linear Discriminant Analysis module'''
+'''Support Vector Machine module.'''
 from typing import Optional
 
-import numpy as np
 import pandas as pd
 
-from sklearn.discriminant_analysis import LinearDiscriminantAnalysis as LD
-from sklearn.model_selection import train_test_split
-from sklearn.metrics import confusion_matrix, classification_report
+from sklearn.svm import SVC
 
 from chemfusekit.lldf import LLDFModel
-from chemfusekit.__utils import graph_output, run_split_test
+from chemfusekit.__utils import GraphMode, run_split_test, print_confusion_matrix
 
-class LDASettings:
-    '''Holds the settings for the LDA object.'''
-    def __init__(self, components: int = 3, output: bool = False, test_split: bool = False):
-        if components <= 2:
-            raise ValueError("Invalid component number: must be a > 1 integer.")
-        if test_split is True and output is False:
+
+
+class SVMSettings:
+    '''Holds the settings for the SVM object.'''
+    def __init__(self, kernel: str = 'linear', output: GraphMode = GraphMode.NONE,
+                 test_split: bool = False):
+        if kernel not in ['linear', 'poly', 'gaussian', 'sigmoid']:
+            raise ValueError("Invalid type: must be linear, poly, gaussian or sigmoid")
+        if test_split is True and output is GraphMode.NONE:
             raise Warning(
                 "You selected test_split but it won't run because you disabled the output."
             )
-        self.components = components
+        self.kernel = kernel
         self.output = output
         self.test_split = test_split
 
-class LDA:
-    '''Class to store the data, methods and artifacts for Linear Discriminant Analysis'''
-    def __init__(self, lldf_model: LLDFModel, settings: LDASettings):
+
+class SVM:
+    '''Class for Support Vector Machine analysis of the data'''
+    def __init__(self, fused_data: LLDFModel, settings: SVMSettings):
+        self.fused_data = fused_data
         self.settings = settings
-        self.x_data = lldf_model.x_data
-        self.x_train = lldf_model.x_train
-        self.y = lldf_model.y
-        self.model: Optional[LD] = None
-
-    def lda(self):
-        '''Performs Linear Discriminant Analysis'''
-
-        lda = LD(n_components=self.settings.components) # N-1 where N are the classes
-        scores_lda = lda.fit(self.x_data, self.y).transform(self.x_data)
-
-        if self.settings.output:
-            print(f"LDA scores:\n{scores_lda}")
-            print(lda.priors_)
-            print(lda.means_)
-            print(lda.coef_[0:self.settings.components,:])
-            pred=lda.predict(self.x_data)
-            print(np.unique(pred, return_counts=True))
-
-            print(confusion_matrix(pred, self.y))
-            print(classification_report(self.y, pred, digits=2))
-
-        lv_cols = [f'LV{i+1}' for i in range(self.settings.components)]
-        scores = pd.DataFrame(data = scores_lda, columns = lv_cols) # latent variables
-        scores.index = self.x_data.index
-        y_dataframe = pd.DataFrame(self.y, columns=['Substance'])
-
-        scores = pd.concat([scores, y_dataframe], axis = 1)
-
-        # Store the traiend model
-        self.model = lda
-
-        # Show graphs if required by the user
-        if self.settings.output:
-            graph_output(scores, self.model, "Linear Discriminant Analysis")
-
-            # Run split tests if required by the user
-            if self.settings.test_split:
-                run_split_test(
-                    (scores.drop('Substance', axis=1).values),
-                    self.y,
-                    LD(n_components=self.settings.components)
-                )
+        self.model: Optional[SVC] = None
+
+
+    def svm(self):
+        '''Performs Support Vector Machine analysis'''
+
+        # Linear kernel
+        if self.settings.kernel == 'linear':
+            svm_model = SVC(kernel='linear', probability=True)
+        # Polynomial kernel
+        elif self.settings.kernel == 'poly':
+            svm_model = SVC(kernel='poly', degree=8)
+        # Gaussian kernel - radial basis function
+        elif self.settings.kernel == 'gaussian':
+            svm_model = SVC(kernel='rbf')
+        # Sigmoid classifier
+        elif self.settings.kernel == 'sigmoid':
+            svm_model = SVC(kernel='sigmoid')
+        else:
+            raise ValueError(f"SVM: this type of kernel does not exist ({self.settings.kernel=})")
+
+        svm_model.fit(self.fused_data.x_data, self.fused_data.y)
+        self.model = svm_model
+
+        predictions = svm_model.predict(self.fused_data.x_data)
+        print_confusion_matrix(
+            self.fused_data.y,
+            predictions,
+            "Confusion matrix based on the whole data set",
+            mode=self.settings.output
+        )
+
+        if self.settings.test_split:
+            run_split_test(
+                x=self.fused_data.x_data,
+                y=self.fused_data.y,
+                model=SVC(kernel=self.settings.kernel),
+                mode=self.settings.output
+            )
+
 
     def predict(self, x_data: pd.DataFrame):
-        '''Performs LDA prediction once the model is trained.'''
-        if x_data is None:
-            raise TypeError("X data for LDA prediction must be non-empty.")
+        '''Performs SVM prediction once the model is trained'''
         if self.model is None:
-            raise RuntimeError("The LDA model is not trained yet!")
+            raise RuntimeError("The model hasn't been trained yet!")
+        if x_data is None:
+            raise TypeError("X data for prediction cannot be empty.")
 
-        y_pred = self.model.predict(x_data)
-        return y_pred
+        return self.model.predict(x_data)
```

### Comparing `chemfusekit-1.1.1b1/chemfusekit/lldf.py` & `chemfusekit-1.1.1b2/chemfusekit/lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/chemfusekit/lr.py` & `chemfusekit-1.1.1b2/chemfusekit/lr.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,37 +2,38 @@
 from typing import Optional
 
 import numpy as np
 import pandas as pd
 
 from sklearn.linear_model import LogisticRegression
 
-from chemfusekit.__utils import run_split_test, print_confusion_matrix
+from chemfusekit.__utils import run_split_test, print_confusion_matrix, print_table, GraphMode
 
 class LRSettings:
     '''Holds the settings for the LR object.'''
-    def __init__(self, algorithm: str = 'liblinear', output: bool = False,
+    def __init__(self, algorithm: str = 'liblinear', output: GraphMode = GraphMode.NONE,
                  test_split: bool = False):
         if algorithm not in [
             'lbfgs',
             'liblinear',
             'newton-cg',
             'newton-cholesky',
             'sag',
             'saga'
         ]:
             raise ValueError(f"{algorithm}: this algorithm does not exist.")
-        if test_split is True and output is False:
+        if test_split is True and output is GraphMode.NONE:
             raise Warning(
                 "You selected test_split but it won't run because you disabled the output."
             )
         self.algorithm = algorithm
         self.output = output
         self.test_split = test_split
 
+
 class LR:
     '''Class to store the data, methods and artifacts for Logistic Regression'''
     def __init__(self, settings: LRSettings, array_scores: np.ndarray, y: np.ndarray):
         self.settings = settings
         self.array_scores = array_scores
         self.y = y
         self.model: Optional[LogisticRegression] = None
@@ -44,22 +45,25 @@
         model = LogisticRegression(
             solver=self.settings.algorithm,
             random_state=0,
             class_weight='balanced',
             max_iter=10000
         ).fit(self.array_scores, self.y)
 
-        if self.settings.output:
-            #we can see the classes the model used
-            print(model.classes_)
-            # See the intercept of the model
-            print(model.intercept_)
-            # See the coefficients of the model - that can be easily interpreted
-            # (correlating or not with y)
-            print(model.coef_)
+        # See the classes the model used
+        classes = np.unique(self.y)
+        classes = classes.reshape((1, len(classes)))
+        coefficients = model.coef_.transpose()
+        intercepts = model.intercept_.reshape((1, len(model.intercept_)))
+        print_table(
+            ["Class"] + [f"Coefficient {i+1}" for i in range(model.coef_.shape[1])] + ["Intercept (bias)"],
+            np.concatenate((classes, coefficients, intercepts)),
+            "LR Coefficients",
+            self.settings.output
+        )
 
         '''
         Evaluate the model: each sample has a probability of belonging to Positive
         or Negative outcome. Class 0 is Negative, class 1 is Positive.  If the value
         of the first column (probability of being Negative) is higher than 0.5, we
         have a Negative sample. Otherwise, it will be Positive
         '''
@@ -69,41 +73,63 @@
 
         # This tells us the accuracy of our model in calibration
         scores = model.score(self.array_scores, self.y)
 
         # Save the trained model
         self.model = model
 
-        if self.settings.output:
-            print(probabilities)
-            print(predictions)
-            print(scores)
-
-            print_confusion_matrix(
-                self.y,
-                predictions,
-                "Confusion Matrix based on whole data set",
-            )
+        sample_column = self.y.reshape((1, self.y.shape[0]))
+        pred_column = predictions.reshape((1, predictions.shape[0]))
+        prob_column = probabilities.transpose()
+
+        print_table(
+            np.concatenate((np.asarray(["Real sample", "Prediction"]), classes.reshape(17, ))),
+            np.concatenate((
+                sample_column,
+                pred_column,
+                prob_column
+            )),
+            f"LR Predictions with class probabilities (overall score: {scores}",
+            self.settings.output
+        )
+
+        print_confusion_matrix(
+            self.y,
+            predictions,
+            "Confusion Matrix based on whole data set",
+            self.settings.output
+        )
 
-        if self.settings.test_split and self.settings.output:
+        if self.settings.test_split:
             split_model = LogisticRegression(
-                solver='lbfgs',
+                solver=self.settings.algorithm,
                 random_state=0,
                 class_weight='balanced',
                 max_iter=10000
             )
 
-            run_split_test(self.array_scores, self.y, split_model, extended=True)
+            run_split_test(
+                self.array_scores,
+                self.y,
+                split_model,
+                extended=True,
+                mode=self.settings.output
+            )
 
     def predict(self, x_sample: pd.DataFrame):
         '''Performs LR prediction once the model is trained.'''
         if self.model is None:
             raise RuntimeError("The LR model is not trained yet!")
 
         prediction = self.model.predict(x_sample)
         probabilities = self.model.predict_proba(x_sample)
 
-        if self.settings.output:
-            print(prediction)
-            print(probabilities)
+        classes = self.model.classes_.reshape((self.model.classes_.shape[0], ))
+        probabilities = probabilities.reshape((self.model.classes_.shape[0], ))
+        print_table(
+            classes,
+            probabilities,
+            f"Predicted class: {prediction}. Scores:",
+            mode=self.settings.output
+        )
 
         return prediction
```

### Comparing `chemfusekit-1.1.1b1/chemfusekit/pca.py` & `chemfusekit-1.1.1b2/chemfusekit/pca.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,21 @@
 import matplotlib.pyplot as plt
 
 from sklearn.decomposition import PCA as PC
 
 import scipy.stats
 
 from chemfusekit.lldf import LLDFModel
+from chemfusekit.__utils import print_table, GraphMode
 
 class PCASettings:
     '''Holds the settings for the PCA object.'''
     def __init__(self, target_variance: float = 0.95,
                  confidence_level: float = 0.05,
-                 initial_components: int = 10, output: bool = False):
+                 initial_components: int = 10, output: GraphMode = GraphMode.NONE):
         if target_variance < 0:
             raise ValueError("Target variance should be positive or null.")
         if confidence_level < 0 or confidence_level > 1:
             raise ValueError("Confidence level should be between 0 and 1.")
         if initial_components < 3:
             raise ValueError("Initial components should be at least 3.")
         self.target_variance = target_variance
@@ -48,41 +49,54 @@
         pca.fit_transform(x_data)
 
         # Define the class vector (discrete/categorical variable)
         # y_dataframe = pd.DataFrame(self.fused_data.y, columns=['Substance'])
         # classes = y_dataframe.astype('category') (a cosa serve?)
         out_sum = np.cumsum(pca.explained_variance_ratio_)
 
-        if self.settings.output:
-            print("Proportion of Variance Explained : ", pca.explained_variance_ratio_)
-            print("Cumulative Prop. Variance Explained: ", out_sum)
-
         # Autoselect the number of components
         for i,x in enumerate(out_sum):
             if x >= self.settings.target_variance:
                 self.components = i
                 break
         self.components = max(self.components, 3)
 
-        if self.settings.output:
-            print(f"Running PCA with {self.components} components")
+        compsexpv = [[(i+1), pca.explained_variance_ratio_[i]] for i in np.arange(pca.n_components_)]
+        comps, expv = zip(*compsexpv)
+        print_table(
+            ["Components", "Explained Variance"],
+            [comps, expv],
+            "Proportion of Variance Explained",
+            mode=self.settings.output
+        )
 
+        if self.settings.output is GraphMode.GRAPHIC:
             # PCA scree plot
             pc_values = np.arange(pca.n_components_) + 1
             plt.plot(pc_values, pca.explained_variance_ratio_, 'ro-', linewidth=2)
             plt.title('Scree Plot')
             plt.xlabel('Principal Component')
             plt.ylabel('Proportion of Variance Explained')
             plt.show()
 
+        compsexpv = [[(i+1), out_sum[i]] for i in np.arange(pca.n_components_)]
+        comps, expv = zip(*compsexpv)
+        print_table(
+            ["Components", "Cumulative Explained Variance"],
+            [comps, expv],
+            "Cumulative Proportion of Variance Explained",
+            mode=self.settings.output
+        )
+
+        if self.settings.output is GraphMode.GRAPHIC:
             # Cumulative explained variance ratio
             plt.plot(pc_values, out_sum, 'ro-', linewidth=2)
-            plt.title('Scree Plot')
+            plt.title('Scree Plot (cumulative)')
             plt.xlabel('Principal Component')
-            plt.ylabel('Cumulative Prop. Variance Explained')
+            plt.ylabel('Cumulative Proportional Variance Explained')
             plt.show()
 
         # Run PCA producing the pca_model with a proper number of components
         pca = PC(n_components=self.components)
         self.pca_model = pca
         self.pca_model.fit_transform(x_data)
 
@@ -93,43 +107,53 @@
         x_train = self.fused_data.x_train
 
         # Prepare the Scores dataframe (and concatenate the original 'Region' variable)
         pc_cols = [f"PC{i+1}" for i in range(self.components)]
         scores = pd.DataFrame(data=self.pca_model.fit_transform(x_data), columns=pc_cols)
         scores.index = x_data.index
         scores = pd.concat([scores, x_train.Substance], axis = 1)
-        if self.settings.output:
-            print(f"Scores:\n{scores}")
+        
+        print_table(
+            pc_cols + ['Substance'],
+            [scores.iloc[:,i] for i in range(scores.shape[1])],
+            "PCA scores for each component",
+            self.settings.output
+        )
 
         # Prepare the loadings dataframe
         loadings = pd.DataFrame(
             self.pca_model.components_.T,
             columns=pc_cols,
             index=x_data.columns
         )
         loadings["Attributes"] = loadings.index
-        if self.settings.output:
-            print(f"Loadings:\n{loadings}")
+    
+        print_table(
+            pc_cols + ['Retention Time'],
+            [loadings.iloc[:,i] for i in range(loadings.shape[1])],
+            "PCA Loadings",
+            self.settings.output
+        )
 
-        if self.settings.output:
+        if self.settings.output is GraphMode.GRAPHIC:
             # View the scores plot using plotly library
             fig = px.scatter(
                 scores,
                 x="PC1",
                 y="PC2",
                 color="Substance",
                 hover_data=['Substance'],
                 hover_name=x_data.index
             )
             fig.update_xaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_yaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_layout(
                 height=600,
                 width=800,
-                title_text='Scores Plot colored by Substance')
+                title_text='PCA Scores Plot colored by Substance')
             fig.show()
 
             # Plot 3D scores
             fig = px.scatter_3d(
                 scores,
                 x='PC1',
                 y='PC2',
@@ -169,15 +193,15 @@
 
         # Create a dataframe using only T2 and Q-residuals
         hot_q_data = pd.DataFrame(
             {'T2': tsq, 'Qres': q, 'Substance': x_train.Substance},
             index = x_data.index
         )
 
-        if self.settings.output:
+        if self.settings.output is GraphMode.GRAPHIC:
             # Plot the Hotelling T2 vs Q-residuals plot
             fig = px.scatter(
                 hot_q_data,
                 x="T2",
                 y="Qres",
                 hover_data={'Sample': (hot_q_data.index)},
                 color = "Substance"
@@ -199,15 +223,15 @@
         normalized_hot_q_data = {
             'T2': normalized_tsq,
             'Qres': normalized_q,
             'Substance': x_train.Substance
         }
         normalized_hot_q_data = pd.DataFrame(normalized_hot_q_data, index=x_data.index)
 
-        if self.settings.output:
+        if self.settings.output is GraphMode.GRAPHIC:
             # Plot the normalized Hotelling T2 vs Q-residuals plot
             fig_normalized = px.scatter(
                 normalized_hot_q_data,
                 x="T2",
                 y="Qres",
                 hover_data={'Sample': (normalized_hot_q_data.index)},
                 color="Substance"
@@ -218,16 +242,20 @@
             fig_normalized.update_layout(
                 height=600,
                 width=800,
                 title_text="Normalized Hotelling's T2 vs Q-residuals"
             )
             fig_normalized.show()
 
+
         # Assuming 'scores' is your DataFrame with the 'class' column
         # Drop the 'class' column before converting to NumPy array
         array_scores = scores.drop('Substance', axis=1).values
 
-        if self.settings.output:
-            print(f"Original DataFrame:\n{scores}")
-            print(f"\nNumPy Array without 'Substance' column:\n{array_scores}")
+        print_table(
+            pc_cols,
+            [array_scores[:,i] for i in range(array_scores.shape[1])],
+            "Array without 'Substance' column",
+            self.settings.output
+        )
 
         self.array_scores = array_scores
```

### Comparing `chemfusekit-1.1.1b1/chemfusekit/plsda.py` & `chemfusekit-1.1.1b2/chemfusekit/plsda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 '''Partial Least Squares Discriminant Analysis module.'''
+from copy import copy
 from typing import Optional
 
 import pandas as pd
 import numpy as np
 
 import plotly.express as px
 
 from sklearn.cross_decomposition import PLSRegression as PLSR
 
 from chemfusekit.lldf import LLDFModel
-from chemfusekit.__utils import print_confusion_matrix, run_split_test
+from chemfusekit.__utils import GraphMode, print_table, print_confusion_matrix, run_split_test
 
 
 class PLSDASettings:
     '''Holds the settings for the PLSDA object.'''
-    def __init__(self, n_components: int = 3, output: bool = False, test_split: bool = False):
+    def __init__(self, n_components: int = 3, output: GraphMode = GraphMode.NONE,
+                 test_split: bool = False):
         if n_components < 1:
             raise ValueError("Invalid n_components number: should be a positive integer.")
-        if test_split is True and output is False:
+        if test_split is True and output is GraphMode.NONE:
             raise Warning(
                 "You selected test_split but it won't run because you disabled the output."
             )
         self.n_components = n_components
         self.output = output
         self.test_split = test_split
 
+
 class PLSDA:
     '''
     Class to store the data, methods and artifacts for Partial Least Squares
     Discriminant Analysis
     '''
     def __init__(self, settings: PLSDASettings, fused_data: LLDFModel):
         self.settings = settings
@@ -37,38 +40,48 @@
 
     def plsda(self):
         '''Performs Partial Least Squares Discriminant Analysis'''
         x = self.fused_data.x_data
         y = self.fused_data.x_train.Substance.astype('category').cat.codes
 
         regr_pls = PLSR(n_components=self.settings.n_components)
-        regr_pls.fit_transform(x,y)
+        regr_pls.fit_transform(x, y)
 
         # Save the model
-        self.model = regr_pls
+        self.model = copy(regr_pls)
 
-        if self.settings.output:
-            # Re-create the model
-            regr_pls_2 = PLSR(n_components=self.settings.n_components)
-            regr_pls_2.fit_transform(x,y)
-
-            # Scores
-            scores = regr_pls_2.x_scores_
-            lv_cols = [f"LV{i+1}" for i in range(self.settings.n_components)]
-            scores = pd.DataFrame(scores, columns = lv_cols)
-            scores.index = self.fused_data.x_train.index
-            y = self.fused_data.x_train.Substance
-            scores = pd.concat([scores, y], axis = 1)
-            print(scores)
-
-            # Loadings
-            loadings = pd.DataFrame(regr_pls.x_loadings_,columns = lv_cols)
-            loadings["Attributes"] = self.fused_data.x_train.iloc[:,1:].columns
-            print(loadings)
+        # Re-create the model
+        regr_pls_2 = PLSR(n_components=self.settings.n_components)
+        regr_pls_2.fit_transform(x, y)
+
+        # Scores and loadings
+        lv_cols = [f"LV{i + 1}" for i in range(self.settings.n_components)]
+        scores = pd.DataFrame(regr_pls_2.x_scores_, columns=lv_cols)
+        scores.index = self.fused_data.x_train.index
+        y = self.fused_data.x_train.Substance
+        scores = pd.concat([scores, y], axis=1)
+
+        print_table(
+            scores.columns,
+            scores.transpose(),
+            "PLSDA scores by substance",
+            self.settings.output
+        )
+
+        # Loadings
+        loadings = pd.DataFrame(regr_pls.x_loadings_, columns=lv_cols)
+        loadings["Attributes"] = self.fused_data.x_train.iloc[:, 1:].columns
+        print_table(
+            loadings.columns,
+            loadings.transpose(),
+            "PLSDA Loadings",
+            self.settings.output
+        )
 
+        if self.settings.output is GraphMode.GRAPHIC:
             # Scores plot
             fig = px.scatter(scores, x="LV1", y="LV2", color="Substance", hover_data=['Substance'])
             fig.update_xaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_yaxes(zeroline=True, zerolinewidth=1, zerolinecolor='Black')
             fig.update_layout(
                 height=600,
                 width=800,
@@ -92,29 +105,45 @@
             fig.update_traces(textposition='top center')
             fig.update_layout(
                 height=600,
                 width=800,
                 title_text='Loadings Plot')
             fig.show()
 
-
             # Predictions
             pred = regr_pls.predict(x)
-            pred = np.int8(np.abs(np.around(pred, decimals=0)))
-            print(f"Predicted data:\n\n{pred}")
+            pred = np.int8(np.round(pred, decimals=0))
+            classes = np.unique(y)
+            for i in range(len(np.unique(pred)) - len(classes)):
+                classes = np.append(classes, f'Unknown substance {i}')
+            predicted_substances = [classes[p-1] for p in pred]
+            print_table(
+                ["Sample number", "True", "Predicted"],
+                np.stack((
+                    [f"{i+1}" for i in range(len(pred))],
+                    y,
+                    predicted_substances
+                )),
+                "True and predicted substances",
+                self.settings.output
+            )
 
             # Print confusion matrix
             y = self.fused_data.x_train.Substance.astype('category').cat.codes 
-            print_confusion_matrix(y, pred, "Confusion Matrix based on training set")
-
+            print_confusion_matrix(
+                y,
+                pred,
+                "Confusion Matrix based on training set",
+                self.settings.output
+            )
 
         if self.settings.output and self.settings.test_split:
             x = self.fused_data.x_data
             y = self.fused_data.x_train.Substance.astype('category').cat.codes
-            run_split_test(x, y, PLSR(self.settings.n_components))
+            run_split_test(x, y, PLSR(self.settings.n_components), mode=self.settings.output)
 
     def predict(self, x_data: pd.DataFrame):
         '''Performs PLSDA prediction once the model is trained.'''
         if x_data is None:
             raise TypeError("X data for PLSDA prediction must be non-empty.")
         if self.model is None:
             raise RuntimeError("The PLSDA model is not trained yet!")
```

### Comparing `chemfusekit-1.1.1b1/docs/README.md` & `chemfusekit-1.1.1b2/docs/README.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docusaurus.config.js` & `chemfusekit-1.1.1b2/docs/docusaurus.config.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
 import {
     themes as prismThemes
 } from 'prism-react-renderer';
 const simplePlantUML = require("@akebifiky/remark-simple-plantuml");
 
 /** @type {import('@docusaurus/types').Config} */
 const config = {
-    title: 'ChemFuseKit`: Colab Data Fusion and Analysis',
+    title: 'ChemFuseKit: Colab Data Fusion and Analysis',
     tagline: 'Chemometrics on the go',
     favicon: 'img/favicon.ico',
 
     // Set the production url of your site here
     url: 'https://f-aguzzi.github.io',
     // Set the /<baseUrl>/ pathname under which your site is served
     // For GitHub pages deployment, it is often '/<projectName>/'
```

### Comparing `chemfusekit-1.1.1b1/docs/package-lock.json` & `chemfusekit-1.1.1b2/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/package.json` & `chemfusekit-1.1.1b2/docs/package.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/sidebars.js` & `chemfusekit-1.1.1b2/docs/sidebars.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/complete-workflow.md` & `chemfusekit-1.1.1b2/docs/docs/complete-workflow.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/tutorial.md` & `chemfusekit-1.1.1b2/docs/docs/tutorial.md`

 * *Files 12% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 from chemfusekit.pca import PCASettings, PCA
 
 # Initialize the settings for Principal Component Analysis
 pca_settings = PCASettings(
     target_variance=0.99,   # the minimum acceptable level of cumulative explained covariance
     confidence_level=0.05,  # the desired level of confidence
     initial_components=10,  # the initial amount of components for the iterative analysis
-    output=True # graphs will be printed
+    output=GraphMode.GRAPHIC    # graphs will be printed
 )
 
 # Initialize and run the PCA class
 pca = PCA(lldf.fused_data, pca_settings)
 pca.pca()
 
 # Print the number of components and the statistics
@@ -80,15 +80,16 @@
 component than what we figured out from the `PCA` analysis of the previous step.
 
 ```python
 from chemfusekit.lda import LDASettings, LDA
 
 settings = LDASettings(
     components=(pca.components - 1),    # one less component than the number determined by PCA
-    output=True # graphs will be printed
+    output=GraphMode.GRAPHIC,   # graphs will be printed
+    test_split=True # Split testing is enabled
 )
 
 # Initialize and run the LDA class
 lda = LDA(lldf.fused_data, settings)
 lda.lda()
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/knn/knn.md` & `chemfusekit-1.1.1b2/docs/docs/knn/knn.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/knn/knnsettings.md` & `chemfusekit-1.1.1b2/docs/docs/knn/knnsettings.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ```python
 KNNSettings(
   n_neighbors: int,
   metric: str | Callable,
   weights: str | Callable,
   algorithm: str,
-  output: bool,
+  output: GraphMode,
   test_split: false
 )
 ```
 
 ## Fields and constructor parameters
 - `n_neighbors`: the amount of components to be used in the `KNN` model. Defaults to 15.
 - `metric`: the distance metric for the model. It can take one of the following values:
@@ -32,31 +32,31 @@
   or be a callable object.
 - `algorithm`: the algorithm for the model. It can take one of the following values:
     - `auto`
     - `ball_tree`
     - `kd_tree`
     - `brute`
   or be a callable object.
-- `output`: toggles graph output. Defaults to `False`.
+- `output`: toggles graph output mode. Defaults to [`GraphMode.NONE`](../utils/graphmode.md).
 - `test_split`: toggles the training split test phase. Defaults to `False`. Requires `output` to be set to `True` to work.
 
 The constructor raises:
 - `ValueError("Invalid n_neighbors number: should be a positive integer.")` if the number of components is not valid.
 - `ValueError("Invalid metric: should be 'minkwoski', 'precomputed', 'euclidean' or a callable.")` if the chosen metric is neither available nor a callable function.
 - `ValueError("Invalid weight: should be 'uniform', 'distance' or a callable")` if the chosen weight is neither available nor a callable function.
 - `ValueError("Invalid algorithm: should be 'auto', 'ball_tree', 'kd_tree' or 'brute'.")` if the chosen algotithm does not exist.
 - `Warning("You selected test_split but it won't run because you disabled the output.")` if `test_split` is run with `output` set to false (split tests only produce graphical output, and are useless when run with disabled output).
 
 ## Example
 
 ```python
-from chemfusekit.knn import KNNSettings
+from chemfusekit.knn import KNNSettings, GraphMode
 
 settings = KNNSettings(
     n_neighbors=20,     # pick 20 neighbors
     metric='minkowski', # choose the metric
     weights='distance', # choose the weight metric
     algorithm='auto',   # the best algorithm gets chosen automatically
-    output=True,    # graph output is enabled
+    output=GraphMode.GRAPHIC, # graph output is enabled
     test_split=True # the model will be split-tested at the end of the training
 )
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/lda/lda.md` & `chemfusekit-1.1.1b2/docs/docs/lda/lda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/lda/ldasettings.md` & `chemfusekit-1.1.1b2/docs/docs/lda/ldasettings.md`

 * *Files 17% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 # LDASettings class
 
 Holds the settings for the [`LDA`](./lda.md) object.
 
 ## Syntax
 
 ```python
-LDASettings(components: int, output: bool, split_test: bool)
+LDASettings(components: int, output: GraphMode, split_test: bool)
 ```
 
 ## Fields and constructor parameters
 
 - `components`: the amount of components to be used in the LDA model. Defaults to 3.
-- `output`: toggles graph output. Defaults to `False`.
+- `output`: toggles graph output. Defaults to [`GraphMode.NONE`](../utils/graphmode.md).
 - `test_split`: toggles split testing. Defaults to `False`.
 
 
 The constructor raises:
 - `ValueError("Invalid component number: must be a > 1 integer.")` if the number of
   components is not valid.
 - `Warning("You selected test_split but it won't run because you disabled the output.")` if split tests are run with `output` disabled
 
 ## Example
 
 ```python
-from chemfusekit.lda import LDASettings
+from chemfusekit.lda import LDASettings, GraphMode
 
 settings = LDASettings(
     components=(pca.components - 1),    # one less component than the number determined by PCA
-    output=True,  # graphs will be printed
+    output=GraphMode.GRAPHIC, # graphs will be printed
     test_split=True # split testing is enabled
 )
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/lldf/lldf.md` & `chemfusekit-1.1.1b2/docs/docs/lldf/lldf.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/lldf/lldfsettings.md` & `chemfusekit-1.1.1b2/docs/docs/lldf/lldfsettings.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/lr/lr.md` & `chemfusekit-1.1.1b2/docs/docs/lr/lr.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/lr/lrsettings.md` & `chemfusekit-1.1.1b2/docs/docs/lr/lrsettings.md`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,38 @@
 # LRSettings class
 
 Holds the settings for the [`LR`](./lr.md) object.
 
 ## Syntax
 
 ```python
-LRSettings(algorithm: str, output: bool)
+LRSettings(algorithm: str, output: GraphMode, test_split: bool)
 ```
 
 ## Fields and constructor parameters
 
 - `algorithm`: the amount of components to be used in the LDA model. Defaults to
   `liblinear`.  Other available options:
     - `lbfgs`
     - `newton-cg`
     - `newton-cholesky`
     - `sag`
     - `saga`
-- `output`: toggles graph output. Defaults to `False`.
+- `output`: toggles graph output. Defaults to [`GraphMode.NONE`](../utils/graphmode.md).
 - `test_split`: toggles split testing. Defaults to `False`.
 
 The constructor raises:
 - `ValueError("This algorithm does not exist.")` if the selected `algorithm`
   is not a valid option.
 - `Warning("You selected test_split but it won't run because you disabled the output.")` if split tests are run with `output` disabled
 
 ## Example
 
 ```python
-from chemfusekit.lr import LRSettings
+from chemfusekit.lr import LRSettings, GraphMode
 
 settings = LRSettings(
     algorithm='newton-cg',
-    output=True,  # graphs will be printed
+    output=GraphMode.GRAPHIC,   # graphs will be printed
     test_split=True # split testing is enabled
 )
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/pca/pca.md` & `chemfusekit-1.1.1b2/docs/docs/pca/pca.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/pca/pcasettings.md` & `chemfusekit-1.1.1b2/docs/docs/pca/pcasettings.md`

 * *Files 18% similar despite different names*

```diff
@@ -9,33 +9,33 @@
 ## Syntax
 
 ```python
 PCASettings(
   target_variance: float,
   confidence_level: float,
   initial_components: int,
-  output: bool
+  output: GraphMode
 )
 ```
 
 ## Fields and constructor parameters
 
 - `target_variance`: the minimum cumulative explained variance to reach in the analysis.
   Defaults to 0.95.
 - `confidence_level`: the confidence level for statistical tests. Defaults to 0.05.
 - `initial_components`: the minimum amount of components to be used in the PCA model.
   Defaults to 10.
-- `output`: toggles graph output. Defaults to `False`.
+- `output`: toggles graph output. Defaults to [`GraphMode.NONE`](../utils/graphmode.md).
 
 ## Example
 
 ```python
-from chemfusekit.pca import PCASettings
+from chemfusekit.pca import PCASettings, GraphMode
 
 # Initialize the settings for Principal Component Analysis
 pca_settings = PCASettings(
     target_variance=0.99,
     confidence_level=0.05,
     initial_components=10,
-    output=True # graphs will be printed
+    output=GraphMode.GRAPHIC  # graphs will be printed
 )
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/plsda/plsda.md` & `chemfusekit-1.1.1b2/docs/docs/plsda/plsda.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/docs/plsda/plsdasettings.md` & `chemfusekit-1.1.1b2/docs/docs/svm/svmsettings.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 ---
 sidebar_position: 2
 ---
 
-# PLSDASettings class
+# SVMSettings class
 
-Holds the settings for the [`PLSDA`](./plsda.md) object.
+Holds the settings for the [`SVM`](./svm.md) object.
 
 ## Syntax
 
 ```python
-PLSDASettings(n_components: int, output: bool, test_split: bool)
+SVMSettings(kernel: str, output: GraphMode, test_split: bool)
 ```
 
 ## Fields and constructor parameters
 
-- `n_components`: number of components for the PLSDA analysis. Defaults to 3.
-- `output`: toggles graph output. Defaults to `False`.
-- `test_split`: toggles the training split test phase. Defaults to `False`. Requires `output` to be set to `True` to work.
+- `kernel`: the type of kernel to use in the SVM analysis. Available options:
+  - `linear`
+  - `poly`
+  - `gaussian`
+  - `sigmoid`
+  Defaults to `linear`.
+- `output`: toggles graph output. Defaults to [`GraphMode.NONE`](../utils/graphmode.md).
+- `test_split`: toggles split testing. Defaults to `False`.
 
 The constructor raises:
-- `ValueError("Invalid n_components number: should be a positive integer.")` if the number of components is below 1.
-- `Warning("You selected test_split but it won't run because you disabled the output.")` if `test_split` is run with `output` set to false (split tests only produce graphical output, and are useless when run with disabled output).
+- `ValueError("Invalid type: must be linear, poly, gaussian or sigmoid")` if the selected kernel is not one of the available
+- `Warning("You selected test_split but it won't run because you disabled the output.")` if split tests are run with `output` disabled
 
 ## Example
 
 ```python
-from chemfusekit.plsda import PLSDASettings
+from chemfusekit.svm import SVMSettings, GraphMode
 
-# Initialize the settings for Partial Least Squares Discriminant Analysis
-plsda_settings = PLSDASettings(
-    components=5,
-    output=True, # graphs will be printed
-    test_split=False    # no split testing
+# Initialize the settings for Support Vector Machine
+svm_settings = SVMSettings(
+    type='linear',
+    output=GraphMode.GRAPHIC,   # graphs will be printed
+    test_split=True # split testing is enabled
 )
 ```
```

### Comparing `chemfusekit-1.1.1b1/docs/docs/svm/svm.md` & `chemfusekit-1.1.1b2/docs/docs/svm/svm.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/components/HomepageFeatures/index.js` & `chemfusekit-1.1.1b2/docs/src/components/HomepageFeatures/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/css/custom.css` & `chemfusekit-1.1.1b2/docs/src/css/custom.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/index.js` & `chemfusekit-1.1.1b2/docs/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/continuous-integration.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/continuous-integration.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/process-model.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/process-model.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/project-philosophy.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/project-philosophy.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/project-plan.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/project-plan.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/requirements-specification.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/requirements-specification.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/src/pages/project/use-cases.md` & `chemfusekit-1.1.1b2/docs/src/pages/project/use-cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/colab-logo.svg` & `chemfusekit-1.1.1b2/docs/static/img/colab-logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/docusaurus-social-card.jpg` & `chemfusekit-1.1.1b2/docs/static/img/docusaurus-social-card.jpg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/docusaurus.png` & `chemfusekit-1.1.1b2/docs/static/img/docusaurus.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/favicon.ico` & `chemfusekit-1.1.1b2/docs/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/happy-woman.svg` & `chemfusekit-1.1.1b2/docs/static/img/happy-woman.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/logo.svg` & `chemfusekit-1.1.1b2/docs/static/img/logo.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/docs/static/img/magnifying-glass.svg` & `chemfusekit-1.1.1b2/docs/static/img/magnifying-glass.svg`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Beartype.md` & `chemfusekit-1.1.1b2/notes/Beartype.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Constructors.md` & `chemfusekit-1.1.1b2/notes/Constructors.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Conventional Commits.md` & `chemfusekit-1.1.1b2/notes/Conventional Commits.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Kanban.md` & `chemfusekit-1.1.1b2/notes/Kanban.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Use Case Diagram.md` & `chemfusekit-1.1.1b2/notes/Use Case Diagram.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/core-plugins-migration.json` & `chemfusekit-1.1.1b2/notes/.obsidian/core-plugins-migration.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/workspace.json` & `chemfusekit-1.1.1b2/notes/.obsidian/workspace.json`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/plugins/calendar/main.js` & `chemfusekit-1.1.1b2/notes/.obsidian/plugins/calendar/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/main.js` & `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-kanban/styles.css` & `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-kanban/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/main.js` & `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/main.js`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/.obsidian/plugins/obsidian-plantuml/styles.css` & `chemfusekit-1.1.1b2/notes/.obsidian/plugins/obsidian-plantuml/styles.css`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-04-19.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-04-19.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-04-20.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-04-20.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-04-22.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-04-22.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-04-23.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-04-23.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-06.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-06.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-07.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-07.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-08.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-08.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-09.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-09.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-17.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-17.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/Devlog/2024-05-18.md` & `chemfusekit-1.1.1b2/notes/Devlog/2024-05-18.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/UML/Process state machine.md` & `chemfusekit-1.1.1b2/notes/UML/Process state machine.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/UML/Sequence.md` & `chemfusekit-1.1.1b2/notes/UML/Sequence.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/notes/UML/Use cases.md` & `chemfusekit-1.1.1b2/notes/UML/Use cases.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/tests/qepas.xlsx` & `chemfusekit-1.1.1b2/tests/qepas.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/tests/rt.xlsx` & `chemfusekit-1.1.1b2/tests/rt.xlsx`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/tests/test_knn.py` & `chemfusekit-1.1.1b2/tests/test_knn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''This module contains the test cases for the KNN module.'''
 import unittest
 
 import pandas as pd
 import numpy as np
 
-from chemfusekit.knn import KNNSettings, KNN
+from chemfusekit.knn import KNNSettings, KNN, GraphMode
 from chemfusekit.lldf import LLDFSettings, LLDF, LLDFModel
 
 class TestKNN(unittest.TestCase):
     '''Test suite for the KNN module.'''
 
     def test_knn_settings(self):
         '''Test case against settings errors.'''
@@ -49,23 +49,23 @@
         with self.assertRaises(ValueError):
             KNNSettings(algorithm='invalid attribute') # Non-existent technique
         for x in ['auto', 'ball_tree', 'kd_tree', 'brute']:
             KNNSettings(algorithm=x)    # Correct values (shouldn't raise anything)
 
         # output parameter
         with self.assertRaises(TypeError):
-            KNNSettings(output=3)   # Wrong type (not a bool)
+            KNNSettings(output=3)   # Wrong type (not a GraphMode enum)
 
         # test_split parameter
         with self.assertRaises(TypeError):
             KNNSettings(test_split=3)   # Wrong type (not a bool)
 
         # output and test_split incompatibilities
         with self.assertRaises(Warning):
-            KNNSettings(output=False, test_split=True)
+            KNNSettings(output=GraphMode.NONE, test_split=True)
 
     def test_knn_constructor(self):
         '''Test case against constructor errors.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
@@ -101,16 +101,21 @@
         lldf.lldf()
 
         # Set up and run KNN (no output)
         knn_settings = KNNSettings()
         knn = KNN(knn_settings, lldf.fused_data)
         knn.knn()
 
-        # With output
-        knn_settings = KNNSettings(output=True)
+        # With graph output
+        knn_settings = KNNSettings(output=GraphMode.GRAPHIC)
+        knn = KNN(knn_settings, lldf.fused_data)
+        knn.knn()
+
+        # With text output
+        knn_settings = KNNSettings(output=GraphMode.TEXT)
         knn = KNN(knn_settings, lldf.fused_data)
         knn.knn()
 
     def test_prediction(self):
         '''Test case against prediction parameter issues.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
```

### Comparing `chemfusekit-1.1.1b1/tests/test_lda.py` & `chemfusekit-1.1.1b2/tests/test_lda.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 '''This module contains the test cases for the LDA module.'''
 import unittest
-from chemfusekit.lda import LDASettings, LDA
+from chemfusekit.lda import LDASettings, LDA, GraphMode
 from chemfusekit.lldf import LLDFSettings, LLDF
 
 class TestLDA(unittest.TestCase):
     '''Test suite for the LDA module.'''
 
     def test_lda_settings(self):
         '''Test case against settings errors.'''
         # Check for negative component rejection
         with self.assertRaises(ValueError):
-            LDASettings(components=-3, output=True)
+            LDASettings(components=-3, output=GraphMode.TEXT)
         # Check if split tests with no output cause warnings:
         with self.assertRaises(Warning):
-            LDASettings(output=False,test_split=True)
+            LDASettings(output=GraphMode.NONE, test_split=True)
 
     def test_lda_constructor(self):
         '''Test case against constructor parameter issues.'''
 
         # Create an LLDF model and initialize it
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
@@ -55,26 +55,31 @@
             rt_path='tests/rt.xlsx',
             rt_sheet='Sheet1',
             preprocessing='snv'
         )
         lldf = LLDF(lldf_settings)
         lldf.lldf()
 
-        # Create an LDA object and train it, with true output
-        lda_settings = LDASettings(output=True)
+        # Create an LDA object and train it, with graphical output
+        lda_settings = LDASettings(output=GraphMode.GRAPHIC)
         lda = LDA(lldf.fused_data, lda_settings)
         lda.lda()
 
-        # Create an LDA object and train it, with false output
-        lda_settings = LDASettings(output=False)
+        # Create an LDA object and train it, with text output
+        lda_settings = LDASettings(output=GraphMode.TEXT)
+        lda = LDA(lldf.fused_data, lda_settings)
+        lda.lda()
+
+        # Create an LDA object and train it, with no output
+        lda_settings = LDASettings(output=GraphMode.NONE)
         lda = LDA(lldf.fused_data, lda_settings)
         lda.lda()
 
         # Create an LDA object and train it, with true output and split tests
-        lda_settings = LDASettings(output=True, test_split=True)
+        lda_settings = LDASettings(output=GraphMode.TEXT, test_split=True)
         lda = LDA(lldf.fused_data, lda_settings)
         lda.lda()
 
     def test_lda_predict(self):
         '''Test case against prediction parameter issues.'''        
 
         # Create an LLDF model and initialize it
```

### Comparing `chemfusekit-1.1.1b1/tests/test_lldf.py` & `chemfusekit-1.1.1b2/tests/test_lldf.py`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/tests/test_lr.py` & `chemfusekit-1.1.1b2/tests/test_lr.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,57 +2,57 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 
 from chemfusekit.lldf import LLDFSettings, LLDF
 from chemfusekit.pca import PCASettings, PCA
-from chemfusekit.lr import LRSettings, LR
+from chemfusekit.lr import LRSettings, LR, GraphMode
 
 class TestLR(unittest.TestCase):
     '''Test suite for the LR module.'''
 
     def test_lr_settings(self):
         '''Test case against settings input errors.'''
         # Should raise an exception when the algorithm is not available
         with self.assertRaises(ValueError):
             LRSettings(
                 algorithm='unknown',
-                output=True,
+                output=GraphMode.NONE,
                 test_split=True
             )
 
         # Should raise an exception when any of the inputs is a null value
         with self.assertRaises(TypeError):
             LRSettings(
                 algorithm=None,
-                output=True,
+                output=GraphMode.NONE,
                 test_split=True
             )
         with self.assertRaises(TypeError):
             LRSettings(
                 algorithm='liblinear',
                 output=None,
                 test_split=True
             ) 
         with self.assertRaises(TypeError):
             LRSettings(
                 algorithm='liblinear',
-                output=True,
+                output=GraphMode.NONE,
                 test_split=None
             )
         
         # Check if split tests with no output cause warnings:
         with self.assertRaises(Warning):
-            LRSettings(output=False,test_split=True)
+            LRSettings(output=GraphMode.NONE, test_split=True)
 
         # Should not raise any exception when the input is correct
         LRSettings(
             algorithm='liblinear',
-            output=False
+            output=GraphMode.TEXT
         )
 
     def test_lr_constructor(self):
         '''Test case against constructor input errors.'''
         # Should raise an exception when the inputs are null
         with self.assertRaises(TypeError):
             LR(
@@ -99,19 +99,34 @@
         pca.pca_stats()
 
         # With no output
         lr_settings = LRSettings()
         lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
         lr.lr()
 
-        # With output and split tests
-        lr_settings = LRSettings(output=True, test_split=True)
+        # With text output
+        lr_settings = LRSettings(output=GraphMode.TEXT)
         lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
         lr.lr()
 
+        # With graph output
+        # With text output
+        lr_settings = LRSettings(output=GraphMode.GRAPHIC)
+        lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
+        lr.lr()
+
+        # With text output and split tests
+        lr_settings = LRSettings(output=GraphMode.TEXT, test_split=True)
+        lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
+        lr.lr()
+
+        # With graph output and split tests
+        lr_settings = LRSettings(output=GraphMode.GRAPHIC, test_split=True)
+        lr = LR(lr_settings, pca.array_scores, lldf.fused_data.y)
+        lr.lr()
 
     def test_lr_predict(self):
         '''Test case against prediction input errors.'''
         # Set up the model
         lr_settings = LRSettings()
         lr = LR(lr_settings, np.asarray([7.02, 8.11]), np.asarray([43.1, 0.06]))
```

### Comparing `chemfusekit-1.1.1b1/tests/test_pca.py` & `chemfusekit-1.1.1b2/tests/test_pca.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''This module contains the test cases for the PCA module.'''
 import unittest
-from chemfusekit.pca import PCASettings, PCA
+import copy
+from chemfusekit.pca import PCASettings, PCA, GraphMode
 from chemfusekit.lldf import LLDFSettings, LLDF
 
 class TestPCA(unittest.TestCase):
     '''Test suite for the PCA module.'''
 
     def test_pca_settings(self):
         '''Test case against settings errors.'''
@@ -21,15 +22,15 @@
             PCASettings(initial_components=2)
 
         # Now try with no mistakes:
         PCASettings(
             target_variance=0.98,
             confidence_level=0.9,
             initial_components=8,
-            output=True
+            output=GraphMode.GRAPHIC
         )
 
     def test_pca_constructor(self):
         '''Test case against constructor parameter issues.'''
 
         # Create a LLDF model and initialize it
         lldf_settings = LLDFSettings(
@@ -71,25 +72,47 @@
             rt_path='tests/rt.xlsx',
             rt_sheet='Sheet1',
             preprocessing='snv'
         )
         lldf = LLDF(lldf_settings)
         lldf.lldf()
 
-        # Set up and execute PCA
-        pca_settings = PCASettings(output=True)
+        # Set up and execute PCA (graph output)
+        pca_settings = PCASettings(output=GraphMode.GRAPHIC)
         pca = PCA(lldf.fused_data, pca_settings)
         pca.pca()
 
         # Save the results
-        result_true_components = pca.components
-        result_true_array_scores = pca.array_scores
+        result_true_components = copy.deepcopy(pca.components)
+        result_true_array_scores = copy.deepcopy(pca.array_scores)
 
         # Set up and execute PCA (again)
-        pca_settings = PCASettings(output=False)
+        pca_settings = PCASettings(output=GraphMode.NONE)
+        pca = PCA(lldf.fused_data, pca_settings)
+        pca.pca()
+
+       # Save the results
+        result_false_components = pca.components
+        result_false_array_scores = pca.array_scores
+
+        self.assertEqual(result_true_components, result_false_components)
+        self.assertEqual(result_true_array_scores, result_false_array_scores)
+
+
+        # Set up and execute PCA (text output)
+        pca_settings = PCASettings(output=GraphMode.GRAPHIC)
+        pca = PCA(lldf.fused_data, pca_settings)
+        pca.pca()
+
+        # Save the results
+        result_true_components = copy.deepcopy(pca.components)
+        result_true_array_scores = copy.deepcopy(pca.array_scores)
+
+        # Set up and execute PCA (again)
+        pca_settings = PCASettings(output=GraphMode.NONE)
         pca = PCA(lldf.fused_data, pca_settings)
         pca.pca()
 
        # Save the results
         result_false_components = pca.components
         result_false_array_scores = pca.array_scores
```

### Comparing `chemfusekit-1.1.1b1/tests/test_plsda.py` & `chemfusekit-1.1.1b2/tests/test_plsda.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 '''This module contains the test cases for the KNN module.'''
 import unittest
 
 import numpy as np
 import pandas as pd
 
-from chemfusekit.plsda import PLSDASettings, PLSDA
+from chemfusekit.plsda import PLSDASettings, PLSDA, GraphMode
 from chemfusekit.lldf import LLDFSettings, LLDF, LLDFModel
 
+
 class TestPLSDA(unittest.TestCase):
     '''Test suite for the PLSDA module.'''
 
     def test_plsda_settings(self):
         '''Test case against settings errors.'''
 
         # n_components parameter
@@ -26,15 +27,15 @@
 
         # test_split parameter
         with self.assertRaises(TypeError):
             PLSDASettings(test_split=3)   # Wrong type (not a bool)
 
         # output and test_split incompatibilities
         with self.assertRaises(Warning):
-            PLSDASettings(output=False, test_split=True)
+            PLSDASettings(output=GraphMode.NONE, test_split=True)
 
     def test_plsda_constructor(self):
         '''Test case against constructor errors.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
             qepas_sheet='Sheet1',
@@ -70,16 +71,31 @@
         lldf.lldf()
 
         # Set up and run PLSDA (no output)
         plsda_settings = PLSDASettings()
         plsda = PLSDA(plsda_settings, lldf.fused_data)
         plsda.plsda()
 
-        # Run with output and split testing
-        plsda_settings = PLSDASettings(output=True, test_split=True)
+        # Set up and run PLSDA with text output
+        plsda_settings = PLSDASettings(output=GraphMode.TEXT)
+        plsda = PLSDA(plsda_settings, lldf.fused_data)
+        plsda.plsda()
+
+        # Set up and run PLSDA with graphical output
+        plsda_settings = PLSDASettings(output=GraphMode.GRAPHIC)
+        plsda = PLSDA(plsda_settings, lldf.fused_data)
+        plsda.plsda()
+
+        # Run with text output and split testing
+        plsda_settings = PLSDASettings(output=GraphMode.TEXT, test_split=True)
+        plsda = PLSDA(plsda_settings, lldf.fused_data)
+        plsda.plsda()
+
+        # Run with graphical output and split testing
+        plsda_settings = PLSDASettings(output=GraphMode.GRAPHIC, test_split=True)
         plsda = PLSDA(plsda_settings, lldf.fused_data)
         plsda.plsda() 
     
     def test_prediction(self):
         '''Test case against prediction parameter issues.'''
         # Perform preliminary data fusion
         lldf_settings = LLDFSettings(
```

### Comparing `chemfusekit-1.1.1b1/tests/test_svm.py` & `chemfusekit-1.1.1b2/tests/test_svm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 '''This module contains the test cases for the SVM module.'''
 import unittest
-from chemfusekit.svm import SVMSettings, SVM
+from chemfusekit.svm import SVMSettings, SVM, GraphMode
 from chemfusekit.lldf import LLDFSettings, LLDF
 
 class TestSVM(unittest.TestCase):
     '''Test suite for the LDA module.'''
 
     def test_svm_settings(self):
         '''Test case against settings errors.'''
         # Test against null type
         with self.assertRaises(TypeError):
-            SVMSettings(None, False, False)
+            SVMSettings(None, GraphMode.NONE, False)
         # Test against null output selector
         with self.assertRaises(TypeError):
             SVMSettings('linear', None, False)
         # Test against null test_split selector
         with self.assertRaises(TypeError):
-            SVMSettings('linear', None, False)
+            SVMSettings('linear', GraphMode.NONE, None)
         # Test against non-existent kernels
-        with self.assertRaises(TypeError):
-            SVMSettings('linear', False, None)
+        with self.assertRaises(ValueError):
+            SVMSettings('non-existent', GraphMode.NONE, False)
 
         # Check if split tests with no output cause warnings:
         with self.assertRaises(Warning):
-            SVMSettings(output=False,test_split=True)
+            SVMSettings(output=GraphMode.NONE, test_split=True)
 
         # Now call with proper values:
-        SVMSettings(kernel='gaussian', output=True, test_split=False)
-
+        SVMSettings(kernel='gaussian', output=GraphMode.GRAPHIC, test_split=False)
 
     def test_svm_constructor(self):
         '''Test case against constructor parameter issues.'''
 
         # Create an LLDF model and initialize it
         lldf_settings = LLDFSettings(
             qepas_path='tests/qepas.xlsx',
@@ -70,22 +69,26 @@
             rt_path='tests/rt.xlsx',
             rt_sheet='Sheet1',
             preprocessing='snv'
         )
         lldf = LLDF(lldf_settings)
         lldf.lldf()
 
-        # Create an SVM object and train it, with true output
-        svm_settings = SVMSettings(output=True)
+        # Create an SVM object and train it, with no output
+        svm_settings = SVMSettings(output=GraphMode.NONE)
         svm = SVM(lldf.fused_data, svm_settings)
         svm.svm()
 
+        # Create an SVM object and train it, with graphical output
+        svm_settings = SVMSettings(output=GraphMode.GRAPHIC)
+        svm = SVM(lldf.fused_data, svm_settings)
+        svm.svm()
 
-        # Create an SVM object and train it, with false output
-        svm_settings = SVMSettings(output=True)
+        # Create an SVM object and train it, with text output
+        svm_settings = SVMSettings(output=GraphMode.TEXT)
         svm = SVM(lldf.fused_data, svm_settings)
         svm.svm()
 
     def test_svm_predict(self):
         '''Test case against prediction parameter issues.'''        
 
         # Create an LLDF model and initialize it
```

### Comparing `chemfusekit-1.1.1b1/thesis/0-header.md` & `chemfusekit-1.1.1b2/thesis/0-header.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/thesis/1-abstract.md` & `chemfusekit-1.1.1b2/thesis/1-abstract.md`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/thesis/logo-unibg.png` & `chemfusekit-1.1.1b2/thesis/logo-unibg.png`

 * *Files identical despite different names*

### Comparing `chemfusekit-1.1.1b1/pyproject.toml` & `chemfusekit-1.1.1b2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 [project]
 name = "chemfusekit"
-version = "1.1.1b1"
+version = "1.1.1b2"
 description = "A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis."
 authors = [
     { name = "Federico Aguzzi", email = "62149513+f-aguzzi@users.noreply.github.com" }
 ]
 dependencies = [
     "numpy>=1.26.4",
     "scipy>=1.13.0",
     "matplotlib>=3.8.4",
     "pandas>=2.2.2",
     "seaborn>=0.13.2",
     "openpyxl>=3.1.2",
     "scikit-learn>=1.4.2",
     "plotly>=5.22.0",
     "beartype>=0.18.5",
+    "nbformat>=4.2.0",
+    "tabulate>=0.9.0",
 ]
 readme = "readme.md"
 repository = "https://github.com/f-aguzzi/tesi"
 documentation = "https://f-aguzzi.github.io/tesi/"
 requires-python = ">= 3.8"
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = [
     "pylint>=3.1.1",
+    "ipykernel>=6.29.4",
 ]
 
 [tool.rye.scripts]
 test = "python -m unittest discover tests"
 pylint-local = "pylint chemfusekit/**/*.py"
 pylint-ci = "pylint --disable=C0114,C0115,C0116 --exit-zero chemfusekit/**/*.py"
 pylint-score-ci = "pylint --disable=all --enable=metrics --output-format=text chemfusekit/**/.py"
```

### Comparing `chemfusekit-1.1.1b1/readme.md` & `chemfusekit-1.1.1b2/readme.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # `chemfusekit`: Data Fusion and Analysis in Colab
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/f-aguzzi/tesi/actions/workflows/pylint.yml/badge.svg)](https://github.com/f-aguzzi/tesi/)
 [![Unittest](https://github.com/f-aguzzi/tesi/actions/workflows/unittest.yml/badge.svg)](https://github.com/f-aguzzi/tesi/)
 [![](https://img.shields.io/badge/Read_the_docs-GitHub_Pages-darkorange)](https://f-aguzzi.github.io/tesi/)
-[![Try It On Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/cda_example_notebook.ipynb)
-
+[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_example_notebook.ipynb)
 <p align="center">
   <img src="https://raw.githubusercontent.com/f-aguzzi/tesi/main/docs/static/img/logo.svg" alt="Library Logo" style="width: 20%;">
 </p>
 
 A minimal Python / Jupyter Notebook / Colab library for data fusion and
 chemometrical analysis.
 
@@ -30,15 +29,15 @@
 pip install chemfusekit
 ```
 
 <br />
 
 You can also try this demo:
 
-[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/cda_example_notebook.ipynb)
+[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_notebook.ipynb)
 
 and find instructions [here](https://f-aguzzi.github.io/tesi/docs/tutorial).
 
 <br />
 
 ## Features
 
@@ -46,12 +45,12 @@
   precision of your chemometrical analysis
 - **model training**: train, save and load statistical models
 - **data classification**: use your models to classify and predict
 
 Here's a list of the currently available modules:
 - **LLDF**: *Low-Level Data Fusion*
 - **PCA**: *Principal Component Analysis*
-- **LDA**: *Linear Discriminant Analysis*
-- **SVM**: *Support Vector Machine*
-- **LR**: *Logistic Regression*
-- **KNN**: *k_Neighbors Analysis*
-- **PLSDA**: *Partial Least Squres Discriminant Analysis*
+- **LDA**: *Linear Discriminant Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_notebook.ipynb))
+- **SVM**: *Support Vector Machine* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/svm_notebook.ipynb))
+- **LR**: *Logistic Regression* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lr_notebook.ipynb))
+- **KNN**: *k_Neighbors Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/knn_notebook.ipynb))
+- **PLSDA**: *Partial Least Squres Discriminant Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/plsda_notebook.ipynb))
```

### Comparing `chemfusekit-1.1.1b1/PKG-INFO` & `chemfusekit-1.1.1b2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.3
 Name: chemfusekit
-Version: 1.1.1b1
+Version: 1.1.1b2
 Summary: A minimal Python / Jupyter Notebook / Colab library for data fusion and chemometrical analysis.
 Author-email: Federico Aguzzi <62149513+f-aguzzi@users.noreply.github.com>
 Requires-Python: >=3.8
 Requires-Dist: beartype>=0.18.5
 Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: nbformat>=4.2.0
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: openpyxl>=3.1.2
 Requires-Dist: pandas>=2.2.2
 Requires-Dist: plotly>=5.22.0
 Requires-Dist: scikit-learn>=1.4.2
 Requires-Dist: scipy>=1.13.0
 Requires-Dist: seaborn>=0.13.2
+Requires-Dist: tabulate>=0.9.0
 Description-Content-Type: text/markdown
 
 # `chemfusekit`: Data Fusion and Analysis in Colab
 
 [![linting: pylint](https://img.shields.io/badge/linting-pylint-yellowgreen)](https://github.com/pylint-dev/pylint)
 [![Pylint](https://github.com/f-aguzzi/tesi/actions/workflows/pylint.yml/badge.svg)](https://github.com/f-aguzzi/tesi/)
 [![Unittest](https://github.com/f-aguzzi/tesi/actions/workflows/unittest.yml/badge.svg)](https://github.com/f-aguzzi/tesi/)
 [![](https://img.shields.io/badge/Read_the_docs-GitHub_Pages-darkorange)](https://f-aguzzi.github.io/tesi/)
-[![Try It On Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/cda_example_notebook.ipynb)
-
+[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_example_notebook.ipynb)
 <p align="center">
   <img src="https://raw.githubusercontent.com/f-aguzzi/tesi/main/docs/static/img/logo.svg" alt="Library Logo" style="width: 20%;">
 </p>
 
 A minimal Python / Jupyter Notebook / Colab library for data fusion and
 chemometrical analysis.
 
@@ -47,15 +48,15 @@
 pip install chemfusekit
 ```
 
 <br />
 
 You can also try this demo:
 
-[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/cda_example_notebook.ipynb)
+[![Try It In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_notebook.ipynb)
 
 and find instructions [here](https://f-aguzzi.github.io/tesi/docs/tutorial).
 
 <br />
 
 ## Features
 
@@ -63,12 +64,12 @@
   precision of your chemometrical analysis
 - **model training**: train, save and load statistical models
 - **data classification**: use your models to classify and predict
 
 Here's a list of the currently available modules:
 - **LLDF**: *Low-Level Data Fusion*
 - **PCA**: *Principal Component Analysis*
-- **LDA**: *Linear Discriminant Analysis*
-- **SVM**: *Support Vector Machine*
-- **LR**: *Logistic Regression*
-- **KNN**: *k_Neighbors Analysis*
-- **PLSDA**: *Partial Least Squres Discriminant Analysis*
+- **LDA**: *Linear Discriminant Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lda_notebook.ipynb))
+- **SVM**: *Support Vector Machine* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/svm_notebook.ipynb))
+- **LR**: *Logistic Regression* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/pca_lr_notebook.ipynb))
+- **KNN**: *k_Neighbors Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/knn_notebook.ipynb))
+- **PLSDA**: *Partial Least Squres Discriminant Analysis* ([demo](https://colab.research.google.com/github/f-aguzzi/tesi/blob/main/examples/plsda_notebook.ipynb))
```

