# Comparing `tmp/sxs-2023.1.0.tar.gz` & `tmp/sxs-2023.1.1.tar.gz`

## Comparing `sxs-2023.1.0.tar` & `sxs-2023.1.1.tar`

### file list

```diff
@@ -1,116 +1,118 @@
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.1.0/.codecov.yml
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.1.0/CITATION.cff
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sxs-2023.1.0/mkdocs.yml
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/scripts/parse_bump_rule.py
--rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.1.0/.github/workflows/pr_rtd_link.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/index.md -> ../README.md
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/mathematica.md
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/catalog.md
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/horizons.md
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/load.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/metadata.md
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/time_series.md
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/api/waveforms.md
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/html/main.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/images/favicon.ico
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/javascript/mathjax.js
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/stylesheets/extra.css
--rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/00-Introduction.ipynb
--rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/01-Metadata.ipynb
--rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/02-Catalog.ipynb
--rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/03-Horizons.ipynb
--rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/04-Waveforms.ipynb
--rw-r--r--   0        0        0  2744681 2020-02-02 00:00:00.000000 sxs-2023.1.0/docs/tutorials/05-PreprocessingForFFTs.ipynb
--rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/__version__.py
--rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/handlers.py
--rw-r--r--   0        0        0    39641 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/time_series.py
--rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/__init__.py
--rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/catalog.py
--rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/caltechdata/login.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/__init__.py
--rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/catalog.py
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/create.py
--rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/catalog/description.py
--rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/__init__.py
--rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/spec_horizons_h5.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/horizons/xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/metadata/__init__.py
--rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/metadata/metadata.py
--rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/__init__.py
--rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/bitwise.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/dicts.py
--rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/downloads.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/files.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/formats.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/inspire.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/monotonicity.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/pretty_print.py
--rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/select.py
--rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/smooth_functions.py
--rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/sxs_directories.py
--rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/sxs_identifiers.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/url.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/__init__.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/greedy_spline.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/linear_bisection.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/peak_greed.py
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/decimation/suppression.py
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/__init__.py
--rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/comparisons.py
--rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/conversion.py
--rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/dataset.py
--rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/horizons.py
--rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/metadata.py
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/waveform_amp_phase.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/lvcnr/waveforms.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/__init__.py
--rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/ads.py
--rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/arxiv.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/fairchild_report.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/inspire.py
--rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/journal_abbreviations.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/utilities/references/references.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/__init__.py
--rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/alignment.py
--rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/memory.py
--rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/mode_utilities.py
--rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/transformations.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_grid.py
--rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_mixin.py
--rw-r--r--   0        0        0    56594 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_modes.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/waveform_signal.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/__init__.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/lvc.py
--rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/nrar.py
--rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
--rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
--rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/waveforms/format_handlers/spectre_cce_v1.py
--rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/__init__.py
--rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/catalog.py
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/creators.py
--rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/simannex.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/surrogatemodeling.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/__init__.py
--rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/deposit.py
--rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/login.py
--rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.1.0/sxs/zenodo/api/records.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/__init__.py
--rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_catalog.py
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_horizons.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_loader.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_metadata.py
--rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_time_series.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_transformations.py
--rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_utilities.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_waveform_rotations.py
--rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.1.0/tests/test_waveforms.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.1.0/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.1.0/LICENSE
--rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 sxs-2023.1.0/README.md
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 sxs-2023.1.0/pyproject.toml
--rw-r--r--   0        0        0     9329 2020-02-02 00:00:00.000000 sxs-2023.1.0/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 sxs-2023.1.1/.codecov.yml
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 sxs-2023.1.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 sxs-2023.1.1/CITATION.cff
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 sxs-2023.1.1/juliapkg.json
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 sxs-2023.1.1/mkdocs.yml
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 sxs-2023.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 sxs-2023.1.1/.github/scripts/parse_bump_rule.py
+-rw-r--r--   0        0        0     6519 2020-02-02 00:00:00.000000 sxs-2023.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 sxs-2023.1.1/.github/workflows/pr_rtd_link.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/index.md -> ../README.md
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/mathematica.md
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/catalog.md
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/horizons.md
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/load.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/metadata.md
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/time_series.md
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/api/waveforms.md
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/html/main.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/images/favicon.ico
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/javascript/mathjax.js
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0   415059 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/00-Introduction.ipynb
+-rw-r--r--   0        0        0    14108 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/01-Metadata.ipynb
+-rw-r--r--   0        0        0  4116002 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/02-Catalog.ipynb
+-rw-r--r--   0        0        0  1366385 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/03-Horizons.ipynb
+-rw-r--r--   0        0        0  6774633 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/04-Waveforms.ipynb
+-rw-r--r--   0        0        0  2744774 2020-02-02 00:00:00.000000 sxs-2023.1.1/docs/tutorials/05-PreprocessingForFFTs.ipynb
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/__version__.py
+-rw-r--r--   0        0        0    20929 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/handlers.py
+-rw-r--r--   0        0        0    39641 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/time_series.py
+-rw-r--r--   0        0        0    14761 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/caltechdata/__init__.py
+-rw-r--r--   0        0        0     4914 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/caltechdata/catalog.py
+-rw-r--r--   0        0        0    21546 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/caltechdata/login.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/catalog/__init__.py
+-rw-r--r--   0        0        0    26481 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/catalog/catalog.py
+-rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/catalog/create.py
+-rw-r--r--   0        0        0    10830 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/catalog/description.py
+-rw-r--r--   0        0        0    16265 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/horizons/__init__.py
+-rw-r--r--   0        0        0     3642 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/horizons/spec_horizons_h5.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/horizons/xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/julia/__init__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/metadata/__init__.py
+-rw-r--r--   0        0        0    27679 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/metadata/metadata.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/__init__.py
+-rw-r--r--   0        0        0    13205 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/bitwise.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/dicts.py
+-rw-r--r--   0        0        0     4488 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/downloads.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/files.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/formats.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/inspire.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/monotonicity.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/pretty_print.py
+-rw-r--r--   0        0        0     6727 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/select.py
+-rw-r--r--   0        0        0     9077 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/smooth_functions.py
+-rw-r--r--   0        0        0     9676 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/sxs_directories.py
+-rw-r--r--   0        0        0     3339 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/sxs_identifiers.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/url.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/decimation/__init__.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/decimation/greedy_spline.py
+-rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/decimation/linear_bisection.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/decimation/peak_greed.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/decimation/suppression.py
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/__init__.py
+-rw-r--r--   0        0        0    12386 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/comparisons.py
+-rw-r--r--   0        0        0    12083 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/conversion.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/dataset.py
+-rw-r--r--   0        0        0    10447 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/horizons.py
+-rw-r--r--   0        0        0    12385 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/metadata.py
+-rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/waveform_amp_phase.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/lvcnr/waveforms.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/__init__.py
+-rw-r--r--   0        0        0     8591 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/ads.py
+-rw-r--r--   0        0        0     4250 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/arxiv.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/fairchild_report.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/inspire.py
+-rw-r--r--   0        0        0    31018 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/journal_abbreviations.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/utilities/references/references.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/__init__.py
+-rw-r--r--   0        0        0    12418 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/alignment.py
+-rw-r--r--   0        0        0     7763 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/memory.py
+-rw-r--r--   0        0        0     5253 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/mode_utilities.py
+-rw-r--r--   0        0        0     9124 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/transformations.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/waveform_grid.py
+-rw-r--r--   0        0        0     1179 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/waveform_mixin.py
+-rw-r--r--   0        0        0    56594 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/waveform_modes.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/waveform_signal.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/__init__.py
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/lvc.py
+-rw-r--r--   0        0        0    20431 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/nrar.py
+-rw-r--r--   0        0        0    27340 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     2348 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py
+-rw-r--r--   0        0        0     3929 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/waveforms/format_handlers/spectre_cce_v1.py
+-rw-r--r--   0        0        0    25890 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/__init__.py
+-rw-r--r--   0        0        0    28737 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/catalog.py
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/creators.py
+-rw-r--r--   0        0        0     4491 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/simannex.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/surrogatemodeling.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/api/__init__.py
+-rw-r--r--   0        0        0    36946 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/api/deposit.py
+-rw-r--r--   0        0        0    18007 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/api/login.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 sxs-2023.1.1/sxs/zenodo/api/records.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     9273 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_catalog.py
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_horizons.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_loader.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_metadata.py
+-rw-r--r--   0        0        0    13883 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_time_series.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_transformations.py
+-rw-r--r--   0        0        0    18128 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_utilities.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_waveform_rotations.py
+-rw-r--r--   0        0        0    11597 2020-02-02 00:00:00.000000 sxs-2023.1.1/tests/test_waveforms.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 sxs-2023.1.1/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 sxs-2023.1.1/LICENSE
+-rw-r--r--   0        0        0     5859 2020-02-02 00:00:00.000000 sxs-2023.1.1/README.md
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 sxs-2023.1.1/pyproject.toml
+-rw-r--r--   0        0        0     9362 2020-02-02 00:00:00.000000 sxs-2023.1.1/PKG-INFO
```

### Comparing `sxs-2023.1.0/mkdocs.yml` & `sxs-2023.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/.github/workflows/build.yml` & `sxs-2023.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/mathematica.md` & `sxs-2023.1.1/docs/mathematica.md`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/images/favicon.ico` & `sxs-2023.1.1/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/00-Introduction.ipynb` & `sxs-2023.1.1/docs/tutorials/00-Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/01-Metadata.ipynb` & `sxs-2023.1.1/docs/tutorials/01-Metadata.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/02-Catalog.ipynb` & `sxs-2023.1.1/docs/tutorials/02-Catalog.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/03-Horizons.ipynb` & `sxs-2023.1.1/docs/tutorials/03-Horizons.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/04-Waveforms.ipynb` & `sxs-2023.1.1/docs/tutorials/04-Waveforms.ipynb`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/docs/tutorials/05-PreprocessingForFFTs.ipynb` & `sxs-2023.1.1/docs/tutorials/05-PreprocessingForFFTs.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9967757936507937%*

 * *Differences: {"'cells'": "{20: {'source': ['The pre-processed signal may look pretty strange, but it has two "*

 * *            '*very* important features: the signal is periodic, and the signal is smooth.  As '*

 * *            'explained in [the paper](https://arxiv.org/abs/2405.06197), this results in '*

 * *            'frequency-domain data that more accurately reflects the true physical signal.  But '*

 * *            "these features would not be present with standard signal-processing techniques.']}}",*

 * * "'metadata'": "{'language_inf […]*

```diff
@@ -409,15 +409,15 @@
                 "plt.legend();"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "The pre-processed signal may look absurd, but it has two *very* important features: the signal is periodic, and the signal is smooth.  As explained in [the paper](https://arxiv.org/abs/2405.06197), this results in frequency-domain data that more accurately reflects the true physical signal."
+                "The pre-processed signal may look pretty strange, but it has two *very* important features: the signal is periodic, and the signal is smooth.  As explained in [the paper](https://arxiv.org/abs/2405.06197), this results in frequency-domain data that more accurately reflects the true physical signal.  But these features would not be present with standard signal-processing techniques."
             ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "notes",
             "language": "python",
@@ -429,13 +429,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.9"
+            "version": "3.11.8"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 2
 }
```

### Comparing `sxs-2023.1.0/sxs/__init__.py` & `sxs-2023.1.1/sxs/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/handlers.py` & `sxs-2023.1.1/sxs/handlers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/time_series.py` & `sxs-2023.1.1/sxs/time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/caltechdata/__init__.py` & `sxs-2023.1.1/sxs/caltechdata/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/caltechdata/catalog.py` & `sxs-2023.1.1/sxs/caltechdata/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/caltechdata/login.py` & `sxs-2023.1.1/sxs/caltechdata/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/catalog/catalog.py` & `sxs-2023.1.1/sxs/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/catalog/create.py` & `sxs-2023.1.1/sxs/catalog/create.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/catalog/description.py` & `sxs-2023.1.1/sxs/catalog/description.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/horizons/__init__.py` & `sxs-2023.1.1/sxs/horizons/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/horizons/spec_horizons_h5.py` & `sxs-2023.1.1/sxs/horizons/spec_horizons_h5.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/horizons/xor_multishuffle_bzip2.py` & `sxs-2023.1.1/sxs/horizons/xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/metadata/metadata.py` & `sxs-2023.1.1/sxs/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/__init__.py` & `sxs-2023.1.1/sxs/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/bitwise.py` & `sxs-2023.1.1/sxs/utilities/bitwise.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/dicts.py` & `sxs-2023.1.1/sxs/utilities/dicts.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/downloads.py` & `sxs-2023.1.1/sxs/utilities/downloads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/files.py` & `sxs-2023.1.1/sxs/utilities/files.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/formats.py` & `sxs-2023.1.1/sxs/utilities/formats.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/inspire.py` & `sxs-2023.1.1/sxs/utilities/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/monotonicity.py` & `sxs-2023.1.1/sxs/utilities/monotonicity.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/pretty_print.py` & `sxs-2023.1.1/sxs/utilities/pretty_print.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/select.py` & `sxs-2023.1.1/sxs/utilities/select.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/smooth_functions.py` & `sxs-2023.1.1/sxs/utilities/smooth_functions.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/sxs_directories.py` & `sxs-2023.1.1/sxs/utilities/sxs_directories.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/sxs_identifiers.py` & `sxs-2023.1.1/sxs/utilities/sxs_identifiers.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/url.py` & `sxs-2023.1.1/sxs/utilities/url.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/decimation/__init__.py` & `sxs-2023.1.1/sxs/utilities/decimation/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/decimation/greedy_spline.py` & `sxs-2023.1.1/sxs/utilities/decimation/greedy_spline.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/decimation/linear_bisection.py` & `sxs-2023.1.1/sxs/utilities/decimation/linear_bisection.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/decimation/peak_greed.py` & `sxs-2023.1.1/sxs/utilities/decimation/peak_greed.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/decimation/suppression.py` & `sxs-2023.1.1/sxs/utilities/decimation/suppression.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/__init__.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/comparisons.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/comparisons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/conversion.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/conversion.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/dataset.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/dataset.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/horizons.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/metadata.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/waveform_amp_phase.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/waveform_amp_phase.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/lvcnr/waveforms.py` & `sxs-2023.1.1/sxs/utilities/lvcnr/waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/references/ads.py` & `sxs-2023.1.1/sxs/utilities/references/ads.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/references/arxiv.py` & `sxs-2023.1.1/sxs/utilities/references/arxiv.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/references/fairchild_report.py` & `sxs-2023.1.1/sxs/utilities/references/fairchild_report.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/references/inspire.py` & `sxs-2023.1.1/sxs/utilities/references/inspire.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/utilities/references/journal_abbreviations.py` & `sxs-2023.1.1/sxs/utilities/references/journal_abbreviations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/__init__.py` & `sxs-2023.1.1/sxs/waveforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/alignment.py` & `sxs-2023.1.1/sxs/waveforms/alignment.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/memory.py` & `sxs-2023.1.1/sxs/waveforms/memory.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/mode_utilities.py` & `sxs-2023.1.1/sxs/waveforms/mode_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/transformations.py` & `sxs-2023.1.1/sxs/waveforms/transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/waveform_mixin.py` & `sxs-2023.1.1/sxs/waveforms/waveform_mixin.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/waveform_modes.py` & `sxs-2023.1.1/sxs/waveforms/waveform_modes.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/format_handlers/lvc.py` & `sxs-2023.1.1/sxs/waveforms/format_handlers/lvc.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/format_handlers/nrar.py` & `sxs-2023.1.1/sxs/waveforms/format_handlers/nrar.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py` & `sxs-2023.1.1/sxs/waveforms/format_handlers/rotating_paired_diff_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py` & `sxs-2023.1.1/sxs/waveforms/format_handlers/rotating_paired_xor_multishuffle_bzip2.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/waveforms/format_handlers/spectre_cce_v1.py` & `sxs-2023.1.1/sxs/waveforms/format_handlers/spectre_cce_v1.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/__init__.py` & `sxs-2023.1.1/sxs/zenodo/__init__.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/catalog.py` & `sxs-2023.1.1/sxs/zenodo/catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/creators.py` & `sxs-2023.1.1/sxs/zenodo/creators.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/simannex.py` & `sxs-2023.1.1/sxs/zenodo/simannex.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/surrogatemodeling.py` & `sxs-2023.1.1/sxs/zenodo/surrogatemodeling.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/api/deposit.py` & `sxs-2023.1.1/sxs/zenodo/api/deposit.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/api/login.py` & `sxs-2023.1.1/sxs/zenodo/api/login.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/sxs/zenodo/api/records.py` & `sxs-2023.1.1/sxs/zenodo/api/records.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/conftest.py` & `sxs-2023.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_catalog.py` & `sxs-2023.1.1/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_horizons.py` & `sxs-2023.1.1/tests/test_horizons.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_loader.py` & `sxs-2023.1.1/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_metadata.py` & `sxs-2023.1.1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_time_series.py` & `sxs-2023.1.1/tests/test_time_series.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_transformations.py` & `sxs-2023.1.1/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_utilities.py` & `sxs-2023.1.1/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_waveform_rotations.py` & `sxs-2023.1.1/tests/test_waveform_rotations.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/tests/test_waveforms.py` & `sxs-2023.1.1/tests/test_waveforms.py`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/.gitignore` & `sxs-2023.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/LICENSE` & `sxs-2023.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/README.md` & `sxs-2023.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sxs-2023.1.0/pyproject.toml` & `sxs-2023.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,16 @@
   "spherical >=1.0",
   "h5py >=3",
   "inflection >=0.5.1",
   "requests >=2.24.0",
   "tqdm >=4.63.1",
   "pytz >=2020.1",
   "urllib3 >=1.25.10",
-  "pandas >=1.1.2"
+  "pandas >=1.1.2",
+  "juliacall >=0.9.20"
 ]
 
 [project.optional-dependencies]
 docs = [
   "mkdocs",
   "mkdocstrings-python",
   "mkdocs-material",
@@ -69,15 +70,16 @@
 [tool.hatch.version]
 path = "sxs/__version__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
-  "pytest-forked >=1.3.0"
+  "pytest-forked >=1.3.0",
+  "juliapkg >=0.1.13"
 ]
 [tool.hatch.envs.default.scripts]
 # Run these as `hatch run test`
 test = "pytest {args:tests}"
 
 [tool.hatch.envs.docs]
 dependencies = [
```

### Comparing `sxs-2023.1.0/PKG-INFO` & `sxs-2023.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sxs
-Version: 2023.1.0
+Version: 2023.1.1
 Summary: Interface to data produced by the Simulating eXtreme Spacetimes collaboration
 Project-URL: Homepage, https://github.com/sxs-collaboration/sxs
 Project-URL: Documentation, https://sxs.readthedocs.io/
 Author-email: Michael Boyle <michael.oliver.boyle@gmail.com>
 License: The MIT License (MIT)
         
         Copyright (c) 2020 Michael Boyle
@@ -33,14 +33,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Requires-Dist: h5py>=3
 Requires-Dist: inflection>=0.5.1
+Requires-Dist: juliacall>=0.9.20
 Requires-Dist: numba>=0.55; implementation_name == 'cpython'
 Requires-Dist: numpy>=1.20
 Requires-Dist: pandas>=1.1.2
 Requires-Dist: pytz>=2020.1
 Requires-Dist: quaternionic>=1.0
 Requires-Dist: requests>=2.24.0
 Requires-Dist: scipy>=1.0
```

