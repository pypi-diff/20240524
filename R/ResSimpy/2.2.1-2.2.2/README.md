# Comparing `tmp/ressimpy-2.2.1.tar.gz` & `tmp/ressimpy-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ressimpy-2.2.1.tar", max compression
+gzip compressed data, was "ressimpy-2.2.2.tar", max compression
```

## Comparing `ressimpy-2.2.1.tar` & `ressimpy-2.2.2.tar`

### file list

```diff
@@ -1,197 +1,197 @@
--rw-r--r--   0        0        0     9156 2024-05-23 10:54:45.719512 ressimpy-2.2.1/LICENSE.MD
--rw-r--r--   0        0        0     5639 2024-05-23 10:54:45.719512 ressimpy-2.2.1/README.md
--rw-r--r--   0        0        0      618 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Aquifer.py
--rw-r--r--   0        0        0    10337 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Completion.py
--rw-r--r--   0        0        0     1496 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Constraint.py
--rw-r--r--   0        0        0     1908 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Constraints.py
--rw-r--r--   0        0        0     6134 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/DataObjectMixin.py
--rw-r--r--   0        0        0     4620 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/DynamicProperty.py
--rw-r--r--   0        0        0      358 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/FluidTypeEnums.py
--rw-r--r--   0        0        0      369 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/FrequencyEnum.py
--rw-r--r--   0        0        0      413 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/GridFunctionTypes.py
--rw-r--r--   0        0        0      168 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/HowEnum.py
--rw-r--r--   0        0        0      214 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/OutputType.py
--rw-r--r--   0        0        0      282 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/PenetrationDirectionEnum.py
--rw-r--r--   0        0        0      253 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/TimeSteppingMethodEnum.py
--rw-r--r--   0        0        0      507 2024-05-23 10:54:45.719512 ressimpy-2.2.1/ResSimpy/Enums/UnitsEnum.py
--rw-r--r--   0        0        0      377 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Enums/WellTypeEnum.py
--rw-r--r--   0        0        0       62 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Enums/__init__.py
--rw-r--r--   0        0        0      727 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Equilibration.py
--rw-r--r--   0        0        0     9413 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/File.py
--rw-r--r--   0        0        0     2262 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/FileBase.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/FileOperations/__init__.py
--rw-r--r--   0        0        0    23494 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/FileOperations/file_operations.py
--rw-r--r--   0        0        0      527 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Gaslift.py
--rw-r--r--   0        0        0     4872 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Grid.py
--rw-r--r--   0        0        0     1713 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/GridArrayFunction.py
--rw-r--r--   0        0        0      393 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Grids.py
--rw-r--r--   0        0        0      584 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Hydraulics.py
--rw-r--r--   0        0        0     3954 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/ISODateTime.py
--rw-r--r--   0        0        0     1443 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Network.py
--rw-r--r--   0        0        0      780 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/FcsConfig.py
--rw-r--r--   0        0        0    27826 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/FcsFile.py
--rw-r--r--   0        0        0    23250 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
--rw-r--r--   0        0        0    22153 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
--rw-r--r--   0        0        0     3386 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py
--rw-r--r--   0        0        0     6493 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
--rw-r--r--   0        0        0     6617 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
--rw-r--r--   0        0        0     6806 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
--rw-r--r--   0        0        0     4085 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py
--rw-r--r--   0        0        0     1286 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
--rw-r--r--   0        0        0     3742 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
--rw-r--r--   0        0        0     6914 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
--rw-r--r--   0        0        0     8652 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
--rw-r--r--   0        0        0     6891 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
--rw-r--r--   0        0        0     2367 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
--rw-r--r--   0        0        0     4496 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
--rw-r--r--   0        0        0     6153 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
--rw-r--r--   0        0        0     6251 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
--rw-r--r--   0        0        0     5980 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
--rw-r--r--   0        0        0      329 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     8755 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
--rw-r--r--   0        0        0    20340 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusCompletion.py
--rw-r--r--   0        0        0    11226 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
--rw-r--r--   0        0        0    33422 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusFile.py
--rw-r--r--   0        0        0     6641 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
--rw-r--r--   0        0        0    14067 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
--rw-r--r--   0        0        0    31597 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
--rw-r--r--   0        0        0     5635 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
--rw-r--r--   0        0        0    20084 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
--rw-r--r--   0        0        0     2715 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusReportingRequests.py
--rw-r--r--   0        0        0     9885 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py
--rw-r--r--   0        0        0     9571 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
--rw-r--r--   0        0        0    15023 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
--rw-r--r--   0        0        0     6523 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py
--rw-r--r--   0        0        0    11737 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
--rw-r--r--   0        0        0     9089 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWell.py
--rw-r--r--   0        0        0     1069 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWellList.py
--rw-r--r--   0        0        0     3043 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWellMod.py
--rw-r--r--   0        0        0    42644 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
--rw-r--r--   0        0        0      822 2024-05-23 10:54:45.723512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
--rw-r--r--   0        0        0       67 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
--rw-r--r--   0        0        0       77 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/DataModels/__init__.py
--rw-r--r--   0        0        0     3820 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusAquiferMethods.py
--rw-r--r--   0        0        0      381 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
--rw-r--r--   0        0        0      106 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusEnums/__init__.py
--rw-r--r--   0        0        0     3810 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusEquilMethods.py
--rw-r--r--   0        0        0     3769 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusGasliftMethods.py
--rw-r--r--   0        0        0       43 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusGrids.py
--rw-r--r--   0        0        0     3858 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusHydraulicsMethods.py
--rw-r--r--   0        0        0       47 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/__init__.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
--rw-r--r--   0        0        0      757 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
--rw-r--r--   0        0        0     1210 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
--rw-r--r--   0        0        0     1368 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
--rw-r--r--   0        0        0      170 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
--rw-r--r--   0        0        0     1159 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
--rw-r--r--   0        0        0     2658 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
--rw-r--r--   0        0        0      795 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
--rw-r--r--   0        0        0     5130 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
--rw-r--r--   0        0        0     2547 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
--rw-r--r--   0        0        0     1579 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
--rw-r--r--   0        0        0      896 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
--rw-r--r--   0        0        0     4957 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
--rw-r--r--   0        0        0      880 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
--rw-r--r--   0        0        0     3121 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
--rw-r--r--   0        0        0     4492 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
--rw-r--r--   0        0        0      306 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
--rw-r--r--   0        0        0      243 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/water_keywords.py
--rw-r--r--   0        0        0      902 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
--rw-r--r--   0        0        0    17362 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusNetwork.py
--rw-r--r--   0        0        0     3717 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusPVTMethods.py
--rw-r--r--   0        0        0     4005 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusRelPermMethods.py
--rw-r--r--   0        0        0    12838 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusReporting.py
--rw-r--r--   0        0        0     3771 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusRockMethods.py
--rw-r--r--   0        0        0     4140 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusSeparatorMethods.py
--rw-r--r--   0        0        0    39541 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusSimulator.py
--rw-r--r--   0        0        0    16873 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusSolverParameters.py
--rw-r--r--   0        0        0     3814 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusValveMethods.py
--rw-r--r--   0        0        0     3809 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusWaterMethods.py
--rw-r--r--   0        0        0    23826 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/NexusWells.py
--rw-r--r--   0        0        0      404 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/__init__.py
--rw-r--r--   0        0        0    23806 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/array_function_operations.py
--rw-r--r--   0        0        0      115 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/constants.py
--rw-r--r--   0        0        0    24849 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/load_wells.py
--rw-r--r--   0        0        0    14120 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/logfile_operations.py
--rw-r--r--   0        0        0    16640 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py
--rw-r--r--   0        0        0     8720 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_collect_tables.py
--rw-r--r--   0        0        0     7294 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_constraint_operations.py
--rw-r--r--   0        0        0    23454 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_file_operations.py
--rw-r--r--   0        0        0     4192 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_load_well_list.py
--rw-r--r--   0        0        0     2323 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_modify_object_in_file.py
--rw-r--r--   0        0        0     8133 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/nexus_remove_object_from_file.py
--rw-r--r--   0        0        0     5422 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/rel_perm_operations.py
--rw-r--r--   0        0        0    18539 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/runcontrol_operations.py
--rw-r--r--   0        0        0    20202 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nexus/structured_grid_operations.py
--rw-r--r--   0        0        0      620 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Node.py
--rw-r--r--   0        0        0      794 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/NodeConnection.py
--rw-r--r--   0        0        0      456 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/NodeConnections.py
--rw-r--r--   0        0        0      398 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/Nodes.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
--rw-r--r--   0        0        0     3041 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
--rw-r--r--   0        0        0     3090 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/__init__.py
--rw-r--r--   0        0        0      199 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/Enums/__init__.py
--rw-r--r--   0        0        0      640 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/Model_Parts/__init__.py
--rw-r--r--   0        0        0     2892 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.727512 ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
--rw-r--r--   0        0        0    11092 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
--rw-r--r--   0        0        0      462 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimWells.py
--rw-r--r--   0        0        0        0 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/OpenGoSim/__init__.py
--rw-r--r--   0        0        0     2561 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/OperationsMixin.py
--rw-r--r--   0        0        0      556 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/PVT.py
--rw-r--r--   0        0        0      581 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/RelPerm.py
--rw-r--r--   0        0        0     6301 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/RelPermEndPoint.py
--rw-r--r--   0        0        0     1624 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Reporting.py
--rw-r--r--   0        0        0      694 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Rock.py
--rw-r--r--   0        0        0      715 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Separator.py
--rw-r--r--   0        0        0     4512 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Simulator.py
--rw-r--r--   0        0        0      407 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/SolverParameter.py
--rw-r--r--   0        0        0      679 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/SolverParameters.py
--rw-r--r--   0        0        0     1260 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Target.py
--rw-r--r--   0        0        0      412 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Targets.py
--rw-r--r--   0        0        0     1223 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMapping.py
--rw-r--r--   0        0        0     2249 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
--rw-r--r--   0        0        0     8727 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
--rw-r--r--   0        0        0    17410 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
--rw-r--r--   0        0        0    31095 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
--rw-r--r--   0        0        0    15398 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
--rw-r--r--   0        0        0       96 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/__init__.py
--rw-r--r--   0        0        0    14870 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/Units.py
--rw-r--r--   0        0        0       45 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Units/__init__.py
--rw-r--r--   0        0        0       95 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/__init__.py
--rw-r--r--   0        0        0     2425 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/factory_methods.py
--rw-r--r--   0        0        0      365 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/general_utilities.py
--rw-r--r--   0        0        0     1955 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/generic_repr.py
--rw-r--r--   0        0        0     1585 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/invert_nexus_map.py
--rw-r--r--   0        0        0      453 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/obj_to_dataframe.py
--rw-r--r--   0        0        0     1364 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/obj_to_table_string.py
--rw-r--r--   0        0        0     2563 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Utils/to_dict_generic.py
--rw-r--r--   0        0        0      591 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Valve.py
--rw-r--r--   0        0        0      593 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Water.py
--rw-r--r--   0        0        0     5023 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Well.py
--rw-r--r--   0        0        0     1287 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/WellConnection.py
--rw-r--r--   0        0        0     1946 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/WellConnections.py
--rw-r--r--   0        0        0     1057 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/WellLists.py
--rw-r--r--   0        0        0      631 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Wellbore.py
--rw-r--r--   0        0        0      439 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Wellbores.py
--rw-r--r--   0        0        0      685 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Wellhead.py
--rw-r--r--   0        0        0      426 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Wellheads.py
--rw-r--r--   0        0        0     3244 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/Wells.py
--rw-r--r--   0        0        0      482 2024-05-23 10:54:56.583497 ressimpy-2.2.1/ResSimpy/__init__.py
--rw-r--r--   0        0        0     2751 2024-05-23 10:54:45.731512 ressimpy-2.2.1/ResSimpy/output_request.py
--rw-r--r--   0        0        0     2641 2024-05-23 10:54:56.579497 ressimpy-2.2.1/pyproject.toml
--rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 ressimpy-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9156 2024-05-24 13:57:24.194024 ressimpy-2.2.2/LICENSE.MD
+-rw-r--r--   0        0        0     5639 2024-05-24 13:57:24.194024 ressimpy-2.2.2/README.md
+-rw-r--r--   0        0        0      618 2024-05-24 13:57:24.194024 ressimpy-2.2.2/ResSimpy/Aquifer.py
+-rw-r--r--   0        0        0    10337 2024-05-24 13:57:24.194024 ressimpy-2.2.2/ResSimpy/Completion.py
+-rw-r--r--   0        0        0     1496 2024-05-24 13:57:24.194024 ressimpy-2.2.2/ResSimpy/Constraint.py
+-rw-r--r--   0        0        0     1908 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Constraints.py
+-rw-r--r--   0        0        0     6134 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/DataObjectMixin.py
+-rw-r--r--   0        0        0     4620 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/DynamicProperty.py
+-rw-r--r--   0        0        0      358 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/FluidTypeEnums.py
+-rw-r--r--   0        0        0      369 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/FrequencyEnum.py
+-rw-r--r--   0        0        0      413 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/GridFunctionTypes.py
+-rw-r--r--   0        0        0      168 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/HowEnum.py
+-rw-r--r--   0        0        0      214 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/OutputType.py
+-rw-r--r--   0        0        0      282 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/PenetrationDirectionEnum.py
+-rw-r--r--   0        0        0      253 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/TimeSteppingMethodEnum.py
+-rw-r--r--   0        0        0      507 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/UnitsEnum.py
+-rw-r--r--   0        0        0      377 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/WellTypeEnum.py
+-rw-r--r--   0        0        0       62 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Enums/__init__.py
+-rw-r--r--   0        0        0      727 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Equilibration.py
+-rw-r--r--   0        0        0     9413 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/File.py
+-rw-r--r--   0        0        0     2262 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/FileBase.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/FileOperations/__init__.py
+-rw-r--r--   0        0        0    23494 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/FileOperations/file_operations.py
+-rw-r--r--   0        0        0      527 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Gaslift.py
+-rw-r--r--   0        0        0     4872 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Grid.py
+-rw-r--r--   0        0        0     1713 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/GridArrayFunction.py
+-rw-r--r--   0        0        0      393 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Grids.py
+-rw-r--r--   0        0        0      584 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Hydraulics.py
+-rw-r--r--   0        0        0     3954 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/ISODateTime.py
+-rw-r--r--   0        0        0     1443 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Network.py
+-rw-r--r--   0        0        0      780 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/FcsConfig.py
+-rw-r--r--   0        0        0    27826 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/FcsFile.py
+-rw-r--r--   0        0        0    23250 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py
+-rw-r--r--   0        0        0    22250 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py
+-rw-r--r--   0        0        0     3386 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNode.py
+-rw-r--r--   0        0        0     6493 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py
+-rw-r--r--   0        0        0     6729 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py
+-rw-r--r--   0        0        0     6912 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodes.py
+-rw-r--r--   0        0        0     4085 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusProc.py
+-rw-r--r--   0        0        0     1286 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusProcs.py
+-rw-r--r--   0        0        0     3742 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusTarget.py
+-rw-r--r--   0        0        0     7022 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusTargets.py
+-rw-r--r--   0        0        0     8652 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py
+-rw-r--r--   0        0        0     7008 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py
+-rw-r--r--   0        0        0     2367 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py
+-rw-r--r--   0        0        0     4496 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py
+-rw-r--r--   0        0        0     6263 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py
+-rw-r--r--   0        0        0     6251 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py
+-rw-r--r--   0        0        0     6081 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py
+-rw-r--r--   0        0        0      329 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     8755 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py
+-rw-r--r--   0        0        0    20340 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusCompletion.py
+-rw-r--r--   0        0        0    11226 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusEquilMethod.py
+-rw-r--r--   0        0        0    33422 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusFile.py
+-rw-r--r--   0        0        0     6641 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py
+-rw-r--r--   0        0        0    14067 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py
+-rw-r--r--   0        0        0    31597 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusPVTMethod.py
+-rw-r--r--   0        0        0     5635 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py
+-rw-r--r--   0        0        0    20084 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py
+-rw-r--r--   0        0        0     2715 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusReportingRequests.py
+-rw-r--r--   0        0        0     9885 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRockMethod.py
+-rw-r--r--   0        0        0     9571 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py
+-rw-r--r--   0        0        0    15023 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusSolverParameter.py
+-rw-r--r--   0        0        0     6523 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusValveMethod.py
+-rw-r--r--   0        0        0    11737 2024-05-24 13:57:24.198024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWaterMethod.py
+-rw-r--r--   0        0        0     9089 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWell.py
+-rw-r--r--   0        0        0     1069 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWellList.py
+-rw-r--r--   0        0        0     3043 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWellMod.py
+-rw-r--r--   0        0        0    42644 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py
+-rw-r--r--   0        0        0      822 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py
+-rw-r--r--   0        0        0       67 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/StructuredGrid/__init__.py
+-rw-r--r--   0        0        0       77 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/DataModels/__init__.py
+-rw-r--r--   0        0        0     3820 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusAquiferMethods.py
+-rw-r--r--   0        0        0      381 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusEnums/DateFormatEnum.py
+-rw-r--r--   0        0        0      106 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusEnums/__init__.py
+-rw-r--r--   0        0        0     3810 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusEquilMethods.py
+-rw-r--r--   0        0        0     3769 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusGasliftMethods.py
+-rw-r--r--   0        0        0       43 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusGrids.py
+-rw-r--r--   0        0        0     3858 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusHydraulicsMethods.py
+-rw-r--r--   0        0        0       47 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/adsorption_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/alphaf_keywords.py
+-rw-r--r--   0        0        0      757 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/choke_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/compressor_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/eos_defaults_keywords.py
+-rw-r--r--   0        0        0     1210 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/equil_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/esp_keywords.py
+-rw-r--r--   0        0        0     1368 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/fluxin_keywords.py
+-rw-r--r--   0        0        0      170 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/gaslift_keywords.py
+-rw-r--r--   0        0        0     1159 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/icd_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/ipr_keywords.py
+-rw-r--r--   0        0        0     2658 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py
+-rw-r--r--   0        0        0      795 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/options_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/polymer_keywords.py
+-rw-r--r--   0        0        0     5130 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/proc_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/pump_keywords.py
+-rw-r--r--   0        0        0     2547 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py
+-rw-r--r--   0        0        0     1579 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py
+-rw-r--r--   0        0        0      896 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/rock_keywords.py
+-rw-r--r--   0        0        0     4957 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py
+-rw-r--r--   0        0        0      880 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/separator_keywords.py
+-rw-r--r--   0        0        0     3121 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py
+-rw-r--r--   0        0        0     4492 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/surface_keywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/tracer_init_keywords.py
+-rw-r--r--   0        0        0      306 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/valve_keywords.py
+-rw-r--r--   0        0        0      243 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/water_keywords.py
+-rw-r--r--   0        0        0      902 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/wells_keywords.py
+-rw-r--r--   0        0        0    17415 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusNetwork.py
+-rw-r--r--   0        0        0     3717 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusPVTMethods.py
+-rw-r--r--   0        0        0     4005 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusRelPermMethods.py
+-rw-r--r--   0        0        0    12838 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusReporting.py
+-rw-r--r--   0        0        0     3771 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusRockMethods.py
+-rw-r--r--   0        0        0     4140 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusSeparatorMethods.py
+-rw-r--r--   0        0        0    39541 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusSimulator.py
+-rw-r--r--   0        0        0    16873 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusSolverParameters.py
+-rw-r--r--   0        0        0     3814 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusValveMethods.py
+-rw-r--r--   0        0        0     3809 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusWaterMethods.py
+-rw-r--r--   0        0        0    23826 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/NexusWells.py
+-rw-r--r--   0        0        0      404 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/__init__.py
+-rw-r--r--   0        0        0    23806 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/array_function_operations.py
+-rw-r--r--   0        0        0      115 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/constants.py
+-rw-r--r--   0        0        0    24849 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/load_wells.py
+-rw-r--r--   0        0        0    14120 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/logfile_operations.py
+-rw-r--r--   0        0        0    16713 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_add_new_object_to_file.py
+-rw-r--r--   0        0        0     9025 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_collect_tables.py
+-rw-r--r--   0        0        0     7536 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_constraint_operations.py
+-rw-r--r--   0        0        0    23776 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_file_operations.py
+-rw-r--r--   0        0        0     4192 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_load_well_list.py
+-rw-r--r--   0        0        0     2323 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_modify_object_in_file.py
+-rw-r--r--   0        0        0     8133 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/nexus_remove_object_from_file.py
+-rw-r--r--   0        0        0     5422 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/rel_perm_operations.py
+-rw-r--r--   0        0        0    18539 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/runcontrol_operations.py
+-rw-r--r--   0        0        0    20202 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nexus/structured_grid_operations.py
+-rw-r--r--   0        0        0      620 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Node.py
+-rw-r--r--   0        0        0      794 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/NodeConnection.py
+-rw-r--r--   0        0        0      456 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/NodeConnections.py
+-rw-r--r--   0        0        0      398 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/Nodes.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.202024 ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/Network/__init__.py
+-rw-r--r--   0        0        0     3041 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py
+-rw-r--r--   0        0        0     3090 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/Enums/SimulationTypeEnum.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/Enums/__init__.py
+-rw-r--r--   0        0        0      640 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/Model_Parts/__init__.py
+-rw-r--r--   0        0        0     2892 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimKeywords/__init__.py
+-rw-r--r--   0        0        0    11092 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimSimulator.py
+-rw-r--r--   0        0        0      462 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimWells.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OpenGoSim/__init__.py
+-rw-r--r--   0        0        0     2562 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/OperationsMixin.py
+-rw-r--r--   0        0        0      556 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/PVT.py
+-rw-r--r--   0        0        0      581 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/RelPerm.py
+-rw-r--r--   0        0        0     6301 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/RelPermEndPoint.py
+-rw-r--r--   0        0        0     1624 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Reporting.py
+-rw-r--r--   0        0        0      694 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Rock.py
+-rw-r--r--   0        0        0      715 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Separator.py
+-rw-r--r--   0        0        0     4512 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Simulator.py
+-rw-r--r--   0        0        0      407 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/SolverParameter.py
+-rw-r--r--   0        0        0      679 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/SolverParameters.py
+-rw-r--r--   0        0        0     1260 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Target.py
+-rw-r--r--   0        0        0      412 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Targets.py
+-rw-r--r--   0        0        0     1223 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMapping.py
+-rw-r--r--   0        0        0     2249 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py
+-rw-r--r--   0        0        0     8727 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py
+-rw-r--r--   0        0        0    17410 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py
+-rw-r--r--   0        0        0    31095 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py
+-rw-r--r--   0        0        0    15398 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py
+-rw-r--r--   0        0        0       96 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/__init__.py
+-rw-r--r--   0        0        0    14870 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/Units.py
+-rw-r--r--   0        0        0       45 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Units/__init__.py
+-rw-r--r--   0        0        0       95 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/__init__.py
+-rw-r--r--   0        0        0     2425 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/factory_methods.py
+-rw-r--r--   0        0        0      365 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/general_utilities.py
+-rw-r--r--   0        0        0     1955 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/generic_repr.py
+-rw-r--r--   0        0        0     1585 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/invert_nexus_map.py
+-rw-r--r--   0        0        0      453 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/obj_to_dataframe.py
+-rw-r--r--   0        0        0     1364 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/obj_to_table_string.py
+-rw-r--r--   0        0        0     2563 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Utils/to_dict_generic.py
+-rw-r--r--   0        0        0      591 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Valve.py
+-rw-r--r--   0        0        0      593 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Water.py
+-rw-r--r--   0        0        0     5023 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Well.py
+-rw-r--r--   0        0        0     1287 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/WellConnection.py
+-rw-r--r--   0        0        0     1946 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/WellConnections.py
+-rw-r--r--   0        0        0     1057 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/WellLists.py
+-rw-r--r--   0        0        0      631 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Wellbore.py
+-rw-r--r--   0        0        0      439 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Wellbores.py
+-rw-r--r--   0        0        0      685 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Wellhead.py
+-rw-r--r--   0        0        0      426 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Wellheads.py
+-rw-r--r--   0        0        0     3244 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/Wells.py
+-rw-r--r--   0        0        0      482 2024-05-24 13:57:34.353999 ressimpy-2.2.2/ResSimpy/__init__.py
+-rw-r--r--   0        0        0     2751 2024-05-24 13:57:24.206024 ressimpy-2.2.2/ResSimpy/output_request.py
+-rw-r--r--   0        0        0     2641 2024-05-24 13:57:34.353999 ressimpy-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0     6529 1970-01-01 00:00:00.000000 ressimpy-2.2.2/PKG-INFO
```

### Comparing `ressimpy-2.2.1/LICENSE.MD` & `ressimpy-2.2.2/LICENSE.MD`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/README.md` & `ressimpy-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Aquifer.py` & `ressimpy-2.2.2/ResSimpy/Aquifer.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Completion.py` & `ressimpy-2.2.2/ResSimpy/Completion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Constraint.py` & `ressimpy-2.2.2/ResSimpy/Constraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Constraints.py` & `ressimpy-2.2.2/ResSimpy/Constraints.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/DataObjectMixin.py` & `ressimpy-2.2.2/ResSimpy/DataObjectMixin.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/DynamicProperty.py` & `ressimpy-2.2.2/ResSimpy/DynamicProperty.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Equilibration.py` & `ressimpy-2.2.2/ResSimpy/Equilibration.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/File.py` & `ressimpy-2.2.2/ResSimpy/File.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/FileBase.py` & `ressimpy-2.2.2/ResSimpy/FileBase.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/FileOperations/file_operations.py` & `ressimpy-2.2.2/ResSimpy/FileOperations/file_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Gaslift.py` & `ressimpy-2.2.2/ResSimpy/Gaslift.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Grid.py` & `ressimpy-2.2.2/ResSimpy/Grid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/GridArrayFunction.py` & `ressimpy-2.2.2/ResSimpy/GridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Hydraulics.py` & `ressimpy-2.2.2/ResSimpy/Hydraulics.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/ISODateTime.py` & `ressimpy-2.2.2/ResSimpy/ISODateTime.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Network.py` & `ressimpy-2.2.2/ResSimpy/Network.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/FcsConfig.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/FcsConfig.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/FcsFile.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/FcsFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusConstraint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusConstraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,16 @@
         _, new_constraints = collect_all_tables_to_objects(surface_file,
                                                            {
                                                                'CONSTRAINTS': NexusConstraint,
                                                                'CONSTRAINT': NexusConstraint,
                                                                'QMULT': NexusConstraint
                                                            },
                                                            start_date=start_date,
-                                                           default_units=default_units)
+                                                           default_units=default_units,
+                                                           date_format=self.__model.date_format)
         self._add_to_memory(new_constraints)
 
     def _add_to_memory(self, additional_constraints: Optional[dict[str, list[NexusConstraint]]]) -> None:
         """Adds additional constraints to memory within the NexusConstraints object.
             If user adds constraints list this will not be reflected in the Nexus deck at this time.
 
         Args:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNode.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNode.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodeConnections.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,16 @@
         raise NotImplementedError('To be implemented')
 
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
         """Calls load connections and appends the list of discovered NodeConnections into the NexusNodeConnection \
             object.
         """
         new_connections, _ = collect_all_tables_to_objects(surface_file, {self.table_header: NexusNodeConnection},
-                                                           start_date=start_date, default_units=default_units)
+                                                           start_date=start_date, default_units=default_units,
+                                                           date_format=self.__parent_network.model.date_format)
         cons_list = new_connections.get(self.table_header)
         self._add_to_memory(cons_list)
 
     def _add_to_memory(self, additional_list: Optional[Sequence[NexusNodeConnection]]) -> None:
         """Extends the nodes object by a list of nodes provided to it.
 
         Args:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusNodes.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusNodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,16 @@
 
         Raises:
             TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
 
         """
         new_nodes, _ = collect_all_tables_to_objects(surface_file, {'NODES': NexusNode},
                                                      start_date=start_date,
-                                                     default_units=default_units)
+                                                     default_units=default_units,
+                                                     date_format=self.__parent_network.model.date_format)
         nodes_list = new_nodes.get('NODES')
         self._add_to_memory(nodes_list)
 
     def _add_to_memory(self, additional_list: Optional[list[NexusNode]]) -> None:
         """Extends the nodes object by a list of nodes provided to it.
 
         Args:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusProc.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusProc.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusProcs.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusProcs.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusTarget.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusTarget.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusTargets.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusTargets.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 
         Raises:
             TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
 
         """
         new_targets, _ = collect_all_tables_to_objects(surface_file, {'TARGET': NexusTarget},
                                                        start_date=start_date,
-                                                       default_units=default_units)
+                                                       default_units=default_units,
+                                                       date_format=self.__parent_network.model.date_format)
         cons_list = new_targets.get('TARGET')
         self._add_to_memory(cons_list)
 
     def _add_to_memory(self, additional_list: Optional[list[NexusTarget]]) -> None:
         """Extends the targets object by a list of targets provided to it.
 
         Args:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellConnections.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,16 @@
     def get_overview(self) -> str:
         raise NotImplementedError('To be implemented')
 
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
         new_well_connections, _ = collect_all_tables_to_objects(surface_file, {'WELLS': NexusWellConnection,
                                                                                'GASWELLS': NexusWellConnection},
                                                                 start_date=start_date,
-                                                                default_units=default_units)
+                                                                default_units=default_units,
+                                                                date_format=self.__parent_network.model.date_format)
         cons_list = new_well_connections.get('WELLS')
         gas_cons_list = new_well_connections.get('GASWELLS')
         self._add_to_memory(cons_list)
         self._add_to_memory(gas_cons_list)
 
     def remove(self, obj_to_remove: dict[str, None | str | float | int] | UUID) -> None:
         """Remove a wellbore from the network based on the properties matching a dictionary or id.
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellbores.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,16 @@
 
     def get_overview(self) -> str:
         raise NotImplementedError('To be implemented')
 
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
         new_wellbores, _ = collect_all_tables_to_objects(surface_file, {'WELLBORE': NexusWellbore},
                                                          start_date=start_date,
-                                                         default_units=default_units)
+                                                         default_units=default_units,
+                                                         date_format=self.__parent_network.model.date_format)
         cons_list = new_wellbores.get('WELLBORE')
         self._add_to_memory(cons_list)
 
     def _add_to_memory(self, additional_list: Optional[list[NexusWellbore]]) -> None:
         """Extends the nodes object by a list of wellbores provided to it.
 
         Args:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/Network/NexusWellheads.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,16 @@
 
     def get_overview(self) -> str:
         raise NotImplementedError('To be implemented')
 
     def load(self, surface_file: File, start_date: str, default_units: UnitSystem) -> None:
         new_wellheads, _ = collect_all_tables_to_objects(surface_file, {'WELLHEAD': NexusWellhead},
                                                          start_date=start_date,
-                                                         default_units=default_units)
+                                                         default_units=default_units,
+                                                         date_format=self.__parent_network.model.date_format)
         wellheads_list = new_wellheads.get('WELLHEAD')
         self._add_to_memory(wellheads_list)
 
     def _add_to_memory(self, additional_list: Optional[list[NexusWellhead]]) -> None:
         """Extends the wellhead object by a list of wellheads provided to it.
 
         Args:
@@ -88,23 +89,23 @@
             obj_to_remove (UUID | dict[str, None | str | float | int]): UUID of the wellhead to remove or a dictionary \
             with sufficient matching parameters to uniquely identify a wellhead
 
         """
         self.__remove_object_operations.remove_object_from_network_main(
             obj_to_remove, self._network_element_name, self.__wellheads)
 
-    def add(self, obj_to_remove: dict[str, None | str | float | int]) -> None:
+    def add(self, obj_to_add: dict[str, None | str | float | int]) -> None:
         """Adds a wellhead to a network, taking a dictionary with properties for the new wellhead.
 
         Args:
-            obj_to_remove (dict[str, None | str | float | int]): dictionary taking all the properties for the new
+            obj_to_add (dict[str, None | str | float | int]): dictionary taking all the properties for the new
             wellhead.
             Requires date and a name.
         """
-        new_object = self.__add_object_operations.add_network_obj(obj_to_remove, NexusWellhead, self.__parent_network)
+        new_object = self.__add_object_operations.add_network_obj(obj_to_add, NexusWellhead, self.__parent_network)
         self._add_to_memory([new_object])
 
     def modify(self, obj_to_modify: dict[str, None | str | float | int],
                new_properties: dict[str, None | str | float | int]) -> None:
         """Modifies an existing wellhead based on a matching dictionary of properties.
         (partial matches allowed if precisely 1 matching node is found).
         Updates the properties with properties in the new_properties dictionary.
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusAquiferMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusCompletion.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusEquilMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusEquilMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusFile.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusFile.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusGasliftMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusHydraulicsMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusPVTMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusPVTMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRelPermMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusReportingRequests.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusReportingRequests.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusRockMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusRockMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusSeparatorMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusSolverParameter.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusSolverParameter.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusValveMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusValveMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWaterMethod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWaterMethod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWell.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWellList.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWellList.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/NexusWellMod.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/NexusWellMod.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGrid.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py` & `ressimpy-2.2.2/ResSimpy/Nexus/DataModels/StructuredGrid/NexusGridArrayFunction.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusAquiferMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusAquiferMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusEquilMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusEquilMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusGasliftMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusGasliftMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusHydraulicsMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusHydraulicsMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/aquifer_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/equil_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/equil_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/hyd_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/nexus_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/options_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/options_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/proc_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/proc_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/pvt_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/relpm_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/rock_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/rock_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/runcontrol_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/separator_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/separator_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/structured_grid_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/surface_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/surface_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusKeywords/wells_keywords.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusKeywords/wells_keywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusNetwork.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusNetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,14 +232,15 @@
                           'TARGET': NexusTarget,
                           'GUIDERATE': None,
                           'PROCS': None,
                           'WELLLIST': NexusWellList,
                           },
                 start_date=self.__model.start_date,
                 default_units=self.__model.default_units,
+                date_format=self.__model.date_format
             )
             self.nodes._add_to_memory(type_check_lists(nexus_obj_dict.get('NODES')))
             self.connections._add_to_memory(type_check_lists(nexus_obj_dict.get('NODECON')))
             self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLS')))
             self.well_connections._add_to_memory(type_check_lists(nexus_obj_dict.get('GASWELLS')))
             self.wellheads._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLHEAD')))
             self.wellbores._add_to_memory(type_check_lists(nexus_obj_dict.get('WELLBORE')))
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusPVTMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusPVTMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusRelPermMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusRelPermMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusReporting.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusReporting.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusRockMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusRockMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusSeparatorMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusSeparatorMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusSimulator.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusSimulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusSolverParameters.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusSolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusValveMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusValveMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusWaterMethods.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusWaterMethods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/NexusWells.py` & `ressimpy-2.2.2/ResSimpy/Nexus/NexusWells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/array_function_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/array_function_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/load_wells.py` & `ressimpy-2.2.2/ResSimpy/Nexus/load_wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/logfile_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/logfile_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_add_new_object_to_file.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_add_new_object_to_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,13 +300,14 @@
     def add_network_obj(self, node_to_add: dict[str, None | str | float | int], obj_type: type[T],
                         network: NexusNetwork) -> T:
         network.get_load_status()
         file_to_add_to = network.get_network_file()
         if self.obj_type is not None:
             obj_type = self.obj_type
         name, date = self.check_name_date(node_to_add)
-        new_object = obj_type(node_to_add)
+        date_format = network.model.date_format
+        new_object = obj_type(node_to_add, date_format=date_format)
         file_as_list = file_to_add_to.get_flat_list_str_file
         if file_as_list is None:
             raise ValueError(f'No file content found in the surface file specified at {file_to_add_to.location}')
         self.add_object_to_file(date, file_as_list, file_to_add_to, new_object, node_to_add)
         return new_object
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_collect_tables.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_collect_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,37 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
 from ResSimpy.File import File
 from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
 from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.Nexus.nexus_constraint_operations import load_inline_constraints
 from ResSimpy.Nexus.nexus_file_operations import check_property_in_line, check_token, get_expected_token_value, \
     check_list_tokens, load_table_to_objects
 from ResSimpy.Nexus.nexus_load_well_list import load_well_lists
 
 
 # TODO refactor the collection of tables to an object with proper typing
 def collect_all_tables_to_objects(nexus_file: File, table_object_map: dict[str, Any], start_date: Optional[str],
-                                  default_units: Optional[UnitSystem]) -> \
+                                  default_units: Optional[UnitSystem], date_format: DateFormat) -> \
         tuple[dict[str, list[Any]], dict[str, list[NexusConstraint]]]:
     """Loads all tables from a given file.
 
     Args:
     ----
-    nexus_file (File): NexusFile representation of the file.
-    table_object_map (dict[str, Storage_Object]): dictionary containing the name of the table as keys and \
-                the object type to store the data from each row into. Require objects to have a get_keyword_mapping \
-                function
-    model: (NexusSimulator): main simulator object
-    start_date (Optional[str]): The model start date.
-    default_units (Optional[UnitSystem]): The default unit system the Nexus model is set to.
+        nexus_file (File): NexusFile representation of the file.
+        table_object_map (dict[str, Storage_Object]): dictionary containing the name of the table as keys and \
+                    the object type to store the data from each row into. Require objects to have a get_keyword_mapping\
+                    function
+        model: (NexusSimulator): main simulator object
+        start_date (Optional[str]): The model start date.
+        default_units (Optional[UnitSystem]): The default unit system the Nexus model is set to.
+        date_format (Optional[DateFormat]): The date format of the object.
 
     Raises:
     ------
     TypeError: if the unit system found in the property check is not a valid enum UnitSystem.
 
     Returns:
     -------
@@ -90,37 +92,38 @@
                                         current_date=current_date,
                                         unit_system=unit_system,
                                         property_map=property_map,
                                         existing_constraints=nexus_constraints,
                                         nexus_file=nexus_file,
                                         start_line_index=table_start,
                                         network_names=network_names,
+                                        date_format=date_format
                                         )
 
             elif token_found == 'QMULT' or token_found == 'CONSTRAINT':
                 list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
                                                      row_object=table_object_map[token_found],
                                                      property_map=property_map,
                                                      current_date=current_date,
                                                      unit_system=unit_system,
                                                      nexus_obj_dict=nexus_constraints,
-                                                     preserve_previous_object_attributes=True)
+                                                     preserve_previous_object_attributes=True, date_format=date_format)
 
             elif token_found == 'WELLLIST':
                 list_objects = load_well_lists(file_as_list=file_as_list[table_start-1:table_end],
                                                current_date=current_date,
                                                previous_well_lists=nexus_object_results[token_found],
                                                )
 
             else:
                 list_objects = load_table_to_objects(file_as_list=file_as_list[table_start:table_end],
                                                      row_object=table_object_map[token_found],
                                                      property_map=property_map,
                                                      current_date=current_date,
-                                                     unit_system=unit_system)
+                                                     unit_system=unit_system, date_format=date_format)
 
             # store objects found into right dictionary
             list_of_token_obj = nexus_object_results[token_found]
             # This statement ensures that CONSTRAINT that are found in tables are actually added to the dictionary
             # under the same key as constraints to preserve their order
             if (token_found == 'CONSTRAINT' or token_found == 'QMULT') and list_objects is not None:
                 for constraint, id_index in list_objects:
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_constraint_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_constraint_operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """Key functions for reading in nexus constraints and populating objects with the data."""
 from __future__ import annotations
 
 from typing import Optional, TYPE_CHECKING
 
 from ResSimpy.Nexus.DataModels.Network.NexusConstraint import NexusConstraint
 from ResSimpy.Enums.UnitsEnum import UnitSystem
+from ResSimpy.Nexus.NexusEnums.DateFormatEnum import DateFormat
 from ResSimpy.Nexus.nexus_file_operations import get_next_value, correct_datatypes
 from ResSimpy.Utils.invert_nexus_map import nexus_keyword_to_attribute_name
 import fnmatch
 
 if TYPE_CHECKING:
     from ResSimpy.File import File
 
 
 def load_inline_constraints(file_as_list: list[str], constraint: type[NexusConstraint], current_date: Optional[str],
                             unit_system: UnitSystem, property_map: dict[str, tuple[str, type]],
                             existing_constraints: dict[str, list[NexusConstraint]], nexus_file: File,
-                            start_line_index: int, network_names: Optional[list[str]] = None) -> None:
+                            start_line_index: int, date_format: DateFormat,
+                            network_names: Optional[list[str]] = None) -> None:
     """Loads table of constraints with the wellname/node first and the constraints following inline
         uses previous set of constraints as still applied to the well.
 
     Args:
     ----
         file_as_list (list[str]): file represented as a list of strings
         constraint (NexusConstraint): object to store the attributes extracted from each row.
@@ -29,14 +31,15 @@
         property_map (dict[str, tuple[str, type]]): Mapping of nexus keywords to attributes
         existing_constraints (dict[str, NexusConstraint]): all existing constraints from previous lines of the \
             surface file
         nexus_file (File): The Nexus file containing the constraints.
         start_line_index (int): The index of the line in the file to start loading from.
         network_names (Optional[list[str]]): list of names for all nodes, wells and connections in a nexus network.
             Used in deriving constraints from wildcards. Defaults to None
+        date_format (Optional[DateFormat]): The date format of the object.
 
     Returns:
     -------
         dict[UUID, int]: dictionary of object locations derived from inline table.
     """
 
     for index, line in enumerate(file_as_list):
@@ -104,19 +107,19 @@
             if well_constraints is not None:
                 latest_constraint = well_constraints[-1]
                 if latest_constraint.date == current_date:
                     latest_constraint.update(properties_dict, nones_overwrite)
                     nexus_file.add_object_locations(latest_constraint.id, [index + start_line_index])
                 else:
                     # otherwise take a copy of the previous constraint and add the additional properties
-                    new_constraint = constraint(properties_dict)
+                    new_constraint = constraint(properties_dict, date_format=date_format)
                     well_constraints.append(new_constraint)
                     nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
             else:
-                new_constraint = constraint(properties_dict)
+                new_constraint = constraint(properties_dict, date_format=date_format)
                 existing_constraints[name_of_node] = [new_constraint]
                 nexus_file.add_object_locations(new_constraint.id, [index + start_line_index])
 
 
 def __clear_constraints(token_value: str, constraint: type[NexusConstraint]) -> dict[str, None]:
     """Replicates behaviour of the clear keyword in nexus constraints by creating a dictionary filled with
     Nones for the relevant parameters.
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_file_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_file_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -398,15 +398,16 @@
 
         keyword_store[column] = value
         trimmed_line = trimmed_line.replace(value, "", 1)
     return valid_line, keyword_store
 
 
 def load_table_to_objects(file_as_list: list[str], row_object: Any, property_map: dict[str, tuple[str, type]],
-                          current_date: Optional[str] = None, unit_system: Optional[UnitSystem] = None,
+                          date_format: DateFormat, current_date: Optional[str] = None,
+                          unit_system: Optional[UnitSystem] = None,
                           nexus_obj_dict: Optional[dict[str, list[Any]]] = None,
                           preserve_previous_object_attributes: bool = False,
                           ) -> list[tuple[Any, int]]:
     """Loads a table row by row to an object provided in the row_object.
 
     Args:
         file_as_list (list[str]): file represented as a list of strings.
@@ -417,14 +418,16 @@
         current_date (Optional[str]): date/time at which the object was found within a recurrent file
         unit_system (Optional[UnitSystem): most recent UnitSystem enum of the file where the object was found
         nexus_obj_dict (Optional[dict[str, list[Any]]]): list of objects to append to. \
             If None creates an empty list to populate.
         preserve_previous_object_attributes (bool): If True the code will find the latest object with a matching name\
             attribute and will update the object to reflect the latest additional attributes and overriding all \
             matching attributes. Must have a .update() method implemented and a name
+        date_format (Optional[DateFormat]): The date format of the object.
+
     Returns:
         list[obj]: list of tuples containing instances of the class provided for the row_object,
         populated with attributes from the property map dictionary and the line index where it was found
     """
     keyword_map = {x: y[0] for x, y in property_map.items()}
     header_index, headers = get_table_header(file_as_list, keyword_map)
     table_as_list = file_as_list[header_index + 1::]
@@ -457,19 +460,22 @@
                 if new_object_date is not None and new_object_date == current_date:
                     # otherwise just update the object inplace and don't add it to the return list
                     existing_constraint.update(keyword_store)
                     # add just the id back in to track the lines where it came from in the file
                     return_objects.append((existing_constraint.id, index))
                     continue
                 else:
-                    new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
+                    new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system,
+                                            date_format=date_format)
             else:
-                new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
+                new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system,
+                                        date_format=date_format)
         else:
-            new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system)
+            new_object = row_object(properties_dict=keyword_store, date=current_date, unit_system=unit_system,
+                                    date_format=date_format)
 
         return_objects.append((new_object, index))
     return return_objects
 
 
 def check_list_tokens(list_tokens: list[str], line: str) -> Optional[str]:
     """Checks a list of tokens for whether it exists in a string and returns the token that matched.
```

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_load_well_list.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_load_well_list.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_modify_object_in_file.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_modify_object_in_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/nexus_remove_object_from_file.py` & `ressimpy-2.2.2/ResSimpy/Nexus/nexus_remove_object_from_file.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/rel_perm_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/rel_perm_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/runcontrol_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/runcontrol_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Nexus/structured_grid_operations.py` & `ressimpy-2.2.2/ResSimpy/Nexus/structured_grid_operations.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Node.py` & `ressimpy-2.2.2/ResSimpy/Node.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/NodeConnection.py` & `ressimpy-2.2.2/ResSimpy/NodeConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py` & `ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/OpenGoSimCompletion.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py` & `ressimpy-2.2.2/ResSimpy/OpenGoSim/DataModels/OpenGoSimWell.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py` & `ressimpy-2.2.2/ResSimpy/OpenGoSim/Model_Parts/OpenGoSimNetwork.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py` & `ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimKeywords/OpenGoSimKeywords.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OpenGoSim/OpenGoSimSimulator.py` & `ressimpy-2.2.2/ResSimpy/OpenGoSim/OpenGoSimSimulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/OperationsMixin.py` & `ressimpy-2.2.2/ResSimpy/OperationsMixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Any, Sequence, Optional, TYPE_CHECKING
 from uuid import UUID
 
 import pandas as pd
 
 from ResSimpy.Enums.UnitsEnum import UnitSystem
 from ResSimpy.File import File
+
 if TYPE_CHECKING:
     from ResSimpy.Nexus.NexusNetwork import Network
 
 
 class NetworkOperationsMixIn(ABC):
     def __init__(self, parent_network: Network) -> None:
         """Initialises the NetworkOperationsMixIn class.
```

### Comparing `ressimpy-2.2.1/ResSimpy/PVT.py` & `ressimpy-2.2.2/ResSimpy/PVT.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/RelPerm.py` & `ressimpy-2.2.2/ResSimpy/RelPerm.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/RelPermEndPoint.py` & `ressimpy-2.2.2/ResSimpy/RelPermEndPoint.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Reporting.py` & `ressimpy-2.2.2/ResSimpy/Reporting.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Rock.py` & `ressimpy-2.2.2/ResSimpy/Rock.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Separator.py` & `ressimpy-2.2.2/ResSimpy/Separator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Simulator.py` & `ressimpy-2.2.2/ResSimpy/Simulator.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/SolverParameters.py` & `ressimpy-2.2.2/ResSimpy/SolverParameters.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Target.py` & `ressimpy-2.2.2/ResSimpy/Target.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/BaseUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/CompletionUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/ConstraintUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/DynamicPropertyUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py` & `ressimpy-2.2.2/ResSimpy/Units/AttributeMappings/NetworkUnitMapping.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Units/Units.py` & `ressimpy-2.2.2/ResSimpy/Units/Units.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Utils/factory_methods.py` & `ressimpy-2.2.2/ResSimpy/Utils/factory_methods.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Utils/generic_repr.py` & `ressimpy-2.2.2/ResSimpy/Utils/generic_repr.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Utils/invert_nexus_map.py` & `ressimpy-2.2.2/ResSimpy/Utils/invert_nexus_map.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Utils/obj_to_table_string.py` & `ressimpy-2.2.2/ResSimpy/Utils/obj_to_table_string.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Utils/to_dict_generic.py` & `ressimpy-2.2.2/ResSimpy/Utils/to_dict_generic.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Valve.py` & `ressimpy-2.2.2/ResSimpy/Valve.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Water.py` & `ressimpy-2.2.2/ResSimpy/Water.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Well.py` & `ressimpy-2.2.2/ResSimpy/Well.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/WellConnection.py` & `ressimpy-2.2.2/ResSimpy/WellConnection.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/WellConnections.py` & `ressimpy-2.2.2/ResSimpy/WellConnections.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/WellLists.py` & `ressimpy-2.2.2/ResSimpy/WellLists.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Wellbore.py` & `ressimpy-2.2.2/ResSimpy/Wellbore.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Wellhead.py` & `ressimpy-2.2.2/ResSimpy/Wellhead.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/Wells.py` & `ressimpy-2.2.2/ResSimpy/Wells.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/ResSimpy/output_request.py` & `ressimpy-2.2.2/ResSimpy/output_request.py`

 * *Files identical despite different names*

### Comparing `ressimpy-2.2.1/pyproject.toml` & `ressimpy-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ResSimpy"
-version = "2.2.1" # Set at build time
+version = "2.2.2" # Set at build time
 description = "A Python library for working with Reservoir Simulator Models."
 authors = ["BP"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["ResSimpy", "Reservoir Engineering"]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `ressimpy-2.2.1/PKG-INFO` & `ressimpy-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResSimpy
-Version: 2.2.1
+Version: 2.2.2
 Summary: A Python library for working with Reservoir Simulator Models.
 License: Apache-2.0
 Keywords: ResSimpy,Reservoir Engineering
 Author: BP
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

