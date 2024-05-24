# Comparing `tmp/pypanther-0.1.1a2.tar.gz` & `tmp/pypanther-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypanther-0.1.1a2.tar", max compression
+gzip compressed data, was "pypanther-0.1.1a3.tar", max compression
```

## Comparing `pypanther-0.1.1a2.tar` & `pypanther-0.1.1a3.tar`

### file list

```diff
@@ -1,564 +1,565 @@
--rw-r--r--   0        0        0    34523 2024-05-22 19:16:21.930547 pypanther-0.1.1a2/LICENSE.txt
--rw-r--r--   0        0        0       80 2024-05-03 18:47:26.705553 pypanther-0.1.1a2/README.md
--rw-r--r--   0        0        0      185 2024-05-23 22:00:33.237693 pypanther-0.1.1a2/pypanther/__init__.py
--rw-r--r--   0        0        0    24586 2024-05-24 15:16:21.423666 pypanther-0.1.1a2/pypanther/base.py
--rw-r--r--   0        0        0      490 2024-05-23 22:00:33.238107 pypanther-0.1.1a2/pypanther/cache.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:14.952849 pypanther-0.1.1a2/pypanther/data_models/__init__.py
--rw-r--r--   0        0        0     1387 2024-05-24 12:40:14.944512 pypanther-0.1.1a2/pypanther/data_models/asana_data_model.py
--rw-r--r--   0        0        0     1544 2024-05-24 12:40:14.933036 pypanther-0.1.1a2/pypanther/data_models/atlassian_data_model.py
--rw-r--r--   0        0        0      607 2024-05-24 12:40:14.942246 pypanther-0.1.1a2/pypanther/data_models/aws_alb_data_model.py
--rw-r--r--   0        0        0     2214 2024-05-24 12:40:14.938734 pypanther-0.1.1a2/pypanther/data_models/aws_cloudtrail_data_model.py
--rw-r--r--   0        0        0     1465 2024-05-24 12:40:14.929894 pypanther-0.1.1a2/pypanther/data_models/aws_eks_data_model.py
--rw-r--r--   0        0        0      630 2024-05-24 12:40:14.936327 pypanther-0.1.1a2/pypanther/data_models/aws_s3_data_model.py
--rw-r--r--   0        0        0      593 2024-05-24 12:40:14.939270 pypanther-0.1.1a2/pypanther/data_models/aws_vpcdns_data_model.py
--rw-r--r--   0        0        0      742 2024-05-24 12:40:14.928634 pypanther-0.1.1a2/pypanther/data_models/aws_vpcflow_data_model.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.927521 pypanther-0.1.1a2/pypanther/data_models/azure_signin_data_model.py
--rw-r--r--   0        0        0      941 2024-05-24 12:40:14.941146 pypanther-0.1.1a2/pypanther/data_models/box_data_model.py
--rw-r--r--   0        0        0      873 2024-05-24 12:40:14.939822 pypanther-0.1.1a2/pypanther/data_models/cisco_umbrella_data_model.py
--rw-r--r--   0        0        0      653 2024-05-24 12:40:14.943897 pypanther-0.1.1a2/pypanther/data_models/cloudflare_firewall_data_model.py
--rw-r--r--   0        0        0      729 2024-05-24 12:40:14.928057 pypanther-0.1.1a2/pypanther/data_models/cloudflare_httpreq_data_model.py
--rw-r--r--   0        0        0     1853 2024-05-24 12:40:14.943403 pypanther-0.1.1a2/pypanther/data_models/crowdstrike_fdr_data_model.py
--rw-r--r--   0        0        0     5215 2024-05-24 12:40:14.934292 pypanther-0.1.1a2/pypanther/data_models/gcp_data_model.py
--rw-r--r--   0        0        0     1613 2024-05-24 12:40:14.937900 pypanther-0.1.1a2/pypanther/data_models/github_data_model.py
--rw-r--r--   0        0        0     1669 2024-05-24 12:40:14.935584 pypanther-0.1.1a2/pypanther/data_models/gsuite_data_model.py
--rw-r--r--   0        0        0     1864 2024-05-24 12:40:14.940562 pypanther-0.1.1a2/pypanther/data_models/notion_data_model.py
--rw-r--r--   0        0        0     2070 2024-05-24 12:40:14.937166 pypanther-0.1.1a2/pypanther/data_models/okta_data_model.py
--rw-r--r--   0        0        0     1467 2024-05-24 12:40:14.932330 pypanther-0.1.1a2/pypanther/data_models/onelogin_data_model.py
--rw-r--r--   0        0        0      730 2024-05-24 12:40:14.934876 pypanther-0.1.1a2/pypanther/data_models/onepassword_itemusage_data_model.py
--rw-r--r--   0        0        0     1058 2024-05-24 12:40:14.941731 pypanther-0.1.1a2/pypanther/data_models/onepassword_signinattempt_data_model.py
--rw-r--r--   0        0        0     1742 2024-05-24 12:40:14.930685 pypanther-0.1.1a2/pypanther/data_models/panther_audit_data_model.py
--rw-r--r--   0        0        0      613 2024-05-24 12:40:14.929135 pypanther-0.1.1a2/pypanther/data_models/slack_accesslogs_data_model.py
--rw-r--r--   0        0        0      711 2024-05-24 12:40:14.942793 pypanther-0.1.1a2/pypanther/data_models/slack_auditlogs_data_model.py
--rw-r--r--   0        0        0      500 2024-05-24 12:40:14.926474 pypanther-0.1.1a2/pypanther/data_models/slack_integrationlogs_data_model.py
--rw-r--r--   0        0        0     2714 2024-05-24 12:40:14.931651 pypanther-0.1.1a2/pypanther/data_models/zendesk_data_model.py
--rw-r--r--   0        0        0      886 2024-05-24 12:40:14.926019 pypanther-0.1.1a2/pypanther/data_models/zoom_activity_data_model.py
--rw-r--r--   0        0        0     1887 2024-05-24 12:40:14.925345 pypanther-0.1.1a2/pypanther/data_models/zoom_operation_data_model.py
--rw-r--r--   0        0        0     2682 2024-05-23 22:00:33.243958 pypanther-0.1.1a2/pypanther/get.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:13.778915 pypanther-0.1.1a2/pypanther/helpers/__init__.py
--rw-r--r--   0        0        0     2107 2024-05-24 12:40:14.169513 pypanther-0.1.1a2/pypanther/helpers/gcp_base_helpers.py
--rw-r--r--   0        0        0      781 2024-05-24 12:40:14.303335 pypanther-0.1.1a2/pypanther/helpers/gcp_environment.py
--rw-r--r--   0        0        0     1417 2024-05-24 12:40:13.948393 pypanther-0.1.1a2/pypanther/helpers/panther_asana_helpers.py
--rw-r--r--   0        0        0     1597 2024-05-24 12:40:14.156772 pypanther-0.1.1a2/pypanther/helpers/panther_audit.py
--rw-r--r--   0        0        0      555 2024-05-24 12:40:13.952837 pypanther-0.1.1a2/pypanther/helpers/panther_auth0_helpers.py
--rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.099017 pypanther-0.1.1a2/pypanther/helpers/panther_azuresignin_helpers.py
--rw-r--r--   0        0        0    19692 2024-05-24 12:40:14.264799 pypanther-0.1.1a2/pypanther/helpers/panther_base_helpers.py
--rw-r--r--   0        0        0     4529 2024-05-24 12:40:14.146111 pypanther-0.1.1a2/pypanther/helpers/panther_box_helpers.py
--rw-r--r--   0        0        0     2267 2024-05-24 12:40:13.916642 pypanther-0.1.1a2/pypanther/helpers/panther_cloudflare_helpers.py
--rw-r--r--   0        0        0      507 2024-05-24 12:40:14.148779 pypanther-0.1.1a2/pypanther/helpers/panther_config.py
--rw-r--r--   0        0        0      891 2024-05-24 12:40:14.103142 pypanther-0.1.1a2/pypanther/helpers/panther_config_defaults.py
--rw-r--r--   0        0        0     1043 2024-05-24 12:40:13.795713 pypanther-0.1.1a2/pypanther/helpers/panther_config_overrides.py
--rw-r--r--   0        0        0     3465 2024-05-24 12:40:13.831736 pypanther-0.1.1a2/pypanther/helpers/panther_default.py
--rw-r--r--   0        0        0     1288 2024-05-24 12:40:13.811022 pypanther-0.1.1a2/pypanther/helpers/panther_duo_helpers.py
--rw-r--r--   0        0        0     1118 2024-05-24 12:40:14.384435 pypanther-0.1.1a2/pypanther/helpers/panther_event_type_helpers.py
--rw-r--r--   0        0        0    12436 2024-05-24 12:40:14.482779 pypanther-0.1.1a2/pypanther/helpers/panther_greynoise_helpers.py
--rw-r--r--   0        0        0    38305 2024-05-24 12:40:13.902461 pypanther-0.1.1a2/pypanther/helpers/panther_iocs.py
--rw-r--r--   0        0        0     6497 2024-05-24 12:40:14.002454 pypanther-0.1.1a2/pypanther/helpers/panther_ipinfo_helpers.py
--rw-r--r--   0        0        0     2154 2024-05-24 12:40:14.015836 pypanther-0.1.1a2/pypanther/helpers/panther_lookuptable_helpers.py
--rw-r--r--   0        0        0      387 2024-05-24 12:40:14.270284 pypanther-0.1.1a2/pypanther/helpers/panther_mongodb_helpers.py
--rw-r--r--   0        0        0      340 2024-05-24 12:40:13.834434 pypanther-0.1.1a2/pypanther/helpers/panther_notion_helpers.py
--rw-r--r--   0        0        0    13096 2024-05-24 12:40:14.370655 pypanther-0.1.1a2/pypanther/helpers/panther_oss_helpers.py
--rw-r--r--   0        0        0      610 2024-05-24 12:40:13.801982 pypanther-0.1.1a2/pypanther/helpers/panther_snyk_helpers.py
--rw-r--r--   0        0        0      492 2024-05-24 12:40:14.307780 pypanther-0.1.1a2/pypanther/helpers/panther_tailscale_helpers.py
--rw-r--r--   0        0        0      567 2024-05-24 12:40:14.312664 pypanther-0.1.1a2/pypanther/helpers/panther_tines_helpers.py
--rw-r--r--   0        0        0     1542 2024-05-24 12:40:14.379643 pypanther-0.1.1a2/pypanther/helpers/panther_tor_helpers.py
--rw-r--r--   0        0        0     3084 2024-05-24 12:40:13.935600 pypanther-0.1.1a2/pypanther/helpers/panther_zoom_helpers.py
--rw-r--r--   0        0        0    13022 2024-05-23 22:06:29.350498 pypanther-0.1.1a2/pypanther/log_types.py
--rw-r--r--   0        0        0     1322 2024-05-24 13:47:47.094872 pypanther-0.1.1a2/pypanther/main.py
--rw-r--r--   0        0        0      824 2024-05-23 22:00:33.250813 pypanther-0.1.1a2/pypanther/register.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.351956 pypanther-0.1.1a2/pypanther/rules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356408 pypanther-0.1.1a2/pypanther/rules/asana_rules/__init__.py
--rw-r--r--   0        0        0     4055 2024-05-24 15:16:21.424215 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_service_account_created.py
--rw-r--r--   0        0        0     3227 2024-05-24 15:16:21.424547 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_team_privacy_public.py
--rw-r--r--   0        0        0     3249 2024-05-24 15:16:21.425052 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
--rw-r--r--   0        0        0     3218 2024-05-24 15:16:21.425432 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
--rw-r--r--   0        0        0     3406 2024-05-24 15:16:21.425777 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
--rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.426151 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
--rw-r--r--   0        0        0     3733 2024-05-24 15:16:21.426488 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_new_admin.py
--rw-r--r--   0        0        0     3228 2024-05-24 15:16:21.426739 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_org_export.py
--rw-r--r--   0        0        0     3711 2024-05-24 15:16:21.427013 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
--rw-r--r--   0        0        0     3615 2024-05-24 15:16:21.427323 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
--rw-r--r--   0        0        0     3484 2024-05-24 15:16:21.427559 pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355786 pypanther-0.1.1a2/pypanther/rules/atlassian_rules/__init__.py
--rw-r--r--   0        0        0     4877 2024-05-24 15:16:21.428031 pypanther-0.1.1a2/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352374 pypanther-0.1.1a2/pypanther/rules/auth0_rules/__init__.py
--rw-r--r--   0        0        0    44986 2024-05-24 15:16:21.428415 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_custom_role_created.py
--rw-r--r--   0        0        0    15412 2024-05-24 15:16:21.428810 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_integration_installed.py
--rw-r--r--   0        0        0    23138 2024-05-24 15:16:21.429303 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
--rw-r--r--   0        0        0    23488 2024-05-24 15:16:21.429696 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
--rw-r--r--   0        0        0    34159 2024-05-24 15:16:21.430104 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
--rw-r--r--   0        0        0    23642 2024-05-24 15:16:21.430380 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
--rw-r--r--   0        0        0    22663 2024-05-24 15:16:21.430665 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
--rw-r--r--   0        0        0    19817 2024-05-24 15:16:21.431047 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
--rw-r--r--   0        0        0    17279 2024-05-24 15:16:21.431316 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
--rw-r--r--   0        0        0    18166 2024-05-24 15:16:21.431594 pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354895 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/__init__.py
--rw-r--r--   0        0        0    11009 2024-05-24 15:16:21.431991 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
--rw-r--r--   0        0        0     8189 2024-05-24 15:16:21.432404 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
--rw-r--r--   0        0        0     7038 2024-05-24 15:16:21.432638 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
--rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.432859 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
--rw-r--r--   0        0        0     7212 2024-05-24 15:16:21.433158 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
--rw-r--r--   0        0        0     4460 2024-05-24 12:40:19.072096 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
--rw-r--r--   0        0        0     6992 2024-05-24 15:16:21.433498 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
--rw-r--r--   0        0        0     6551 2024-05-24 15:16:21.433773 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
--rw-r--r--   0        0        0     6538 2024-05-24 15:16:21.434033 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
--rw-r--r--   0        0        0    20551 2024-05-24 15:16:21.434298 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
--rw-r--r--   0        0        0     4027 2024-05-24 12:40:19.137363 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
--rw-r--r--   0        0        0     5596 2024-05-24 15:16:21.434553 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
--rw-r--r--   0        0        0     5699 2024-05-24 15:16:21.434870 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
--rw-r--r--   0        0        0     2281 2024-05-24 15:16:21.435209 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
--rw-r--r--   0        0        0     6712 2024-05-24 15:16:21.435527 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
--rw-r--r--   0        0        0    17193 2024-05-24 12:40:19.013686 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
--rw-r--r--   0        0        0    22406 2024-05-24 15:16:21.435872 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
--rw-r--r--   0        0        0     7244 2024-05-24 15:16:21.436155 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
--rw-r--r--   0        0        0     6874 2024-05-24 15:16:21.436423 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
--rw-r--r--   0        0        0     8171 2024-05-24 15:16:21.436705 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
--rw-r--r--   0        0        0     5159 2024-05-24 15:16:21.436966 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
--rw-r--r--   0        0        0    30269 2024-05-24 15:16:21.437319 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
--rw-r--r--   0        0        0     8600 2024-05-24 15:16:21.437710 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
--rw-r--r--   0        0        0    39729 2024-05-24 15:16:21.437986 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
--rw-r--r--   0        0        0    27319 2024-05-24 12:40:19.153333 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
--rw-r--r--   0        0        0    26728 2024-05-24 12:40:19.048210 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
--rw-r--r--   0        0        0     7262 2024-05-24 15:16:21.438351 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
--rw-r--r--   0        0        0     8581 2024-05-24 12:40:19.131595 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
--rw-r--r--   0        0        0     6105 2024-05-24 15:16:21.438771 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
--rw-r--r--   0        0        0    12705 2024-05-24 12:40:19.146336 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
--rw-r--r--   0        0        0    13749 2024-05-24 12:40:19.032961 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
--rw-r--r--   0        0        0     7140 2024-05-24 15:16:21.439018 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
--rw-r--r--   0        0        0    10477 2024-05-24 15:16:21.439288 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
--rw-r--r--   0        0        0     9036 2024-05-24 15:16:21.439564 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
--rw-r--r--   0        0        0     3375 2024-05-24 15:16:21.439795 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
--rw-r--r--   0        0        0     5202 2024-05-24 15:16:21.440052 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
--rw-r--r--   0        0        0    11250 2024-05-24 15:16:21.440309 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
--rw-r--r--   0        0        0     5716 2024-05-24 12:40:19.030090 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
--rw-r--r--   0        0        0     9720 2024-05-24 15:16:21.440570 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
--rw-r--r--   0        0        0    26986 2024-05-24 12:40:19.164857 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
--rw-r--r--   0        0        0     7813 2024-05-24 15:16:21.440884 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
--rw-r--r--   0        0        0    16362 2024-05-24 15:16:21.441210 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
--rw-r--r--   0        0        0    14625 2024-05-24 15:16:21.441626 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
--rw-r--r--   0        0        0    17386 2024-05-24 15:16:21.441875 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
--rw-r--r--   0        0        0     7466 2024-05-24 15:16:21.442158 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
--rw-r--r--   0        0        0    18968 2024-05-24 15:16:21.442383 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
--rw-r--r--   0        0        0     4655 2024-05-24 15:16:21.442623 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
--rw-r--r--   0        0        0    10739 2024-05-24 15:16:21.442885 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
--rw-r--r--   0        0        0     3920 2024-05-24 15:16:21.443092 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
--rw-r--r--   0        0        0     5811 2024-05-24 15:16:21.443361 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
--rw-r--r--   0        0        0     7502 2024-05-24 15:16:21.443687 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
--rw-r--r--   0        0        0    12275 2024-05-24 15:16:21.443990 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
--rw-r--r--   0        0        0    11502 2024-05-24 15:16:21.444278 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
--rw-r--r--   0        0        0     5556 2024-05-24 15:16:21.444534 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
--rw-r--r--   0        0        0     7544 2024-05-24 15:16:21.444768 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
--rw-r--r--   0        0        0     5177 2024-05-24 12:40:19.036764 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
--rw-r--r--   0        0        0     6464 2024-05-24 15:16:21.445000 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
--rw-r--r--   0        0        0     8683 2024-05-24 12:40:19.124611 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
--rw-r--r--   0        0        0     5962 2024-05-24 15:16:21.445244 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
--rw-r--r--   0        0        0     6768 2024-05-24 15:16:21.445508 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
--rw-r--r--   0        0        0     7010 2024-05-24 15:16:21.445747 pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352785 pypanther-0.1.1a2/pypanther/rules/aws_eks_rules/__init__.py
--rw-r--r--   0        0        0     9686 2024-05-24 15:16:21.446020 pypanther-0.1.1a2/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
--rw-r--r--   0        0        0    17799 2024-05-24 15:16:21.446254 pypanther-0.1.1a2/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354748 pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/__init__.py
--rw-r--r--   0        0        0     5356 2024-05-24 15:16:21.446559 pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
--rw-r--r--   0        0        0     5377 2024-05-24 15:16:21.446848 pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
--rw-r--r--   0        0        0     5403 2024-05-24 15:16:21.447130 pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355307 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/__init__.py
--rw-r--r--   0        0        0     4688 2024-05-24 15:16:21.447407 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
--rw-r--r--   0        0        0     2546 2024-05-24 12:40:19.231135 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
--rw-r--r--   0        0        0     6263 2024-05-24 15:16:21.447657 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
--rw-r--r--   0        0        0     1983 2024-05-24 12:40:19.239787 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
--rw-r--r--   0        0        0     8734 2024-05-24 12:40:19.236359 pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355429 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/__init__.py
--rw-r--r--   0        0        0     6776 2024-05-24 15:16:21.447901 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
--rw-r--r--   0        0        0     1326 2024-05-24 15:16:21.448149 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
--rw-r--r--   0        0        0     2524 2024-05-24 12:40:19.241211 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
--rw-r--r--   0        0        0     2484 2024-05-24 12:40:19.248154 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
--rw-r--r--   0        0        0     2913 2024-05-24 12:40:19.246794 pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355171 pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/__init__.py
--rw-r--r--   0        0        0     7964 2024-05-24 15:16:21.448405 pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_failed_signins.py
--rw-r--r--   0        0        0    15752 2024-05-24 15:16:21.448657 pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_legacyauth.py
--rw-r--r--   0        0        0    17539 2024-05-24 15:16:21.448880 pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353050 pypanther-0.1.1a2/pypanther/rules/box_rules/__init__.py
--rw-r--r--   0        0        0     2120 2024-05-24 15:16:21.449114 pypanther-0.1.1a2/pypanther/rules/box_rules/box_access_granted.py
--rw-r--r--   0        0        0     2855 2024-05-24 15:16:21.449326 pypanther-0.1.1a2/pypanther/rules/box_rules/box_anomalous_download.py
--rw-r--r--   0        0        0     2730 2024-05-24 12:40:18.694430 pypanther-0.1.1a2/pypanther/rules/box_rules/box_event_triggered_externally.py
--rw-r--r--   0        0        0     3638 2024-05-24 12:40:18.687439 pypanther-0.1.1a2/pypanther/rules/box_rules/box_item_shared_externally.py
--rw-r--r--   0        0        0     4252 2024-05-24 15:16:21.449561 pypanther-0.1.1a2/pypanther/rules/box_rules/box_malicious_content.py
--rw-r--r--   0        0        0     2110 2024-05-24 15:16:21.449767 pypanther-0.1.1a2/pypanther/rules/box_rules/box_new_login.py
--rw-r--r--   0        0        0     2808 2024-05-24 15:16:21.449973 pypanther-0.1.1a2/pypanther/rules/box_rules/box_policy_violation.py
--rw-r--r--   0        0        0     4201 2024-05-24 15:16:21.450221 pypanther-0.1.1a2/pypanther/rules/box_rules/box_suspicious_login_or_session.py
--rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.450435 pypanther-0.1.1a2/pypanther/rules/box_rules/box_untrusted_device.py
--rw-r--r--   0        0        0     2352 2024-05-24 15:16:21.450657 pypanther-0.1.1a2/pypanther/rules/box_rules/box_user_downloads.py
--rw-r--r--   0        0        0     3165 2024-05-24 15:16:21.450863 pypanther-0.1.1a2/pypanther/rules/box_rules/box_user_permission_updates.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355655 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/__init__.py
--rw-r--r--   0        0        0     3299 2024-05-24 15:16:21.451080 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
--rw-r--r--   0        0        0     3023 2024-05-24 15:16:21.451306 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
--rw-r--r--   0        0        0     3473 2024-05-24 15:16:21.451550 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
--rw-r--r--   0        0        0     2248 2024-05-24 15:16:21.451767 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
--rw-r--r--   0        0        0     2577 2024-05-24 15:16:21.451988 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
--rw-r--r--   0        0        0    11303 2024-05-24 15:16:21.452260 pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355556 pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
--rw-r--r--   0        0        0     1787 2024-05-24 15:16:21.452540 pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
--rw-r--r--   0        0        0     1414 2024-05-24 12:40:19.250591 pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
--rw-r--r--   0        0        0     1903 2024-05-24 12:40:19.253188 pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354017 pypanther-0.1.1a2/pypanther/rules/cloudflare_rules/__init__.py
--rw-r--r--   0        0        0     4969 2024-05-24 15:16:21.452875 pypanther-0.1.1a2/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
--rw-r--r--   0        0        0     7563 2024-05-24 12:40:18.920956 pypanther-0.1.1a2/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355030 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/__init__.py
--rw-r--r--   0        0        0    29385 2024-05-24 15:16:21.453267 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
--rw-r--r--   0        0        0     8177 2024-05-24 15:16:21.453668 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
--rw-r--r--   0        0        0     9893 2024-05-24 15:16:21.453945 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
--rw-r--r--   0        0        0     9855 2024-05-24 15:16:21.454211 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
--rw-r--r--   0        0        0    10420 2024-05-24 15:16:21.454477 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
--rw-r--r--   0        0        0    12177 2024-05-24 12:40:19.187772 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
--rw-r--r--   0        0        0    11711 2024-05-24 12:40:19.205936 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
--rw-r--r--   0        0        0    18680 2024-05-24 15:16:21.454710 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
--rw-r--r--   0        0        0    18887 2024-05-24 15:16:21.454956 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
--rw-r--r--   0        0        0    15614 2024-05-24 15:16:21.455287 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
--rw-r--r--   0        0        0     7208 2024-05-24 15:16:21.455541 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
--rw-r--r--   0        0        0     9722 2024-05-24 15:16:21.455811 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
--rw-r--r--   0        0        0    13594 2024-05-24 15:16:21.456062 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
--rw-r--r--   0        0        0     9703 2024-05-24 15:16:21.456322 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
--rw-r--r--   0        0        0    10006 2024-05-24 15:16:21.456575 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
--rw-r--r--   0        0        0    17357 2024-05-24 15:16:21.456795 pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354190 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/__init__.py
--rw-r--r--   0        0        0     6793 2024-05-24 15:16:21.457052 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
--rw-r--r--   0        0        0     9494 2024-05-24 15:16:21.457293 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_external_share.py
--rw-r--r--   0        0        0     8238 2024-05-24 15:16:21.457569 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
--rw-r--r--   0        0        0    11142 2024-05-24 15:16:21.457840 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
--rw-r--r--   0        0        0     5131 2024-05-24 15:16:21.458095 pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353471 pypanther-0.1.1a2/pypanther/rules/duo_rules/__init__.py
--rw-r--r--   0        0        0     2088 2024-05-24 15:16:21.458537 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
--rw-r--r--   0        0        0     2175 2024-05-24 15:16:21.460660 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
--rw-r--r--   0        0        0     2244 2024-05-24 15:16:21.460989 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
--rw-r--r--   0        0        0     2241 2024-05-24 15:16:21.461264 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_create_admin.py
--rw-r--r--   0        0        0     2508 2024-05-24 15:16:21.461517 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_lockout.py
--rw-r--r--   0        0        0     2658 2024-05-24 15:16:21.461765 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
--rw-r--r--   0        0        0     1968 2024-05-24 15:16:21.461984 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
--rw-r--r--   0        0        0     3144 2024-05-24 15:16:21.462206 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
--rw-r--r--   0        0        0     2208 2024-05-24 15:16:21.462435 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_policy_updated.py
--rw-r--r--   0        0        0     3376 2024-05-24 15:16:21.462674 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
--rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.462911 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
--rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.463155 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
--rw-r--r--   0        0        0     3152 2024-05-24 15:16:21.463423 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_anomalous_push.py
--rw-r--r--   0        0        0     3058 2024-05-24 15:16:21.463696 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
--rw-r--r--   0        0        0     5450 2024-05-24 15:16:21.463967 pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353698 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/__init__.py
--rw-r--r--   0        0        0     9839 2024-05-24 15:16:21.464276 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
--rw-r--r--   0        0        0    12333 2024-05-24 15:16:21.464557 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
--rw-r--r--   0        0        0     7045 2024-05-24 15:16:21.464840 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
--rw-r--r--   0        0        0     7839 2024-05-24 15:16:21.465105 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
--rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465357 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
--rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465626 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
--rw-r--r--   0        0        0    19128 2024-05-24 15:16:21.465900 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
--rw-r--r--   0        0        0    10432 2024-05-24 15:16:21.466320 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
--rw-r--r--   0        0        0    15433 2024-05-24 15:16:21.466688 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
--rw-r--r--   0        0        0     9149 2024-05-24 15:16:21.467069 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
--rw-r--r--   0        0        0     6818 2024-05-24 15:16:21.467438 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
--rw-r--r--   0        0        0     8941 2024-05-24 15:16:21.467837 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
--rw-r--r--   0        0        0     3831 2024-05-24 15:16:21.468230 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
--rw-r--r--   0        0        0     4527 2024-05-24 15:16:21.468564 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
--rw-r--r--   0        0        0    15793 2024-05-24 15:16:21.468870 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
--rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.469204 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
--rw-r--r--   0        0        0     9941 2024-05-24 15:16:21.469591 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
--rw-r--r--   0        0        0     3579 2024-05-24 15:16:21.469975 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
--rw-r--r--   0        0        0     4115 2024-05-24 15:16:21.470322 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
--rw-r--r--   0        0        0     6785 2024-05-24 15:16:21.470690 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
--rw-r--r--   0        0        0     6585 2024-05-24 15:16:21.471079 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
--rw-r--r--   0        0        0     7304 2024-05-24 15:16:21.471358 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
--rw-r--r--   0        0        0     9263 2024-05-24 15:16:21.471651 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
--rw-r--r--   0        0        0    11294 2024-05-24 15:16:21.471923 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
--rw-r--r--   0        0        0     7615 2024-05-24 15:16:21.472188 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
--rw-r--r--   0        0        0     7079 2024-05-24 15:16:21.472435 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
--rw-r--r--   0        0        0    10607 2024-05-24 15:16:21.472706 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
--rw-r--r--   0        0        0     4068 2024-05-24 15:16:21.473027 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
--rw-r--r--   0        0        0     7714 2024-05-24 15:16:21.473395 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
--rw-r--r--   0        0        0    11742 2024-05-24 15:16:21.473678 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
--rw-r--r--   0        0        0    10816 2024-05-24 15:16:21.473953 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
--rw-r--r--   0        0        0     2275 2024-05-24 15:16:21.474180 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
--rw-r--r--   0        0        0     2911 2024-05-24 15:16:21.474491 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
--rw-r--r--   0        0        0    13058 2024-05-24 12:40:18.866059 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
--rw-r--r--   0        0        0    10910 2024-05-24 15:16:21.474877 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
--rw-r--r--   0        0        0     9626 2024-05-24 15:16:21.475160 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
--rw-r--r--   0        0        0    10164 2024-05-24 15:16:21.475430 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
--rw-r--r--   0        0        0    11767 2024-05-24 15:16:21.475792 pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352868 pypanther-0.1.1a2/pypanther/rules/gcp_http_lb_rules/__init__.py
--rw-r--r--   0        0        0     5908 2024-05-24 15:16:21.476184 pypanther-0.1.1a2/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356266 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/__init__.py
--rw-r--r--   0        0        0     4559 2024-05-24 15:16:21.476451 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
--rw-r--r--   0        0        0     6701 2024-05-24 12:40:19.340583 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
--rw-r--r--   0        0        0     2251 2024-05-24 15:16:21.476747 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
--rw-r--r--   0        0        0     3530 2024-05-24 15:16:21.477098 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
--rw-r--r--   0        0        0     3433 2024-05-24 15:16:21.477323 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
--rw-r--r--   0        0        0    12867 2024-05-24 15:16:21.477684 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
--rw-r--r--   0        0        0     3499 2024-05-24 15:16:21.477988 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
--rw-r--r--   0        0        0    14878 2024-05-24 15:16:21.478411 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
--rw-r--r--   0        0        0    11462 2024-05-24 15:16:21.478669 pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352570 pypanther-0.1.1a2/pypanther/rules/github_rules/__init__.py
--rw-r--r--   0        0        0     5241 2024-05-24 12:40:18.616900 pypanther-0.1.1a2/pypanther/rules/github_rules/github_action_failed.py
--rw-r--r--   0        0        0    14192 2024-05-24 15:16:21.478946 pypanther-0.1.1a2/pypanther/rules/github_rules/github_advanced_security_change.py
--rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.479163 pypanther-0.1.1a2/pypanther/rules/github_rules/github_branch_policy_override.py
--rw-r--r--   0        0        0     2030 2024-05-24 15:16:21.479385 pypanther-0.1.1a2/pypanther/rules/github_rules/github_branch_protection_disabled.py
--rw-r--r--   0        0        0     2223 2024-05-24 15:16:21.479616 pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_auth_modified.py
--rw-r--r--   0        0        0     2409 2024-05-24 15:16:21.479861 pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_ip_allowlist.py
--rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.480172 pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_moderators_add.py
--rw-r--r--   0        0        0     2302 2024-05-24 15:16:21.480396 pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_modified.py
--rw-r--r--   0        0        0     3381 2024-05-24 15:16:21.480613 pypanther-0.1.1a2/pypanther/rules/github_rules/github_organization_app_integration_installed.py
--rw-r--r--   0        0        0     2847 2024-05-24 15:16:21.480830 pypanther-0.1.1a2/pypanther/rules/github_rules/github_public_repository_created.py
--rw-r--r--   0        0        0     2762 2024-05-24 15:16:21.481050 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_collaborator_change.py
--rw-r--r--   0        0        0     1446 2024-05-24 15:16:21.481310 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_created.py
--rw-r--r--   0        0        0     2501 2024-05-24 15:16:21.481577 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_hook_modified.py
--rw-r--r--   0        0        0     4211 2024-05-24 15:16:21.482079 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_initial_access.py
--rw-r--r--   0        0        0     1890 2024-05-24 15:16:21.482329 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_visibility_change.py
--rw-r--r--   0        0        0     5328 2024-05-24 15:16:21.482612 pypanther-0.1.1a2/pypanther/rules/github_rules/github_repository_transfer.py
--rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.482858 pypanther-0.1.1a2/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
--rw-r--r--   0        0        0     3326 2024-05-24 15:16:21.483159 pypanther-0.1.1a2/pypanther/rules/github_rules/github_team_modified.py
--rw-r--r--   0        0        0     1622 2024-05-24 15:16:21.483409 pypanther-0.1.1a2/pypanther/rules/github_rules/github_user_access_key_created.py
--rw-r--r--   0        0        0     1725 2024-05-24 15:16:21.483706 pypanther-0.1.1a2/pypanther/rules/github_rules/github_user_role_updated.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356132 pypanther-0.1.1a2/pypanther/rules/gitlab_rules/__init__.py
--rw-r--r--   0        0        0     2333 2024-05-24 15:16:21.484015 pypanther-0.1.1a2/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
--rw-r--r--   0        0        0     2789 2024-05-24 15:16:21.484312 pypanther-0.1.1a2/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352688 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/__init__.py
--rw-r--r--   0        0        0     2521 2024-05-24 15:16:21.484638 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
--rw-r--r--   0        0        0     2631 2024-05-24 15:16:21.484883 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
--rw-r--r--   0        0        0     3188 2024-05-24 15:16:21.485119 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
--rw-r--r--   0        0        0     2947 2024-05-24 15:16:21.485352 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
--rw-r--r--   0        0        0     1749 2024-05-24 15:16:21.485594 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
--rw-r--r--   0        0        0     6365 2024-05-24 15:16:21.485875 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
--rw-r--r--   0        0        0     4716 2024-05-24 15:16:21.486157 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
--rw-r--r--   0        0        0     1593 2024-05-24 15:16:21.486399 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
--rw-r--r--   0        0        0     2190 2024-05-24 15:16:21.486639 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
--rw-r--r--   0        0        0     1614 2024-05-24 15:16:21.486861 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
--rw-r--r--   0        0        0     2739 2024-05-24 15:16:21.487116 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
--rw-r--r--   0        0        0     4429 2024-05-24 15:16:21.487415 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
--rw-r--r--   0        0        0     3205 2024-05-24 15:16:21.487780 pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354403 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/__init__.py
--rw-r--r--   0        0        0     4360 2024-05-24 15:16:21.488109 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
--rw-r--r--   0        0        0     6479 2024-05-24 15:16:21.488371 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
--rw-r--r--   0        0        0     6692 2024-05-24 15:16:21.488623 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
--rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.488868 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
--rw-r--r--   0        0        0     4631 2024-05-24 15:16:21.489112 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
--rw-r--r--   0        0        0     1947 2024-05-24 15:16:21.489391 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
--rw-r--r--   0        0        0     5772 2024-05-24 15:16:21.489802 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
--rw-r--r--   0        0        0     2325 2024-05-24 12:40:18.988544 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
--rw-r--r--   0        0        0     4324 2024-05-24 12:40:18.990649 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
--rw-r--r--   0        0        0     1451 2024-05-24 15:16:21.490098 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
--rw-r--r--   0        0        0     1984 2024-05-24 15:16:21.490412 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
--rw-r--r--   0        0        0     1949 2024-05-24 15:16:21.490708 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
--rw-r--r--   0        0        0     3035 2024-05-24 15:16:21.491052 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
--rw-r--r--   0        0        0     3459 2024-05-24 12:40:18.954789 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
--rw-r--r--   0        0        0     2728 2024-05-24 15:16:21.491353 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
--rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.491620 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
--rw-r--r--   0        0        0     2006 2024-05-24 15:16:21.491969 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
--rw-r--r--   0        0        0     3443 2024-05-24 15:16:21.492331 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
--rw-r--r--   0        0        0     2573 2024-05-24 15:16:21.492593 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
--rw-r--r--   0        0        0     2189 2024-05-24 15:16:21.492877 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
--rw-r--r--   0        0        0     2707 2024-05-24 15:16:21.493162 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
--rw-r--r--   0        0        0     6820 2024-05-24 15:16:21.493443 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
--rw-r--r--   0        0        0     4999 2024-05-24 15:16:21.493742 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
--rw-r--r--   0        0        0     6038 2024-05-24 15:16:21.493994 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
--rw-r--r--   0        0        0     5438 2024-05-24 15:16:21.494274 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
--rw-r--r--   0        0        0     5208 2024-05-24 15:16:21.494563 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
--rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.494909 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
--rw-r--r--   0        0        0     4963 2024-05-24 15:16:21.495174 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
--rw-r--r--   0        0        0     5209 2024-05-24 15:16:21.495453 pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353938 pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/__init__.py
--rw-r--r--   0        0        0    10537 2024-05-24 12:40:18.909156 pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
--rw-r--r--   0        0        0     4546 2024-05-24 15:16:21.495759 pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
--rw-r--r--   0        0        0    25444 2024-05-24 12:40:18.913974 pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354103 pypanther-0.1.1a2/pypanther/rules/indicator_creation_rules/__init__.py
--rw-r--r--   0        0        0     4649 2024-05-24 15:16:21.496043 pypanther-0.1.1a2/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
--rw-r--r--   0        0        0     4396 2024-05-24 15:16:21.496301 pypanther-0.1.1a2/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353568 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/__init__.py
--rw-r--r--   0        0        0     4569 2024-05-24 15:16:21.496570 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
--rw-r--r--   0        0        0     9668 2024-05-24 15:16:21.496852 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
--rw-r--r--   0        0        0     6301 2024-05-24 15:16:21.497132 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
--rw-r--r--   0        0        0    10170 2024-05-24 15:16:21.497409 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
--rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.497661 pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352474 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/__init__.py
--rw-r--r--   0        0        0     3349 2024-05-24 15:16:21.497893 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
--rw-r--r--   0        0        0     2854 2024-05-24 15:16:21.498106 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
--rw-r--r--   0        0        0     2697 2024-05-24 15:16:21.498314 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
--rw-r--r--   0        0        0     4160 2024-05-24 15:16:21.498569 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
--rw-r--r--   0        0        0     4357 2024-05-24 15:16:21.498812 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
--rw-r--r--   0        0        0     3944 2024-05-24 15:16:21.499034 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
--rw-r--r--   0        0        0     2270 2024-05-24 15:16:21.499318 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
--rw-r--r--   0        0        0     3341 2024-05-24 15:16:21.499611 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
--rw-r--r--   0        0        0     3201 2024-05-24 15:16:21.499917 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
--rw-r--r--   0        0        0     4756 2024-05-24 15:16:21.500167 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
--rw-r--r--   0        0        0     3421 2024-05-24 15:16:21.500388 pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352276 pypanther-0.1.1a2/pypanther/rules/netskope_rules/__init__.py
--rw-r--r--   0        0        0     2974 2024-05-24 15:16:21.500620 pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
--rw-r--r--   0        0        0     3556 2024-05-24 15:16:21.500849 pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_admin_user_change.py
--rw-r--r--   0        0        0     2713 2024-05-24 15:16:21.501051 pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_many_deletes.py
--rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.501271 pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_personnel_action.py
--rw-r--r--   0        0        0     3159 2024-05-24 15:16:21.501490 pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353782 pypanther-0.1.1a2/pypanther/rules/notion_rules/__init__.py
--rw-r--r--   0        0        0    16708 2024-05-24 15:16:21.501785 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_account_changed_after_login.py
--rw-r--r--   0        0        0     1529 2024-05-24 12:40:18.870179 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
--rw-r--r--   0        0        0    15410 2024-05-24 15:16:21.502697 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_login_from_new_location.py
--rw-r--r--   0        0        0     3273 2024-05-24 15:16:21.503542 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_many_pages_deleted.py
--rw-r--r--   0        0        0     3269 2024-05-24 15:16:21.503922 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_many_pages_exported.py
--rw-r--r--   0        0        0     1747 2024-05-24 15:16:21.504555 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
--rw-r--r--   0        0        0     5395 2024-05-24 15:16:21.504913 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
--rw-r--r--   0        0        0     1641 2024-05-24 15:16:21.505220 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_shared_to_web.py
--rw-r--r--   0        0        0     2869 2024-05-24 15:16:21.505506 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_scim_token_generated.py
--rw-r--r--   0        0        0     3872 2024-05-24 15:16:21.505825 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
--rw-r--r--   0        0        0     4470 2024-05-24 15:16:21.506092 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
--rw-r--r--   0        0        0     2995 2024-05-24 15:16:21.506343 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
--rw-r--r--   0        0        0     3264 2024-05-24 15:16:21.506586 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_exported.py
--rw-r--r--   0        0        0     4548 2024-05-24 15:16:21.506857 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
--rw-r--r--   0        0        0     4402 2024-05-24 15:16:21.507127 pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356572 pypanther-0.1.1a2/pypanther/rules/okta_rules/__init__.py
--rw-r--r--   0        0        0     3624 2024-05-24 15:16:21.507388 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_account_support_access.py
--rw-r--r--   0        0        0     3475 2024-05-24 15:16:21.507645 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
--rw-r--r--   0        0        0     7243 2024-05-24 15:16:21.507905 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_admin_role_assigned.py
--rw-r--r--   0        0        0     7625 2024-05-24 15:16:21.508163 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
--rw-r--r--   0        0        0     2638 2024-05-24 15:16:21.508396 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_api_key_created.py
--rw-r--r--   0        0        0     2483 2024-05-24 15:16:21.508645 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_api_key_revoked.py
--rw-r--r--   0        0        0     9042 2024-05-24 15:16:21.508933 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
--rw-r--r--   0        0        0     7515 2024-05-24 15:16:21.509199 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
--rw-r--r--   0        0        0     7396 2024-05-24 15:16:21.509456 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
--rw-r--r--   0        0        0     8132 2024-05-24 15:16:21.509731 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_idp_create_modify.py
--rw-r--r--   0        0        0     8222 2024-05-24 12:40:19.414785 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_idp_signin.py
--rw-r--r--   0        0        0    13813 2024-05-24 15:16:21.510023 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
--rw-r--r--   0        0        0    13457 2024-05-24 15:16:21.510285 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
--rw-r--r--   0        0        0    10936 2024-05-24 15:16:21.510562 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_password_accessed.py
--rw-r--r--   0        0        0     7709 2024-05-24 15:16:21.510819 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
--rw-r--r--   0        0        0     7652 2024-05-24 15:16:21.511084 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
--rw-r--r--   0        0        0    19397 2024-05-24 15:16:21.511361 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
--rw-r--r--   0        0        0    10687 2024-05-24 15:16:21.511669 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_rate_limits.py
--rw-r--r--   0        0        0     4995 2024-05-24 15:16:21.511930 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_support_reset.py
--rw-r--r--   0        0        0     9198 2024-05-24 15:16:21.512255 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
--rw-r--r--   0        0        0     6846 2024-05-24 15:16:21.512684 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_account_locked.py
--rw-r--r--   0        0        0     7006 2024-05-24 15:16:21.513054 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
--rw-r--r--   0        0        0     4170 2024-05-24 15:16:21.513390 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_reset.py
--rw-r--r--   0        0        0     5452 2024-05-24 15:16:21.513642 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
--rw-r--r--   0        0        0     8388 2024-05-24 15:16:21.513988 pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352956 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/__init__.py
--rw-r--r--   0        0        0     3840 2024-05-24 15:16:21.514248 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
--rw-r--r--   0        0        0     1955 2024-05-24 15:16:21.514508 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
--rw-r--r--   0        0        0     2473 2024-05-24 15:16:21.514744 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
--rw-r--r--   0        0        0     2280 2024-05-24 15:16:21.514994 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
--rw-r--r--   0        0        0     2187 2024-05-24 15:16:21.515230 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_password_changed.py
--rw-r--r--   0        0        0     2656 2024-05-24 15:16:21.515454 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
--rw-r--r--   0        0        0     1879 2024-05-24 15:16:21.515683 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
--rw-r--r--   0        0        0     1921 2024-05-24 15:16:21.515917 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
--rw-r--r--   0        0        0     1848 2024-05-24 15:16:21.516156 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
--rw-r--r--   0        0        0     2545 2024-05-24 15:16:21.516389 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
--rw-r--r--   0        0        0     1995 2024-05-24 15:16:21.516648 pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353133 pypanther-0.1.1a2/pypanther/rules/onepassword_rules/__init__.py
--rw-r--r--   0        0        0     4565 2024-05-24 12:40:18.700457 pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
--rw-r--r--   0        0        0     3917 2024-05-24 12:40:18.705317 pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
--rw-r--r--   0        0        0     4427 2024-05-24 15:16:21.516925 pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356027 pypanther-0.1.1a2/pypanther/rules/osquery_rules/__init__.py
--rw-r--r--   0        0        0     4038 2024-05-24 15:16:21.517176 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
--rw-r--r--   0        0        0     3398 2024-05-24 12:40:19.326027 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
--rw-r--r--   0        0        0     3580 2024-05-24 15:16:21.517419 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
--rw-r--r--   0        0        0     2965 2024-05-24 15:16:21.517652 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
--rw-r--r--   0        0        0     2596 2024-05-24 15:16:21.517917 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
--rw-r--r--   0        0        0     2203 2024-05-24 15:16:21.518208 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
--rw-r--r--   0        0        0     4057 2024-05-24 15:16:21.518697 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
--rw-r--r--   0        0        0     3670 2024-05-24 15:16:21.519188 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
--rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.519514 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_ossec.py
--rw-r--r--   0        0        0     3545 2024-05-24 15:16:21.519928 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_outdated.py
--rw-r--r--   0        0        0     3674 2024-05-24 15:16:21.520400 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_outdated_macos.py
--rw-r--r--   0        0        0     3730 2024-05-24 15:16:21.520712 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_ssh_listener.py
--rw-r--r--   0        0        0     5583 2024-05-24 15:16:21.521025 pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353388 pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.521335 pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
--rw-r--r--   0        0        0     2520 2024-05-24 15:16:21.521649 pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_saml_modified.py
--rw-r--r--   0        0        0     8355 2024-05-24 15:16:21.521983 pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
--rw-r--r--   0        0        0     9712 2024-05-24 15:16:21.522331 pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_user_modified.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354643 pypanther-0.1.1a2/pypanther/rules/salesforce_rules/__init__.py
--rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.522688 pypanther-0.1.1a2/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353299 pypanther-0.1.1a2/pypanther/rules/sentinelone_rules/__init__.py
--rw-r--r--   0        0        0     7210 2024-05-24 15:16:21.522968 pypanther-0.1.1a2/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
--rw-r--r--   0        0        0     6468 2024-05-24 15:16:21.523217 pypanther-0.1.1a2/pypanther/rules/sentinelone_rules/sentinelone_threats.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355907 pypanther-0.1.1a2/pypanther/rules/slack_rules/__init__.py
--rw-r--r--   0        0        0    10097 2024-05-24 15:16:21.523488 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_access_expanded.py
--rw-r--r--   0        0        0     8839 2024-05-24 15:16:21.523750 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_added.py
--rw-r--r--   0        0        0     6576 2024-05-24 15:16:21.524038 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_removed.py
--rw-r--r--   0        0        0     4668 2024-05-24 15:16:21.524305 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_application_dos.py
--rw-r--r--   0        0        0     4933 2024-05-24 15:16:21.524549 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_dlp_modified.py
--rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.524759 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_config_changed.py
--rw-r--r--   0        0        0     3415 2024-05-24 15:16:21.524967 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
--rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.525183 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
--rw-r--r--   0        0        0     5881 2024-05-24 15:16:21.525433 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_idp_configuration_change.py
--rw-r--r--   0        0        0     4687 2024-05-24 15:16:21.525677 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_information_barrier_modified.py
--rw-r--r--   0        0        0     3317 2024-05-24 15:16:21.525905 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
--rw-r--r--   0        0        0     6985 2024-05-24 15:16:21.526152 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
--rw-r--r--   0        0        0     3440 2024-05-24 15:16:21.526377 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
--rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526613 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_org_created.py
--rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526854 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_org_deleted.py
--rw-r--r--   0        0        0     3301 2024-05-24 15:16:21.527063 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
--rw-r--r--   0        0        0     3398 2024-05-24 15:16:21.527272 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
--rw-r--r--   0        0        0     3578 2024-05-24 15:16:21.527470 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_private_channel_made_public.py
--rw-r--r--   0        0        0     4137 2024-05-24 15:16:21.527694 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
--rw-r--r--   0        0        0     3543 2024-05-24 15:16:21.527892 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_service_owner_transferred.py
--rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.528118 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_sso_settings_changed.py
--rw-r--r--   0        0        0     7385 2024-05-24 15:16:21.528386 pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356824 pypanther-0.1.1a2/pypanther/rules/snyk_rules/__init__.py
--rw-r--r--   0        0        0     2612 2024-05-24 15:16:21.528608 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_misc_settings.py
--rw-r--r--   0        0        0     4557 2024-05-24 15:16:21.528844 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_org_settings.py
--rw-r--r--   0        0        0     4554 2024-05-24 15:16:21.529080 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_ou_change.py
--rw-r--r--   0        0        0     4870 2024-05-24 15:16:21.529343 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_project_settings.py
--rw-r--r--   0        0        0     5423 2024-05-24 15:16:21.529632 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_role_change.py
--rw-r--r--   0        0        0    12013 2024-05-24 15:16:21.529916 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_svcacct_change.py
--rw-r--r--   0        0        0     3957 2024-05-24 15:16:21.530136 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
--rw-r--r--   0        0        0     6252 2024-05-24 15:16:21.530401 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_policysetting.py
--rw-r--r--   0        0        0     2564 2024-05-24 15:16:21.530613 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_sso.py
--rw-r--r--   0        0        0     5837 2024-05-24 15:16:21.530857 pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_user_mgmt.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352089 pypanther-0.1.1a2/pypanther/rules/standard_rules/__init__.py
--rw-r--r--   0        0        0    10977 2024-05-24 15:16:21.531147 pypanther-0.1.1a2/pypanther/rules/standard_rules/admin_assigned.py
--rw-r--r--   0        0        0    16941 2024-05-24 15:16:21.531423 pypanther-0.1.1a2/pypanther/rules/standard_rules/brute_force_by_ip.py
--rw-r--r--   0        0        0    36744 2024-05-24 15:16:21.531830 pypanther-0.1.1a2/pypanther/rules/standard_rules/impossible_travel_login.py
--rw-r--r--   0        0        0     9765 2024-05-24 12:40:18.497546 pypanther-0.1.1a2/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
--rw-r--r--   0        0        0     8211 2024-05-24 15:16:21.532115 pypanther-0.1.1a2/pypanther/rules/standard_rules/mfa_disabled.py
--rw-r--r--   0        0        0     9929 2024-05-24 12:40:18.501241 pypanther-0.1.1a2/pypanther/rules/standard_rules/standard_dns_base64.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353861 pypanther-0.1.1a2/pypanther/rules/tailscale_rules/__init__.py
--rw-r--r--   0        0        0     4635 2024-05-24 15:16:21.532365 pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
--rw-r--r--   0        0        0     4871 2024-05-24 15:16:21.532637 pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
--rw-r--r--   0        0        0     4652 2024-05-24 15:16:21.532895 pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356684 pypanther-0.1.1a2/pypanther/rules/tines_rules/__init__.py
--rw-r--r--   0        0        0     2570 2024-05-24 15:16:21.533184 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
--rw-r--r--   0        0        0     2810 2024-05-24 15:16:21.533820 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_custom_ca.py
--rw-r--r--   0        0        0     3526 2024-05-24 15:16:21.534457 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
--rw-r--r--   0        0        0     2873 2024-05-24 15:16:21.534800 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_global_resource_destruction.py
--rw-r--r--   0        0        0     2933 2024-05-24 15:16:21.535126 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_sso_settings.py
--rw-r--r--   0        0        0     2751 2024-05-24 15:16:21.535504 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_story_items_destruction.py
--rw-r--r--   0        0        0     2721 2024-05-24 15:16:21.535880 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
--rw-r--r--   0        0        0     2666 2024-05-24 15:16:21.536177 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_team_destruction.py
--rw-r--r--   0        0        0     3973 2024-05-24 15:16:21.536516 pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_tenant_authtoken.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352185 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/__init__.py
--rw-r--r--   0        0        0     3761 2024-05-24 15:16:21.536795 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
--rw-r--r--   0        0        0     2958 2024-05-24 15:16:21.537085 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
--rw-r--r--   0        0        0     3194 2024-05-24 15:16:21.537365 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_new_owner.py
--rw-r--r--   0        0        0     3703 2024-05-24 15:16:21.537713 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
--rw-r--r--   0        0        0     2948 2024-05-24 15:16:21.538004 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
--rw-r--r--   0        0        0     2760 2024-05-24 15:16:21.538287 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_role.py
--rw-r--r--   0        0        0     3913 2024-05-24 15:16:21.538522 pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
--rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353216 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/__init__.py
--rw-r--r--   0        0        0     2676 2024-05-24 15:16:21.538757 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
--rw-r--r--   0        0        0     2345 2024-05-24 15:16:21.538977 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
--rw-r--r--   0        0        0     2816 2024-05-24 15:16:21.539207 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
--rw-r--r--   0        0        0     2746 2024-05-24 15:16:21.539448 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
--rw-r--r--   0        0        0     3344 2024-05-24 15:16:21.539654 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
--rw-r--r--   0        0        0     3544 2024-05-24 15:16:21.539868 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
--rw-r--r--   0        0        0     2606 2024-05-24 15:16:21.540096 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
--rw-r--r--   0        0        0     4606 2024-05-24 15:16:21.540333 pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
--rw-r--r--   0        0        0     4490 2024-05-24 13:47:47.095050 pypanther-0.1.1a2/pypanther/upload.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095097 pypanther-0.1.1a2/pypanther/vendor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095354 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095410 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/__init__.py
--rw-r--r--   0        0        0    16541 2024-05-24 13:47:47.095519 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/client.py
--rw-r--r--   0        0        0      624 2024-05-24 13:47:47.095629 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/errors.py
--rw-r--r--   0        0        0      159 2024-05-24 13:47:47.095796 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
--rw-r--r--   0        0        0      802 2024-05-24 13:47:47.095929 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
--rw-r--r--   0        0        0    13035 2024-05-24 13:47:47.096074 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/lambda_client.py
--rw-r--r--   0        0        0    25446 2024-05-24 13:47:47.096146 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
--rw-r--r--   0        0        0     1606 2024-05-24 13:47:47.096405 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/cli_output.py
--rw-r--r--   0        0        0      738 2024-05-24 13:47:47.096498 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/command/standard_args.py
--rw-r--r--   0        0        0      676 2024-05-24 13:47:47.096574 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/constants.py
--rw-r--r--   0        0        0     2541 2024-05-24 13:47:47.096824 pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/util.py
--rw-r--r--   0        0        0      274 2024-05-23 22:00:33.355426 pypanther-0.1.1a2/pypanther/wrap.py
--rw-r--r--   0        0        0     1720 2024-05-24 15:16:21.540597 pypanther-0.1.1a2/pyproject.toml
--rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 pypanther-0.1.1a2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-22 19:16:21.930547 pypanther-0.1.1a3/LICENSE.txt
+-rw-r--r--   0        0        0       80 2024-05-03 18:47:26.705553 pypanther-0.1.1a3/README.md
+-rw-r--r--   0        0        0      185 2024-05-23 22:00:33.237693 pypanther-0.1.1a3/pypanther/__init__.py
+-rw-r--r--   0        0        0    24586 2024-05-24 15:16:21.423666 pypanther-0.1.1a3/pypanther/base.py
+-rw-r--r--   0        0        0      490 2024-05-23 22:00:33.238107 pypanther-0.1.1a3/pypanther/cache.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:14.952849 pypanther-0.1.1a3/pypanther/data_models/__init__.py
+-rw-r--r--   0        0        0     1387 2024-05-24 12:40:14.944512 pypanther-0.1.1a3/pypanther/data_models/asana_data_model.py
+-rw-r--r--   0        0        0     1544 2024-05-24 12:40:14.933036 pypanther-0.1.1a3/pypanther/data_models/atlassian_data_model.py
+-rw-r--r--   0        0        0      607 2024-05-24 12:40:14.942246 pypanther-0.1.1a3/pypanther/data_models/aws_alb_data_model.py
+-rw-r--r--   0        0        0     2214 2024-05-24 12:40:14.938734 pypanther-0.1.1a3/pypanther/data_models/aws_cloudtrail_data_model.py
+-rw-r--r--   0        0        0     1465 2024-05-24 12:40:14.929894 pypanther-0.1.1a3/pypanther/data_models/aws_eks_data_model.py
+-rw-r--r--   0        0        0      630 2024-05-24 12:40:14.936327 pypanther-0.1.1a3/pypanther/data_models/aws_s3_data_model.py
+-rw-r--r--   0        0        0      593 2024-05-24 12:40:14.939270 pypanther-0.1.1a3/pypanther/data_models/aws_vpcdns_data_model.py
+-rw-r--r--   0        0        0      742 2024-05-24 12:40:14.928634 pypanther-0.1.1a3/pypanther/data_models/aws_vpcflow_data_model.py
+-rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.927521 pypanther-0.1.1a3/pypanther/data_models/azure_signin_data_model.py
+-rw-r--r--   0        0        0      941 2024-05-24 12:40:14.941146 pypanther-0.1.1a3/pypanther/data_models/box_data_model.py
+-rw-r--r--   0        0        0      873 2024-05-24 12:40:14.939822 pypanther-0.1.1a3/pypanther/data_models/cisco_umbrella_data_model.py
+-rw-r--r--   0        0        0      653 2024-05-24 12:40:14.943897 pypanther-0.1.1a3/pypanther/data_models/cloudflare_firewall_data_model.py
+-rw-r--r--   0        0        0      729 2024-05-24 12:40:14.928057 pypanther-0.1.1a3/pypanther/data_models/cloudflare_httpreq_data_model.py
+-rw-r--r--   0        0        0     1853 2024-05-24 12:40:14.943403 pypanther-0.1.1a3/pypanther/data_models/crowdstrike_fdr_data_model.py
+-rw-r--r--   0        0        0     5215 2024-05-24 12:40:14.934292 pypanther-0.1.1a3/pypanther/data_models/gcp_data_model.py
+-rw-r--r--   0        0        0     1613 2024-05-24 12:40:14.937900 pypanther-0.1.1a3/pypanther/data_models/github_data_model.py
+-rw-r--r--   0        0        0     1669 2024-05-24 12:40:14.935584 pypanther-0.1.1a3/pypanther/data_models/gsuite_data_model.py
+-rw-r--r--   0        0        0     1864 2024-05-24 12:40:14.940562 pypanther-0.1.1a3/pypanther/data_models/notion_data_model.py
+-rw-r--r--   0        0        0     2070 2024-05-24 12:40:14.937166 pypanther-0.1.1a3/pypanther/data_models/okta_data_model.py
+-rw-r--r--   0        0        0     1467 2024-05-24 12:40:14.932330 pypanther-0.1.1a3/pypanther/data_models/onelogin_data_model.py
+-rw-r--r--   0        0        0      730 2024-05-24 12:40:14.934876 pypanther-0.1.1a3/pypanther/data_models/onepassword_itemusage_data_model.py
+-rw-r--r--   0        0        0     1058 2024-05-24 12:40:14.941731 pypanther-0.1.1a3/pypanther/data_models/onepassword_signinattempt_data_model.py
+-rw-r--r--   0        0        0     1742 2024-05-24 12:40:14.930685 pypanther-0.1.1a3/pypanther/data_models/panther_audit_data_model.py
+-rw-r--r--   0        0        0      613 2024-05-24 12:40:14.929135 pypanther-0.1.1a3/pypanther/data_models/slack_accesslogs_data_model.py
+-rw-r--r--   0        0        0      711 2024-05-24 12:40:14.942793 pypanther-0.1.1a3/pypanther/data_models/slack_auditlogs_data_model.py
+-rw-r--r--   0        0        0      500 2024-05-24 12:40:14.926474 pypanther-0.1.1a3/pypanther/data_models/slack_integrationlogs_data_model.py
+-rw-r--r--   0        0        0     2714 2024-05-24 12:40:14.931651 pypanther-0.1.1a3/pypanther/data_models/zendesk_data_model.py
+-rw-r--r--   0        0        0      886 2024-05-24 12:40:14.926019 pypanther-0.1.1a3/pypanther/data_models/zoom_activity_data_model.py
+-rw-r--r--   0        0        0     1887 2024-05-24 12:40:14.925345 pypanther-0.1.1a3/pypanther/data_models/zoom_operation_data_model.py
+-rw-r--r--   0        0        0     2682 2024-05-23 22:00:33.243958 pypanther-0.1.1a3/pypanther/get.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:13.778915 pypanther-0.1.1a3/pypanther/helpers/__init__.py
+-rw-r--r--   0        0        0     2107 2024-05-24 12:40:14.169513 pypanther-0.1.1a3/pypanther/helpers/gcp_base_helpers.py
+-rw-r--r--   0        0        0      781 2024-05-24 12:40:14.303335 pypanther-0.1.1a3/pypanther/helpers/gcp_environment.py
+-rw-r--r--   0        0        0     1417 2024-05-24 12:40:13.948393 pypanther-0.1.1a3/pypanther/helpers/panther_asana_helpers.py
+-rw-r--r--   0        0        0     1597 2024-05-24 12:40:14.156772 pypanther-0.1.1a3/pypanther/helpers/panther_audit.py
+-rw-r--r--   0        0        0      555 2024-05-24 12:40:13.952837 pypanther-0.1.1a3/pypanther/helpers/panther_auth0_helpers.py
+-rw-r--r--   0        0        0     1191 2024-05-24 12:40:14.099017 pypanther-0.1.1a3/pypanther/helpers/panther_azuresignin_helpers.py
+-rw-r--r--   0        0        0    19692 2024-05-24 12:40:14.264799 pypanther-0.1.1a3/pypanther/helpers/panther_base_helpers.py
+-rw-r--r--   0        0        0     4529 2024-05-24 12:40:14.146111 pypanther-0.1.1a3/pypanther/helpers/panther_box_helpers.py
+-rw-r--r--   0        0        0     2267 2024-05-24 12:40:13.916642 pypanther-0.1.1a3/pypanther/helpers/panther_cloudflare_helpers.py
+-rw-r--r--   0        0        0      507 2024-05-24 12:40:14.148779 pypanther-0.1.1a3/pypanther/helpers/panther_config.py
+-rw-r--r--   0        0        0      891 2024-05-24 12:40:14.103142 pypanther-0.1.1a3/pypanther/helpers/panther_config_defaults.py
+-rw-r--r--   0        0        0     1043 2024-05-24 12:40:13.795713 pypanther-0.1.1a3/pypanther/helpers/panther_config_overrides.py
+-rw-r--r--   0        0        0     3465 2024-05-24 12:40:13.831736 pypanther-0.1.1a3/pypanther/helpers/panther_default.py
+-rw-r--r--   0        0        0     1288 2024-05-24 12:40:13.811022 pypanther-0.1.1a3/pypanther/helpers/panther_duo_helpers.py
+-rw-r--r--   0        0        0     1118 2024-05-24 12:40:14.384435 pypanther-0.1.1a3/pypanther/helpers/panther_event_type_helpers.py
+-rw-r--r--   0        0        0    12436 2024-05-24 12:40:14.482779 pypanther-0.1.1a3/pypanther/helpers/panther_greynoise_helpers.py
+-rw-r--r--   0        0        0    38305 2024-05-24 12:40:13.902461 pypanther-0.1.1a3/pypanther/helpers/panther_iocs.py
+-rw-r--r--   0        0        0     6497 2024-05-24 12:40:14.002454 pypanther-0.1.1a3/pypanther/helpers/panther_ipinfo_helpers.py
+-rw-r--r--   0        0        0     2154 2024-05-24 12:40:14.015836 pypanther-0.1.1a3/pypanther/helpers/panther_lookuptable_helpers.py
+-rw-r--r--   0        0        0      387 2024-05-24 12:40:14.270284 pypanther-0.1.1a3/pypanther/helpers/panther_mongodb_helpers.py
+-rw-r--r--   0        0        0      340 2024-05-24 12:40:13.834434 pypanther-0.1.1a3/pypanther/helpers/panther_notion_helpers.py
+-rw-r--r--   0        0        0    13096 2024-05-24 12:40:14.370655 pypanther-0.1.1a3/pypanther/helpers/panther_oss_helpers.py
+-rw-r--r--   0        0        0      610 2024-05-24 12:40:13.801982 pypanther-0.1.1a3/pypanther/helpers/panther_snyk_helpers.py
+-rw-r--r--   0        0        0      492 2024-05-24 12:40:14.307780 pypanther-0.1.1a3/pypanther/helpers/panther_tailscale_helpers.py
+-rw-r--r--   0        0        0      567 2024-05-24 12:40:14.312664 pypanther-0.1.1a3/pypanther/helpers/panther_tines_helpers.py
+-rw-r--r--   0        0        0     1542 2024-05-24 12:40:14.379643 pypanther-0.1.1a3/pypanther/helpers/panther_tor_helpers.py
+-rw-r--r--   0        0        0     3084 2024-05-24 12:40:13.935600 pypanther-0.1.1a3/pypanther/helpers/panther_zoom_helpers.py
+-rw-r--r--   0        0        0    13022 2024-05-23 22:06:29.350498 pypanther-0.1.1a3/pypanther/log_types.py
+-rw-r--r--   0        0        0     1322 2024-05-24 13:47:47.094872 pypanther-0.1.1a3/pypanther/main.py
+-rw-r--r--   0        0        0      824 2024-05-23 22:00:33.250813 pypanther-0.1.1a3/pypanther/register.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.351956 pypanther-0.1.1a3/pypanther/rules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356408 pypanther-0.1.1a3/pypanther/rules/asana_rules/__init__.py
+-rw-r--r--   0        0        0     4055 2024-05-24 15:16:21.424215 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_service_account_created.py
+-rw-r--r--   0        0        0     3227 2024-05-24 15:16:21.424547 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_team_privacy_public.py
+-rw-r--r--   0        0        0     3249 2024-05-24 15:16:21.425052 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py
+-rw-r--r--   0        0        0     3218 2024-05-24 15:16:21.425432 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py
+-rw-r--r--   0        0        0     3406 2024-05-24 15:16:21.425777 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py
+-rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.426151 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py
+-rw-r--r--   0        0        0     3733 2024-05-24 15:16:21.426488 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_new_admin.py
+-rw-r--r--   0        0        0     3228 2024-05-24 15:16:21.426739 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_org_export.py
+-rw-r--r--   0        0        0     3711 2024-05-24 15:16:21.427013 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py
+-rw-r--r--   0        0        0     3615 2024-05-24 15:16:21.427323 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py
+-rw-r--r--   0        0        0     3484 2024-05-24 15:16:21.427559 pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_saml_optional.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355786 pypanther-0.1.1a3/pypanther/rules/atlassian_rules/__init__.py
+-rw-r--r--   0        0        0     4877 2024-05-24 15:16:21.428031 pypanther-0.1.1a3/pypanther/rules/atlassian_rules/user_logged_in_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352374 pypanther-0.1.1a3/pypanther/rules/auth0_rules/__init__.py
+-rw-r--r--   0        0        0    44986 2024-05-24 15:16:21.428415 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_custom_role_created.py
+-rw-r--r--   0        0        0    15412 2024-05-24 15:16:21.428810 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_integration_installed.py
+-rw-r--r--   0        0        0    23138 2024-05-24 15:16:21.429303 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py
+-rw-r--r--   0        0        0    23488 2024-05-24 15:16:21.429696 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py
+-rw-r--r--   0        0        0    34159 2024-05-24 15:16:21.430104 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py
+-rw-r--r--   0        0        0    23642 2024-05-24 15:16:21.430380 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py
+-rw-r--r--   0        0        0    22663 2024-05-24 15:16:21.430665 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py
+-rw-r--r--   0        0        0    19817 2024-05-24 15:16:21.431047 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py
+-rw-r--r--   0        0        0    17279 2024-05-24 15:16:21.431316 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_invitation_created.py
+-rw-r--r--   0        0        0    18166 2024-05-24 15:16:21.431594 pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354895 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/__init__.py
+-rw-r--r--   0        0        0    11009 2024-05-24 15:16:21.431991 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py
+-rw-r--r--   0        0        0     8189 2024-05-24 15:16:21.432404 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py
+-rw-r--r--   0        0        0     7038 2024-05-24 15:16:21.432638 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py
+-rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.432859 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py
+-rw-r--r--   0        0        0     7212 2024-05-24 15:16:21.433158 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py
+-rw-r--r--   0        0        0     4460 2024-05-24 12:40:19.072096 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py
+-rw-r--r--   0        0        0     6992 2024-05-24 15:16:21.433498 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py
+-rw-r--r--   0        0        0     6551 2024-05-24 15:16:21.433773 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py
+-rw-r--r--   0        0        0     6538 2024-05-24 15:16:21.434033 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py
+-rw-r--r--   0        0        0    20551 2024-05-24 15:16:21.434298 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py
+-rw-r--r--   0        0        0     4027 2024-05-24 12:40:19.137363 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py
+-rw-r--r--   0        0        0     5596 2024-05-24 15:16:21.434553 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py
+-rw-r--r--   0        0        0     5699 2024-05-24 15:16:21.434870 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py
+-rw-r--r--   0        0        0     2281 2024-05-24 15:16:21.435209 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py
+-rw-r--r--   0        0        0     6712 2024-05-24 15:16:21.435527 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py
+-rw-r--r--   0        0        0    17193 2024-05-24 12:40:19.013686 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py
+-rw-r--r--   0        0        0    22406 2024-05-24 15:16:21.435872 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py
+-rw-r--r--   0        0        0     7244 2024-05-24 15:16:21.436155 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py
+-rw-r--r--   0        0        0     6874 2024-05-24 15:16:21.436423 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py
+-rw-r--r--   0        0        0     8171 2024-05-24 15:16:21.436705 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py
+-rw-r--r--   0        0        0     5159 2024-05-24 15:16:21.436966 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py
+-rw-r--r--   0        0        0    30269 2024-05-24 15:16:21.437319 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py
+-rw-r--r--   0        0        0     8600 2024-05-24 15:16:21.437710 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py
+-rw-r--r--   0        0        0    39729 2024-05-24 15:16:21.437986 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py
+-rw-r--r--   0        0        0    27319 2024-05-24 12:40:19.153333 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py
+-rw-r--r--   0        0        0    26728 2024-05-24 12:40:19.048210 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py
+-rw-r--r--   0        0        0     7262 2024-05-24 15:16:21.438351 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py
+-rw-r--r--   0        0        0     8581 2024-05-24 12:40:19.131595 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py
+-rw-r--r--   0        0        0     6105 2024-05-24 15:16:21.438771 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py
+-rw-r--r--   0        0        0    12705 2024-05-24 12:40:19.146336 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py
+-rw-r--r--   0        0        0    13749 2024-05-24 12:40:19.032961 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py
+-rw-r--r--   0        0        0     7140 2024-05-24 15:16:21.439018 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py
+-rw-r--r--   0        0        0    10477 2024-05-24 15:16:21.439288 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py
+-rw-r--r--   0        0        0     9036 2024-05-24 15:16:21.439564 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py
+-rw-r--r--   0        0        0     3375 2024-05-24 15:16:21.439795 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py
+-rw-r--r--   0        0        0     5202 2024-05-24 15:16:21.440052 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py
+-rw-r--r--   0        0        0    11250 2024-05-24 15:16:21.440309 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py
+-rw-r--r--   0        0        0     5716 2024-05-24 12:40:19.030090 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py
+-rw-r--r--   0        0        0     9720 2024-05-24 15:16:21.440570 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py
+-rw-r--r--   0        0        0    26986 2024-05-24 12:40:19.164857 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py
+-rw-r--r--   0        0        0     7813 2024-05-24 15:16:21.440884 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py
+-rw-r--r--   0        0        0    16362 2024-05-24 15:16:21.441210 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py
+-rw-r--r--   0        0        0    14625 2024-05-24 15:16:21.441626 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py
+-rw-r--r--   0        0        0    17386 2024-05-24 15:16:21.441875 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py
+-rw-r--r--   0        0        0     7466 2024-05-24 15:16:21.442158 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py
+-rw-r--r--   0        0        0    18968 2024-05-24 15:16:21.442383 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py
+-rw-r--r--   0        0        0     4655 2024-05-24 15:16:21.442623 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py
+-rw-r--r--   0        0        0    10739 2024-05-24 15:16:21.442885 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py
+-rw-r--r--   0        0        0     3920 2024-05-24 15:16:21.443092 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py
+-rw-r--r--   0        0        0     5811 2024-05-24 15:16:21.443361 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py
+-rw-r--r--   0        0        0     7502 2024-05-24 15:16:21.443687 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py
+-rw-r--r--   0        0        0    12275 2024-05-24 15:16:21.443990 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py
+-rw-r--r--   0        0        0    11502 2024-05-24 15:16:21.444278 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py
+-rw-r--r--   0        0        0     5556 2024-05-24 15:16:21.444534 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py
+-rw-r--r--   0        0        0     7544 2024-05-24 15:16:21.444768 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py
+-rw-r--r--   0        0        0     5177 2024-05-24 12:40:19.036764 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py
+-rw-r--r--   0        0        0     6464 2024-05-24 15:16:21.445000 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py
+-rw-r--r--   0        0        0     8683 2024-05-24 12:40:19.124611 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py
+-rw-r--r--   0        0        0     5962 2024-05-24 15:16:21.445244 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py
+-rw-r--r--   0        0        0     6768 2024-05-24 15:16:21.445508 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py
+-rw-r--r--   0        0        0     7010 2024-05-24 15:16:21.445747 pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352785 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/__init__.py
+-rw-r--r--   0        0        0     9686 2024-05-24 15:16:21.446020 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py
+-rw-r--r--   0        0        0    17799 2024-05-24 15:16:21.446254 pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354748 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/__init__.py
+-rw-r--r--   0        0        0     5356 2024-05-24 15:16:21.446559 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py
+-rw-r--r--   0        0        0     5377 2024-05-24 15:16:21.446848 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py
+-rw-r--r--   0        0        0     5403 2024-05-24 15:16:21.447130 pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355307 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/__init__.py
+-rw-r--r--   0        0        0     4688 2024-05-24 15:16:21.447407 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_error.py
+-rw-r--r--   0        0        0     2546 2024-05-24 12:40:19.231135 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py
+-rw-r--r--   0        0        0     6263 2024-05-24 15:16:21.447657 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py
+-rw-r--r--   0        0        0     1983 2024-05-24 12:40:19.239787 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py
+-rw-r--r--   0        0        0     8734 2024-05-24 12:40:19.236359 pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355429 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/__init__.py
+-rw-r--r--   0        0        0     6776 2024-05-24 15:16:21.447901 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py
+-rw-r--r--   0        0        0     1326 2024-05-24 15:16:21.448149 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py
+-rw-r--r--   0        0        0     2524 2024-05-24 12:40:19.241211 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py
+-rw-r--r--   0        0        0     2484 2024-05-24 12:40:19.248154 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py
+-rw-r--r--   0        0        0     2913 2024-05-24 12:40:19.246794 pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355171 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/__init__.py
+-rw-r--r--   0        0        0     7964 2024-05-24 15:16:21.448405 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_failed_signins.py
+-rw-r--r--   0        0        0    15752 2024-05-24 15:16:21.448657 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_legacyauth.py
+-rw-r--r--   0        0        0    17539 2024-05-24 15:16:21.448880 pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353050 pypanther-0.1.1a3/pypanther/rules/box_rules/__init__.py
+-rw-r--r--   0        0        0     2120 2024-05-24 15:16:21.449114 pypanther-0.1.1a3/pypanther/rules/box_rules/box_access_granted.py
+-rw-r--r--   0        0        0     2855 2024-05-24 15:16:21.449326 pypanther-0.1.1a3/pypanther/rules/box_rules/box_anomalous_download.py
+-rw-r--r--   0        0        0     2730 2024-05-24 12:40:18.694430 pypanther-0.1.1a3/pypanther/rules/box_rules/box_event_triggered_externally.py
+-rw-r--r--   0        0        0     3638 2024-05-24 12:40:18.687439 pypanther-0.1.1a3/pypanther/rules/box_rules/box_item_shared_externally.py
+-rw-r--r--   0        0        0     4252 2024-05-24 15:16:21.449561 pypanther-0.1.1a3/pypanther/rules/box_rules/box_malicious_content.py
+-rw-r--r--   0        0        0     2110 2024-05-24 15:16:21.449767 pypanther-0.1.1a3/pypanther/rules/box_rules/box_new_login.py
+-rw-r--r--   0        0        0     2808 2024-05-24 15:16:21.449973 pypanther-0.1.1a3/pypanther/rules/box_rules/box_policy_violation.py
+-rw-r--r--   0        0        0     4201 2024-05-24 15:16:21.450221 pypanther-0.1.1a3/pypanther/rules/box_rules/box_suspicious_login_or_session.py
+-rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.450435 pypanther-0.1.1a3/pypanther/rules/box_rules/box_untrusted_device.py
+-rw-r--r--   0        0        0     2352 2024-05-24 15:16:21.450657 pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_downloads.py
+-rw-r--r--   0        0        0     3165 2024-05-24 15:16:21.450863 pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_permission_updates.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355655 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/__init__.py
+-rw-r--r--   0        0        0     3299 2024-05-24 15:16:21.451080 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py
+-rw-r--r--   0        0        0     3023 2024-05-24 15:16:21.451306 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py
+-rw-r--r--   0        0        0     3473 2024-05-24 15:16:21.451550 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py
+-rw-r--r--   0        0        0     2248 2024-05-24 15:16:21.451767 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_flagged.py
+-rw-r--r--   0        0        0     2577 2024-05-24 15:16:21.451988 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py
+-rw-r--r--   0        0        0    11303 2024-05-24 15:16:21.452260 pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355556 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/__init__.py
+-rw-r--r--   0        0        0     1787 2024-05-24 15:16:21.452540 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py
+-rw-r--r--   0        0        0     1414 2024-05-24 12:40:19.250591 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py
+-rw-r--r--   0        0        0     1903 2024-05-24 12:40:19.253188 pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354017 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/__init__.py
+-rw-r--r--   0        0        0     4969 2024-05-24 15:16:21.452875 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py
+-rw-r--r--   0        0        0     7563 2024-05-24 12:40:18.920956 pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355030 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/__init__.py
+-rw-r--r--   0        0        0    29385 2024-05-24 15:16:21.453267 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py
+-rw-r--r--   0        0        0     8177 2024-05-24 15:16:21.453668 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py
+-rw-r--r--   0        0        0     9893 2024-05-24 15:16:21.453945 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py
+-rw-r--r--   0        0        0     9855 2024-05-24 15:16:21.454211 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py
+-rw-r--r--   0        0        0    10420 2024-05-24 15:16:21.454477 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py
+-rw-r--r--   0        0        0    12177 2024-05-24 12:40:19.187772 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py
+-rw-r--r--   0        0        0    11711 2024-05-24 12:40:19.205936 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py
+-rw-r--r--   0        0        0    18680 2024-05-24 15:16:21.454710 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py
+-rw-r--r--   0        0        0    18887 2024-05-24 15:16:21.454956 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py
+-rw-r--r--   0        0        0    15614 2024-05-24 15:16:21.455287 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py
+-rw-r--r--   0        0        0     7208 2024-05-24 15:16:21.455541 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py
+-rw-r--r--   0        0        0     9722 2024-05-24 15:16:21.455811 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py
+-rw-r--r--   0        0        0    13594 2024-05-24 15:16:21.456062 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py
+-rw-r--r--   0        0        0     9703 2024-05-24 15:16:21.456322 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py
+-rw-r--r--   0        0        0    10006 2024-05-24 15:16:21.456575 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py
+-rw-r--r--   0        0        0    17357 2024-05-24 15:16:21.456795 pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354190 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/__init__.py
+-rw-r--r--   0        0        0     6793 2024-05-24 15:16:21.457052 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py
+-rw-r--r--   0        0        0     9494 2024-05-24 15:16:21.457293 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_external_share.py
+-rw-r--r--   0        0        0     8238 2024-05-24 15:16:21.457569 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py
+-rw-r--r--   0        0        0    11142 2024-05-24 15:16:21.457840 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py
+-rw-r--r--   0        0        0     5131 2024-05-24 15:16:21.458095 pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353471 pypanther-0.1.1a3/pypanther/rules/duo_rules/__init__.py
+-rw-r--r--   0        0        0     2088 2024-05-24 15:16:21.458537 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py
+-rw-r--r--   0        0        0     2175 2024-05-24 15:16:21.460660 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py
+-rw-r--r--   0        0        0     2244 2024-05-24 15:16:21.460989 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py
+-rw-r--r--   0        0        0     2241 2024-05-24 15:16:21.461264 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_create_admin.py
+-rw-r--r--   0        0        0     2508 2024-05-24 15:16:21.461517 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_lockout.py
+-rw-r--r--   0        0        0     2658 2024-05-24 15:16:21.461765 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py
+-rw-r--r--   0        0        0     1968 2024-05-24 15:16:21.461984 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py
+-rw-r--r--   0        0        0     3144 2024-05-24 15:16:21.462206 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py
+-rw-r--r--   0        0        0     2208 2024-05-24 15:16:21.462435 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_policy_updated.py
+-rw-r--r--   0        0        0     3376 2024-05-24 15:16:21.462674 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py
+-rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.462911 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py
+-rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.463155 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_action_fraudulent.py
+-rw-r--r--   0        0        0     3152 2024-05-24 15:16:21.463423 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_anomalous_push.py
+-rw-r--r--   0        0        0     3058 2024-05-24 15:16:21.463696 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_bypass_code_used.py
+-rw-r--r--   0        0        0     5450 2024-05-24 15:16:21.463967 pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353698 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/__init__.py
+-rw-r--r--   0        0        0     9839 2024-05-24 15:16:21.464276 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py
+-rw-r--r--   0        0        0    12333 2024-05-24 15:16:21.464557 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py
+-rw-r--r--   0        0        0     7045 2024-05-24 15:16:21.464840 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py
+-rw-r--r--   0        0        0     7839 2024-05-24 15:16:21.465105 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py
+-rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465357 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py
+-rw-r--r--   0        0        0     4127 2024-05-24 15:16:21.465626 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py
+-rw-r--r--   0        0        0    19128 2024-05-24 15:16:21.465900 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py
+-rw-r--r--   0        0        0    10432 2024-05-24 15:16:21.466320 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py
+-rw-r--r--   0        0        0    15433 2024-05-24 15:16:21.466688 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py
+-rw-r--r--   0        0        0     9149 2024-05-24 15:16:21.467069 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py
+-rw-r--r--   0        0        0     6818 2024-05-24 15:16:21.467438 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py
+-rw-r--r--   0        0        0     8941 2024-05-24 15:16:21.467837 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py
+-rw-r--r--   0        0        0     3831 2024-05-24 15:16:21.468230 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py
+-rw-r--r--   0        0        0     4527 2024-05-24 15:16:21.468564 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py
+-rw-r--r--   0        0        0    15793 2024-05-24 15:16:21.468870 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py
+-rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.469204 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py
+-rw-r--r--   0        0        0     9941 2024-05-24 15:16:21.469591 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py
+-rw-r--r--   0        0        0     3579 2024-05-24 15:16:21.469975 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py
+-rw-r--r--   0        0        0     4115 2024-05-24 15:16:21.470322 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py
+-rw-r--r--   0        0        0     6785 2024-05-24 15:16:21.470690 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py
+-rw-r--r--   0        0        0     6585 2024-05-24 15:16:21.471079 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py
+-rw-r--r--   0        0        0     7304 2024-05-24 15:16:21.471358 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py
+-rw-r--r--   0        0        0     9263 2024-05-24 15:16:21.471651 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py
+-rw-r--r--   0        0        0    11294 2024-05-24 15:16:21.471923 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py
+-rw-r--r--   0        0        0     7615 2024-05-24 15:16:21.472188 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py
+-rw-r--r--   0        0        0     7079 2024-05-24 15:16:21.472435 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py
+-rw-r--r--   0        0        0    10607 2024-05-24 15:16:21.472706 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py
+-rw-r--r--   0        0        0     4068 2024-05-24 15:16:21.473027 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py
+-rw-r--r--   0        0        0     7714 2024-05-24 15:16:21.473395 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py
+-rw-r--r--   0        0        0    11742 2024-05-24 15:16:21.473678 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py
+-rw-r--r--   0        0        0    10816 2024-05-24 15:16:21.473953 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py
+-rw-r--r--   0        0        0     2275 2024-05-24 15:16:21.474180 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py
+-rw-r--r--   0        0        0     2911 2024-05-24 15:16:21.474491 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py
+-rw-r--r--   0        0        0    13058 2024-05-24 12:40:18.866059 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py
+-rw-r--r--   0        0        0    10910 2024-05-24 15:16:21.474877 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py
+-rw-r--r--   0        0        0     9626 2024-05-24 15:16:21.475160 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py
+-rw-r--r--   0        0        0    10164 2024-05-24 15:16:21.475430 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py
+-rw-r--r--   0        0        0    11767 2024-05-24 15:16:21.475792 pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352868 pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/__init__.py
+-rw-r--r--   0        0        0     5908 2024-05-24 15:16:21.476184 pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356266 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/__init__.py
+-rw-r--r--   0        0        0     4559 2024-05-24 15:16:21.476451 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py
+-rw-r--r--   0        0        0     6701 2024-05-24 12:40:19.340583 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py
+-rw-r--r--   0        0        0     2251 2024-05-24 15:16:21.476747 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py
+-rw-r--r--   0        0        0     3530 2024-05-24 15:16:21.477098 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py
+-rw-r--r--   0        0        0     3433 2024-05-24 15:16:21.477323 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py
+-rw-r--r--   0        0        0    12867 2024-05-24 15:16:21.477684 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py
+-rw-r--r--   0        0        0     3499 2024-05-24 15:16:21.477988 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py
+-rw-r--r--   0        0        0    14878 2024-05-24 15:16:21.478411 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py
+-rw-r--r--   0        0        0    11462 2024-05-24 15:16:21.478669 pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352570 pypanther-0.1.1a3/pypanther/rules/github_rules/__init__.py
+-rw-r--r--   0        0        0     5241 2024-05-24 12:40:18.616900 pypanther-0.1.1a3/pypanther/rules/github_rules/github_action_failed.py
+-rw-r--r--   0        0        0    14192 2024-05-24 15:16:21.478946 pypanther-0.1.1a3/pypanther/rules/github_rules/github_advanced_security_change.py
+-rw-r--r--   0        0        0     2028 2024-05-24 15:16:21.479163 pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_policy_override.py
+-rw-r--r--   0        0        0     2030 2024-05-24 15:16:21.479385 pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_protection_disabled.py
+-rw-r--r--   0        0        0     2223 2024-05-24 15:16:21.479616 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_auth_modified.py
+-rw-r--r--   0        0        0     2409 2024-05-24 15:16:21.479861 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_ip_allowlist.py
+-rw-r--r--   0        0        0     2212 2024-05-24 15:16:21.480172 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_moderators_add.py
+-rw-r--r--   0        0        0     2302 2024-05-24 15:16:21.480396 pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_modified.py
+-rw-r--r--   0        0        0     3381 2024-05-24 15:16:21.480613 pypanther-0.1.1a3/pypanther/rules/github_rules/github_organization_app_integration_installed.py
+-rw-r--r--   0        0        0     2847 2024-05-24 15:16:21.480830 pypanther-0.1.1a3/pypanther/rules/github_rules/github_public_repository_created.py
+-rw-r--r--   0        0        0     2762 2024-05-24 15:16:21.481050 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_collaborator_change.py
+-rw-r--r--   0        0        0     1446 2024-05-24 15:16:21.481310 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_created.py
+-rw-r--r--   0        0        0     2501 2024-05-24 15:16:21.481577 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_hook_modified.py
+-rw-r--r--   0        0        0     4211 2024-05-24 15:16:21.482079 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_initial_access.py
+-rw-r--r--   0        0        0     1890 2024-05-24 15:16:21.482329 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_visibility_change.py
+-rw-r--r--   0        0        0     5328 2024-05-24 15:16:21.482612 pypanther-0.1.1a3/pypanther/rules/github_rules/github_repository_transfer.py
+-rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.482858 pypanther-0.1.1a3/pypanther/rules/github_rules/github_secret_scanning_alert_created.py
+-rw-r--r--   0        0        0     3326 2024-05-24 15:16:21.483159 pypanther-0.1.1a3/pypanther/rules/github_rules/github_team_modified.py
+-rw-r--r--   0        0        0     1622 2024-05-24 15:16:21.483409 pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_access_key_created.py
+-rw-r--r--   0        0        0     1725 2024-05-24 15:16:21.483706 pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_role_updated.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356132 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/__init__.py
+-rw-r--r--   0        0        0     2333 2024-05-24 15:16:21.484015 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0     2789 2024-05-24 15:16:21.484312 pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352688 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-24 15:16:21.484638 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py
+-rw-r--r--   0        0        0     2631 2024-05-24 15:16:21.484883 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py
+-rw-r--r--   0        0        0     3188 2024-05-24 15:16:21.485119 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py
+-rw-r--r--   0        0        0     2947 2024-05-24 15:16:21.485352 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py
+-rw-r--r--   0        0        0     1749 2024-05-24 15:16:21.485594 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py
+-rw-r--r--   0        0        0     6365 2024-05-24 15:16:21.485875 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py
+-rw-r--r--   0        0        0     4716 2024-05-24 15:16:21.486157 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py
+-rw-r--r--   0        0        0     1593 2024-05-24 15:16:21.486399 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py
+-rw-r--r--   0        0        0     2190 2024-05-24 15:16:21.486639 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py
+-rw-r--r--   0        0        0     1614 2024-05-24 15:16:21.486861 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py
+-rw-r--r--   0        0        0     2739 2024-05-24 15:16:21.487116 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py
+-rw-r--r--   0        0        0     4429 2024-05-24 15:16:21.487415 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py
+-rw-r--r--   0        0        0     3205 2024-05-24 15:16:21.487780 pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354403 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/__init__.py
+-rw-r--r--   0        0        0     4360 2024-05-24 15:16:21.488109 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py
+-rw-r--r--   0        0        0     6479 2024-05-24 15:16:21.488371 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py
+-rw-r--r--   0        0        0     6692 2024-05-24 15:16:21.488623 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py
+-rw-r--r--   0        0        0     5269 2024-05-24 15:16:21.488868 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py
+-rw-r--r--   0        0        0     4631 2024-05-24 15:16:21.489112 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py
+-rw-r--r--   0        0        0     1947 2024-05-24 15:16:21.489391 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py
+-rw-r--r--   0        0        0     5772 2024-05-24 15:16:21.489802 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py
+-rw-r--r--   0        0        0     2325 2024-05-24 12:40:18.988544 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py
+-rw-r--r--   0        0        0     4324 2024-05-24 12:40:18.990649 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py
+-rw-r--r--   0        0        0     1451 2024-05-24 15:16:21.490098 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py
+-rw-r--r--   0        0        0     1984 2024-05-24 15:16:21.490412 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py
+-rw-r--r--   0        0        0     1949 2024-05-24 15:16:21.490708 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py
+-rw-r--r--   0        0        0     3035 2024-05-24 15:16:21.491052 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py
+-rw-r--r--   0        0        0     3459 2024-05-24 12:40:18.954789 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py
+-rw-r--r--   0        0        0     2728 2024-05-24 15:16:21.491353 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py
+-rw-r--r--   0        0        0     3373 2024-05-24 15:16:21.491620 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py
+-rw-r--r--   0        0        0     2006 2024-05-24 15:16:21.491969 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py
+-rw-r--r--   0        0        0     3443 2024-05-24 15:16:21.492331 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py
+-rw-r--r--   0        0        0     2573 2024-05-24 15:16:21.492593 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py
+-rw-r--r--   0        0        0     2189 2024-05-24 15:16:21.492877 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py
+-rw-r--r--   0        0        0     2707 2024-05-24 15:16:21.493162 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py
+-rw-r--r--   0        0        0     6820 2024-05-24 15:16:21.493443 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py
+-rw-r--r--   0        0        0     4999 2024-05-24 15:16:21.493742 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py
+-rw-r--r--   0        0        0     6038 2024-05-24 15:16:21.493994 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py
+-rw-r--r--   0        0        0     5438 2024-05-24 15:16:21.494274 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py
+-rw-r--r--   0        0        0     5208 2024-05-24 15:16:21.494563 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py
+-rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.494909 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py
+-rw-r--r--   0        0        0     4963 2024-05-24 15:16:21.495174 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py
+-rw-r--r--   0        0        0     5209 2024-05-24 15:16:21.495453 pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353938 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/__init__.py
+-rw-r--r--   0        0        0    10537 2024-05-24 12:40:18.909156 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py
+-rw-r--r--   0        0        0     4546 2024-05-24 15:16:21.495759 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py
+-rw-r--r--   0        0        0    25444 2024-05-24 12:40:18.913974 pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354103 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/__init__.py
+-rw-r--r--   0        0        0     4649 2024-05-24 15:16:21.496043 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py
+-rw-r--r--   0        0        0     4396 2024-05-24 15:16:21.496301 pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_user_account_logging.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353568 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/__init__.py
+-rw-r--r--   0        0        0     4569 2024-05-24 15:16:21.496570 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py
+-rw-r--r--   0        0        0     9668 2024-05-24 15:16:21.496852 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py
+-rw-r--r--   0        0        0     6301 2024-05-24 15:16:21.497132 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py
+-rw-r--r--   0        0        0    10170 2024-05-24 15:16:21.497409 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py
+-rw-r--r--   0        0        0     5158 2024-05-24 15:16:21.497661 pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352474 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/__init__.py
+-rw-r--r--   0        0        0     3349 2024-05-24 15:16:21.497893 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py
+-rw-r--r--   0        0        0     2854 2024-05-24 15:16:21.498106 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py
+-rw-r--r--   0        0        0     2697 2024-05-24 15:16:21.498314 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py
+-rw-r--r--   0        0        0     4160 2024-05-24 15:16:21.498569 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py
+-rw-r--r--   0        0        0     4357 2024-05-24 15:16:21.498812 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py
+-rw-r--r--   0        0        0     3944 2024-05-24 15:16:21.499034 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py
+-rw-r--r--   0        0        0     2270 2024-05-24 15:16:21.499318 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py
+-rw-r--r--   0        0        0     3341 2024-05-24 15:16:21.499611 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py
+-rw-r--r--   0        0        0     3201 2024-05-24 15:16:21.499917 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py
+-rw-r--r--   0        0        0     4756 2024-05-24 15:16:21.500167 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py
+-rw-r--r--   0        0        0     3421 2024-05-24 15:16:21.500388 pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352276 pypanther-0.1.1a3/pypanther/rules/netskope_rules/__init__.py
+-rw-r--r--   0        0        0     2974 2024-05-24 15:16:21.500620 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_logged_out.py
+-rw-r--r--   0        0        0     3556 2024-05-24 15:16:21.500849 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_user_change.py
+-rw-r--r--   0        0        0     2713 2024-05-24 15:16:21.501051 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_many_deletes.py
+-rw-r--r--   0        0        0     2902 2024-05-24 15:16:21.501271 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_personnel_action.py
+-rw-r--r--   0        0        0     3159 2024-05-24 15:16:21.501490 pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353782 pypanther-0.1.1a3/pypanther/rules/notion_rules/__init__.py
+-rw-r--r--   0        0        0    16708 2024-05-24 15:16:21.501785 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_account_changed_after_login.py
+-rw-r--r--   0        0        0     1529 2024-05-24 12:40:18.870179 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py
+-rw-r--r--   0        0        0    15410 2024-05-24 15:16:21.502697 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_new_location.py
+-rw-r--r--   0        0        0     3273 2024-05-24 15:16:21.503542 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_deleted.py
+-rw-r--r--   0        0        0     3269 2024-05-24 15:16:21.503922 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_exported.py
+-rw-r--r--   0        0        0     1747 2024-05-24 15:16:21.504555 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_api.py
+-rw-r--r--   0        0        0     5395 2024-05-24 15:16:21.504913 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py
+-rw-r--r--   0        0        0     1641 2024-05-24 15:16:21.505220 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_shared_to_web.py
+-rw-r--r--   0        0        0     2869 2024-05-24 15:16:21.505506 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_scim_token_generated.py
+-rw-r--r--   0        0        0     3872 2024-05-24 15:16:21.505825 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_sharing_settings_updated.py
+-rw-r--r--   0        0        0     4470 2024-05-24 15:16:21.506092 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_teamspace_owner_added.py
+-rw-r--r--   0        0        0     2995 2024-05-24 15:16:21.506343 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py
+-rw-r--r--   0        0        0     3264 2024-05-24 15:16:21.506586 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_exported.py
+-rw-r--r--   0        0        0     4548 2024-05-24 15:16:21.506857 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py
+-rw-r--r--   0        0        0     4402 2024-05-24 15:16:21.507127 pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356572 pypanther-0.1.1a3/pypanther/rules/okta_rules/__init__.py
+-rw-r--r--   0        0        0     3624 2024-05-24 15:16:21.507388 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_account_support_access.py
+-rw-r--r--   0        0        0     3475 2024-05-24 15:16:21.507645 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py
+-rw-r--r--   0        0        0     7243 2024-05-24 15:16:21.507905 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_role_assigned.py
+-rw-r--r--   0        0        0     7625 2024-05-24 15:16:21.508163 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py
+-rw-r--r--   0        0        0     2638 2024-05-24 15:16:21.508396 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_created.py
+-rw-r--r--   0        0        0     2483 2024-05-24 15:16:21.508645 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_revoked.py
+-rw-r--r--   0        0        0     9042 2024-05-24 15:16:21.508933 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py
+-rw-r--r--   0        0        0     7515 2024-05-24 15:16:21.509199 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py
+-rw-r--r--   0        0        0     7396 2024-05-24 15:16:21.509456 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py
+-rw-r--r--   0        0        0     8132 2024-05-24 15:16:21.509731 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_create_modify.py
+-rw-r--r--   0        0        0     8222 2024-05-24 12:40:19.414785 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_signin.py
+-rw-r--r--   0        0        0    13813 2024-05-24 15:16:21.510023 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py
+-rw-r--r--   0        0        0    13457 2024-05-24 15:16:21.510285 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_org2org_creation_modification.py
+-rw-r--r--   0        0        0    10936 2024-05-24 15:16:21.510562 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_accessed.py
+-rw-r--r--   0        0        0     7709 2024-05-24 15:16:21.510819 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py
+-rw-r--r--   0        0        0     7652 2024-05-24 15:16:21.511084 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py
+-rw-r--r--   0        0        0    19397 2024-05-24 15:16:21.511361 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_potentially_stolen_session.py
+-rw-r--r--   0        0        0    10687 2024-05-24 15:16:21.511669 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_rate_limits.py
+-rw-r--r--   0        0        0     4995 2024-05-24 15:16:21.511930 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_support_reset.py
+-rw-r--r--   0        0        0     9198 2024-05-24 15:16:21.512255 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py
+-rw-r--r--   0        0        0     6846 2024-05-24 15:16:21.512684 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_account_locked.py
+-rw-r--r--   0        0        0     7006 2024-05-24 15:16:21.513054 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py
+-rw-r--r--   0        0        0     4170 2024-05-24 15:16:21.513390 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset.py
+-rw-r--r--   0        0        0     5452 2024-05-24 15:16:21.513642 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py
+-rw-r--r--   0        0        0     8388 2024-05-24 15:16:21.513988 pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352956 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/__init__.py
+-rw-r--r--   0        0        0     3840 2024-05-24 15:16:21.514248 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py
+-rw-r--r--   0        0        0     1955 2024-05-24 15:16:21.514508 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py
+-rw-r--r--   0        0        0     2473 2024-05-24 15:16:21.514744 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py
+-rw-r--r--   0        0        0     2280 2024-05-24 15:16:21.514994 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_accessed.py
+-rw-r--r--   0        0        0     2187 2024-05-24 15:16:21.515230 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_changed.py
+-rw-r--r--   0        0        0     2656 2024-05-24 15:16:21.515454 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py
+-rw-r--r--   0        0        0     1879 2024-05-24 15:16:21.515683 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py
+-rw-r--r--   0        0        0     1921 2024-05-24 15:16:21.515917 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py
+-rw-r--r--   0        0        0     1848 2024-05-24 15:16:21.516156 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py
+-rw-r--r--   0        0        0     2545 2024-05-24 15:16:21.516389 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py
+-rw-r--r--   0        0        0     1995 2024-05-24 15:16:21.516648 pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_assumed.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353133 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/__init__.py
+-rw-r--r--   0        0        0     4565 2024-05-24 12:40:18.700457 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py
+-rw-r--r--   0        0        0     3917 2024-05-24 12:40:18.705317 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py
+-rw-r--r--   0        0        0     4427 2024-05-24 15:16:21.516925 pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_unusual_client.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356027 pypanther-0.1.1a3/pypanther/rules/osquery_rules/__init__.py
+-rw-r--r--   0        0        0     4038 2024-05-24 15:16:21.517176 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py
+-rw-r--r--   0        0        0     3398 2024-05-24 12:40:19.326027 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py
+-rw-r--r--   0        0        0     3580 2024-05-24 15:16:21.517419 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py
+-rw-r--r--   0        0        0     2965 2024-05-24 15:16:21.517652 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py
+-rw-r--r--   0        0        0     2596 2024-05-24 15:16:21.517917 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py
+-rw-r--r--   0        0        0     2203 2024-05-24 15:16:21.518208 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py
+-rw-r--r--   0        0        0     4057 2024-05-24 15:16:21.518697 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py
+-rw-r--r--   0        0        0     3670 2024-05-24 15:16:21.519188 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py
+-rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.519514 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ossec.py
+-rw-r--r--   0        0        0     3545 2024-05-24 15:16:21.519928 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated.py
+-rw-r--r--   0        0        0     3674 2024-05-24 15:16:21.520400 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated_macos.py
+-rw-r--r--   0        0        0     3730 2024-05-24 15:16:21.520712 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ssh_listener.py
+-rw-r--r--   0        0        0     5583 2024-05-24 15:16:21.521025 pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_suspicious_cron.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353388 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/__init__.py
+-rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.521335 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_detection_deleted.py
+-rw-r--r--   0        0        0     2520 2024-05-24 15:16:21.521649 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_saml_modified.py
+-rw-r--r--   0        0        0     8355 2024-05-24 15:16:21.521983 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py
+-rw-r--r--   0        0        0     9712 2024-05-24 15:16:21.522331 pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_user_modified.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.354643 pypanther-0.1.1a3/pypanther/rules/salesforce_rules/__init__.py
+-rw-r--r--   0        0        0     4572 2024-05-24 15:16:21.522688 pypanther-0.1.1a3/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353299 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/__init__.py
+-rw-r--r--   0        0        0     7210 2024-05-24 15:16:21.522968 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py
+-rw-r--r--   0        0        0     6468 2024-05-24 15:16:21.523217 pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_threats.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.355907 pypanther-0.1.1a3/pypanther/rules/slack_rules/__init__.py
+-rw-r--r--   0        0        0    10097 2024-05-24 15:16:21.523488 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_access_expanded.py
+-rw-r--r--   0        0        0     8839 2024-05-24 15:16:21.523750 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_added.py
+-rw-r--r--   0        0        0     6576 2024-05-24 15:16:21.524038 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_removed.py
+-rw-r--r--   0        0        0     4668 2024-05-24 15:16:21.524305 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_application_dos.py
+-rw-r--r--   0        0        0     4933 2024-05-24 15:16:21.524549 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_dlp_modified.py
+-rw-r--r--   0        0        0     3472 2024-05-24 15:16:21.524759 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_config_changed.py
+-rw-r--r--   0        0        0     3415 2024-05-24 15:16:21.524967 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py
+-rw-r--r--   0        0        0     3320 2024-05-24 15:16:21.525183 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_unenrolled.py
+-rw-r--r--   0        0        0     5881 2024-05-24 15:16:21.525433 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_idp_configuration_change.py
+-rw-r--r--   0        0        0     4687 2024-05-24 15:16:21.525677 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_information_barrier_modified.py
+-rw-r--r--   0        0        0     3317 2024-05-24 15:16:21.525905 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py
+-rw-r--r--   0        0        0     6985 2024-05-24 15:16:21.526152 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py
+-rw-r--r--   0        0        0     3440 2024-05-24 15:16:21.526377 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_mfa_settings_changed.py
+-rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526613 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_created.py
+-rw-r--r--   0        0        0     2829 2024-05-24 15:16:21.526854 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_deleted.py
+-rw-r--r--   0        0        0     3301 2024-05-24 15:16:21.527063 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_passthrough_anomaly.py
+-rw-r--r--   0        0        0     3398 2024-05-24 15:16:21.527272 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py
+-rw-r--r--   0        0        0     3578 2024-05-24 15:16:21.527470 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_private_channel_made_public.py
+-rw-r--r--   0        0        0     4137 2024-05-24 15:16:21.527694 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py
+-rw-r--r--   0        0        0     3543 2024-05-24 15:16:21.527892 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_service_owner_transferred.py
+-rw-r--r--   0        0        0     3385 2024-05-24 15:16:21.528118 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_sso_settings_changed.py
+-rw-r--r--   0        0        0     7385 2024-05-24 15:16:21.528386 pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_user_privilege_escalation.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356824 pypanther-0.1.1a3/pypanther/rules/snyk_rules/__init__.py
+-rw-r--r--   0        0        0     2612 2024-05-24 15:16:21.528608 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_misc_settings.py
+-rw-r--r--   0        0        0     4557 2024-05-24 15:16:21.528844 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_org_settings.py
+-rw-r--r--   0        0        0     4554 2024-05-24 15:16:21.529080 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_ou_change.py
+-rw-r--r--   0        0        0     4870 2024-05-24 15:16:21.529343 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_project_settings.py
+-rw-r--r--   0        0        0     5423 2024-05-24 15:16:21.529632 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_role_change.py
+-rw-r--r--   0        0        0    12013 2024-05-24 15:16:21.529916 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_svcacct_change.py
+-rw-r--r--   0        0        0     3957 2024-05-24 15:16:21.530136 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_externalaccess.py
+-rw-r--r--   0        0        0     6252 2024-05-24 15:16:21.530401 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_policysetting.py
+-rw-r--r--   0        0        0     2564 2024-05-24 15:16:21.530613 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_sso.py
+-rw-r--r--   0        0        0     5837 2024-05-24 15:16:21.530857 pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_user_mgmt.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352089 pypanther-0.1.1a3/pypanther/rules/standard_rules/__init__.py
+-rw-r--r--   0        0        0    10977 2024-05-24 15:16:21.531147 pypanther-0.1.1a3/pypanther/rules/standard_rules/admin_assigned.py
+-rw-r--r--   0        0        0    16941 2024-05-24 15:16:21.531423 pypanther-0.1.1a3/pypanther/rules/standard_rules/brute_force_by_ip.py
+-rw-r--r--   0        0        0    36744 2024-05-24 15:16:21.531830 pypanther-0.1.1a3/pypanther/rules/standard_rules/impossible_travel_login.py
+-rw-r--r--   0        0        0     9765 2024-05-24 12:40:18.497546 pypanther-0.1.1a3/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py
+-rw-r--r--   0        0        0     8211 2024-05-24 15:16:21.532115 pypanther-0.1.1a3/pypanther/rules/standard_rules/mfa_disabled.py
+-rw-r--r--   0        0        0     9929 2024-05-24 12:40:18.501241 pypanther-0.1.1a3/pypanther/rules/standard_rules/standard_dns_base64.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353861 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/__init__.py
+-rw-r--r--   0        0        0     4635 2024-05-24 15:16:21.532365 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_https_disabled.py
+-rw-r--r--   0        0        0     4871 2024-05-24 15:16:21.532637 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py
+-rw-r--r--   0        0        0     4652 2024-05-24 15:16:21.532895 pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.356684 pypanther-0.1.1a3/pypanther/rules/tines_rules/__init__.py
+-rw-r--r--   0        0        0     2570 2024-05-24 15:16:21.533184 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_actions_disabled_changes.py
+-rw-r--r--   0        0        0     2810 2024-05-24 15:16:21.533820 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_custom_ca.py
+-rw-r--r--   0        0        0     3526 2024-05-24 15:16:21.534457 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py
+-rw-r--r--   0        0        0     2873 2024-05-24 15:16:21.534800 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_global_resource_destruction.py
+-rw-r--r--   0        0        0     2933 2024-05-24 15:16:21.535126 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_sso_settings.py
+-rw-r--r--   0        0        0     2751 2024-05-24 15:16:21.535504 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_items_destruction.py
+-rw-r--r--   0        0        0     2721 2024-05-24 15:16:21.535880 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_jobs_clearance.py
+-rw-r--r--   0        0        0     2666 2024-05-24 15:16:21.536177 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_team_destruction.py
+-rw-r--r--   0        0        0     3973 2024-05-24 15:16:21.536516 pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_tenant_authtoken.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.352185 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/__init__.py
+-rw-r--r--   0        0        0     3761 2024-05-24 15:16:21.536795 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py
+-rw-r--r--   0        0        0     2958 2024-05-24 15:16:21.537085 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_api_token.py
+-rw-r--r--   0        0        0     3194 2024-05-24 15:16:21.537365 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_owner.py
+-rw-r--r--   0        0        0     3703 2024-05-24 15:16:21.537713 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py
+-rw-r--r--   0        0        0     2948 2024-05-24 15:16:21.538004 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_assumption.py
+-rw-r--r--   0        0        0     2760 2024-05-24 15:16:21.538287 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_role.py
+-rw-r--r--   0        0        0     3913 2024-05-24 15:16:21.538522 pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_suspension.py
+-rw-r--r--   0        0        0        0 2024-05-24 12:40:18.353216 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/__init__.py
+-rw-r--r--   0        0        0     2676 2024-05-24 15:16:21.538757 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py
+-rw-r--r--   0        0        0     2345 2024-05-24 15:16:21.538977 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py
+-rw-r--r--   0        0        0     2816 2024-05-24 15:16:21.539207 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py
+-rw-r--r--   0        0        0     2746 2024-05-24 15:16:21.539448 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py
+-rw-r--r--   0        0        0     3344 2024-05-24 15:16:21.539654 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py
+-rw-r--r--   0        0        0     3544 2024-05-24 15:16:21.539868 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py
+-rw-r--r--   0        0        0     2606 2024-05-24 15:16:21.540096 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py
+-rw-r--r--   0        0        0     4606 2024-05-24 15:16:21.540333 pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py
+-rw-r--r--   0        0        0     4490 2024-05-24 13:47:47.095050 pypanther-0.1.1a3/pypanther/upload.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095097 pypanther-0.1.1a3/pypanther/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095354 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 13:47:47.095410 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/__init__.py
+-rw-r--r--   0        0        0    16541 2024-05-24 13:47:47.095519 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/client.py
+-rw-r--r--   0        0        0      624 2024-05-24 13:47:47.095629 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/errors.py
+-rw-r--r--   0        0        0      159 2024-05-24 13:47:47.095796 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload.graphql
+-rw-r--r--   0        0        0      802 2024-05-24 13:47:47.095929 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql
+-rw-r--r--   0        0        0     1439 2024-05-24 17:25:24.652928 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/introspection_query.graphql
+-rw-r--r--   0        0        0    13035 2024-05-24 13:47:47.096074 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/lambda_client.py
+-rw-r--r--   0        0        0    25446 2024-05-24 13:47:47.096146 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py
+-rw-r--r--   0        0        0     1606 2024-05-24 13:47:47.096405 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/cli_output.py
+-rw-r--r--   0        0        0      738 2024-05-24 13:47:47.096498 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/command/standard_args.py
+-rw-r--r--   0        0        0      676 2024-05-24 13:47:47.096574 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/constants.py
+-rw-r--r--   0        0        0     2541 2024-05-24 13:47:47.096824 pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/util.py
+-rw-r--r--   0        0        0      274 2024-05-23 22:00:33.355426 pypanther-0.1.1a3/pypanther/wrap.py
+-rw-r--r--   0        0        0     1720 2024-05-24 17:25:24.653486 pypanther-0.1.1a3/pyproject.toml
+-rw-r--r--   0        0        0     1034 1970-01-01 00:00:00.000000 pypanther-0.1.1a3/PKG-INFO
```

### Comparing `pypanther-0.1.1a2/LICENSE.txt` & `pypanther-0.1.1a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/base.py` & `pypanther-0.1.1a3/pypanther/base.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/asana_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/asana_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/atlassian_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/atlassian_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_alb_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_alb_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_cloudtrail_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_cloudtrail_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_eks_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_eks_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_s3_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_s3_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_vpcdns_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_vpcdns_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/aws_vpcflow_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/aws_vpcflow_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/azure_signin_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/azure_signin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/box_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/box_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/cisco_umbrella_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/cisco_umbrella_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/cloudflare_firewall_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/cloudflare_firewall_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/cloudflare_httpreq_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/cloudflare_httpreq_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/crowdstrike_fdr_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/crowdstrike_fdr_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/gcp_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/gcp_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/github_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/github_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/gsuite_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/gsuite_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/notion_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/notion_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/okta_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/okta_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/onelogin_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/onelogin_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/onepassword_itemusage_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/onepassword_itemusage_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/onepassword_signinattempt_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/onepassword_signinattempt_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/panther_audit_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/panther_audit_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/slack_accesslogs_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/slack_accesslogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/slack_auditlogs_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/slack_auditlogs_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/zendesk_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/zendesk_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/zoom_activity_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/zoom_activity_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/data_models/zoom_operation_data_model.py` & `pypanther-0.1.1a3/pypanther/data_models/zoom_operation_data_model.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/get.py` & `pypanther-0.1.1a3/pypanther/get.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/gcp_base_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/gcp_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/gcp_environment.py` & `pypanther-0.1.1a3/pypanther/helpers/gcp_environment.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_asana_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_asana_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_audit.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_audit.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_auth0_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_auth0_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_azuresignin_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_azuresignin_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_base_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_base_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_box_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_box_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_cloudflare_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_cloudflare_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_config_defaults.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_config_defaults.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_config_overrides.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_config_overrides.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_default.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_default.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_duo_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_duo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_event_type_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_event_type_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_greynoise_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_greynoise_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_iocs.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_iocs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_ipinfo_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_ipinfo_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_lookuptable_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_lookuptable_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_oss_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_oss_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_snyk_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_snyk_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_tines_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_tines_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_tor_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_tor_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/helpers/panther_zoom_helpers.py` & `pypanther-0.1.1a3/pypanther/helpers/panther_zoom_helpers.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/log_types.py` & `pypanther-0.1.1a3/pypanther/log_types.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/main.py` & `pypanther-0.1.1a3/pypanther/main.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/register.py` & `pypanther-0.1.1a3/pypanther/register.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_service_account_created.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_service_account_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_team_privacy_public.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_team_privacy_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_default_session_duration_never.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_email_domain_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_form_link_auth_requirement_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_guest_invite_permissions_anyone.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_new_admin.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_new_admin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_org_export.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_org_export.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_password_requirements_simple.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_require_app_approvals_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/asana_rules/asana_workspace_saml_optional.py` & `pypanther-0.1.1a3/pypanther/rules/asana_rules/asana_workspace_saml_optional.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/atlassian_rules/user_logged_in_as_user.py` & `pypanther-0.1.1a3/pypanther/rules/atlassian_rules/user_logged_in_as_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_custom_role_created.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_custom_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_integration_installed.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_integration_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_factor_setting_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_policy_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_mfa_risk_assessment_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_post_login_action_flow.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_user_invitation_created.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_invitation_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py` & `pypanther-0.1.1a3/pypanther/rules/auth0_rules/auth0_user_joined_tenant.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ami_modified_for_public_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_account_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_password_policy_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_stopped.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_cloudtrail_unsuccessful_mfa_attempt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_codebuild_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_config_service_disabled_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_login_without_saml.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_console_root_login_failed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_ebs_encryption_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_gateway_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_manual_security_group_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_monitoring.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_network_acl_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_route_table_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_security_group_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_startup_script_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_traffic_mirroring.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vpc_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ec2_vulnerable_xz_image_launched.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_crud.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ecr_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_anything_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_assume_role_blocklist_ignored.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_compromised_key_quarantine.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_entity_created_without_cloudformation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_group_read_only_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_iam_user_recon_denied.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_ipset_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_key_compromised.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_kms_cmk_loss.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_lambda_crud.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_macie_evasion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_modify_cloud_compute_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_network_acl_permissive_entry.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_manual_snapshot_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_master_pass_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_publicrestore.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_rds_snapshot_shared.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_resource_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_access_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_root_password_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_s3_bucket_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_saml_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_security_configuration_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_securityhub_finding_evasion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_snapshot_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_software_discovery.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unauthorized_api_call.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_unused_region.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_update_credentials.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_user_login_profile_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py` & `pypanther-0.1.1a3/pypanther/rules/aws_cloudtrail_rules/aws_waf_disassociation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py` & `pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/source_ip_multiple_403.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py` & `pypanther-0.1.1a3/pypanther/rules/aws_eks_rules/system_namespace_public_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py` & `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_high_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py` & `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_low_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py` & `pypanther-0.1.1a3/pypanther/rules/aws_guardduty_rules/aws_guardduty_med_sev_findings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_access_error.py` & `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_error.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py` & `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_access_ip_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py` & `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_insecure_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py` & `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unauthenticated_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py` & `pypanther-0.1.1a3/pypanther/rules/aws_s3_rules/aws_s3_unknown_requester_get_object.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py` & `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_dns_crypto_domain.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py` & `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_healthy_log_status.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py` & `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py` & `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_inbound_traffic_port_blocklist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py` & `pypanther-0.1.1a3/pypanther/rules/aws_vpc_flow_rules/aws_vpc_unapproved_outbound_dns.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_failed_signins.py` & `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_failed_signins.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_legacyauth.py` & `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_legacyauth.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py` & `pypanther-0.1.1a3/pypanther/rules/azure_signin_rules/azure_risklevel_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_access_granted.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_access_granted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_anomalous_download.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_anomalous_download.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_event_triggered_externally.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_event_triggered_externally.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_item_shared_externally.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_item_shared_externally.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_malicious_content.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_malicious_content.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_new_login.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_new_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_policy_violation.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_policy_violation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_suspicious_login_or_session.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_suspicious_login_or_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_untrusted_device.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_untrusted_device.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_user_downloads.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_downloads.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/box_rules/box_user_permission_updates.py` & `pypanther-0.1.1a3/pypanther/rules/box_rules/box_user_permission_updates.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_admin_grant.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_api_key_created_retrieved.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_data_forwarder_stopped.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_flagged.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_flagged.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_audit_user_added_outside_org.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/carbonblack_rules/cb_passthrough.py` & `pypanther-0.1.1a3/pypanther/rules/carbonblack_rules/cb_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py` & `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/domain_blocked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py` & `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/fuzzy_matching_domains.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py` & `pypanther-0.1.1a3/pypanther/rules/cisco_umbrella_dns_rules/suspicious_domains.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py` & `pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_firewall_ddos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py` & `pypanther-0.1.1a3/pypanther/rules/cloudflare_rules/cloudflare_httpreq_bot_high_volume.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_base64_encoded_args.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_connection_to_embargoed_country.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_credential_dumping_tool.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_cryptomining_tools.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_detection_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_dns_request.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_lolbas.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_add_trusted_cert.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_osascript_administrator.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_macos_plutil_usage.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_real_time_response_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_remote_access_tool_execution.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_reverse_shell_tool_executed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_systemlog_tampering.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_unusual_parent_child_processes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py` & `pypanther-0.1.1a3/pypanther/rules/crowdstrike_rules/crowdstrike_wmi_query_detection.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py` & `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_admin_sign_in_as_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_external_share.py` & `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_external_share.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py` & `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_linked_team_application_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py` & `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_ownership_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py` & `pypanther-0.1.1a3/pypanther/rules/dropbox_rules/dropbox_user_disabled_2fa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_app_integration_secret_key_viewed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_bypass_code_viewed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_create_admin.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_create_admin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_lockout.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_lockout.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_marked_push_fraudulent.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_mfa_restrictions_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_new_admin_api_app_integration.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_policy_updated.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_policy_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_sso_saml_requirement_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_admin_user_mfa_bypass_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_action_fraudulent.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_action_fraudulent.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_anomalous_push.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_anomalous_push.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_bypass_code_used.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_bypass_code_used.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py` & `pypanther-0.1.1a3/pypanther/rules/duo_rules/duo_user_endpoint_failure_multi.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_access_attempts_violating_vpc_service_controls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_bigquery_large_scan.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloud_storage_buckets_modified_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudbuild_potential_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_cloudfunctions_functions_update.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_computeinstances_create_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_destructive_queries.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_dns_zone_modified_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_firewall_rule_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_iam_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_gcs_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_corp_email.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_custom_role_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_org_folder_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_roles_update_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_account_key_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_get_access_token_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_service_accounts_sign_blob.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_iam_serviceaccounts_signjwt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_inbound_sso_profile_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_log_bucket_or_sink_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_settings_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_logging_sink_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_permissions_granted_to_create_or_manage_service_account_key.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_privilege_escalation_by_deployments_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_access_denied.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_service_account_or_keys_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_serviceusage_apikeys_create_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_sql_config_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_storage_hmac_keys_create.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_unused_regions.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_user_added_to_iap_protected_service.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_vpc_flow_logs_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workforce_pool_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_audit_rules/gcp_workload_identity_pool_created_or_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_http_lb_rules/gcp_access_attempts_violating_iap_access_controls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_cron_job_created_or_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_exec_into_pod.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_ioc_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_new_daemonset_deployed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_attached_to_node_host_network.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_create_or_modify_host_path_vol_mount.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_pod_using_host_pid_namespace.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_privileged_pod_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py` & `pypanther-0.1.1a3/pypanther/rules/gcp_k8s_rules/gcp_k8s_service_type_node_port_deployed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_action_failed.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_action_failed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_advanced_security_change.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_advanced_security_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_branch_policy_override.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_policy_override.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_branch_protection_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_branch_protection_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_auth_modified.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_auth_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_ip_allowlist.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_ip_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_moderators_add.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_moderators_add.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_org_modified.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_org_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_organization_app_integration_installed.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_organization_app_integration_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_public_repository_created.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_public_repository_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_collaborator_change.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_collaborator_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_created.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_hook_modified.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_hook_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_initial_access.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_initial_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repo_visibility_change.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repo_visibility_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_repository_transfer.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_repository_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_secret_scanning_alert_created.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_secret_scanning_alert_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_team_modified.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_team_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_user_access_key_created.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_access_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/github_rules/github_user_role_updated.py` & `pypanther-0.1.1a3/pypanther/rules/github_rules/github_user_role_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py` & `pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_audit_password_reset_multiple_emails.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py` & `pypanther-0.1.1a3/pypanther/rules/gitlab_rules/gitlab_production_password_reset_multiple_emails.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_auth_errors.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_company_domain_login_without_saml.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_create_user_accounts.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_local_user_login_without_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_lock_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_long_lived_certs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_network_scanning.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_root_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_saml_login_not_company_domain.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py` & `pypanther-0.1.1a3/pypanther/rules/gravitational_teleport_rules/teleport_suspicious_commands.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_admin_custom_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_advanced_protection_program.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_marketplace_new_domain_application.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/google_workspace_apps_new_mobile_app_installed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_advanced_protection.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_calendar_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_doc_ownership_transfer.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_external_forwarding.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_google_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_gov_attack.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_group_banned_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_leaked_password.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_login_type.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_compromise.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_screen_unlock_fail.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_mobile_device_suspicious_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_passthrough_rule.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_suspicious_logins.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_two_step_verification.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_user_suspended.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_calendar_external_sharing.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_data_export_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_default_routing_rule.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_enhanced_predelivery_scanning.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_gmail_security_sandbox_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_enforce_strong_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_password_reuse_enabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_activityevent_rules/gsuite_workspace_trusted_domains_allowlist.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_external_share.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_overly_visible.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py` & `pypanther-0.1.1a3/pypanther/rules/gsuite_reports_rules/gsuite_drive_visibility_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py` & `pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_aws_account_logging.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/indicator_creation_rules/new_user_account_logging.py` & `pypanther-0.1.1a3/pypanther/rules/indicator_creation_rules/new_user_account_logging.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py` & `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_brute_force_login_by_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py` & `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_external_sharing.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft365_mfa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py` & `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_exchange_external_forwarding.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py` & `pypanther-0.1.1a3/pypanther/rules/microsoft_rules/microsoft_graph_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_2fa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_access_allowed_from_anywhere.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_alerting_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_atlas_api_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_external_user_invited_no_config.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_identity_provider_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_logging_toggled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_org_membership_restriction_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_created_or_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py` & `pypanther-0.1.1a3/pypanther/rules/mongodb_rules/mongodb_user_roles_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_admin_logged_out.py` & `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_logged_out.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_admin_user_change.py` & `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_admin_user_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_many_deletes.py` & `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_many_deletes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_personnel_action.py` & `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_personnel_action.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py` & `pypanther-0.1.1a3/pypanther/rules/netskope_rules/netskope_unauthorized_api_calls.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_account_changed_after_login.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_account_changed_after_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_blocked_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_login_from_new_location.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_login_from_new_location.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_many_pages_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_many_pages_exported.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_many_pages_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_accessible_to_api.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_api.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_accessible_to_guests.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_page_shared_to_web.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_page_shared_to_web.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_scim_token_generated.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_scim_token_generated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_sharing_settings_updated.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_sharing_settings_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_teamspace_owner_added.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_teamspace_owner_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_audit_log_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_exported.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_exported.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_enforce_saml_sso_config_updated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py` & `pypanther-0.1.1a3/pypanther/rules/notion_rules/notion_workspace_settings_public_homepage_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_account_support_access.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_account_support_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_disabled_mfa.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_admin_role_assigned.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_admin_role_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_anonymizing_vpn_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_api_key_created.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_api_key_revoked.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_api_key_revoked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_refresh_access_token_reuse.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_app_unauthorized_access_attempt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_group_admin_role_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_idp_create_modify.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_create_modify.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_idp_signin.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_idp_signin.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_new_behavior_accessing_admin_console.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_org2org_creation_modification.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_org2org_creation_modification.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_password_accessed.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_accessed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_password_extraction_via_scim.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_phishing_attempt_blocked_by_fastpass.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_potentially_stolen_session.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_potentially_stolen_session.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_rate_limits.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_rate_limits.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_support_reset.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_support_reset.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_threatinsight_security_threat_detected.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_account_locked.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_account_locked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_factor_suspend.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_reset.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_mfa_reset_all.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py` & `pypanther-0.1.1a3/pypanther/rules/okta_rules/okta_user_reported_suspicious_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_active_login_activity.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_failed_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_high_risk_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_password_accessed.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_accessed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_password_changed.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_password_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_remove_authentication_factor.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_threshold_accounts_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_unauthorized_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_account_locked.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onelogin_rules/onelogin_user_assumed.py` & `pypanther-0.1.1a3/pypanther/rules/onelogin_rules/onelogin_user_assumed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py` & `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_lut_sensitive_item_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py` & `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_sensitive_item_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/onepassword_rules/onepassword_unusual_client.py` & `pypanther-0.1.1a3/pypanther/rules/onepassword_rules/onepassword_unusual_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_aws_commands.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_logins_non_office.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_linux_mac_vulnerable_xz_liblzma.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_application_firewall.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_enable_auto_update.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_osx_attacks_keyboard_events.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_mac_unwanted_chrome_extensions.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_ossec.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ossec.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_outdated.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_outdated_macos.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_outdated_macos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_ssh_listener.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_ssh_listener.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/osquery_rules/osquery_suspicious_cron.py` & `pypanther-0.1.1a3/pypanther/rules/osquery_rules/osquery_suspicious_cron.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_detection_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_detection_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_saml_modified.py` & `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_saml_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py` & `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_sensitive_role_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/panther_audit_rules/panther_user_modified.py` & `pypanther-0.1.1a3/pypanther/rules/panther_audit_rules/panther_user_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py` & `pypanther-0.1.1a3/pypanther/rules/salesforce_rules/salesforce_admin_login_as_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py` & `pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_alert_passthrough.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/sentinelone_rules/sentinelone_threats.py` & `pypanther-0.1.1a3/pypanther/rules/sentinelone_rules/sentinelone_threats.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_access_expanded.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_access_expanded.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_added.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_added.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_app_removed.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_app_removed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_application_dos.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_application_dos.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_dlp_modified.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_dlp_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_config_changed.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_config_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_slackbot_unenrolled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_ekm_unenrolled.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_ekm_unenrolled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_idp_configuration_change.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_idp_configuration_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_information_barrier_modified.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_information_barrier_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_intune_mdm_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_legal_hold_policy_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_mfa_settings_changed.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_mfa_settings_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_org_created.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_created.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_org_deleted.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_org_deleted.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_passthrough_anomaly.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_passthrough_anomaly.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_potentially_malicious_file_shared.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_private_channel_made_public.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_private_channel_made_public.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_privilege_changed_to_user.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_service_owner_transferred.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_service_owner_transferred.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_sso_settings_changed.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_sso_settings_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/slack_rules/slack_user_privilege_escalation.py` & `pypanther-0.1.1a3/pypanther/rules/slack_rules/slack_user_privilege_escalation.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_misc_settings.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_misc_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_org_settings.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_org_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_ou_change.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_ou_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_project_settings.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_project_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_role_change.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_role_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_svcacct_change.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_svcacct_change.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_externalaccess.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_externalaccess.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_policysetting.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_policysetting.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_system_sso.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_system_sso.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/snyk_rules/snyk_user_mgmt.py` & `pypanther-0.1.1a3/pypanther/rules/snyk_rules/snyk_user_mgmt.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/admin_assigned.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/admin_assigned.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/brute_force_by_ip.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/brute_force_by_ip.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/impossible_travel_login.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/impossible_travel_login.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/malicious_sso_dns_lookup.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/mfa_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/mfa_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/standard_rules/standard_dns_base64.py` & `pypanther-0.1.1a3/pypanther/rules/standard_rules/standard_dns_base64.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_https_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_https_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_machine_approval_requirements_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/tailscale_rules/tailscale_magicdns_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_actions_disabled_changes.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_actions_disabled_changes.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_custom_ca.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_custom_ca.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_enqueued_retrying_job_deletion.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_global_resource_destruction.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_global_resource_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_sso_settings.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_sso_settings.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_story_items_destruction.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_items_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_story_jobs_clearance.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_story_jobs_clearance.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_team_destruction.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_team_destruction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/tines_rules/tines_tenant_authtoken.py` & `pypanther-0.1.1a3/pypanther/rules/tines_rules/tines_tenant_authtoken.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_mobile_app_access.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_new_api_token.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_api_token.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_new_owner.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_new_owner.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_sensitive_data_redaction.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_assumption.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_assumption.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_role.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zendesk_rules/zendesk_user_suspension.py` & `pypanther-0.1.1a3/pypanther/rules/zendesk_rules/zendesk_user_suspension.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_all_meetings_secured_with_one_option_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_automatic_sign_out_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_new_meeting_passcode_required_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_operation_passcode_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_method_modified.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_sign_in_requirements_changed.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_two_factor_authentication_disabled.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py` & `pypanther-0.1.1a3/pypanther/rules/zoom_operation_rules/zoom_user_promoted_to_privileged_role.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/upload.py` & `pypanther-0.1.1a3/pypanther/upload.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/client.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/errors.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/errors.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/graphql/async_bulk_upload_status.graphql`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/lambda_client.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/lambda_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/backend/public_api_client.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/cli_output.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/cli_output.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/command/standard_args.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/command/standard_args.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/constants.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/constants.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pypanther/vendor/panther_analysis_tool/util.py` & `pypanther-0.1.1a3/pypanther/vendor/panther_analysis_tool/util.py`

 * *Files identical despite different names*

### Comparing `pypanther-0.1.1a2/pyproject.toml` & `pypanther-0.1.1a3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypanther"
-version = "0.1.1a2"
+version = "0.1.1a3"
 description = ""
 authors = ["Panther Labs Inc <pypi@runpanther.io>"]
 readme = "README.md"
 keywords = ["Security", "CLI"]
 classifiers = [
     "Operating System :: OS Independent",
 ]
```

### Comparing `pypanther-0.1.1a2/PKG-INFO` & `pypanther-0.1.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypanther
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: 
 License: AGPL-3.0-only
 Keywords: Security,CLI
 Author: Panther Labs Inc
 Author-email: pypi@runpanther.io
 Requires-Python: ==3.11.*
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

