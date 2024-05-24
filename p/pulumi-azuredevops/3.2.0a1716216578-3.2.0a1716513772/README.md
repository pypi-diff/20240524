# Comparing `tmp/pulumi_azuredevops-3.2.0a1716216578.tar.gz` & `tmp/pulumi_azuredevops-3.2.0a1716513772.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_azuredevops-3.2.0a1716216578.tar", last modified: Mon May 20 14:53:41 2024, max compression
+gzip compressed data, was "pulumi_azuredevops-3.2.0a1716513772.tar", last modified: Fri May 24 01:27:48 2024, max compression
```

## Comparing `pulumi_azuredevops-3.2.0a1716216578.tar` & `pulumi_azuredevops-3.2.0a1716513772.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/
--rw-r--r--   0 runner    (1001) docker     (127)    24210 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   158510 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/area_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_auto_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_build_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_comment_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_merge_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_min_reviewers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_status_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_work_item_linking.py
--rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    29671 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_definition_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    30214 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_folder_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_approval.py
--rw-r--r--   0 runner    (1001) docker     (127)    35637 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_branch_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    55861 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_business_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_exclusive_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_required_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    34798 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/elastic_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/environment_resource_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/feed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/feed_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_agent_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_area.py
--rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_build_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_client_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_feed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_git_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_iteration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_securityrole_definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_service_endpoint_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_azurecr.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_teams.py
--rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23698 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_repository_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    29707 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23886 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group_entitlement.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/iterative_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/library_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)   205734 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24778 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/pipeline_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    23664 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_features.py
--rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_pipeline_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_author_email_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20576 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_case_enforcement.py
--rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_check_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    21739 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_file_path_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_max_file_size.py
--rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_max_path_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_reserved_names.py
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/resource_authorization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/securityrole_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_artifactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    27779 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_ecr.py
--rw-r--r--   0 runner    (1001) docker     (127)    62516 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_bit_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_docker_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    23777 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_generic_git.py
--rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_git_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
--rw-r--r--   0 runner    (1001) docker     (127)    32463 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_npm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    24022 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_service_fabric.py
--rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_sonar_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_sonar_qube.py
--rw-r--r--   0 runner    (1001) docker     (127)    22837 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)    25424 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_argocd.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_externaltfs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jenkins.py
--rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_maven.py
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_nuget.py
--rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23121 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/servicehook_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/tagging_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team_administrators.py
--rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team_members.py
--rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/variable_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/variable_group_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/work_item_query_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/workitem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-20 14:53:41.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-20 14:53:41.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:53:41.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 14:53:41.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 14:53:41.000000 pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 14:53:35.000000 pulumi_azuredevops-3.2.0a1716216578/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:53:41.542218 pulumi_azuredevops-3.2.0a1716216578/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/
+-rw-r--r--   0 runner    (1001) docker     (127)    24210 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   160660 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23266 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/area_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_auto_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18335 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_build_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_comment_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16855 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_merge_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17325 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_min_reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17299 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_status_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16789 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_work_item_linking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43455 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29671 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_definition_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10895 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30214 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_folder_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25760 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_approval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35637 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_branch_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55861 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_business_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18520 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_exclusive_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21392 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_required_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34798 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/elastic_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11395 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22178 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/environment_resource_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13596 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/feed_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5454 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_agent_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_build_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_client_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5523 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_feed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8405 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_git_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4866 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8393 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_securityrole_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15707 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_service_endpoint_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12948 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_azurecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5577 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_teams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7872 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23698 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42476 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18613 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_repository_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19248 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29707 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23886 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group_entitlement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20701 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/iterative_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19301 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/library_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   207828 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24778 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/pipeline_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23664 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12459 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32422 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26371 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_pipeline_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29398 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21620 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_author_email_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20576 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_case_enforcement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17753 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_check_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21739 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_file_path_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20083 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_max_file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19847 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_max_path_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17651 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_reserved_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/resource_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11723 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/securityrole_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23858 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_artifactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27779 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20863 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_dev_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30713 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_ecr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62516 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17152 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_bit_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26204 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_docker_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23777 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_generic_git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20850 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_git_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17710 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32463 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18125 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_npm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19876 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24022 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_service_fabric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16799 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_sonar_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18533 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_sonar_qube.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22837 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25424 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_argocd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_externaltfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24453 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_gcp_terraform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_incomingwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25618 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25690 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25108 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26424 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_maven.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25697 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_nuget.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19931 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_octopusdeploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23121 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17931 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/servicehook_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30457 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/servicehook_storage_queue_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18494 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/tagging_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21800 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18624 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team_administrators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17677 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21625 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24376 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/variable_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22391 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/variable_group_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25781 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/work_item_query_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25497 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/workitem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-05-24 01:27:48.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5767 2024-05-24 01:27:48.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 01:27:48.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 01:27:48.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-24 01:27:48.000000 pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-24 01:27:41.000000 pulumi_azuredevops-3.2.0a1716513772/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 01:27:48.059716 pulumi_azuredevops-3.2.0a1716513772/setup.cfg
```

### Comparing `pulumi_azuredevops-3.2.0a1716216578/PKG-INFO` & `pulumi_azuredevops-3.2.0a1716513772/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.2.0a1716216578
+Version: 3.2.0a1716513772
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.2.0a1716216578/README.md` & `pulumi_azuredevops-3.2.0a1716513772/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/__init__.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/_inputs.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -958,42 +958,56 @@
 
 @pulumi.input_type
 class BranchPolicyStatusCheckSettingsScopeArgs:
     def __init__(__self__, *,
                  match_type: Optional[pulumi.Input[str]] = None,
                  repository_id: Optional[pulumi.Input[str]] = None,
                  repository_ref: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] match_type: The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
+        :param pulumi.Input[str] repository_id: The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
+        :param pulumi.Input[str] repository_ref: The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
+        """
         if match_type is not None:
             pulumi.set(__self__, "match_type", match_type)
         if repository_id is not None:
             pulumi.set(__self__, "repository_id", repository_id)
         if repository_ref is not None:
             pulumi.set(__self__, "repository_ref", repository_ref)
 
     @property
     @pulumi.getter(name="matchType")
     def match_type(self) -> Optional[pulumi.Input[str]]:
+        """
+        The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
+        """
         return pulumi.get(self, "match_type")
 
     @match_type.setter
     def match_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "match_type", value)
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> Optional[pulumi.Input[str]]:
+        """
+        The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
+        """
         return pulumi.get(self, "repository_id")
 
     @repository_id.setter
     def repository_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository_id", value)
 
     @property
     @pulumi.getter(name="repositoryRef")
     def repository_ref(self) -> Optional[pulumi.Input[str]]:
+        """
+        The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
+        """
         return pulumi.get(self, "repository_ref")
 
     @repository_ref.setter
     def repository_ref(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "repository_ref", value)
 
 
@@ -1294,20 +1308,30 @@
         pulumi.set(self, "includes", value)
 
 
 @pulumi.input_type
 class BuildDefinitionFeatureArgs:
     def __init__(__self__, *,
                  skip_first_run: Optional[pulumi.Input[bool]] = None):
+        """
+        :param pulumi.Input[bool] skip_first_run: Trigger the pipeline to run after the creation. Defaults to `true`.
+               
+               > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
+        """
         if skip_first_run is not None:
             pulumi.set(__self__, "skip_first_run", skip_first_run)
 
     @property
     @pulumi.getter(name="skipFirstRun")
     def skip_first_run(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Trigger the pipeline to run after the creation. Defaults to `true`.
+
+        > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
+        """
         return pulumi.get(self, "skip_first_run")
 
     @skip_first_run.setter
     def skip_first_run(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_first_run", value)
 
 
@@ -3010,59 +3034,59 @@
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationBasicArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str],
                  username: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] password: The ArgoCD password.
-        :param pulumi.Input[str] username: The ArgoCD user name.
+        :param pulumi.Input[str] password: ArgoCD Password.
+        :param pulumi.Input[str] username: ArgoCD Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
         """
-        The ArgoCD password.
+        ArgoCD Password.
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def username(self) -> pulumi.Input[str]:
         """
-        The ArgoCD user name.
+        ArgoCD Username.
         """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: pulumi.Input[str]):
         pulumi.set(self, "username", value)
 
 
 @pulumi.input_type
 class ServiceendpointArgocdAuthenticationTokenArgs:
     def __init__(__self__, *,
                  token: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] token: The ArgoCD access token.
+        :param pulumi.Input[str] token: Authentication Token generated through ArgoCD.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
         """
-        The ArgoCD access token.
+        Authentication Token generated through ArgoCD.
         """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
```

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/_utilities.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/area_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/area_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_auto_reviewers.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_auto_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_build_validation.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_build_validation.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_comment_resolution.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_comment_resolution.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_merge_types.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_merge_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_min_reviewers.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_min_reviewers.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_status_check.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_status_check.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/branch_policy_work_item_linking.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/branch_policy_work_item_linking.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_definition.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_definition_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_definition_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_folder.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/build_folder_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/build_folder_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_approval.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_approval.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_branch_control.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_branch_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_business_hours.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_business_hours.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_exclusive_lock.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_exclusive_lock.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/check_required_template.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/check_required_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/__init__.pyi` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/config/vars.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/elastic_pool.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/elastic_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/environment.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/environment_resource_kubernetes.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/environment_resource_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/feed.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/feed_permission.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/feed_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_agent_queue.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_agent_queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_area.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_area.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_build_definition.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_build_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_client_config.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_client_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_environment.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_feed.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_feed.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_git_repository.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_git_repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_group.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_groups.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_group.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_groups.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_identity_users.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_identity_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_iteration.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_iteration.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_pool.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_pools.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_project.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_projects.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_projects.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_repositories.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_repositories.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_securityrole_definitions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_securityrole_definitions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_service_endpoint_github.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_service_endpoint_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_azurecr.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_azurecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_npm.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_serviceendpoint_sonarcloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_team.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_teams.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_users.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/get_variable_group.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/get_variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_repository_branch.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_repository_branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/git_repository_file.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/git_repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group_entitlement.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group_entitlement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/group_membership.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/iterative_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/iterative_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/library_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/library_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/outputs.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1035,34 +1035,48 @@
         BranchPolicyStatusCheckSettingsScope.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  match_type: Optional[str] = None,
                  repository_id: Optional[str] = None,
                  repository_ref: Optional[str] = None):
+        """
+        :param str match_type: The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
+        :param str repository_id: The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
+        :param str repository_ref: The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
+        """
         if match_type is not None:
             pulumi.set(__self__, "match_type", match_type)
         if repository_id is not None:
             pulumi.set(__self__, "repository_id", repository_id)
         if repository_ref is not None:
             pulumi.set(__self__, "repository_ref", repository_ref)
 
     @property
     @pulumi.getter(name="matchType")
     def match_type(self) -> Optional[str]:
+        """
+        The match type to use when applying the policy. Supported values are `Exact` (default), `Prefix` or `DefaultBranch`.
+        """
         return pulumi.get(self, "match_type")
 
     @property
     @pulumi.getter(name="repositoryId")
     def repository_id(self) -> Optional[str]:
+        """
+        The repository ID. Needed only if the scope of the policy will be limited to a single repository. If `match_type` is `DefaultBranch`, this should not be defined.
+        """
         return pulumi.get(self, "repository_id")
 
     @property
     @pulumi.getter(name="repositoryRef")
     def repository_ref(self) -> Optional[str]:
+        """
+        The ref pattern to use for the match when `match_type` other than `DefaultBranch`. If `match_type` is `Exact`, this should be a qualified ref such as `refs/heads/master`. If `match_type` is `Prefix`, this should be a ref path such as `refs/heads/releases`.
+        """
         return pulumi.get(self, "repository_ref")
 
 
 @pulumi.output_type
 class BranchPolicyWorkItemLinkingSettings(dict):
     def __init__(__self__, *,
                  scopes: Sequence['outputs.BranchPolicyWorkItemLinkingSettingsScope']):
@@ -1375,20 +1389,30 @@
 
     def get(self, key: str, default = None) -> Any:
         BuildDefinitionFeature.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  skip_first_run: Optional[bool] = None):
+        """
+        :param bool skip_first_run: Trigger the pipeline to run after the creation. Defaults to `true`.
+               
+               > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
+        """
         if skip_first_run is not None:
             pulumi.set(__self__, "skip_first_run", skip_first_run)
 
     @property
     @pulumi.getter(name="skipFirstRun")
     def skip_first_run(self) -> Optional[bool]:
+        """
+        Trigger the pipeline to run after the creation. Defaults to `true`.
+
+        > **Note** The first run(`skip_first_run = false`) will only be triggered on create. If the first run fails, the build definition will still be marked as successfully created. A warning message indicating the inability to run pipeline will be displayed.
+        """
         return pulumi.get(self, "skip_first_run")
 
 
 @pulumi.output_type
 class BuildDefinitionPullRequestTrigger(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3166,51 +3190,51 @@
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationBasic(dict):
     def __init__(__self__, *,
                  password: str,
                  username: str):
         """
-        :param str password: The ArgoCD password.
-        :param str username: The ArgoCD user name.
+        :param str password: ArgoCD Password.
+        :param str username: ArgoCD Username.
         """
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter
     def password(self) -> str:
         """
-        The ArgoCD password.
+        ArgoCD Password.
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def username(self) -> str:
         """
-        The ArgoCD user name.
+        ArgoCD Username.
         """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ServiceendpointArgocdAuthenticationToken(dict):
     def __init__(__self__, *,
                  token: str):
         """
-        :param str token: The ArgoCD access token.
+        :param str token: Authentication Token generated through ArgoCD.
         """
         pulumi.set(__self__, "token", token)
 
     @property
     @pulumi.getter
     def token(self) -> str:
         """
-        The ArgoCD access token.
+        Authentication Token generated through ArgoCD.
         """
         return pulumi.get(self, "token")
 
 
 @pulumi.output_type
 class ServiceendpointExternaltfsAuthPersonal(dict):
     @staticmethod
```

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/pipeline_authorization.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/pipeline_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/pool.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_features.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/project_pipeline_settings.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/project_pipeline_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/provider.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/queue.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/queue.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_author_email_pattern.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_author_email_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_case_enforcement.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_case_enforcement.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_check_credentials.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_check_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_file_path_pattern.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_file_path_pattern.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_max_file_size.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_max_file_size.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_max_path_length.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_max_path_length.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/repository_policy_reserved_names.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/repository_policy_reserved_names.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/resource_authorization.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/resource_authorization.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/securityrole_assignment.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/securityrole_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_artifactory.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_artifactory.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_aws.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_aws.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_dev_ops.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_dev_ops.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_ecr.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_ecr.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_azure_rm.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_azure_rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_bit_bucket.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_bit_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_docker_registry.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_docker_registry.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_generic.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_generic.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_generic_git.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_generic_git.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_git_hub.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_git_hub.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_git_hub_enterprise.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_kubernetes.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_kubernetes.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_npm.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_npm.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_pipeline.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_service_fabric.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_service_fabric.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_sonar_cloud.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_sonar_cloud.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_sonar_qube.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_sonar_qube.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/service_endpoint_ssh.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/service_endpoint_ssh.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_argocd.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_argocd.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_externaltfs.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_externaltfs.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_gcp_terraform.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_gcp_terraform.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_incomingwebhook.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_incomingwebhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jenkins.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jenkins.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_artifactory_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_distribution_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_platform_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_jfrog_xray_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_maven.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_maven.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_nexus.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_nexus.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_nuget.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_nuget.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_octopusdeploy.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_octopusdeploy.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/serviceendpoint_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/serviceendpoint_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/servicehook_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/servicehook_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/servicehook_storage_queue_pipelines.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/servicehook_storage_queue_pipelines.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/tagging_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/tagging_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team_administrators.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team_administrators.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/team_members.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/team_members.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/user.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/variable_group.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/variable_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/variable_group_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/variable_group_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/work_item_query_permissions.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/work_item_query_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops/workitem.py` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops/workitem.py`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/PKG-INFO` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_azuredevops
-Version: 3.2.0a1716216578
+Version: 3.2.0a1716513772
 Summary: A Pulumi package for creating and managing Azure DevOps.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-azuredevops
 Keywords: pulumi,azuredevops
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pulumi_azuredevops.egg-info/SOURCES.txt` & `pulumi_azuredevops-3.2.0a1716513772/pulumi_azuredevops.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_azuredevops-3.2.0a1716216578/pyproject.toml` & `pulumi_azuredevops-3.2.0a1716513772/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_azuredevops"
   description = "A Pulumi package for creating and managing Azure DevOps."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "azuredevops"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.2.0a1716216578"
+  version = "3.2.0a1716513772"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-azuredevops"
 
 [build-system]
```

