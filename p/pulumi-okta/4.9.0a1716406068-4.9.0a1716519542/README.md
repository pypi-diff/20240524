# Comparing `tmp/pulumi_okta-4.9.0a1716406068.tar.gz` & `tmp/pulumi_okta-4.9.0a1716519542.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.9.0a1716406068.tar", last modified: Wed May 22 19:32:15 2024, max compression
+gzip compressed data, was "pulumi_okta-4.9.0a1716519542.tar", last modified: Fri May 24 03:03:23 2024, max compression
```

## Comparing `pulumi_okta-4.9.0a1716406068.tar` & `pulumi_okta-4.9.0a1716519542.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.820307 pulumi_okta-4.9.0a1716406068/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70310 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.828307 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/access_policy_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    63791 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    40308 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    32373 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)   146700 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/oauth_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   137735 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    72763 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    59398 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    66043 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    91374 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    23559 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    51344 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.828307 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    47855 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)    47497 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    20026 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    47422 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24328 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)    31125 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/customized_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_default_signin_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_log_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_org_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.832307 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (127)    87393 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)    83406 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    72932 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.836307 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/link_value.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/log_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.836307 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    36750 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    80451 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14142 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_android.py
--rw-r--r--   0 runner    (1001) docker     (127)    48216 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_chromeos.py
--rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_macos.py
--rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    69208 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    13242 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    79597 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (127)    49623 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (127)    69718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (127)    65321 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    71399 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    34771 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_rule_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/preview_signin_page.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    97718 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:32:15.840307 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 19:32:15.000000 pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 19:32:09.000000 pulumi_okta-4.9.0a1716406068/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 19:32:15.844307 pulumi_okta-4.9.0a1716406068/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.167278 pulumi_okta-4.9.0a1716519542/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-24 03:03:23.167278 pulumi_okta-4.9.0a1716519542/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.147278 pulumi_okta-4.9.0a1716519542/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (127)    21451 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70310 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21362 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11759 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15332 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.151278 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15781 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9829 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/access_policy_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63791 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36995 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40308 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18000 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32373 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14663 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146700 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10037 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9431 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16081 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/oauth_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15419 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137735 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72763 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59398 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67402 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18032 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10001 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66043 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91374 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23559 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51344 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.155278 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7689 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23481 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24634 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17596 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47855 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47497 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20026 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23943 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47422 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24328 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31125 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12900 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.155278 pulumi_okta-4.9.0a1716519542/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/customized_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17334 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39467 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15162 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18426 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.155278 pulumi_okta-4.9.0a1716519542/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3266 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7227 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9207 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_default_signin_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_log_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7087 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5349 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_org_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3783 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.155278 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3811 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7209 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15123 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24099 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20849 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13713 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47772 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.159278 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9046 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17915 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87393 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83406 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15030 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72932 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.159278 pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18791 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/link_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/log_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.159278 pulumi_okta-4.9.0a1716519542/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26287 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36750 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8652 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80451 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.163278 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14274 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22720 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_android.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48216 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_chromeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17935 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56471 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_macos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71871 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69208 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13374 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79597 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49623 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32999 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30687 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69718 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13701 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65321 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71399 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11656 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34771 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_rule_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18616 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/preview_signin_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.163278 pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23800 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23808 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13898 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21186 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42952 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.163278 pulumi_okta-4.9.0a1716519542/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12562 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.167278 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25124 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3535 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21707 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97718 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9967 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13653 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8844 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52236 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 03:03:23.167278 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-24 03:03:23.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6015 2024-05-24 03:03:23.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 03:03:23.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-24 03:03:23.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-24 03:03:23.000000 pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 03:03:17.000000 pulumi_okta-4.9.0a1716519542/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 03:03:23.167278 pulumi_okta-4.9.0a1716519542/setup.cfg
```

### Comparing `pulumi_okta-4.9.0a1716406068/PKG-INFO` & `pulumi_okta-4.9.0a1716519542/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1716406068
+Version: 4.9.0a1716519542
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1716406068/README.md` & `pulumi_okta-4.9.0a1716519542/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/__init__.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/_utilities.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/__init__.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/access_policy_assignment.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/access_policy_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_app.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_app.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_oauth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/oauth_role_assignment.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/oauth_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/swa.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/three_field.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app/user.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/get_server_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/auth_server_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/authenticator.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/behaviour.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/brand.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/config/__init__.pyi` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/config/vars.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/customized_signin_page.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/customized_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/domain_verification.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_customization.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_domain_verification.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/email_sender.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/email_sender_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/factor/factor.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/factor_totp.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_app_user_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_auth_server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_auth_server_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_behaviours.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brand.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_brand.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_brands.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_brands.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_default_signin_page.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_default_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_domain.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_email_customization.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_email_customizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_groups.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_log_stream.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_network_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_org_metadata.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_org_metadata.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_template.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_templates.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_theme.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_themes.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_themes.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_trusted_origins.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/get_user_security_questions.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_everyone_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_group.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/get_rule.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/get_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/group.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/role.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group/rule.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group_memberships.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_metadata_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/get_social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/idp/social.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/hook.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/link_definition.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/link_value.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/log_stream.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/log_stream.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/network/zone.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/org_configuration.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/org_support.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -377,37 +377,37 @@
 
 @pulumi.input_type
 class RuleSignonFactorSequenceSecondaryCriteriaArgs:
     def __init__(__self__, *,
                  factor_type: pulumi.Input[str],
                  provider: pulumi.Input[str]):
         """
-        :param pulumi.Input[str] factor_type: Type of a Factor
-        :param pulumi.Input[str] provider: Factor provider
+        :param pulumi.Input[str] factor_type: Factor type of the additional authentication step.
+        :param pulumi.Input[str] provider: Provider of the additional authentication step.
         """
         pulumi.set(__self__, "factor_type", factor_type)
         pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="factorType")
     def factor_type(self) -> pulumi.Input[str]:
         """
-        Type of a Factor
+        Factor type of the additional authentication step.
         """
         return pulumi.get(self, "factor_type")
 
     @factor_type.setter
     def factor_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "factor_type", value)
 
     @property
     @pulumi.getter
     def provider(self) -> pulumi.Input[str]:
         """
-        Factor provider
+        Provider of the additional authentication step.
         """
         return pulumi.get(self, "provider")
 
     @provider.setter
     def provider(self, value: pulumi.Input[str]):
         pulumi.set(self, "provider", value)
```

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_android.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_android.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_chromeos.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_chromeos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_ios.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_ios.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_macos.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_macos.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/device_assurance_windows.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/device_assurance_windows.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/get_default_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -372,30 +372,30 @@
         RuleSignonFactorSequenceSecondaryCriteria.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  factor_type: str,
                  provider: str):
         """
-        :param str factor_type: Type of a Factor
-        :param str provider: Factor provider
+        :param str factor_type: Factor type of the additional authentication step.
+        :param str provider: Provider of the additional authentication step.
         """
         pulumi.set(__self__, "factor_type", factor_type)
         pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="factorType")
     def factor_type(self) -> str:
         """
-        Type of a Factor
+        Factor type of the additional authentication step.
         """
         return pulumi.get(self, "factor_type")
 
     @property
     @pulumi.getter
     def provider(self) -> str:
         """
-        Factor provider
+        Provider of the additional authentication step.
         """
         return pulumi.get(self, "provider")
```

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/password.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy/signon.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/preview_signin_page.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/preview_signin_page.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/provider.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/resource_set.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/role_subscription.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/template_sms.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/theme.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/get_users.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/outputs.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user/user_type.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.9.0a1716519542/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.9.0a1716406068
+Version: 4.9.0a1716519542
 Summary: A Pulumi package for creating and managing okta resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi,okta
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_okta-4.9.0a1716406068/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.9.0a1716519542/pulumi_okta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.9.0a1716406068/pyproject.toml` & `pulumi_okta-4.9.0a1716519542/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_okta"
   description = "A Pulumi package for creating and managing okta resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "okta"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.9.0a1716406068"
+  version = "4.9.0a1716519542"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-okta"
 
 [build-system]
```

