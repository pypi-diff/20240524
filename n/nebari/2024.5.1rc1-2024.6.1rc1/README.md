# Comparing `tmp/nebari-2024.5.1rc1.tar.gz` & `tmp/nebari-2024.6.1rc1.tar.gz`

## Comparing `nebari-2024.5.1rc1.tar` & `nebari-2024.6.1rc1.tar`

### file list

```diff
@@ -1,429 +1,432 @@
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.cirun.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/MANIFEST.in
--rw-r--r--   0        0        0    88441 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/RELEASE.md
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/SECURITY.md
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/flake.lock
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/flake.nix
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/pytest.ini
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/release-notes-sync-config.yaml
--rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/actions/publish-from-template/action.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/actions/publish-from-template/render_template.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/failed-workflow-issue-templates/test-provider.md
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/generate_cli_doc.yml
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/release-notes-sync.yaml
--rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/release.yaml
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/run-precommit.yaml
--rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test-provider.yaml
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test.yaml
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_aws_integration.yaml
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_conda_build.yaml
--rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_do_integration.yaml
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_gcp_integration.yaml
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_helm_charts.yaml
--rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/test_local_integration.yaml
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.github/workflows/typing.yaml
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/Makefile
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/README.md
--rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/cli.html
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/cli.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/conf.py
--rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/docs-sphinx/index.rst
--rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/aws-force-destroy.py
--rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/aws-force-destroy.sh
--rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/helm-validate.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/scripts/keycloak-export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/__init__.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/_version.py
--rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/cli.py
--rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/config.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/constants.py
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/deploy.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/deprecate.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/destroy.py
--rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/initialize.py
--rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/keycloak.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/render.py
--rw-r--r--   0        0        0    32645 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/upgrade.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/utils.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/git.py
--rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/terraform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/__init__.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/common.py
--rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/github.py
--rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/gitlab.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cicd/linter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/__init__.py
--rw-r--r--   0        0        0    38090 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
--rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/azure_cloud.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/commons.py
--rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/digital_ocean.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/cloud/google_cloud.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/dns/__init__.py
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/dns/cloudflare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/oauth/__init__.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/provider/oauth/auth0.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/__init__.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/base.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/tf_objects.py
--rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/bootstrap/__init__.py
--rw-r--r--   0        0        0    33679 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
--rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
--rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
--rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
--rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
--rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
--rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
--rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
--rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
--rw-r--r--   0        0        0    22150 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
--rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
--rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
--rw-r--r--   0        0        0     4548 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
--rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
--rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
--rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
--rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
--rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
--rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
--rw-r--r--   0        0        0     9433 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
--rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
--rw-r--r--   0        0        0    20109 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
--rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
--rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
--rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
--rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
--rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
--rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
--rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
--rw-r--r--   0        0        0     1470 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
--rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/__init__.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
--rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/__init__.py
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/deploy.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/destroy.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/dev.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/info.py
--rw-r--r--   0        0        0    37041 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/init.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/keycloak.py
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/render.py
--rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/support.py
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/upgrade.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/_nebari/subcommands/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/__init__.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/__main__.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/hookspecs.py
--rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/plugins.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/src/nebari/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/conftest.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/__init__.py
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/config_mod_utils.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/kube_api.py
--rw-r--r--   0        0        0    16519 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/navigator.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/playwright_fixtures.py
--rw-r--r--   0        0        0    10512 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/run_notebook.py
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/notebooks/test_notebook_output.ipynb
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/common/tests/test_notebook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/constants.py
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_dask_gateway.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_grafana_api.py
--rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
--rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/test_loki_deployment.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/utils.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress.json
--rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/package-lock.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/package.json
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/.gitignore
--rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/integration/main.js
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/plugins/index.js
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/cypress/support/index.js
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/.env.tpl
--rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/README.md
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_e2e/playwright/test_playwright.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/__init__.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/conftest.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/deployment_fixtures.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_all_clouds.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_gpu.py
--rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_integration/test_preemptible.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/__init__.py
--rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/conftest.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_deploy.py
--rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_dev.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_init.py
--rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_init_repository.py
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_keycloak.py
--rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_support.py
--rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_upgrade.py
--rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_cli_validate.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_commons.py
--rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_dependencies.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_init.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_links.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_provider.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_render.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_schema.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/test_upgrade.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/utils.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
--rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-custom.yaml
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.extra-inputs.yaml
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
--rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/LICENSE
--rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/README.md
--rw-r--r--   0        0        0     3844 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/pyproject.toml
--rw-r--r--   0        0        0    12422 2020-02-02 00:00:00.000000 nebari-2024.5.1rc1/PKG-INFO
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.cirun.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/MANIFEST.in
+-rw-r--r--   0        0        0    89400 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/RELEASE.md
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/SECURITY.md
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/flake.lock
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/flake.nix
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/pytest.ini
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/release-notes-sync-config.yaml
+-rw-r--r--   0        0        0     3992 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/actions/publish-from-template/action.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/actions/publish-from-template/render_template.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/failed-workflow-issue-templates/test-provider.md
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/generate_cli_doc.yml
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/release-notes-sync.yaml
+-rw-r--r--   0        0        0     1927 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/release.yaml
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/run-precommit.yaml
+-rw-r--r--   0        0        0     6206 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test-provider.yaml
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_aws_integration.yaml
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_conda_build.yaml
+-rw-r--r--   0        0        0     2729 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_do_integration.yaml
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_gcp_integration.yaml
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_helm_charts.yaml
+-rw-r--r--   0        0        0     5981 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/test_local_integration.yaml
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.github/workflows/typing.yaml
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/Makefile
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/README.md
+-rw-r--r--   0        0        0    46502 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/cli.html
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/cli.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/conf.py
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/docs-sphinx/index.rst
+-rw-r--r--   0        0        0    14306 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/scripts/aws-force-destroy.py
+-rwxr-xr-x   0        0        0     8475 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/scripts/aws-force-destroy.sh
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/scripts/helm-validate.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/scripts/keycloak-export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/__init__.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/_version.py
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/cli.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/config.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/constants.py
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/deploy.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/deprecate.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/destroy.py
+-rw-r--r--   0        0        0    11202 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/initialize.py
+-rw-r--r--   0        0        0     5781 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/keycloak.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/render.py
+-rw-r--r--   0        0        0    36524 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/upgrade.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/utils.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/git.py
+-rw-r--r--   0        0        0     8126 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/terraform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cicd/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cicd/common.py
+-rw-r--r--   0        0        0     9739 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cicd/github.py
+-rw-r--r--   0        0        0     2106 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cicd/gitlab.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cicd/linter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/__init__.py
+-rw-r--r--   0        0        0    38090 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/amazon_web_services.py
+-rw-r--r--   0        0        0     5093 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/azure_cloud.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/commons.py
+-rw-r--r--   0        0        0     3867 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/digital_ocean.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/cloud/google_cloud.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/dns/__init__.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/dns/cloudflare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/oauth/__init__.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/provider/oauth/auth0.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/__init__.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/base.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/tf_objects.py
+-rw-r--r--   0        0        0     2997 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/bootstrap/__init__.py
+-rw-r--r--   0        0        0    33853 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/locals.tf
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf
+-rw-r--r--   0        0        0     1787 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/versions.tf
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/variables.tf
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/main.tf
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/outputs.tf
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/outputs.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/outputs.tf
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/outputs.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/outputs.tf
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/registry/variables.tf
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/main.tf
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/outputs.tf
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/s3/variables.tf
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/providers.tf
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/versions.tf
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/main.tf
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/registry/variables.tf
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/providers.tf
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/versions.tf
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/main.tf
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/variable.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/registry/versions.tf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/existing/main.tf
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/versions.tf
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/service_account.tf
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/templates/kubeconfig.yaml
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/main.tf
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/network/variables.tf
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/main.tf
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/registry/variables.tf
+-rw-r--r--   0        0        0     2497 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf
+-rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/variables.tf
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/locals.tf
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/outputs.tf
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/versions.tf
+-rw-r--r--   0        0        0     9777 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/outputs.tf
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/external-container-registry.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/locals.tf
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/versions.tf
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/variables.tf
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/main.tf
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/initialization/variables.tf
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/variables.tf
+-rw-r--r--   0        0        0    57723 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf
+-rw-r--r--   0        0        0    10148 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/main.tf
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/outputs.tf
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/versions.tf
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/outputs.tf
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/outputs.tf
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/providers.tf
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/versions.tf
+-rw-r--r--   0        0        0    22571 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/forward-auth.tf
+-rw-r--r--   0        0        0     4481 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub_ssh.tf
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/locals.tf
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/providers.tf
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/versions.tf
+-rw-r--r--   0        0        0     5460 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/outputs.tf
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/outputs.tf
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/variables.tf
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/output.tf
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/variables.tf
+-rw-r--r--   0        0        0    16354 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/values.yaml
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/versions.tf
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf
+-rw-r--r--   0        0        0     5210 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf
+-rw-r--r--   0        0        0     4560 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf
+-rw-r--r--   0        0        0     6543 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py
+-rw-r--r--   0        0        0     3917 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/outputs.tf
+-rw-r--r--   0        0        0     5567 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py
+-rw-r--r--   0        0        0    10699 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/outputs.tf
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf
+-rw-r--r--   0        0        0     3947 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/ipython/ipython_config.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/01-theme.py
+-rw-r--r--   0        0        0     2690 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py
+-rw-r--r--   0        0        0    20109 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py
+-rw-r--r--   0        0        0     5427 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/04-auth.py
+-rw-r--r--   0        0        0     4347 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bash_logout
+-rw-r--r--   0        0        0     4768 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/main.tf
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/versions.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/values.yaml
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/values.yaml
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/versions.tf
+-rw-r--r--   0        0        0    26841 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json
+-rw-r--r--   0        0        0    15913 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json
+-rw-r--r--   0        0        0    34598 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json
+-rw-r--r--   0        0        0    52146 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json
+-rw-r--r--   0        0        0    28438 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_minio.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_promtail.yaml
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/outputs.tf
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/values.yaml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/outputs.tf
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/values.yaml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/helm-extension.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/nebari-config.tf
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/providers.tf
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/versions.tf
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/main.tf
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf
+-rw-r--r--   0        0        0     9983 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/__init__.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/output.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/main.tf
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/spaces/versions.tf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/modules/terraform-state/versions.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/existing/main.tf
+-rw-r--r--   0        0        0      592 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/main.tf
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/main.tf
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/terraform-state/variables.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/local/main.tf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/__init__.py
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/deploy.py
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/destroy.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/dev.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/info.py
+-rw-r--r--   0        0        0    37041 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/init.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/keycloak.py
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/render.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/support.py
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/upgrade.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/_nebari/subcommands/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/nebari/__init__.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/nebari/__main__.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/nebari/hookspecs.py
+-rw-r--r--   0        0        0     4350 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/nebari/plugins.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/src/nebari/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/conftest.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/__init__.py
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/config_mod_utils.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/kube_api.py
+-rw-r--r--   0        0        0    17004 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/navigator.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/playwright_fixtures.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/run_notebook.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/notebooks/test_notebook_output.ipynb
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/common/tests/test_notebook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/constants.py
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/test_dask_gateway.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/test_grafana_api.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/test_jupyterhub_api.py
+-rw-r--r--   0        0        0     4101 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py
+-rw-r--r--   0        0        0     4329 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/test_loki_deployment.py
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/utils.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress.json
+-rw-r--r--   0        0        0   147508 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/package-lock.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/package.json
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress/.gitignore
+-rw-r--r--   0        0        0     2936 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress/integration/main.js
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress/plugins/index.js
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/cypress/support/index.js
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/playwright/.env.tpl
+-rw-r--r--   0        0        0     7127 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/playwright/README.md
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_e2e/playwright/test_playwright.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/__init__.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/conftest.py
+-rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/deployment_fixtures.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/test_all_clouds.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/test_gpu.py
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_integration/test_preemptible.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/__init__.py
+-rw-r--r--   0        0        0     5973 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/conftest.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_deploy.py
+-rw-r--r--   0        0        0     7261 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_dev.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_init.py
+-rw-r--r--   0        0        0     6479 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_init_repository.py
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_keycloak.py
+-rw-r--r--   0        0        0     6529 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_support.py
+-rw-r--r--   0        0        0    18509 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_upgrade.py
+-rw-r--r--   0        0        0    10490 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_cli_validate.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_commons.py
+-rw-r--r--   0        0        0     5043 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_dependencies.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_init.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_links.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_provider.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_render.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_schema.py
+-rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/test_upgrade.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/utils.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/aws.error.kubernetes-version.yaml
+-rw-r--r--   0        0        0      870 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/do.happy.yaml
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.error.authentication-type-custom.yaml
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.error.extra-inputs.yaml
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.error.project_name.ends_with_special.yaml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.error.project_name.starts_with_number.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.error.project_name.too_long.yaml
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.happy.auth0.yaml
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.happy.github.yaml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.happy.project_name.with_numbers.yaml
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.happy.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/min.happy.jupyterlab.default_settings.yaml
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/min.happy.monitoring.overrides.yaml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/cli_validate/min.happy.yaml
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-users-import.json
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/LICENSE
+-rw-r--r--   0        0        0     9814 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/README.md
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    12422 2020-02-02 00:00:00.000000 nebari-2024.6.1rc1/PKG-INFO
```

### Comparing `nebari-2024.5.1rc1/.cirun.yml` & `nebari-2024.6.1rc1/.cirun.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.pre-commit-config.yaml` & `nebari-2024.6.1rc1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     [pre-commit.ci] Apply automatic pre-commit fixes
   # this does not work on pre-commit ci
   skip: [terraform_fmt]
 
 repos:
   # general
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer
         exclude: "^docs-sphinx/cli.html"
       - id: trailing-whitespace
         exclude: "^docs-sphinx/cli.html"
       - id: check-json
       - id: check-yaml
@@ -47,21 +47,21 @@
             "--ignore-words-list=AKS,aks",
             "--write",
           ]
         language: python
 
   # python
   - repo: https://github.com/psf/black
-    rev: 24.3.0
+    rev: 24.4.2
     hooks:
       - id: black
         args: ["--line-length=88", "--exclude=/src/_nebari/template/"]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.5
+    rev: v0.4.3
     hooks:
       - id: ruff
         args: ["--fix"]
 
   - repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
@@ -69,12 +69,12 @@
         name: isort
         additional_dependencies: [toml]
         files: \.py$
         args: ["--profile", "black"]
 
   # terraform
   - repo: https://github.com/antonbabenko/pre-commit-terraform
-    rev: v1.88.4
+    rev: v1.89.1
     hooks:
       - id: terraform_fmt
         args:
           - --args=-write=true
```

### Comparing `nebari-2024.5.1rc1/CODE_OF_CONDUCT.md` & `nebari-2024.6.1rc1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/CONTRIBUTING.md` & `nebari-2024.6.1rc1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/RELEASE.md` & `nebari-2024.6.1rc1/RELEASE.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,29 @@
 <!-- Note:
 The RELEASE.md file at the root of the Nebari codebase is the source of truth for all release notes.
 If you want to update the release notes, open a PR against nebari-dev/nebari.
 This file is copied to nebari-dev/nebari-docs using a GitHub Action. -->
 
 ---
 
+### Release 2024.5.1 - May 13, 2024
+
+## What's Changed
+
+* make userscheduler run on general node group by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2415>
+* Upgrade to Pydantic V2 by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2348>
+* Pydantic2 PR fix by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2421>
+* remove redundant pydantic class, fix bug by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2426>
+* Update `python-keycloak` version pins constraints by @viniciusdc in <https://github.com/nebari-dev/nebari/pull/2435>
+* add HERA_TOKEN env var to user pods by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2438>
+* fix docs link by @Adam-D-Lewis in <https://github.com/nebari-dev/nebari/pull/2443>
+* Update allowed admin groups by @aktech in <https://github.com/nebari-dev/nebari/pull/2429>
+
+**Full Changelog**: <https://github.com/nebari-dev/nebari/compare/2024.4.1...2024.5.1>
+
 ## Release 2024.4.1 - April 20, 2024
 
 ### What's Changed
 * update azurerm version by @Adam-D-Lewis in https://github.com/nebari-dev/nebari/pull/2370
 * Get JupyterHub `groups` from Keycloak, support `oauthenticator` 16.3+ by @krassowski in https://github.com/nebari-dev/nebari/pull/2361
 * add full names for cloud providers in guided init by @exitflynn in https://github.com/nebari-dev/nebari/pull/2375
 * Add middleware to prefix JupyterHub navbar items with /hub. by @marcelovilla in https://github.com/nebari-dev/nebari/pull/2360
```

### Comparing `nebari-2024.5.1rc1/SECURITY.md` & `nebari-2024.6.1rc1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/flake.lock` & `nebari-2024.6.1rc1/flake.lock`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/flake.nix` & `nebari-2024.6.1rc1/flake.nix`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/PULL_REQUEST_TEMPLATE.md` & `nebari-2024.6.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/config.yml` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/general-issue.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/release-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md` & `nebari-2024.6.1rc1/.github/ISSUE_TEMPLATE/testing-checklist.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/actions/publish-from-template/action.yml` & `nebari-2024.6.1rc1/.github/actions/publish-from-template/action.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/generate_cli_doc.yml` & `nebari-2024.6.1rc1/.github/workflows/generate_cli_doc.yml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/release-notes-sync.yaml` & `nebari-2024.6.1rc1/.github/workflows/release-notes-sync.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/release.yaml` & `nebari-2024.6.1rc1/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/run-precommit.yaml` & `nebari-2024.6.1rc1/.github/workflows/run-precommit.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test-provider.yaml` & `nebari-2024.6.1rc1/.github/workflows/test-provider.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test.yaml` & `nebari-2024.6.1rc1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_aws_integration.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_aws_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_conda_build.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_conda_build.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_do_integration.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_do_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_gcp_integration.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_gcp_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_helm_charts.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_helm_charts.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/test_local_integration.yaml` & `nebari-2024.6.1rc1/.github/workflows/test_local_integration.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.github/workflows/typing.yaml` & `nebari-2024.6.1rc1/.github/workflows/typing.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/docs-sphinx/Makefile` & `nebari-2024.6.1rc1/docs-sphinx/Makefile`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/docs-sphinx/README.md` & `nebari-2024.6.1rc1/docs-sphinx/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/docs-sphinx/cli.html` & `nebari-2024.6.1rc1/docs-sphinx/cli.html`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/scripts/aws-force-destroy.py` & `nebari-2024.6.1rc1/scripts/aws-force-destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/scripts/aws-force-destroy.sh` & `nebari-2024.6.1rc1/scripts/aws-force-destroy.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/scripts/helm-validate.py` & `nebari-2024.6.1rc1/scripts/helm-validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/scripts/keycloak-export.py` & `nebari-2024.6.1rc1/scripts/keycloak-export.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/cli.py` & `nebari-2024.6.1rc1/src/_nebari/cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/config.py` & `nebari-2024.6.1rc1/src/_nebari/config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/constants.py` & `nebari-2024.6.1rc1/src/_nebari/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-CURRENT_RELEASE = "2024.4.1"
+CURRENT_RELEASE = "2024.5.1"
 
 # NOTE: Terraform cannot be upgraded further due to Hashicorp licensing changes
 # implemented in August 2023.
 # https://www.hashicorp.com/license-faq
 TERRAFORM_VERSION = "1.5.7"
 
 # 04-kubernetes-ingress
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/deploy.py` & `nebari-2024.6.1rc1/src/_nebari/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/destroy.py` & `nebari-2024.6.1rc1/src/_nebari/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/initialize.py` & `nebari-2024.6.1rc1/src/_nebari/initialize.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/keycloak.py` & `nebari-2024.6.1rc1/src/_nebari/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/render.py` & `nebari-2024.6.1rc1/src/_nebari/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/upgrade.py` & `nebari-2024.6.1rc1/src/_nebari/upgrade.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 import re
 import secrets
 import string
+import textwrap
 from abc import ABC
 from pathlib import Path
 from typing import Any, ClassVar, Dict
 
 import rich
 from packaging.version import Version
 from pydantic import ValidationError
@@ -769,14 +770,97 @@
                         config[provider_full_name]["node_groups"] = default_node_groups
                 except KeyError:
                     pass
 
         return config
 
 
+class Upgrade_2024_5_1(UpgradeStep):
+    version = "2024.5.1"
+
+    def _version_specific_upgrade(
+        self, config, start_version, config_filename: Path, *args, **kwargs
+    ):
+        rich.print("Ready to upgrade to Nebari version [green]2024.5.1[/green].")
+
+        return config
+
+
+class Upgrade_2024_6_1(UpgradeStep):
+    version = "2024.6.1"
+
+    def _version_specific_upgrade(
+        self, config, start_version, config_filename: Path, *args, **kwargs
+    ):
+        if (provider := config.get("provider", "")) == ProviderEnum.gcp.value:
+            provider_full_name = provider_enum_name_map[provider]
+            if not config.get(provider_full_name, {}).get("node_groups", {}):
+                try:
+                    text = textwrap.dedent(
+                        f"""
+                        The default node groups for GCP have been changed to cost efficient e2 family nodes reducing the running cost of Nebari on GCP by ~50%.
+                        This change will affect your current deployment, and will result in ~15 minutes of downtime during the upgrade step as the node groups are switched out, but shouldn't result in data loss.
+
+                        As always, make sure to backup data before upgrading.  See https://www.nebari.dev/docs/how-tos/manual-backup for more information.
+
+                        Would you like to upgrade to the cost effective node groups [purple]{config_filename}[/purple]?
+                        If not, select "N" and the old default node groups will be added to the nebari config file.
+                    """
+                    )
+                    continue_ = Prompt.ask(
+                        text,
+                        choices=["y", "N"],
+                        default="y",
+                    )
+                    if continue_ == "N":
+                        config[provider_full_name]["node_groups"] = {
+                            "general": {
+                                "instance": "n1-standard-8",
+                                "min_nodes": 1,
+                                "max_nodes": 1,
+                            },
+                            "user": {
+                                "instance": "n1-standard-4",
+                                "min_nodes": 0,
+                                "max_nodes": 5,
+                            },
+                            "worker": {
+                                "instance": "n1-standard-4",
+                                "min_nodes": 0,
+                                "max_nodes": 5,
+                            },
+                        }
+                except KeyError:
+                    pass
+            else:
+                text = textwrap.dedent(
+                    """
+                    The default node groups for GCP have been changed to cost efficient e2 family nodes reducing the running cost of Nebari on GCP by ~50%.
+                    Consider upgrading your node group instance types to the new default configuration.
+
+                    Upgrading your general node will result in ~15 minutes of downtime during the upgrade step as the node groups are switched out, but shouldn't result in data loss.
+
+                    As always, make sure to backup data before upgrading.  See https://www.nebari.dev/docs/how-tos/manual-backup for more information.
+
+                    The new default node groups instances are:
+                """
+                )
+                text += json.dumps(
+                    {
+                        "general": {"instance": "e2-highmem-4"},
+                        "user": {"instance": "e2-standard-4"},
+                        "worker": {"instance": "e2-standard-4"},
+                    },
+                    indent=4,
+                )
+                text += "\n\nHit enter to continue"
+                Prompt.ask(text)
+        return config
+
+
 __rounded_version__ = str(rounded_ver_parse(__version__))
 
 # Manually-added upgrade steps must go above this line
 if not UpgradeStep.has_step(__rounded_version__):
     # Always have a way to upgrade to the latest full version number, even if no customizations
     # Don't let dev/prerelease versions cloud things
     class UpgradeLatest(UpgradeStep):
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/utils.py` & `nebari-2024.6.1rc1/src/_nebari/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/version.py` & `nebari-2024.6.1rc1/src/_nebari/version.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/git.py` & `nebari-2024.6.1rc1/src/_nebari/provider/git.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/terraform.py` & `nebari-2024.6.1rc1/src/_nebari/provider/terraform.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cicd/github.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cicd/github.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cicd/gitlab.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cicd/gitlab.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cicd/linter.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cicd/linter.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cloud/amazon_web_services.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cloud/amazon_web_services.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cloud/azure_cloud.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cloud/azure_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cloud/digital_ocean.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cloud/digital_ocean.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/cloud/google_cloud.py` & `nebari-2024.6.1rc1/src/_nebari/provider/cloud/google_cloud.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/dns/cloudflare.py` & `nebari-2024.6.1rc1/src/_nebari/provider/dns/cloudflare.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/provider/oauth/auth0.py` & `nebari-2024.6.1rc1/src/_nebari/provider/oauth/auth0.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/base.py` & `nebari-2024.6.1rc1/src/_nebari/stages/base.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/tf_objects.py` & `nebari-2024.6.1rc1/src/_nebari/stages/tf_objects.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/bootstrap/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/bootstrap/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
     resource_group_name: str
     node_resource_group_name: str
     vnet_subnet_id: Optional[str] = None
     private_cluster_enabled: bool
     tags: Dict[str, str] = {}
     max_pods: Optional[int] = None
     network_profile: Optional[Dict[str, str]] = None
+    workload_identity_enabled: bool = False
 
 
 class AWSNodeGroupInputVars(schema.Base):
     name: str
     instance_type: str
     gpu: bool = False
     min_size: int
@@ -310,17 +311,17 @@
     max_nodes: Annotated[int, Field(ge=1)] = 1
     preemptible: bool = False
     labels: Dict[str, str] = {}
     guest_accelerators: List[GCPGuestAccelerator] = []
 
 
 DEFAULT_GCP_NODE_GROUPS = {
-    "general": GCPNodeGroup(instance="n1-standard-8", min_nodes=1, max_nodes=1),
-    "user": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
-    "worker": GCPNodeGroup(instance="n1-standard-4", min_nodes=0, max_nodes=5),
+    "general": GCPNodeGroup(instance="e2-highmem-4", min_nodes=1, max_nodes=1),
+    "user": GCPNodeGroup(instance="e2-standard-4", min_nodes=0, max_nodes=5),
+    "worker": GCPNodeGroup(instance="e2-standard-4", min_nodes=0, max_nodes=5),
 }
 
 
 class GoogleCloudPlatformProvider(schema.Base):
     region: str
     project: str
     kubernetes_version: str
@@ -376,14 +377,15 @@
     storage_account_postfix: str
     vnet_subnet_id: Optional[str] = None
     private_cluster_enabled: bool = False
     resource_group_name: Optional[str] = None
     tags: Optional[Dict[str, str]] = {}
     network_profile: Optional[Dict[str, str]] = None
     max_pods: Optional[int] = None
+    workload_identity_enabled: bool = False
 
     @model_validator(mode="before")
     @classmethod
     def _check_credentials(cls, data: Any) -> Any:
         azure_cloud.check_credentials()
         return data
 
@@ -777,14 +779,15 @@
                     suffix=AZURE_NODE_RESOURCE_GROUP_SUFFIX,
                 ),
                 vnet_subnet_id=self.config.azure.vnet_subnet_id,
                 private_cluster_enabled=self.config.azure.private_cluster_enabled,
                 tags=self.config.azure.tags,
                 network_profile=self.config.azure.network_profile,
                 max_pods=self.config.azure.max_pods,
+                workload_identity_enabled=self.config.azure.workload_identity_enabled,
             ).model_dump()
         elif self.config.provider == schema.ProviderEnum.aws:
             return AWSInputVars(
                 name=self.config.escaped_project_name,
                 environment=self.config.namespace,
                 existing_subnet_ids=self.config.amazon_web_services.existing_subnet_ids,
                 existing_security_group_id=self.config.amazon_web_services.existing_security_group_id,
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/accounting/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/efs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kafka/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/autoscaling.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/policy.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/network/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/permissions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/users.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/aws/modules/rds/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/main.tf`

 * *Files 6% similar despite different names*

```diff
@@ -36,10 +36,11 @@
       name          = name
       auto_scale    = true
       instance_type = config.instance
       min_size      = config.min_nodes
       max_size      = config.max_nodes
     }
   ]
-  vnet_subnet_id          = var.vnet_subnet_id
-  private_cluster_enabled = var.private_cluster_enabled
+  vnet_subnet_id            = var.vnet_subnet_id
+  private_cluster_enabled   = var.private_cluster_enabled
+  workload_identity_enabled = var.workload_identity_enabled
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 output "kubernetes_credentials" {
   description = "Parameters needed to connect to kubernetes cluster"
   sensitive   = true
   value = {
-    username               = module.kubernetes.credentials.username
-    password               = module.kubernetes.credentials.password
-    client_certificate     = module.kubernetes.credentials.client_certificate
-    client_key             = module.kubernetes.credentials.client_key
-    cluster_ca_certificate = module.kubernetes.credentials.cluster_ca_certificate
     host                   = module.kubernetes.credentials.endpoint
+    cluster_ca_certificate = module.kubernetes.credentials.cluster_ca_certificate
+    token                  = module.kubernetes.credentials.token
   }
 }
 
 resource "local_file" "kubeconfig" {
   count = var.kubeconfig_filename != null ? 1 : 0
 
   content  = module.kubernetes.kubeconfig
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/variables.tf`

 * *Files 3% similar despite different names*

```diff
@@ -72,7 +72,13 @@
 }
 
 variable "max_pods" {
   description = "Maximum number of pods that can run on a node"
   type        = number
   default     = 60
 }
+
+variable "workload_identity_enabled" {
+  description = "Enable Workload Identity"
+  type        = bool
+  default     = false
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/main.tf`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs/resources/kubernetes_cluster
 resource "azurerm_kubernetes_cluster" "main" {
   name                = var.name
   location            = var.location
   resource_group_name = var.resource_group_name
   tags                = var.tags
 
+  # To enable Azure AD Workload Identity oidc_issuer_enabled must be set to true.
+  oidc_issuer_enabled       = var.workload_identity_enabled
+  workload_identity_enabled = var.workload_identity_enabled
+
   # DNS prefix specified when creating the managed cluster. Changing this forces a new resource to be created.
   dns_prefix = "Nebari" # required
 
   # Azure requires that a new, non-existent Resource Group is used, as otherwise the provisioning of the Kubernetes Service will fail.
   node_resource_group     = var.node_resource_group_name
   private_cluster_enabled = var.private_cluster_enabled
 
@@ -35,14 +39,17 @@
     max_pods            = var.max_pods
     # node_labels          = var.node_labels
     orchestrator_version = var.kubernetes_version
     node_labels = {
       "azure-node-pool" = var.node_groups[0].name
     }
     tags = var.tags
+
+    # temparory_name_for_rotation must be <= 12 characters
+    temporary_name_for_rotation = "${substr(var.node_groups[0].name, 0, 9)}tmp"
   }
 
   sku_tier = "Free" # "Free" [Default] or "Paid"
 
   identity {
     type = "SystemAssigned" # "UserAssigned" or "SystemAssigned".  SystemAssigned identity lifecycles are tied to the AKS Cluster.
   }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/azure/modules/kubernetes/variables.tf`

 * *Files 4% similar despite different names*

```diff
@@ -66,7 +66,13 @@
 }
 
 variable "max_pods" {
   description = "Maximum number of pods that can run on a node"
   type        = number
   default     = 60
 }
+
+variable "workload_identity_enabled" {
+  description = "Enable Workload Identity"
+  type        = bool
+  default     = false
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/do/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/locals.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/gcp/modules/kubernetes/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/metallb.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/infrastructure/template/local/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_ingress/template/modules/kubernetes/ingress/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/cluster-autoscaler/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/extcr/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/aws-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/nvidia-installer/gcp-nvidia-installer.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_initialize/template/modules/traefik_crds/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak/template/modules/kubernetes/keycloak-helm/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/permissions.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/social_auth.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_keycloak_configuration/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from nebari.hookspecs import NebariStage, hookimpl
 
 # check and retry settings
 NUM_ATTEMPTS = 10
 TIMEOUT = 10  # seconds
 
 
+_forwardauth_middleware_name = "traefik-forward-auth"
+
+
 @schema.yaml_object(schema.yaml)
 class AccessEnum(str, enum.Enum):
     all = "all"
     yaml = "yaml"
     keycloak = "keycloak"
 
     @classmethod
@@ -323,14 +326,16 @@
 class KubernetesServicesInputVars(schema.Base):
     name: str
     environment: str
     endpoint: str
     realm_id: str
     node_groups: Dict[str, Dict[str, str]]
     jupyterhub_logout_redirect_url: str = Field(alias="jupyterhub-logout-redirect-url")
+    forwardauth_middleware_name: str = _forwardauth_middleware_name
+    cert_secret_name: Optional[str] = None
 
 
 def _split_docker_image_name(image_name):
     name, tag = image_name.split(":")
     return {"name": name, "tag": tag}
 
 
@@ -379,14 +384,15 @@
     jupyterlab_preferred_dir: Optional[str] = Field(alias="jupyterlab-preferred-dir")
 
 
 class DaskGatewayInputVars(schema.Base):
     dask_worker_image: ImageNameTag = Field(alias="dask-worker-image")
     dask_gateway_profiles: Dict[str, Any] = Field(alias="dask-gateway-profiles")
     cloud_provider: str = Field(alias="cloud-provider")
+    forwardauth_middleware_name: str = _forwardauth_middleware_name
 
 
 class MonitoringInputVars(schema.Base):
     monitoring_enabled: bool = Field(alias="monitoring-enabled")
     minio_enabled: bool = Field(alias="minio-enabled")
     grafana_loki_overrides: List[str] = Field(alias="grafana-loki-overrides")
     grafana_promtail_overrides: List[str] = Field(alias="grafana-promtail-overrides")
@@ -482,14 +488,19 @@
         kubernetes_services_vars = KubernetesServicesInputVars(
             name=self.config.project_name,
             environment=self.config.namespace,
             endpoint=domain,
             realm_id=realm_id,
             node_groups=stage_outputs["stages/02-infrastructure"]["node_selectors"],
             jupyterhub_logout_redirect_url=final_logout_uri,
+            cert_secret_name=(
+                self.config.certificate.secret_name
+                if self.config.certificate.type == "existing"
+                else None
+            ),
         )
 
         conda_store_vars = CondaStoreInputVars(
             conda_store_environments={
                 k: v.model_dump() for k, v in self.config.environments.items()
             },
             conda_store_default_namespace=self.config.conda_store.default_namespace,
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/argo-workflows.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/conda-store.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/dask_gateway.tf`

 * *Files 4% similar despite different names*

```diff
@@ -36,8 +36,10 @@
   conda-store-api-token         = module.kubernetes-conda-store-server.service-tokens.dask-gateway
   conda-store-service-name      = module.kubernetes-conda-store-server.service_name
 
   # profiles
   profiles = var.dask-gateway-profiles
 
   cloud-provider = var.cloud-provider
+
+  forwardauth_middleware_name = var.forwardauth_middleware_name
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/jupyterhub.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/monitoring.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/outputs.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/main.tf`

 * *Files 22% similar despite different names*

```diff
@@ -55,15 +55,27 @@
         }
       }
 
       spec {
         node_selector = {
           "${var.node-group.key}" = var.node-group.value
         }
-
+        dynamic "volume" {
+          for_each = var.cert_secret_name == null ? [] : [1]
+          content {
+            name = "cert-volume"
+            secret {
+              secret_name = var.cert_secret_name
+              items {
+                key  = "tls.crt"
+                path = "tls.crt"
+              }
+            }
+          }
+        }
         container {
           # image = "thomseddon/traefik-forward-auth:2.2.0"
           # Use PR #159 https://github.com/thomseddon/traefik-forward-auth/pull/159
           image = "maxisme/traefik-forward-auth:sha-a98e568"
           name  = "forwardauth-container"
 
           env {
@@ -121,18 +133,34 @@
           }
 
           env {
             name  = "COOKIE_DOMAIN"
             value = var.external-url
           }
 
+          dynamic "env" {
+            for_each = var.cert_secret_name == null ? [] : [1]
+            content {
+              name  = "SSL_CERT_FILE"
+              value = "/config/tls.crt"
+            }
+          }
+
           port {
             container_port = 4181
           }
 
+          dynamic "volume_mount" {
+            for_each = var.cert_secret_name == null ? [] : [1]
+            content {
+              name       = "cert-volume"
+              mount_path = "/config"
+              read_only  = true
+            }
+          }
         }
 
       }
     }
   }
 }
 
@@ -140,20 +168,20 @@
   # This version of the middleware is primarily for the forwardauth service
   # itself, so the callback _oauth url can be centalised (not just under for example /someservice/_oauth).
   # This middleware is in the root namespace, someservice may have its own.
   manifest = {
     apiVersion = "traefik.containo.us/v1alpha1"
     kind       = "Middleware"
     metadata = {
-      name      = "traefik-forward-auth"
+      name      = var.forwardauth_middleware_name
       namespace = var.namespace
     }
     spec = {
       forwardAuth = {
-        address = "http://forwardauth-service:4181"
+        address = "http://${kubernetes_service.forwardauth-service.metadata.0.name}:4181"
         authResponseHeaders = [
           "X-Forwarded-User"
         ]
       }
     }
   }
 }
@@ -171,15 +199,15 @@
       routes = [
         {
           kind  = "Rule"
           match = "Host(`${var.external-url}`) && PathPrefix(`${var.callback-url-path}`)"
 
           middlewares = [
             {
-              name      = "traefik-forward-auth"
+              name      = kubernetes_manifest.forwardauth-middleware.manifest.metadata.name
               namespace = var.namespace
             }
           ]
 
           services = [
             {
               name = kubernetes_service.forwardauth-service.metadata.0.name
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/forwardauth/variables.tf`

 * *Files 21% similar despite different names*

```diff
@@ -22,7 +22,17 @@
 variable "node-group" {
   description = "Node key value pair for bound general resources"
   type = object({
     key   = string
     value = string
   })
 }
+
+variable "forwardauth_middleware_name" {
+  description = "Name of the traefik forward auth middleware"
+  type        = string
+}
+
+variable "cert_secret_name" {
+  description = "Name of the secret containing the certificate"
+  type        = string
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-mount/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/nfs-server/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/argo-workflows/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/output.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/server.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/storage.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/worker.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/conda-store/config/conda_store_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/controler.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/crds.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/gateway.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/middleware.tf`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
       name      = "nebari-dask-gateway-chain" # Updated name to -chain from -cluster to avoid upgrade confusion
       namespace = var.namespace
     }
     spec = {
       chain = {
         middlewares = [
           {
-            name      = "traefik-forward-auth"
+            name      = var.forwardauth_middleware_name
             namespace = var.namespace
           },
           {
             name      = kubernetes_manifest.cluster-middleware-stripprefix.manifest.metadata.name
             namespace = var.namespace
           }
         ]
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/variables.tf`

 * *Files 1% similar despite different names*

```diff
@@ -200,7 +200,11 @@
   type        = string
 }
 
 variable "cloud-provider" {
   description = "Name of the cloud provider to deploy to."
   type        = string
 }
+
+variable "forwardauth_middleware_name" {
+  type = string
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/controller_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/dask-gateway/files/gateway_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/configmaps.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/main.tf`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 resource "helm_release" "jupyterhub" {
   name      = "jupyterhub-${var.namespace}"
   namespace = var.namespace
 
   repository = "https://jupyterhub.github.io/helm-chart/"
   chart      = "jupyterhub"
-  version    = "3.2.1"
+  version    = "4.0.0-0.dev.git.6607.hd1a1130e"
 
   values = concat([
     file("${path.module}/values.yaml"),
     jsonencode({
       # custom values can be accessed via z2jh.get_config('custom.<path>')
       custom = {
         namespace                     = var.namespace
@@ -126,46 +126,47 @@
           name      = "conda-store-shared"
         }]
 
         extraConfig = {
           "01-theme.py"    = file("${path.module}/files/jupyterhub/01-theme.py")
           "02-spawner.py"  = file("${path.module}/files/jupyterhub/02-spawner.py")
           "03-profiles.py" = file("${path.module}/files/jupyterhub/03-profiles.py")
+          "04-auth.py"     = file("${path.module}/files/jupyterhub/04-auth.py")
         }
 
         services = {
           for service in var.services : service => {
             name      = service
             admin     = true
             api_token = random_password.service_token[service].result
           }
         }
 
         # for simple key value configuration with jupyterhub traitlets
         # this hub.config property should be used
         config = {
-          JupyterHub = {
-            authenticator_class = "generic-oauth"
-          }
           Authenticator = {
             enable_auth_state = true
           }
-          GenericOAuthenticator = {
+          KeyCloakOAuthenticator = {
             client_id            = module.jupyterhub-openid-client.config.client_id
             client_secret        = module.jupyterhub-openid-client.config.client_secret
             oauth_callback_url   = "https://${var.external-url}/hub/oauth_callback"
             authorize_url        = module.jupyterhub-openid-client.config.authentication_url
             token_url            = module.jupyterhub-openid-client.config.token_url
             userdata_url         = module.jupyterhub-openid-client.config.userinfo_url
+            realm_api_url        = module.jupyterhub-openid-client.config.realm_api_url
             login_service        = "Keycloak"
             username_claim       = "preferred_username"
             claim_groups_key     = "groups"
+            claim_roles_key      = "roles"
             allowed_groups       = ["/analyst", "/developer", "/admin", "jupyterhub_admin", "jupyterhub_developer"]
             admin_groups         = ["/admin", "jupyterhub_admin"]
             manage_groups        = true
+            manage_roles         = true
             refresh_pre_spawn    = true
             validate_server_cert = false
 
             # deprecated, to be removed (replaced by validate_server_cert)
             tls_verify = false
             # deprecated, to be removed (replaced by username_claim)
             username_key = "preferred_username"
@@ -279,14 +280,18 @@
     "analyst"   = ["jupyterhub_developer"]
   }
   callback-url-paths = [
     "https://${var.external-url}/hub/oauth_callback",
     var.jupyterhub-logout-redirect-url
   ]
   jupyterlab_profiles_mapper = true
+  service-accounts-enabled   = true
+  service-account-roles = [
+    "view-realm", "view-users", "view-clients"
+  ]
 }
 
 
 resource "kubernetes_secret" "argo-workflows-conda-store-token" {
   metadata {
     name      = "argo-workflows-conda-store-token"
     namespace = var.namespace
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/middleware.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/values.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/extras/git_clone_update.sh`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_jupyterlab_pioneer_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyter/jupyter_server_config.py.tpl`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/02-spawner.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,14 @@
             "name": name,
             "display": True,
             "info": {
                 "name": name,
                 "url": url,
                 "external": True,
             },
-            "oauth_no_confirm": True,
         }
 
     c.JupyterHub.services.extend(
         [
             service_for_jhub_apps(name="Argo", url="/argo"),
             service_for_jhub_apps(name="Users", url="/auth/admin/nebari/console/"),
             service_for_jhub_apps(name="Environments", url="/conda-store"),
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterhub/03-profiles.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/jupyterlab/overrides.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.bashrc`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub/files/skel/.profile`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/sftp.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/ssh.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/jupyterhub-ssh/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/outputs.tf`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 output "config" {
   description = "configuration credentials for connecting to openid client"
   value = {
-    client_id     = keycloak_openid_client.main.client_id
-    client_secret = keycloak_openid_client.main.client_secret
+    client_id               = keycloak_openid_client.main.client_id
+    client_secret           = keycloak_openid_client.main.client_secret
+    service_account_user_id = keycloak_openid_client.main.service_account_user_id
 
     authentication_url = "https://${var.external-url}/auth/realms/${var.realm_id}/protocol/openid-connect/auth"
     token_url          = "https://${var.external-url}/auth/realms/${var.realm_id}/protocol/openid-connect/token"
     userinfo_url       = "https://${var.external-url}/auth/realms/${var.realm_id}/protocol/openid-connect/userinfo"
+    realm_api_url      = "https://${var.external-url}/auth/admin/realms/${var.realm_id}"
     callback_urls      = var.callback-url-paths
   }
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,47 @@
-variable "realm_id" {
-  description = "Keycloak realm_id"
+variable "namespace" {
+  description = "deploy monitoring services on this namespace"
   type        = string
+  default     = "dev"
 }
 
 
-variable "client_id" {
-  description = "OpenID Client ID"
+variable "external-url" {
+  description = "External url that jupyterhub cluster is accessible"
   type        = string
 }
 
 
-variable "external-url" {
-  description = "External url for keycloak auth endpoint"
+variable "realm_id" {
+  description = "Keycloak realm for creating oauth client"
   type        = string
 }
 
 
-variable "role_mapping" {
-  description = "Group to role mapping to establish for client"
-  type        = map(list(string))
-  default     = {}
+variable "dashboards" {
+  description = "Enabled grafana dashboards"
+  type        = set(string)
+  default = [
+    "Main",
+  ]
 }
 
+variable "jupyterhub_api_token" {
+  type      = string
+  default   = ""
+  sensitive = true
+}
 
-variable "callback-url-paths" {
-  description = "URLs to use for openid callback"
-  type        = list(string)
+variable "node-group" {
+  description = "Node key value pair for bound resources"
+  type = object({
+    key   = string
+    value = string
+  })
 }
 
-variable "jupyterlab_profiles_mapper" {
-  description = "Create a mapper for jupyterlab_profiles group/user attributes"
-  type        = bool
-  default     = false
+
+variable "overrides" {
+  description = "Grafana helm chart overrides"
+  type        = list(string)
+  default     = []
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/minio/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/keycloak-client/variables.tf`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-variable "namespace" {
-  description = "deploy monitoring services on this namespace"
+variable "realm_id" {
+  description = "Keycloak realm_id"
   type        = string
-  default     = "dev"
 }
 
 
-variable "external-url" {
-  description = "External url that jupyterhub cluster is accessible"
+variable "client_id" {
+  description = "OpenID Client ID"
   type        = string
 }
 
 
-variable "realm_id" {
-  description = "Keycloak realm for creating oauth client"
+variable "external-url" {
+  description = "External url for keycloak auth endpoint"
   type        = string
 }
 
 
-variable "dashboards" {
-  description = "Enabled grafana dashboards"
-  type        = set(string)
-  default = [
-    "Main",
-  ]
+variable "service-accounts-enabled" {
+  description = "Whether the client should have a service account created"
+  type        = bool
+  default     = false
 }
 
-variable "jupyterhub_api_token" {
-  type      = string
-  default   = ""
-  sensitive = true
+variable "service-account-roles" {
+  description = "Roles to be granted to the service account. Requires setting service-accounts-enabled to true."
+  type        = list(string)
+  default     = []
 }
 
-variable "node-group" {
-  description = "Node key value pair for bound resources"
-  type = object({
-    key   = string
-    value = string
-  })
+
+variable "role_mapping" {
+  description = "Group to role mapping to establish for client"
+  type        = map(list(string))
+  default     = {}
 }
 
 
-variable "overrides" {
-  description = "Grafana helm chart overrides"
+variable "callback-url-paths" {
+  description = "URLs to use for openid callback"
   type        = list(string)
-  default     = []
+}
+
+variable "jupyterlab_profiles_mapper" {
+  description = "Create a mapper for jupyterlab_profiles group/user attributes"
+  type        = bool
+  default     = false
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/cluster_information.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/conda_store.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/jupyterhub_dashboard.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/keycloak.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/traefik.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/dashboards/Main/usage_report.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/values_loki.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/monitoring/loki/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/postgresql/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/kubernetes_services/template/modules/kubernetes/services/redis/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -68,13 +68,16 @@
             ]["value"],
             "tf_extensions": [_.model_dump() for _ in self.config.tf_extensions],
             "nebari_config_yaml": self.config.model_dump(),
             "keycloak_nebari_bot_password": stage_outputs[
                 "stages/05-kubernetes-keycloak"
             ]["keycloak_nebari_bot_password"]["value"],
             "helm_extensions": [_.model_dump() for _ in self.config.helm_extensions],
+            "forwardauth_middleware_name": stage_outputs[
+                "stages/07-kubernetes-services"
+            ]["forward-auth-middleware"]["value"]["name"],
         }
 
 
 @hookimpl
 def nebari_stage() -> List[Type[NebariStage]]:
     return [NebariTFExtensionsStage]
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/tf-extensions.tf`

 * *Files 20% similar despite different names*

```diff
@@ -12,10 +12,11 @@
   keycloakadmin    = lookup(each.value, "keycloakadmin", false)
   jwt              = lookup(each.value, "jwt", false)
   nebariconfigyaml = lookup(each.value, "nebariconfigyaml", false)
   external-url     = var.endpoint
   nebari-realm-id  = var.realm_id
 
   keycloak_nebari_bot_password = each.value.keycloakadmin ? var.keycloak_nebari_bot_password : ""
+  forwardauth_middleware_name  = var.forwardauth_middleware_name
 
   envs = lookup(each.value, "envs", [])
 }
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/variables.tf`

 * *Files 25% similar despite different names*

```diff
@@ -27,7 +27,12 @@
   description = "Helm Extensions"
   default     = []
 }
 
 variable "keycloak_nebari_bot_password" {
   description = "Keycloak password for nebari-bot"
 }
+
+variable "forwardauth_middleware_name" {
+  description = "Name of the traefik forward auth middleware"
+  type        = string
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/helm-extensions/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/ingress.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/keycloak-config.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/locals.tf`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 locals {
   middlewares = (var.private) ? ([{
-    name      = "traefik-forward-auth"
+    name      = var.forwardauth_middleware_name
     namespace = var.namespace
   }]) : ([])
 
   oauth2client_envs = (var.oauth2client) ? ([{
     name  = "OAUTH2_AUTHORIZE_URL"
     value = "https://${var.external-url}/auth/realms/${var.nebari-realm-id}/protocol/openid-connect/auth"
     },
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/nebari_tf_extensions/template/modules/nebariextension/variables.tf`

 * *Files 15% similar despite different names*

```diff
@@ -66,7 +66,12 @@
 }
 
 variable "keycloak_nebari_bot_password" {
   description = "Keycloak client password"
   type        = string
   default     = ""
 }
+
+variable "forwardauth_middleware_name" {
+  description = "Name of the traefik forward auth middleware"
+  type        = string
+}
```

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/__init__.py` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/__init__.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/aws/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/azure/modules/terraform-state/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/do/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/main.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf` & `nebari-2024.6.1rc1/src/_nebari/stages/terraform_state/template/gcp/modules/gcs/variables.tf`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/deploy.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/destroy.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/destroy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/dev.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/info.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/init.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/keycloak.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/render.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/support.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/upgrade.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/_nebari/subcommands/validate.py` & `nebari-2024.6.1rc1/src/_nebari/subcommands/validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/nebari/hookspecs.py` & `nebari-2024.6.1rc1/src/nebari/hookspecs.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/nebari/plugins.py` & `nebari-2024.6.1rc1/src/nebari/plugins.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/src/nebari/schema.py` & `nebari-2024.6.1rc1/src/nebari/schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/utils.py` & `nebari-2024.6.1rc1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/common/config_mod_utils.py` & `nebari-2024.6.1rc1/tests/common/config_mod_utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/common/kube_api.py` & `nebari-2024.6.1rc1/tests/common/kube_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/common/navigator.py` & `nebari-2024.6.1rc1/tests/common/navigator.py`

 * *Files 3% similar despite different names*

```diff
@@ -252,15 +252,15 @@
         popup = self._check_for_kernel_popup()
 
         # server is on running and there is a popup
         if popup:
             self._set_environment_via_popup(kernel=None)
 
         # go to Kernel menu
-        kernel_menuitem = self.page.get_by_text("Kernel", exact=True)
+        kernel_menuitem = self.page.get_by_role("menuitem", name="Kernel", exact=True)
         kernel_menuitem.click()
         # shut down multiple running kernels
         with contextlib.suppress(Exception):
             shut_down_all = self.page.get_by_text(
                 "Shut Down All Kernels...", exact=True
             )
             shut_down_all.wait_for(timeout=300, state="attached")
@@ -316,22 +316,31 @@
                     "button", name="No Kernel"
                 ).wait_for(timeout=300, state="attached")
         else:
             # set the environment
             # failure here indicates that the environment doesn't exist either
             # because of incorrect naming syntax or because the env is still
             # being built
-            self.page.get_by_role("combobox").nth(1).select_option(kernel)
-            # click Select to close popup (deal with the two formats of this dialog)
-            try:
-                self.page.get_by_role("button", name="Select Kernel").click()
-            except Exception:
-                self.page.locator("div").filter(has_text="No KernelSelect").get_by_role(
-                    "button", name="Select Kernel"
-                ).click()
+
+            new_launcher_popup = self.page.locator(
+                ".jp-KernelSelector-Dialog .jp-NewLauncher-table table"
+            ).nth(0)
+            if new_launcher_popup.is_visible():
+                # for when the jupyterlab-new-launcher extension is installed
+                new_launcher_popup.locator("td").nth(0).click()
+            else:
+                # for when only the native launcher is available
+                self.page.get_by_role("combobox").nth(1).select_option(kernel)
+                # click Select to close popup (deal with the two formats of this dialog)
+                try:
+                    self.page.get_by_role("button", name="Select Kernel").click()
+                except Exception:
+                    self.page.locator("div").filter(
+                        has_text="No KernelSelect"
+                    ).get_by_role("button", name="Select Kernel").click()
 
     def set_environment(self, kernel):
         """Set environment of a jupyter notebook.
 
         IMPORTANT: The focus MUST be on the notebook on which you want to set
         the environment.
 
@@ -346,15 +355,15 @@
         -------
         None
         """
 
         popup = self._check_for_kernel_popup()
         # if there is not a kernel popup, make it appear
         if not popup:
-            self.page.get_by_text("Kernel", exact=True).click()
+            self.page.get_by_role("menuitem", name="Kernel", exact=True).click()
             self.page.get_by_role("menuitem", name="Change Kernel…").get_by_text(
                 "Change Kernel…"
             ).click()
 
         self._set_environment_via_popup(kernel)
 
         # wait for the jupyter UI to catch up before moving forward
```

### Comparing `nebari-2024.5.1rc1/tests/common/playwright_fixtures.py` & `nebari-2024.6.1rc1/tests/common/playwright_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/common/run_notebook.py` & `nebari-2024.6.1rc1/tests/common/run_notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,15 @@
     def _get_outputs(self) -> List[str]:
         output_elements = self.nav.page.query_selector_all(".jp-OutputArea-output")
         text_content = [element.text_content().strip() for element in output_elements]
         return text_content
 
     def _restart_run_all(self):
         # restart run all cells
-        self.nav.page.get_by_text("Kernel", exact=True).click()
+        self.nav.page.get_by_role("menuitem", name="Kernel", exact=True).click()
         self.nav.page.get_by_role(
             "menuitem", name="Restart Kernel and Run All Cells…"
         ).get_by_text("Restart Kernel and Run All Cells…").click()
 
         # Restart dialog appears most, but not all of the time (e.g. set
         # No Kernel, then Restart Run All)
         restart_dialog_button = self.nav.page.get_by_role(
```

### Comparing `nebari-2024.5.1rc1/tests/common/notebooks/test_notebook_output.ipynb` & `nebari-2024.6.1rc1/tests/common/notebooks/test_notebook_output.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/common/tests/test_notebook.py` & `nebari-2024.6.1rc1/tests/common/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/test_dask_gateway.py` & `nebari-2024.6.1rc1/tests/tests_deployment/test_dask_gateway.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/test_grafana_api.py` & `nebari-2024.6.1rc1/tests/tests_deployment/test_grafana_api.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py` & `nebari-2024.6.1rc1/tests/tests_deployment/test_jupyterhub_ssh.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/test_loki_deployment.py` & `nebari-2024.6.1rc1/tests/tests_deployment/test_loki_deployment.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/utils.py` & `nebari-2024.6.1rc1/tests/tests_deployment/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     if xsrf_token:
         headers["X-XSRFToken"] = xsrf_token
     data = {"note": note, "expires_in": None}
     r = session.post(
         f"https://{constants.NEBARI_HOSTNAME}/hub/api/users/{constants.KEYCLOAK_USERNAME}/tokens",
         headers=headers,
         json=data,
+        verify=False,
     )
 
     return r.json()["token"]
 
 
 def monkeypatch_ssl_context():
     """
```

### Comparing `nebari-2024.5.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb` & `nebari-2024.6.1rc1/tests/tests_deployment/assets/notebook/simple.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/package-lock.json` & `nebari-2024.6.1rc1/tests/tests_e2e/package-lock.json`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/cypress/integration/main.js` & `nebari-2024.6.1rc1/tests/tests_e2e/cypress/integration/main.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -50,16 +50,16 @@
 
             cy.get('#start')
                 .should('contain', 'My Server').click();
 
             cy.get('h1')
                 .should('contain', 'Server Options');
 
-            cy.get('input.btn.btn-jupyter')
-                .should('have.attr', 'value', 'Start').click();
+            cy.get('button.btn.btn-jupyter')
+                .should('contain', 'Start').click();
 
             // Minimal check that JupyterLab has opened
             cy.get('div#jp-MainLogo', {
                 timeout: 60000
             }).should('exist').wait(4000);
 
             // Click VS Code Launcher exists
```

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb` & `nebari-2024.6.1rc1/tests/tests_e2e/cypress/notebooks/BasicTest.ipynb`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/cypress/plugins/index.js` & `nebari-2024.6.1rc1/tests/tests_e2e/cypress/plugins/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/cypress/support/index.js` & `nebari-2024.6.1rc1/tests/tests_e2e/cypress/support/index.js`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/playwright/README.md` & `nebari-2024.6.1rc1/tests/tests_e2e/playwright/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_e2e/playwright/test_playwright.py` & `nebari-2024.6.1rc1/tests/tests_e2e/playwright/test_playwright.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_integration/README.md` & `nebari-2024.6.1rc1/tests/tests_integration/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_integration/deployment_fixtures.py` & `nebari-2024.6.1rc1/tests/tests_integration/deployment_fixtures.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_integration/test_all_clouds.py` & `nebari-2024.6.1rc1/tests/tests_integration/test_all_clouds.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_integration/test_gpu.py` & `nebari-2024.6.1rc1/tests/tests_integration/test_gpu.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_integration/test_preemptible.py` & `nebari-2024.6.1rc1/tests/tests_integration/test_preemptible.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/conftest.py` & `nebari-2024.6.1rc1/tests/tests_unit/conftest.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_deploy.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_deploy.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_dev.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_dev.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_init.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_init_repository.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_init_repository.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_keycloak.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_keycloak.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_support.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_support.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_upgrade.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_cli_validate.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_cli_validate.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_commons.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_commons.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_config.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_config.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_dependencies.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_init.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_init.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_provider.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_provider.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_render.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_render.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_schema.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/test_upgrade.py` & `nebari-2024.6.1rc1/tests/tests_unit/test_upgrade.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/utils.py` & `nebari-2024.6.1rc1/tests/tests_unit/utils.py`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/cli_validate/aws.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/cli_validate/azure.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/do.happy.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/cli_validate/do.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/cli_validate/gcp.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/cli_validate/local.happy.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/cli_validate/local.happy.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310-customauth.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml` & `nebari-2024.6.1rc1/tests/tests_unit/qhub-config-yaml-files-for-upgrade/qhub-config-do-310.yaml`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/.gitignore` & `nebari-2024.6.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/LICENSE` & `nebari-2024.6.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/README.md` & `nebari-2024.6.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `nebari-2024.5.1rc1/pyproject.toml` & `nebari-2024.6.1rc1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -132,29 +132,31 @@
     "keycloak.exceptions",
     "boto3",
     "botocore.exceptions",
 ]
 ignore_missing_imports = true
 
 [tool.ruff]
+extend-exclude = [
+    "src/_nebari/template",
+    "home",
+    "__pycache__"
+]
+
+[tool.ruff.lint]
 select = [
-    "E",
-    "F",
-    "PTH",
+    "E",  # E: pycodestyle rules
+    "F",  # F: pyflakes rules
+    "PTH",  # PTH: flake8-use-pathlib rules
 ]
 ignore = [
     "E501", # Line too long
     "F821", # Undefined name
     "PTH123", # open() should be replaced by Path.open()
 ]
-extend-exclude = [
-    "src/_nebari/template",
-    "home",
-    "__pycache__"
-]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 # Regexes for lines to exclude from consideration
 exclude_also = [
```

### Comparing `nebari-2024.5.1rc1/PKG-INFO` & `nebari-2024.6.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nebari
-Version: 2024.5.1rc1
+Version: 2024.6.1rc1
 Summary: A Jupyter and Dask-powered open source data science platform.
 Project-URL: Documentation, https://www.nebari.dev/docs/welcome
 Project-URL: Source, https://github.com/nebari-dev/nebari
 Author-email: Nebari development team <internal-it@quansight.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Keywords: aws,azure,dask,do,gcp,jupyter,nebari
```

