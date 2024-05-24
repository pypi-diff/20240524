# Comparing `tmp/fermo_core-0.1.0.tar.gz` & `tmp/fermo_core-0.1.1.tar.gz`

## Comparing `fermo_core-0.1.0.tar` & `fermo_core-0.1.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 fermo_core-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/__init__.py
--rw-r--r--   0        0        0     3537 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/config/__init__.py
--rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/config/class_default_settings.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/config/class_logger.py
--rw-r--r--   0        0        0    43465 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/config/schema.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/__init__.py
--rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/class_analysis_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/__init__.py
--rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
--rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
--rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
--rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
--rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
--rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/blank_assigner/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
--rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/feature_filter/__init__.py
--rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/group_assigner/__init__.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/group_factor_assigner/__init__.py
--rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/__init__.py
--rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
--rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
--rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
--rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/score_assigner/__init__.py
--rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/__init__.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
--rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/__init__.py
--rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/class_repository.py
--rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/class_stats.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_feature/__init__.py
--rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_feature_builder.py
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py
--rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
--rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_feature/dataclass_feature.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_sample/__init__.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_sample/class_sample_builder.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_sample/class_samples_director.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/builder_sample/dataclass_sample.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/__init__.py
--rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/class_general_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
--rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/msms_parser/__init__.py
--rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/peaktable_parser/__init__.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/phenotype_parser/__init__.py
--rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/spec_library_parser/__init__.py
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/__init__.py
--rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/additional_module_parameter_managers.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_argparse_manager.py
--rw-r--r--   0        0        0    21122 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_export_manager.py
--rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_file_manager.py
--rw-r--r--   0        0        0    37024 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_parameter_manager.py
--rw-r--r--   0        0        0    20151 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_summary_writer.py
--rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/class_validation_manager.py
--rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/core_module_parameter_managers.py
--rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/input_file_parameter_managers.py
--rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/input_output/output_file_parameter_managers.py
--rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_other_neg.csv
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_other_pos.csv
--rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv
--rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
--rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
--rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/mibig/mibig_cds_count.csv
--rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/ms2deepscore/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/ms2query/neg/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/libraries/ms2query/pos/.placeholder
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/utils/__init__.py
--rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.1.0/fermo_core/utils/utility_method_manager.py
--rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.1.0/.gitignore
--rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.1.0/LICENSE
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 fermo_core-0.1.0/README.md
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5462 2020-02-02 00:00:00.000000 fermo_core-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 fermo_core-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/__init__.py
+-rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/__init__.py
+-rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/class_default_settings.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/class_logger.py
+-rw-r--r--   0        0        0    43465 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/config/schema.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/__init__.py
+-rw-r--r--   0        0        0    10888 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/class_analysis_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/__init__.py
+-rw-r--r--   0        0        0    51559 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py
+-rw-r--r--   0        0        0    20380 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py
+-rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py
+-rw-r--r--   0        0        0    11491 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py
+-rw-r--r--   0        0        0    11818 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py
+-rw-r--r--   0        0        0    11588 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py
+-rw-r--r--   0        0        0    12857 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/__init__.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/__init__.py
+-rw-r--r--   0        0        0     6172 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/__init__.py
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/__init__.py
+-rw-r--r--   0        0        0     7275 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py
+-rw-r--r--   0        0        0     6681 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py
+-rw-r--r--   0        0        0     6605 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py
+-rw-r--r--   0        0        0     7113 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/__init__.py
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/__init__.py
+-rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py
+-rw-r--r--   0        0        0    13360 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/__init__.py
+-rw-r--r--   0        0        0     3967 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/class_repository.py
+-rw-r--r--   0        0        0     9501 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/class_stats.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/__init__.py
+-rw-r--r--   0        0        0     7026 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_feature_builder.py
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py
+-rw-r--r--   0        0        0    15027 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_feature/dataclass_feature.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/__init__.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_sample_builder.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_samples_director.py
+-rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/builder_sample/dataclass_sample.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/__init__.py
+-rw-r--r--   0        0        0     8797 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/class_general_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/__init__.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/__init__.py
+-rw-r--r--   0        0        0     3849 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/__init__.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/__init__.py
+-rw-r--r--   0        0        0     5447 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/__init__.py
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/__init__.py
+-rw-r--r--   0        0        0    20480 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/additional_module_parameter_managers.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_argparse_manager.py
+-rw-r--r--   0        0        0    21122 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_export_manager.py
+-rw-r--r--   0        0        0     2243 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_file_manager.py
+-rw-r--r--   0        0        0    37024 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_parameter_manager.py
+-rw-r--r--   0        0        0    20289 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_summary_writer.py
+-rw-r--r--   0        0        0    15453 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/class_validation_manager.py
+-rw-r--r--   0        0        0     7717 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/core_module_parameter_managers.py
+-rw-r--r--   0        0        0    11622 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/input_file_parameter_managers.py
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/input_output/output_file_parameter_managers.py
+-rw-r--r--   0        0        0    11013 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_neg.csv
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_pos.csv
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv
+-rw-r--r--   0        0        0    14072 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv
+-rw-r--r--   0        0        0    34102 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/mibig/mibig_cds_count.csv
+-rw-r--r--   0        0        0  2878179 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2deepscore/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2query/neg/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/libraries/ms2query/pos/.placeholder
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/utils/__init__.py
+-rw-r--r--   0        0        0    12500 2020-02-02 00:00:00.000000 fermo_core-0.1.1/fermo_core/utils/utility_method_manager.py
+-rw-r--r--   0        0        0     3685 2020-02-02 00:00:00.000000 fermo_core-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fermo_core-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 fermo_core-0.1.1/README.md
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 fermo_core-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6000 2020-02-02 00:00:00.000000 fermo_core-0.1.1/PKG-INFO
```

### Comparing `fermo_core-0.1.0/fermo_core/main.py` & `fermo_core-0.1.1/fermo_core/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
-import platform
+import logging
 import sys
 from datetime import datetime
 from importlib import metadata
 
 from fermo_core.config.class_logger import LoggerSetup
 from fermo_core.data_analysis.class_analysis_manager import AnalysisManager
 from fermo_core.data_processing.parser.class_general_parser import GeneralParser
@@ -62,26 +62,45 @@
     )
     export_manager.run(metadata.version("fermo_core"), starttime)
 
     logger.info("'main': completed all steps - DONE")
     sys.exit(0)
 
 
+def set_log_verboseness_console(logger: logging.Logger, level: str):
+    """Adjust logging settings based on user input
+
+    Attributes:
+        logger: the previously initialized logger
+        level: the logging level
+    """
+    for handler in logger.handlers:
+        if isinstance(handler, logging.StreamHandler) and not isinstance(
+            handler, logging.FileHandler
+        ):
+            if level in ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]:
+                logger.info(f"'LoggerSetup': set verboseness level to '{level}'.")
+                handler.setLevel(getattr(logging, level))
+            else:
+                logger.warning(
+                    "'LoggerSetup': verboseness level invalid. Fall back to level "
+                    "'INFO'."
+                )
+                handler.setLevel(logging.INFO)
+
+
 def main_cli():
     """Interface for installer."""
     start_time = datetime.now()
-    logger.debug(
-        f"Python version: {platform.python_version()}; "
-        f"System: {platform.system()}; "
-        f"System version: {platform.version()};"
-        f"System architecture: {platform.python_version()}"
-    )
-    logger.info(f"Started 'fermo_core' v'{metadata.version('fermo_core')}' as CLI.")
     args = ArgparseManager().run_argparse(metadata.version("fermo_core"), sys.argv[1:])
 
+    set_log_verboseness_console(logger, args.verboseness)
+    logger.info(f"Started 'fermo_core' v'{metadata.version('fermo_core')}' as CLI.")
+    LoggerSetup.log_system_settings(logger)
+
     user_input = FileManager.load_json_file(args.parameters)
     ValidationManager().validate_file_vs_jsonschema(user_input, args.parameters)
 
     param_manager = ParameterManager()
     param_manager.assign_parameters_cli(user_input)
 
     main(param_manager, start_time)
```

### Comparing `fermo_core-0.1.0/fermo_core/config/class_default_settings.py` & `fermo_core-0.1.1/fermo_core/config/class_default_settings.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/config/class_logger.py` & `fermo_core-0.1.1/fermo_core/config/class_logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 import logging
+import platform
 import sys
 from pathlib import Path
 
 import coloredlogs
 
 
 class LoggerSetup:
@@ -62,7 +63,21 @@
         )
         file_handler.setFormatter(file_formatter)
 
         logger.addHandler(console_handler)
         logger.addHandler(file_handler)
 
         return logger
+
+    @staticmethod
+    def log_system_settings(logger: logging.Logger):
+        """Log the system settings
+
+        Attributes:
+            logger: the previously initialized logger
+        """
+        logger.debug(
+            f"Python version: {platform.python_version()}; "
+            f"System: {platform.system()}; "
+            f"System version: {platform.version()};"
+            f"System architecture: {platform.python_version()}"
+        )
```

### Comparing `fermo_core-0.1.0/fermo_core/config/schema.json` & `fermo_core-0.1.1/fermo_core/config/schema.json`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/class_analysis_manager.py` & `fermo_core-0.1.1/fermo_core/data_analysis/class_analysis_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_adduct_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_annotation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_fragment_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_mod_cos_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2deepscore_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_ms2query_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/annotation_manager/class_neutral_loss_annotator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/blank_assigner/class_blank_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py` & `fermo_core-0.1.1/fermo_core/data_analysis/chrom_trace_calculator/class_chrom_trace_calculator.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/feature_filter/class_feature_filter.py` & `fermo_core-0.1.1/fermo_core/data_analysis/feature_filter/class_feature_filter.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/group_assigner/class_group_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/group_assigner/class_group_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/group_factor_assigner/class_group_factor_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_qual_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_conc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phen_quant_perc_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py` & `fermo_core-0.1.1/fermo_core/data_analysis/phenotype_manager/class_phenotype_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/score_assigner/class_score_assigner.py` & `fermo_core-0.1.1/fermo_core/data_analysis/score_assigner/class_score_assigner.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py` & `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_mod_cosine_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py` & `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_ms2deepscore_networker.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py` & `fermo_core-0.1.1/fermo_core/data_analysis/sim_networks_manager/class_sim_networks_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/class_repository.py` & `fermo_core-0.1.1/fermo_core/data_processing/class_repository.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/class_stats.py` & `fermo_core-0.1.1/fermo_core/data_processing/class_stats.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_feature_builder.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_feature_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_general_feature_director.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_general_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_feature/class_specific_feature_director.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/class_specific_feature_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_feature/dataclass_feature.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_feature/dataclass_feature.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_sample/class_sample_builder.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_sample_builder.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_sample/class_samples_director.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/class_samples_director.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/builder_sample/dataclass_sample.py` & `fermo_core-0.1.1/fermo_core/data_processing/builder_sample/dataclass_sample.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/class_general_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/class_general_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/group_metadata_parser/class_fermo_metadata_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/msms_parser/class_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/abc_peaktable_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/peaktable_parser/class_mzmine3_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/phenotype_parser/class_phenotype_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py` & `fermo_core-0.1.1/fermo_core/data_processing/parser/spec_library_parser/class_spec_lib_mgf_parser.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/additional_module_parameter_managers.py` & `fermo_core-0.1.1/fermo_core/input_output/additional_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_argparse_manager.py` & `fermo_core-0.1.1/fermo_core/input_output/class_argparse_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,29 +47,40 @@
 
         Returns:
             argparse object containing command line options.
         """
         parser = argparse.ArgumentParser(
             description=(
                 "#####################################################\n"
+                "\n"
                 f"fermo_core v{version}: command line interface of FERMO.\n"
+                "\n"
                 "#####################################################\n"
-                "Focused on large-scale data processing by advanced users.\n"
-                "For a more user-friendly experience, see fermo.bioinformatics.nl.\n"
-                "More info on usage can be found in the README, docs, or publication.\n"
+                "For detailed information on usage, see the README and Documentation.\n"
+                "See fermo.bioinformatics.nl for a GUI version.\n"
                 "#####################################################\n"
             ),
             formatter_class=argparse.RawTextHelpFormatter,
         )
 
         parser.add_argument(
             "-p",
             "--parameters",
             type=str,
             required=True,
             help=(
-                "Provide a FERMO parameter .json file.\n"
-                "See 'example_data/case_study_parameters.json' for an example or "
-                "consult the documentation.\n"
+                "(Mandatory) Provide a FERMO parameter .json file.\n"
+                "For more information, consult the documentation.\n"
             ),
         )
+
+        parser.add_argument(
+            "-v",
+            "--verboseness",
+            type=str,
+            default="INFO",
+            choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
+            required=False,
+            help=("(Optional) Specify the verboseness of logging. Default: 'INFO'."),
+        )
+
         return parser
```

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_export_manager.py` & `fermo_core-0.1.1/fermo_core/input_output/class_export_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_file_manager.py` & `fermo_core-0.1.1/fermo_core/input_output/class_file_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_parameter_manager.py` & `fermo_core-0.1.1/fermo_core/input_output/class_parameter_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_summary_writer.py` & `fermo_core-0.1.1/fermo_core/input_output/class_summary_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,20 +60,22 @@
             )
 
     def summarize_msmsparameters(self: Self):
         if self.params.MsmsParameters is not None:
             self.summary.append(
                 f"MS/MS fragmentation information was parsed from the file "
                 f"'{self.params.MsmsParameters.filepath.name}' in the format "
-                f"'{self.params.MsmsParameters.format}'."
+                f"'{self.params.MsmsParameters.format}'. "
+                f"MS/MS fragments +- 10 mass units around precursor m/z were removed."
             )
             if self.params.MsmsParameters.rel_int_from > 0:
                 self.summary.append(
                     f"MS/MS fragments with an intensity less than "
-                    f"'{self.params.MsmsParameters.rel_int_from}' were removed."
+                    f"'{self.params.MsmsParameters.rel_int_from}' relative to the "
+                    f"base peak were removed."
                 )
 
     def summarize_phenotypeparameters(self: Self):
         if self.params.PhenotypeParameters is not None:
             self.summary.append(
                 f"Phenotype/bioactivity information was parsed from the file "
                 f"'{self.params.PhenotypeParameters.filepath.name}' in the format "
```

### Comparing `fermo_core-0.1.0/fermo_core/input_output/class_validation_manager.py` & `fermo_core-0.1.1/fermo_core/input_output/class_validation_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/core_module_parameter_managers.py` & `fermo_core-0.1.1/fermo_core/input_output/core_module_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/input_file_parameter_managers.py` & `fermo_core-0.1.1/fermo_core/input_output/input_file_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/input_output/output_file_parameter_managers.py` & `fermo_core-0.1.1/fermo_core/input_output/output_file_parameter_managers.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv` & `fermo_core-0.1.1/fermo_core/libraries/frag_libs/aa_m+h_fragment_series.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_bio_pos.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_bio_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_other_neg.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_neg.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/generic_other_pos.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/generic_other_pos.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_glycosides.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_glycosides.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_nonribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/loss_libs/kersten_ribosomal.csv` & `fermo_core-0.1.1/fermo_core/libraries/loss_libs/kersten_ribosomal.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/mibig/mibig_cds_count.csv` & `fermo_core-0.1.1/fermo_core/libraries/mibig/mibig_cds_count.csv`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf` & `fermo_core-0.1.1/fermo_core/libraries/mibig/pos/mibig_in_silico_spectral_library_3_1.mgf`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/fermo_core/utils/utility_method_manager.py` & `fermo_core-0.1.1/fermo_core/utils/utility_method_manager.py`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/.gitignore` & `fermo_core-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/LICENSE` & `fermo_core-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fermo_core-0.1.0/README.md` & `fermo_core-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,59 @@
 fermo_core
 =========
-`fermo_core` is a Python-based command line tool to process, analyze, and prioritize compounds from metabolomics data. While primarily intended to be the backend processing module of `fermo_gui` of the application FERMO, `fermo_core` can be used independently for large-scale data processing and analysis. This README specifies the use of `fermo_core` as command line interface. 
 
-For a more user-friendly version, see the [FERMO online](https://fermo.bioinformatics.nl). Please also consult the [Documentation](https://mmzdouc.github.io/fermo_docs/).
+[![DOI](https://zenodo.org/badge/671395100.svg)](https://zenodo.org/doi/10.5281/zenodo.11259126) [![PyPI version](https://badge.fury.io/py/fermo_core.svg)](https://badge.fury.io/py/fermo_core)
+
+`fermo_core` is a Python-based command line tool to process, analyze, and prioritize compounds from metabolomics data. While primarily intended to be the backend processing module of `fermo_gui` of the application FERMO, `fermo_core` can be used independently for large-scale data processing and analysis. 
+
+This README specifies the use of `fermo_core` as command line interface. For a more user-friendly version, see the [FERMO online](https://fermo.bioinformatics.nl). Please also consult the [Documentation](https://mmzdouc.github.io/fermo_docs/).
+
 
 Table of Contents
 -----------------
 - [Installation](#installation)
 - [Quick Start](#quick-start)
 - [Usage](#usage)
 - [Attribution](#attribution)
 - [Contributing](#contributing)
 
 ## Installation
 
-### With `hatch`
+### With `pip` from PyPI
+- Install `python 3.11.x`
+- Create a virtual environment (e.g. venv, conda) and activate it
+- Run `pip install fermo_core`
+- Once installed, run as specified in [Run with `pip`](#run-with-pip)
+
+### With `hatch` from GitHub
 - Install `python 3.11.x`
 - Install hatch (e.g. with `pipx install hatch`)
 - Download or clone the [repository](https://github.com/mmzdouc/fermo_core)
 - (Change into the fermo_core base directory if not already present)
 - Run `hatch -v env create`
-- Once installed, run as specified in [Quick Start](#quick-start)
+- Once installed, run as specified in [Run with `hatch`](#run-with-hatch)
 
-### With `conda`
+### With `conda` from GitHub
 - Install conda (e.g. miniconda)
 - Create a conda environment with `conda create --name fermo_core python=3.11`
 - Activate the conda environment with `conda activate fermo_core`
 - Download or clone the [repository](https://github.com/mmzdouc/fermo_core)
 - (Change into the fermo_core base directory if not already present)
 - Run `pip install -e .`
-- Once installed, run as specified in [Quick Start](#quick-start)
+- Once installed, run as specified in [Run with `conda`](#run-with-conda)
 
 ## Quick Start
 
-### With `hatch`:
+### Run with `pip`
+- `fermo_core --parameters <your_parameter_file.json>`
+
+### Run with `hatch`:
 - `hatch run fermo_core --parameters <your_parameter_file.json>`
 
-### With `conda`:
+### Run with `conda`:
 - `python fermo_core/main.py --parameters <your_parameter_file.json>`
 
 ## Usage
 
 `fermo_core` can be used both as a command line interface as well as a library.
 
 All parameters and input data are specified in a `parameters.json` file be formatted following the schema specified in `fermo_core/config/schema.json`. See the example in `example_data/case_study_parameters.json` and/or consult the [Documentation](https://mmzdouc.github.io/fermo_docs/home/core.parameters/).
```

### Comparing `fermo_core-0.1.0/pyproject.toml` & `fermo_core-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fermo_core"
-version = "0.1.0"
+version = "0.1.1"
 description = "Data processing/analysis functionality of metabolomics dashboard FERMO"
 readme = "README.md"
 requires-python = ">=3.11,<3.12"
 license-files = { paths = ["LICENSE"] }
 authors = [
     { name = "Mitja M. Zdouc", email = "zdoucmm@gmail.com" }
 ]
```

### Comparing `fermo_core-0.1.0/PKG-INFO` & `fermo_core-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fermo_core
-Version: 0.1.0
+Version: 0.1.1
 Summary: Data processing/analysis functionality of metabolomics dashboard FERMO
 Project-URL: Website, https://fermo.bioinformatics.nl/
 Project-URL: Repository, https://github.com/mmzdouc/fermo_core
 Project-URL: Documentation, https://mmzdouc.github.io/fermo_docs/
 Author-email: "Mitja M. Zdouc" <zdoucmm@gmail.com>
 License-File: LICENSE
 Keywords: cheminformatics,genomics,metabolomics
@@ -33,51 +33,64 @@
 Requires-Dist: pytest-cov~=4.1.0; extra == 'dev'
 Requires-Dist: pytest~=7.4.2; extra == 'dev'
 Requires-Dist: ruff~=0.4.4; extra == 'dev'
 Description-Content-Type: text/markdown
 
 fermo_core
 =========
-`fermo_core` is a Python-based command line tool to process, analyze, and prioritize compounds from metabolomics data. While primarily intended to be the backend processing module of `fermo_gui` of the application FERMO, `fermo_core` can be used independently for large-scale data processing and analysis. This README specifies the use of `fermo_core` as command line interface. 
 
-For a more user-friendly version, see the [FERMO online](https://fermo.bioinformatics.nl). Please also consult the [Documentation](https://mmzdouc.github.io/fermo_docs/).
+[![DOI](https://zenodo.org/badge/671395100.svg)](https://zenodo.org/doi/10.5281/zenodo.11259126) [![PyPI version](https://badge.fury.io/py/fermo_core.svg)](https://badge.fury.io/py/fermo_core)
+
+`fermo_core` is a Python-based command line tool to process, analyze, and prioritize compounds from metabolomics data. While primarily intended to be the backend processing module of `fermo_gui` of the application FERMO, `fermo_core` can be used independently for large-scale data processing and analysis. 
+
+This README specifies the use of `fermo_core` as command line interface. For a more user-friendly version, see the [FERMO online](https://fermo.bioinformatics.nl). Please also consult the [Documentation](https://mmzdouc.github.io/fermo_docs/).
+
 
 Table of Contents
 -----------------
 - [Installation](#installation)
 - [Quick Start](#quick-start)
 - [Usage](#usage)
 - [Attribution](#attribution)
 - [Contributing](#contributing)
 
 ## Installation
 
-### With `hatch`
+### With `pip` from PyPI
+- Install `python 3.11.x`
+- Create a virtual environment (e.g. venv, conda) and activate it
+- Run `pip install fermo_core`
+- Once installed, run as specified in [Run with `pip`](#run-with-pip)
+
+### With `hatch` from GitHub
 - Install `python 3.11.x`
 - Install hatch (e.g. with `pipx install hatch`)
 - Download or clone the [repository](https://github.com/mmzdouc/fermo_core)
 - (Change into the fermo_core base directory if not already present)
 - Run `hatch -v env create`
-- Once installed, run as specified in [Quick Start](#quick-start)
+- Once installed, run as specified in [Run with `hatch`](#run-with-hatch)
 
-### With `conda`
+### With `conda` from GitHub
 - Install conda (e.g. miniconda)
 - Create a conda environment with `conda create --name fermo_core python=3.11`
 - Activate the conda environment with `conda activate fermo_core`
 - Download or clone the [repository](https://github.com/mmzdouc/fermo_core)
 - (Change into the fermo_core base directory if not already present)
 - Run `pip install -e .`
-- Once installed, run as specified in [Quick Start](#quick-start)
+- Once installed, run as specified in [Run with `conda`](#run-with-conda)
 
 ## Quick Start
 
-### With `hatch`:
+### Run with `pip`
+- `fermo_core --parameters <your_parameter_file.json>`
+
+### Run with `hatch`:
 - `hatch run fermo_core --parameters <your_parameter_file.json>`
 
-### With `conda`:
+### Run with `conda`:
 - `python fermo_core/main.py --parameters <your_parameter_file.json>`
 
 ## Usage
 
 `fermo_core` can be used both as a command line interface as well as a library.
 
 All parameters and input data are specified in a `parameters.json` file be formatted following the schema specified in `fermo_core/config/schema.json`. See the example in `example_data/case_study_parameters.json` and/or consult the [Documentation](https://mmzdouc.github.io/fermo_docs/home/core.parameters/).
```

