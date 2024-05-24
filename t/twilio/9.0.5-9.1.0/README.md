# Comparing `tmp/twilio-9.0.5.tar.gz` & `tmp/twilio-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twilio-9.0.5.tar", last modified: Thu Apr 18 11:21:26 2024, max compression
+gzip compressed data, was "twilio-9.1.0.tar", last modified: Fri May 24 11:14:48 2024, max compression
```

## Comparing `twilio-9.0.5.tar` & `twilio-9.1.0.tar`

### file list

```diff
@@ -1,851 +1,857 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-18 11:21:21.000000 twilio-9.0.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-18 11:21:21.000000 twilio-9.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-18 11:21:21.000000 twilio-9.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-04-18 11:21:26.556312 twilio-9.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-18 11:21:21.000000 twilio-9.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-18 11:21:26.556312 twilio-9.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-18 11:21:21.000000 twilio-9.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.448312 twilio-9.0.5/twilio/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/client_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/instance_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/instance_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/list_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/obsolete.py
--rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/values.py
--rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/http/
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/async_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/http/validation_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/jwt/
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/jwt/access_token/
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/access_token/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/access_token/grants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/jwt/client/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/jwt/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/taskrouter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/taskrouter/capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/jwt/validation/
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/jwt/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/request_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/rest/
--rw-r--r--   0 runner    (1001) docker     (127)    21083 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/rest/accounts/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/AccountsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.452313 twilio-9.0.5/twilio/rest/accounts/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/auth_token_promotion.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.456313 twilio-9.0.5/twilio/rest/accounts/v1/credential/
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/credential/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/credential/public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/safelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/accounts/v1/secondary_auth_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.456313 twilio-9.0.5/twilio/rest/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/ApiBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.456313 twilio-9.0.5/twilio/rest/api/v2010/
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.456313 twilio-9.0.5/twilio/rest/api/v2010/account/
--rw-r--r--   0 runner    (1001) docker     (127)    36211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.456313 twilio-9.0.5/twilio/rest/api/v2010/account/address/
--rw-r--r--   0 runner    (1001) docker     (127)    36104 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/address/dependent_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    48103 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/application.py
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/authorized_connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.460312 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/
--rw-r--r--   0 runner    (1001) docker     (127)    21428 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46942 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    46913 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    46563 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)    46633 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/national.py
--rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
--rw-r--r--   0 runner    (1001) docker     (127)    46633 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (127)    46493 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/balance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.460312 twilio-9.0.5/twilio/rest/api/v2010/account/call/
--rw-r--r--   0 runner    (1001) docker     (127)    91321 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    28364 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    23634 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)    38500 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)    77230 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/siprec.py
--rw-r--r--   0 runner    (1001) docker     (127)    77253 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/user_defined_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.460312 twilio-9.0.5/twilio/rest/api/v2010/account/conference/
--rw-r--r--   0 runner    (1001) docker     (127)    47201 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    77270 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/conference/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    32732 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/conference/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)    26542 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/connect_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/
--rw-r--r--   0 runner    (1001) docker     (127)    73716 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
--rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    37146 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/local.py
--rw-r--r--   0 runner    (1001) docker     (127)    37230 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)    37316 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
--rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/message/
--rw-r--r--   0 runner    (1001) docker     (127)    56916 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/message/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)    27544 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/message/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/new_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/new_signing_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    27506 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/outgoing_caller_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/queue/
--rw-r--r--   0 runner    (1001) docker     (127)    22431 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/queue/member.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/recording/
--rw-r--r--   0 runner    (1001) docker     (127)    37888 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/recording/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/recording/add_on_result/
--rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)    19011 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/recording/transcription.py
--rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/short_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/signing_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/credential_list/
--rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/credential_list/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/
--rw-r--r--   0 runner    (1001) docker     (127)    45630 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.464312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    20984 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/api/v2010/account/sip/ip_access_control_list/
--rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26241 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/transcription.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/api/v2010/account/usage/
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/
--rw-r--r--   0 runner    (1001) docker     (127)    41987 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38631 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/all_time.py
--rw-r--r--   0 runner    (1001) docker     (127)    38539 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/daily.py
--rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/last_month.py
--rw-r--r--   0 runner    (1001) docker     (127)    38631 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/monthly.py
--rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/this_month.py
--rw-r--r--   0 runner    (1001) docker     (127)    38539 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/today.py
--rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/yearly.py
--rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/yesterday.py
--rw-r--r--   0 runner    (1001) docker     (127)    49482 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/usage/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/api/v2010/account/validation_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/autopilot/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/autopilot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/bulkexports/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/BulkexportsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/bulkexports/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/bulkexports/v1/export/
--rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/export/day.py
--rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/export/export_custom_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/export/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/bulkexports/v1/export_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.468312 twilio-9.0.5/twilio/rest/chat/
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/ChatBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    93405 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (127)    28972 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22315 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    26361 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27618 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v2/service/
--rw-r--r--   0 runner    (1001) docker     (127)    67569 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (127)    39130 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22295 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    41118 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    37552 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    33775 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)    29042 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    27055 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.472312 twilio-9.0.5/twilio/rest/chat/v3/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/chat/v3/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/content/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/ContentBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/content/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/content/v1/content/
--rw-r--r--   0 runner    (1001) docker     (127)    33351 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/content/approval_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/content/approval_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/content_and_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/content/v1/legacy_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/ConversationsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37916 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/address_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/v1/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/v1/conversation/
--rw-r--r--   0 runner    (1001) docker     (127)    49916 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/v1/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (127)    36008 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)    40123 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    27241 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    20948 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.476312 twilio-9.0.5/twilio/rest/conversations/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22292 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25073 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/
--rw-r--r--   0 runner    (1001) docker     (127)    51767 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/message/
--rw-r--r--   0 runner    (1001) docker     (127)    37665 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)    42100 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)    28931 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/participant_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/conversations/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)    29689 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26515 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/service/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/conversations/v1/user/
--rw-r--r--   0 runner    (1001) docker     (127)    28023 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/conversations/v1/user/user_conversation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/events/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/EventsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/events/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/event_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/events/v1/schema/
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/schema/schema_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/events/v1/sink/
--rw-r--r--   0 runner    (1001) docker     (127)    22935 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/sink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/sink/sink_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/sink/sink_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.480312 twilio-9.0.5/twilio/rest/events/v1/subscription/
--rw-r--r--   0 runner    (1001) docker     (127)    22612 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/subscription/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20285 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/events/v1/subscription/subscribed_event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.484312 twilio-9.0.5/twilio/rest/flex_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/FlexApiBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/assessments.py
--rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16094 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    47494 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/flex_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_assessments_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_conversations.py
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires.py
--rw-r--r--   0 runner    (1001) docker     (127)    21096 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    26893 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires_question.py
--rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_segments.py
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_settings_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/insights_user_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/
--rw-r--r--   0 runner    (1001) docker     (127)     9253 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/
--rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    20538 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v1/plugin/
--rw-r--r--   0 runner    (1001) docker     (127)    23281 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21468 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin/plugin_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration/
--rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration/configured_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/plugin_version_archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/provisioning_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v1/web_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/flex_api/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v2/flex_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/flex_api/v2/web_channels.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/frontline_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/frontline_api/FrontlineApiBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/frontline_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/frontline_api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/frontline_api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/frontline_api/v1/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/insights/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/InsightsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.488312 twilio-9.0.5/twilio/rest/insights/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/insights/v1/call/
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call/annotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call/call_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    49306 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/call_summaries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/insights/v1/conference/
--rw-r--r--   0 runner    (1001) docker     (127)    31379 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/conference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25261 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/conference/conference_participant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/insights/v1/room/
--rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/room/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/room/participant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/insights/v1/setting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/intelligence/
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/IntelligenceBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/intelligence/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33894 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/intelligence/v2/transcript/
--rw-r--r--   0 runner    (1001) docker     (127)    29041 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/transcript/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/transcript/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/transcript/operator_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/intelligence/v2/transcript/sentence.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/ip_messaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/IpMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/ip_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.492312 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    63691 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/
--rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11550 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v1/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/
--rw-r--r--   0 runner    (1001) docker     (127)    46389 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/binding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/
--rw-r--r--   0 runner    (1001) docker     (127)    30575 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/invite.py
--rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    28805 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/user_binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/user_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/lookups/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/LookupsBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.496312 twilio-9.0.5/twilio/rest/lookups/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/v1/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.500312 twilio-9.0.5/twilio/rest/lookups/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25093 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/lookups/v2/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.500312 twilio-9.0.5/twilio/rest/media/
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/media/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.500312 twilio-9.0.5/twilio/rest/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/MessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.500312 twilio-9.0.5/twilio/rest/messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.500312 twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/
--rw-r--r--   0 runner    (1001) docker     (127)    24690 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
--rw-r--r--   0 runner    (1001) docker     (127)    19921 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/deactivations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/domain_certs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/domain_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/domain_config_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/external_campaign.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/linkshortening_messaging_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/messaging/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    57063 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18351 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/alpha_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/channel_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)    18138 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/short_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/us_app_to_person.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
--rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/tollfree_verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/messaging/v1/usecase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/microvisor/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/MicrovisorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/microvisor/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/account_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/account_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/microvisor/v1/app/
--rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/app/app_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/microvisor/v1/device/
--rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/device/device_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19033 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/microvisor/v1/device/device_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/monitor/MonitorBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/monitor/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/monitor/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22724 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/monitor/v1/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/monitor/v1/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/notify/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/NotifyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/notify/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28093 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/v1/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.504312 twilio-9.0.5/twilio/rest/notify/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    47437 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30277 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/v1/service/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)    25487 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/notify/v1/service/notification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.508312 twilio-9.0.5/twilio/rest/numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/NumbersBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.508312 twilio-9.0.5/twilio/rest/numbers/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/bulk_eligibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/eligibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/porting_bulk_portability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/porting_port_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/porting_port_in_fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/porting_port_in_phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v1/porting_portability.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.508312 twilio-9.0.5/twilio/rest/numbers/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.508312 twilio-9.0.5/twilio/rest/numbers/v2/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (127)    25375 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/bulk_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    35453 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.508312 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)    47565 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/oauth/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/oauth/OauthBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/oauth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/oauth/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/oauth/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/oauth/v1/authorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/oauth/v1/token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/PreviewBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/deployed_devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/
--rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    26786 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    22729 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/hosted_numbers/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/hosted_numbers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/hosted_numbers/authorization_document/
--rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    48458 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/hosted_numbers/hosted_number_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/marketplace/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/marketplace/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.512312 twilio-9.0.5/twilio/rest/preview/marketplace/available_add_on/
--rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/marketplace/available_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16164 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/marketplace/installed_add_on/
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/marketplace/installed_add_on/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/sync/service/
--rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/sync/service/document/
--rw-r--r--   0 runner    (1001) docker     (127)    20550 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    21583 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24068 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/wireless/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/wireless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/wireless/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/wireless/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview/wireless/sim/
--rw-r--r--   0 runner    (1001) docker     (127)    28868 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/wireless/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview/wireless/sim/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview_messaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview_messaging/PreviewMessagingBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview_messaging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.516312 twilio-9.0.5/twilio/rest/preview_messaging/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview_messaging/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview_messaging/v1/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)    13154 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/preview_messaging/v1/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/PricingBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v1/messaging/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/messaging/country.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v1/phone_number/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/phone_number/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/phone_number/country.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v1/voice/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v1/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14471 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/pricing/v2/voice/
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/voice/country.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/pricing/v2/voice/number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/ProxyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/proxy/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/proxy/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    38168 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23884 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/phone_number.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.520312 twilio-9.0.5/twilio/rest/proxy/v1/service/session/
--rw-r--r--   0 runner    (1001) docker     (127)    27772 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21124 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/session/interaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/proxy/v1/service/session/participant/
--rw-r--r--   0 runner    (1001) docker     (127)    22768 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/session/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/proxy/v1/service/short_code.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/routes/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/RoutesBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/routes/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/v2/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/v2/sip_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/routes/v2/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/ServerlessBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/asset/
--rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/asset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/asset/asset_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/build/
--rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/build/build_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/environment/
--rw-r--r--   0 runner    (1001) docker     (127)    21012 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/environment/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    20929 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/environment/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    22601 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/environment/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/function/
--rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/function/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.524312 twilio-9.0.5/twilio/rest/serverless/v1/service/function/function_version/
--rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/function/function_version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/StudioBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/flow/
--rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/
--rw-r--r--   0 runner    (1001) docker     (127)    21371 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/engagement_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/step/
--rw-r--r--   0 runner    (1001) docker     (127)    17220 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/step/step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v2/flow/
--rw-r--r--   0 runner    (1001) docker     (127)    23685 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/
--rw-r--r--   0 runner    (1001) docker     (127)    27159 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_step/
--rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/flow_revision.py
--rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow/flow_test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/studio/v2/flow_validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.528312 twilio-9.0.5/twilio/rest/supersim/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/SupersimBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/supersim/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/esim_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    35353 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/fleet.py
--rw-r--r--   0 runner    (1001) docker     (127)    26669 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/ip_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    17594 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/supersim/v1/network_access_profile/
--rw-r--r--   0 runner    (1001) docker     (127)    20074 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/network_access_profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/settings_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/supersim/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (127)    28737 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/sim/billing_period.py
--rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/sim/sim_ip_address.py
--rw-r--r--   0 runner    (1001) docker     (127)    23006 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/sms_command.py
--rw-r--r--   0 runner    (1001) docker     (127)    26843 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/supersim/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/sync/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/SyncBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/sync/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/sync/v1/service/
--rw-r--r--   0 runner    (1001) docker     (127)    37557 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/sync/v1/service/document/
--rw-r--r--   0 runner    (1001) docker     (127)    25376 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/document/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/document/document_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.532312 twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/
--rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36676 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    22012 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/
--rw-r--r--   0 runner    (1001) docker     (127)    24889 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37235 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
--rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/sync/v1/service/sync_stream/
--rw-r--r--   0 runner    (1001) docker     (127)    22902 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/sync/v1/service/sync_stream/stream_message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/taskrouter/
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/TaskrouterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/taskrouter/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)    44586 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26058 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)    32777 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.536312 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task/
--rw-r--r--   0 runner    (1001) docker     (127)    54579 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    81514 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task/reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23752 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/
--rw-r--r--   0 runner    (1001) docker     (127)    39929 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_bulk_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/
--rw-r--r--   0 runner    (1001) docker     (127)    44060 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    79296 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
--rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13252 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/
--rw-r--r--   0 runner    (1001) docker     (127)    34582 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/trunking/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/TrunkingBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/trunking/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/trunking/v1/trunk/
--rw-r--r--   0 runner    (1001) docker     (127)    40226 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/credential_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    18723 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
--rw-r--r--   0 runner    (1001) docker     (127)    27869 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/origination_url.py
--rw-r--r--   0 runner    (1001) docker     (127)    22464 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/phone_number.py
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trunking/v1/trunk/recording.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.540312 twilio-9.0.5/twilio/rest/trusthub/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/TrusthubBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.544312 twilio-9.0.5/twilio/rest/trusthub/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/compliance_inquiries.py
--rw-r--r--   0 runner    (1001) docker     (127)    27642 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/compliance_registration_inquiries.py
--rw-r--r--   0 runner    (1001) docker     (127)    13514 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/compliance_tollfree_inquiries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.544312 twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/
--rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21885 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
--rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/end_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/end_user_type.py
--rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/supporting_document.py
--rw-r--r--   0 runner    (1001) docker     (127)    14741 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/supporting_document_type.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.544312 twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/
--rw-r--r--   0 runner    (1001) docker     (127)    30129 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    21456 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.544312 twilio-9.0.5/twilio/rest/verify/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/VerifyBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/verify/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/form.py
--rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/safelist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/verify/v2/service/
--rw-r--r--   0 runner    (1001) docker     (127)    62442 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/access_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/verify/v2/service/entity/
--rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/entity/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/verify/v2/service/entity/challenge/
--rw-r--r--   0 runner    (1001) docker     (127)    34465 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/entity/challenge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/entity/challenge/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)    29596 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/entity/factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/entity/new_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/messaging_configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/verify/v2/service/rate_limit/
--rw-r--r--   0 runner    (1001) docker     (127)    21510 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/rate_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/rate_limit/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    22420 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/verification.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/verification_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/service/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/verification_attempt.py
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/verify/v2/verification_attempts_summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.548312 twilio-9.0.5/twilio/rest/video/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/VideoBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/video/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/composition.py
--rw-r--r--   0 runner    (1001) docker     (127)    55002 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/composition_hook.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/composition_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    27316 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/recording_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/video/v1/room/
--rw-r--r--   0 runner    (1001) docker     (127)    38354 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/video/v1/room/participant/
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/participant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/participant/anonymize.py
--rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/participant/published_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/participant/subscribe_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/participant/subscribed_track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/recording_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    24749 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/video/v1/room/room_recording.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/voice/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/VoiceBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/voice/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/archived_call.py
--rw-r--r--   0 runner    (1001) docker     (127)    37489 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/byoc_trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/voice/v1/connection_policy/
--rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/connection_policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29300 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.552312 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/country/
--rw-r--r--   0 runner    (1001) docker     (127)    27348 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/ip_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/voice/v1/source_ip_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio/rest/wireless/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/WirelessBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio/rest/wireless/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27547 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    29959 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/rate_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio/rest/wireless/v1/sim/
--rw-r--r--   0 runner    (1001) docker     (127)    46224 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/sim/data_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/sim/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/rest/wireless/v1/usage_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio/twiml/
--rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/twiml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/twiml/fax_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/twiml/messaging_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    83800 2024-04-18 11:21:21.000000 twilio-9.0.5/twilio/twiml/voice_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 11:21:26.556312 twilio-9.0.5/twilio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-04-18 11:21:26.000000 twilio-9.0.5/twilio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30341 2024-04-18 11:21:26.000000 twilio-9.0.5/twilio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 11:21:26.000000 twilio-9.0.5/twilio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-18 11:21:26.000000 twilio-9.0.5/twilio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-18 11:21:26.000000 twilio-9.0.5/twilio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.991420 twilio-9.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-24 11:14:44.000000 twilio-9.1.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 11:14:44.000000 twilio-9.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-24 11:14:44.000000 twilio-9.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-24 11:14:48.991420 twilio-9.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-05-24 11:14:44.000000 twilio-9.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-24 11:14:48.991420 twilio-9.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-24 11:14:44.000000 twilio-9.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.863418 twilio-9.1.0/twilio/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.867418 twilio-9.1.0/twilio/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8153 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/client_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/instance_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/instance_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/obsolete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5181 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14614 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.867418 twilio-9.1.0/twilio/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/async_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2655 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/http/validation_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.867418 twilio-9.1.0/twilio/jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.867418 twilio-9.1.0/twilio/jwt/access_token/
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/access_token/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4902 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/access_token/grants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/jwt/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/jwt/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/taskrouter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/taskrouter/capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/jwt/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/jwt/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/request_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)    20541 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/AccountsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/accounts/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/auth_token_promotion.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/accounts/v1/credential/
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/credential/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20010 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/credential/public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/safelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6551 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/accounts/v1/secondary_auth_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/ApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8255 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.871418 twilio-9.1.0/twilio/rest/api/v2010/
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.875418 twilio-9.1.0/twilio/rest/api/v2010/account/
+-rw-r--r--   0 runner    (1001) docker     (127)    36211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.875418 twilio-9.1.0/twilio/rest/api/v2010/account/address/
+-rw-r--r--   0 runner    (1001) docker     (127)    36104 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17046 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48103 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.879418 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/
+-rw-r--r--   0 runner    (1001) docker     (127)    21428 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46942 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46913 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46563 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46633 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46703 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46633 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46493 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/balance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.879418 twilio-9.1.0/twilio/rest/api/v2010/account/call/
+-rw-r--r--   0 runner    (1001) docker     (127)    91321 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10658 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28364 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23634 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38500 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77230 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/siprec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77253 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10900 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/conference/
+-rw-r--r--   0 runner    (1001) docker     (127)    47201 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77270 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/conference/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32732 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/conference/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26542 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/connect_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/
+-rw-r--r--   0 runner    (1001) docker     (127)    73716 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)    20753 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37146 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37230 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37316 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17990 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/message/
+-rw-r--r--   0 runner    (1001) docker     (127)    56930 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/message/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27544 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/message/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/new_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/new_signing_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27506 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22200 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)    22431 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19132 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/queue/member.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/recording/
+-rw-r--r--   0 runner    (1001) docker     (127)    37888 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/recording/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/recording/add_on_result/
+-rw-r--r--   0 runner    (1001) docker     (127)    19242 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19011 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/recording/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17377 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/signing_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/
+-rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.883418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/credential_list/
+-rw-r--r--   0 runner    (1001) docker     (127)    21281 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22760 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)    45630 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20443 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20984 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21051 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20167 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/
+-rw-r--r--   0 runner    (1001) docker     (127)    21811 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26241 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18037 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/transcription.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.887418 twilio-9.1.0/twilio/rest/api/v2010/account/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/
+-rw-r--r--   0 runner    (1001) docker     (127)    41987 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38631 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38539 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/daily.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38631 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38539 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/today.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38585 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38723 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49482 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/usage/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/api/v2010/account/validation_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/autopilot/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/autopilot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/bulkexports/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/BulkexportsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/bulkexports/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/bulkexports/v1/export/
+-rw-r--r--   0 runner    (1001) docker     (127)     7083 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14522 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/export/day.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17007 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8224 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/export/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10880 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/bulkexports/v1/export_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/chat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/ChatBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/chat/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27988 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.891418 twilio-9.1.0/twilio/rest/chat/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    93405 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.895418 twilio-9.1.0/twilio/rest/chat/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)    28972 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22315 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27714 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26361 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.895418 twilio-9.1.0/twilio/rest/chat/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12927 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.895418 twilio-9.1.0/twilio/rest/chat/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27618 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.895418 twilio-9.1.0/twilio/rest/chat/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    67569 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22121 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.895418 twilio-9.1.0/twilio/rest/chat/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)    39130 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22295 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41118 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37552 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33775 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22237 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/chat/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    29042 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21912 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27055 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/chat/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/chat/v3/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/content/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/ContentBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/content/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/content/v1/content/
+-rw-r--r--   0 runner    (1001) docker     (127)    33351 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4372 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/content/approval_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/content/approval_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11924 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/content_and_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12123 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v1/legacy_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/content/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11590 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v2/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11920 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/content/v2/content_and_approvals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/conversations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/ConversationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.899418 twilio-9.1.0/twilio/rest/conversations/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37916 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/address_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    12567 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11085 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/conversation/
+-rw-r--r--   0 runner    (1001) docker     (127)    49916 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (127)    36008 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18066 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40123 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27241 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28067 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18747 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20948 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    20028 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22292 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25073 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/
+-rw-r--r--   0 runner    (1001) docker     (127)    51767 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.903418 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/message/
+-rw-r--r--   0 runner    (1001) docker     (127)    37665 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42100 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28931 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19538 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/participant_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22539 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/conversations/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    29689 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26515 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/conversations/v1/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    28023 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25220 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/conversations/v1/user/user_conversation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/events/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/EventsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/events/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/event_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/events/v1/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/schema/schema_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/events/v1/sink/
+-rw-r--r--   0 runner    (1001) docker     (127)    22935 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/sink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/sink/sink_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/sink/sink_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/events/v1/subscription/
+-rw-r--r--   0 runner    (1001) docker     (127)    22612 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/subscription/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20285 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/events/v1/subscription/subscribed_event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.907419 twilio-9.1.0/twilio/rest/flex_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/FlexApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6332 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.911419 twilio-9.1.0/twilio/rest/flex_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10023 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23444 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19865 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16094 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47494 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/flex_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17365 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12881 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_conversations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21096 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26893 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_segments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3334 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/insights_user_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.911419 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/
+-rw-r--r--   0 runner    (1001) docker     (127)     9313 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.911419 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)    21581 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13863 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20538 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/flex_api/v1/plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)    23281 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21534 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin/plugin_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)    20121 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration/configured_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7774 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17816 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8781 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/plugin_version_archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/provisioning_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20826 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v1/web_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/flex_api/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v2/flex_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6020 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/flex_api/v2/web_channels.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/frontline_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/frontline_api/FrontlineApiBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/frontline_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/frontline_api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/frontline_api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10893 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/frontline_api/v1/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/insights/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/InsightsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/insights/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.915419 twilio-9.1.0/twilio/rest/insights/v1/call/
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call/call_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13652 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49306 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/call_summaries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/insights/v1/conference/
+-rw-r--r--   0 runner    (1001) docker     (127)    31379 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/conference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25261 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/conference/conference_participant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/insights/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (127)    25246 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/room/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17902 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/room/participant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9164 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/insights/v1/setting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/intelligence/
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/IntelligenceBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/intelligence/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25378 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/custom_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18160 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7717 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/operator_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/operator_attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/operator_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19137 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/prebuilt_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34129 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/intelligence/v2/transcript/
+-rw-r--r--   0 runner    (1001) docker     (127)    29041 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/transcript/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/transcript/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20410 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/transcript/operator_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/intelligence/v2/transcript/sentence.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/ip_messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/IpMessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.919419 twilio-9.1.0/twilio/rest/ip_messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    63691 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21730 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21823 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    21368 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11550 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21764 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    46389 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17910 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/binding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.923419 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)    30575 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29529 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28805 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26180 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)    24058 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18195 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21481 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/lookups/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/LookupsBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/lookups/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/v1/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/lookups/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25093 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/lookups/v2/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/media/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/MessagingBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.927419 twilio-9.1.0/twilio/rest/messaging/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5613 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/
+-rw-r--r--   0 runner    (1001) docker     (127)    24690 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3582 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19921 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/deactivations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/domain_certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14002 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/domain_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7990 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/external_campaign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/messaging/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    56727 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18351 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/alpha_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/channel_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18416 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18138 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/short_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44053 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59064 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/tollfree_verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/messaging/v1/usecase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/microvisor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/MicrovisorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/microvisor/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17841 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/account_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17726 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/account_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/microvisor/v1/app/
+-rw-r--r--   0 runner    (1001) docker     (127)    15665 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/app/app_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/microvisor/v1/device/
+-rw-r--r--   0 runner    (1001) docker     (127)    20979 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19148 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/device/device_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19033 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/microvisor/v1/device/device_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.931419 twilio-9.1.0/twilio/rest/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/monitor/MonitorBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/monitor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/monitor/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/monitor/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22724 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/monitor/v1/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/monitor/v1/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/notify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/NotifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/notify/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28093 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/v1/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/notify/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    47437 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30277 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/v1/service/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25487 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/notify/v1/service/notification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/NumbersBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.935419 twilio-9.1.0/twilio/rest/numbers/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/bulk_eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/eligibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10133 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_port_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10427 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_port_in_phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8816 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_portability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_webhook_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_webhook_configuration_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v1/porting_webhook_configuration_fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/numbers/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/numbers/v2/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (127)    25375 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22250 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10792 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/bulk_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35453 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)    47565 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13884 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16200 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14152 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18539 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22412 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14800 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/oauth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/oauth/OauthBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/oauth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.939419 twilio-9.1.0/twilio/rest/oauth/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/oauth/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4011 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/oauth/v1/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/oauth/v1/token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/PreviewBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/deployed_devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/
+-rw-r--r--   0 runner    (1001) docker     (127)    22445 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24121 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22166 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26786 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22729 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/hosted_numbers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/hosted_numbers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/hosted_numbers/authorization_document/
+-rw-r--r--   0 runner    (1001) docker     (127)    32383 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25081 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48458 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/marketplace/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/marketplace/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/marketplace/available_add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)    15068 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16164 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/marketplace/installed_add_on/
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18612 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/sync/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    22668 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.943419 twilio-9.1.0/twilio/rest/preview/sync/service/document/
+-rw-r--r--   0 runner    (1001) docker     (127)    20550 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21641 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (127)    18342 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24179 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21583 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (127)    18220 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24068 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/preview/wireless/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/wireless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18914 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/wireless/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22050 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/wireless/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/preview/wireless/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    28868 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/wireless/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview/wireless/sim/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/preview_messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/preview_messaging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/pricing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/PricingBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/pricing/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/pricing/v1/messaging/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14531 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/messaging/country.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/pricing/v1/phone_number/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/phone_number/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14124 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/phone_number/country.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.947419 twilio-9.1.0/twilio/rest/pricing/v1/voice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v1/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/pricing/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14471 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8966 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/pricing/v2/voice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/voice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/voice/country.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/pricing/v2/voice/number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/ProxyBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/proxy/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/proxy/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    38168 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23884 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/phone_number.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/proxy/v1/service/session/
+-rw-r--r--   0 runner    (1001) docker     (127)    27772 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21124 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/session/interaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/proxy/v1/service/session/participant/
+-rw-r--r--   0 runner    (1001) docker     (127)    22768 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23247 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21439 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/proxy/v1/service/short_code.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/routes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/RoutesBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.951419 twilio-9.1.0/twilio/rest/routes/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9727 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/v2/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/v2/sip_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/routes/v2/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/ServerlessBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    25756 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/asset/
+-rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/asset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    20312 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6407 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/build/build_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)    21012 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18052 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/environment/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20929 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/environment/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22601 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/environment/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/function/
+-rw-r--r--   0 runner    (1001) docker     (127)    20931 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/function/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/serverless/v1/service/function/function_version/
+-rw-r--r--   0 runner    (1001) docker     (127)    18096 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/studio/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/StudioBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/studio/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/studio/v1/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)    16407 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.955419 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/
+-rw-r--r--   0 runner    (1001) docker     (127)    21371 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/step/
+-rw-r--r--   0 runner    (1001) docker     (127)    17220 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    27275 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v2/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)    23685 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/
+-rw-r--r--   0 runner    (1001) docker     (127)    27159 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_step/
+-rw-r--r--   0 runner    (1001) docker     (127)    17889 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7716 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/flow_revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7422 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow/flow_test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/studio/v2/flow_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.959419 twilio-9.1.0/twilio/rest/supersim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/SupersimBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/supersim/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23725 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/esim_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35353 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/fleet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26669 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/ip_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17594 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/supersim/v1/network_access_profile/
+-rw-r--r--   0 runner    (1001) docker     (127)    20074 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14219 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/settings_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/supersim/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    28737 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/sim/billing_period.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23006 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/sms_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26843 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/supersim/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/SyncBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/v1/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    37557 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/v1/service/document/
+-rw-r--r--   0 runner    (1001) docker     (127)    25376 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/document/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/document/document_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/
+-rw-r--r--   0 runner    (1001) docker     (127)    25201 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36676 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22012 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.963419 twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/
+-rw-r--r--   0 runner    (1001) docker     (127)    24889 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37235 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21940 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/sync/v1/service/sync_stream/
+-rw-r--r--   0 runner    (1001) docker     (127)    22902 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/taskrouter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/TaskrouterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/taskrouter/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)    44586 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26058 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32777 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task/
+-rw-r--r--   0 runner    (1001) docker     (127)    57338 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81514 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23752 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.967419 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/
+-rw-r--r--   0 runner    (1001) docker     (127)    39929 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_bulk_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18320 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10994 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13380 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21315 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.971419 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)    44060 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79296 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22161 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11730 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13252 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7895 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13545 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.971419 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    34582 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18165 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13564 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.971419 twilio-9.1.0/twilio/rest/trunking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/TrunkingBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.971419 twilio-9.1.0/twilio/rest/trunking/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.971419 twilio-9.1.0/twilio/rest/trunking/v1/trunk/
+-rw-r--r--   0 runner    (1001) docker     (127)    40226 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18353 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/credential_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18723 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27869 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/origination_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22464 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/phone_number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trunking/v1/trunk/recording.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.975419 twilio-9.1.0/twilio/rest/trusthub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/TrusthubBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.975419 twilio-9.1.0/twilio/rest/trusthub/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/compliance_inquiries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27642 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/compliance_registration_inquiries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/compliance_tollfree_inquiries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.975419 twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)    30934 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23440 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21885 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18454 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20563 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/end_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14115 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/end_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13543 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/supporting_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14741 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/supporting_document_type.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.975419 twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/
+-rw-r--r--   0 runner    (1001) docker     (127)    30294 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23134 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21456 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.975419 twilio-9.1.0/twilio/rest/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/VerifyBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.979419 twilio-9.1.0/twilio/rest/verify/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8038 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/safelist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.979419 twilio-9.1.0/twilio/rest/verify/v2/service/
+-rw-r--r--   0 runner    (1001) docker     (127)    62562 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/access_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.979419 twilio-9.1.0/twilio/rest/verify/v2/service/entity/
+-rw-r--r--   0 runner    (1001) docker     (127)    20671 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/entity/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.979419 twilio-9.1.0/twilio/rest/verify/v2/service/entity/challenge/
+-rw-r--r--   0 runner    (1001) docker     (127)    34465 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29596 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/entity/factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16167 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/entity/new_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23302 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/messaging_configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.979419 twilio-9.1.0/twilio/rest/verify/v2/service/rate_limit/
+-rw-r--r--   0 runner    (1001) docker     (127)    21510 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22476 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/verification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/verification_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25394 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/service/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11731 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/verification_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/verify/v2/verification_attempts_summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.983420 twilio-9.1.0/twilio/rest/video/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/VideoBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.983420 twilio-9.1.0/twilio/rest/video/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2972 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35040 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/composition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55002 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/composition_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/composition_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27316 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/recording_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.983420 twilio-9.1.0/twilio/rest/video/v1/room/
+-rw-r--r--   0 runner    (1001) docker     (127)    38354 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.983420 twilio-9.1.0/twilio/rest/video/v1/room/participant/
+-rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/participant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/participant/anonymize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16890 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/participant/published_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17082 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/recording_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24749 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/video/v1/room/room_recording.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.983420 twilio-9.1.0/twilio/rest/voice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/VoiceBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/voice/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/archived_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37489 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/byoc_trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/voice/v1/connection_policy/
+-rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/connection_policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29300 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/country/
+-rw-r--r--   0 runner    (1001) docker     (127)    27348 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7140 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/ip_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19432 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/voice/v1/source_ip_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/wireless/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/WirelessBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/wireless/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27547 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29959 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/rate_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/rest/wireless/v1/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    46224 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14323 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/sim/data_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/sim/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16069 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/rest/wireless/v1/usage_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.987419 twilio-9.1.0/twilio/twiml/
+-rw-r--r--   0 runner    (1001) docker     (127)     3471 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/twiml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/twiml/fax_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/twiml/messaging_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83800 2024-05-24 11:14:44.000000 twilio-9.1.0/twilio/twiml/voice_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 11:14:48.991420 twilio-9.1.0/twilio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12040 2024-05-24 11:14:48.000000 twilio-9.1.0/twilio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30635 2024-05-24 11:14:48.000000 twilio-9.1.0/twilio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 11:14:48.000000 twilio-9.1.0/twilio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-24 11:14:48.000000 twilio-9.1.0/twilio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-24 11:14:48.000000 twilio-9.1.0/twilio.egg-info/top_level.txt
```

### Comparing `twilio-9.0.5/AUTHORS.md` & `twilio-9.1.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/LICENSE` & `twilio-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/PKG-INFO` & `twilio-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 9.0.5
+Version: 9.1.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `twilio-9.0.5/README.md` & `twilio-9.1.0/README.md`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/setup.py` & `twilio-9.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # python setup.py install
 #
 # You need to have the setuptools module installed. Try reading the setuptools
 # documentation: http://pypi.python.org/pypi/setuptools
 
 setup(
     name="twilio",
-    version="9.0.5",
+    version="9.1.0",
     description="Twilio API client and TwiML generator",
     author="Twilio",
     help_center="https://www.twilio.com/help/contact",
     url="https://github.com/twilio/twilio-python/",
     keywords=["twilio", "twiml"],
     python_requires=">=3.7.0",
     install_requires=[
```

### Comparing `twilio-9.0.5/twilio/base/client_base.py` & `twilio-9.1.0/twilio/base/client_base.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/deserialize.py` & `twilio-9.1.0/twilio/base/deserialize.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/domain.py` & `twilio-9.1.0/twilio/base/domain.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/exceptions.py` & `twilio-9.1.0/twilio/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/obsolete.py` & `twilio-9.1.0/twilio/base/obsolete.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/page.py` & `twilio-9.1.0/twilio/base/page.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/serialize.py` & `twilio-9.1.0/twilio/base/serialize.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/base/version.py` & `twilio-9.1.0/twilio/base/version.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/http/__init__.py` & `twilio-9.1.0/twilio/http/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/http/async_http_client.py` & `twilio-9.1.0/twilio/http/async_http_client.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/http/http_client.py` & `twilio-9.1.0/twilio/http/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import logging
 from typing import Dict, Optional, Tuple
 
 from requests import Request, Session, hooks
 from requests.adapters import HTTPAdapter
 
 from twilio.http import HttpClient
@@ -35,15 +36,18 @@
         :param proxy: Http proxy for the requests session
         :param max_retries: Maximum number of retries each request should attempt
         """
         super().__init__(logger, False, timeout)
         self.session = Session() if pool_connections else None
         if self.session and max_retries is not None:
             self.session.mount("https://", HTTPAdapter(max_retries=max_retries))
-
+        if self.session is not None:
+            self.session.mount(
+                "https://", HTTPAdapter(pool_maxsize=min(32, os.cpu_count() + 4))
+            )
         self.request_hooks = request_hooks or hooks.default_hooks()
         self.proxy = proxy if proxy else {}
 
     def request(
         self,
         method: str,
         url: str,
```

### Comparing `twilio-9.0.5/twilio/http/request.py` & `twilio-9.1.0/twilio/http/request.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/http/response.py` & `twilio-9.1.0/twilio/http/response.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/http/validation_client.py` & `twilio-9.1.0/twilio/http/validation_client.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/__init__.py` & `twilio-9.1.0/twilio/jwt/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/access_token/__init__.py` & `twilio-9.1.0/twilio/jwt/access_token/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/access_token/grants.py` & `twilio-9.1.0/twilio/jwt/access_token/grants.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/client/__init__.py` & `twilio-9.1.0/twilio/jwt/client/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/taskrouter/__init__.py` & `twilio-9.1.0/twilio/jwt/taskrouter/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/taskrouter/capabilities.py` & `twilio-9.1.0/twilio/jwt/taskrouter/capabilities.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/jwt/validation/__init__.py` & `twilio-9.1.0/twilio/jwt/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/request_validator.py` & `twilio-9.1.0/twilio/request_validator.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/__init__.py` & `twilio-9.1.0/twilio/rest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,14 @@
     from twilio.rest.events import Events
     from twilio.rest.flex_api import FlexApi
     from twilio.rest.frontline_api import FrontlineApi
     from twilio.rest.insights import Insights
     from twilio.rest.intelligence import Intelligence
     from twilio.rest.ip_messaging import IpMessaging
     from twilio.rest.lookups import Lookups
-    from twilio.rest.preview_messaging import PreviewMessaging
     from twilio.rest.messaging import Messaging
     from twilio.rest.microvisor import Microvisor
     from twilio.rest.monitor import Monitor
     from twilio.rest.notify import Notify
     from twilio.rest.numbers import Numbers
     from twilio.rest.oauth import Oauth
     from twilio.rest.preview import Preview
@@ -131,15 +130,14 @@
         self._events: Optional["Events"] = None
         self._flex_api: Optional["FlexApi"] = None
         self._frontline_api: Optional["FrontlineApi"] = None
         self._insights: Optional["Insights"] = None
         self._intelligence: Optional["Intelligence"] = None
         self._ip_messaging: Optional["IpMessaging"] = None
         self._lookups: Optional["Lookups"] = None
-        self._preview_messaging: Optional["PreviewMessaging"] = None
         self._messaging: Optional["Messaging"] = None
         self._microvisor: Optional["Microvisor"] = None
         self._monitor: Optional["Monitor"] = None
         self._notify: Optional["Notify"] = None
         self._numbers: Optional["Numbers"] = None
         self._oauth: Optional["Oauth"] = None
         self._preview: Optional["Preview"] = None
@@ -324,27 +322,14 @@
         if self._lookups is None:
             from twilio.rest.lookups import Lookups
 
             self._lookups = Lookups(self)
         return self._lookups
 
     @property
-    def preview_messaging(self) -> "PreviewMessaging":
-        """
-        Access the PreviewMessaging Twilio Domain
-
-        :returns: PreviewMessaging Twilio Domain
-        """
-        if self._preview_messaging is None:
-            from twilio.rest.preview_messaging import PreviewMessaging
-
-            self._preview_messaging = PreviewMessaging(self)
-        return self._preview_messaging
-
-    @property
     def messaging(self) -> "Messaging":
         """
         Access the Messaging Twilio Domain
 
         :returns: Messaging Twilio Domain
         """
         if self._messaging is None:
```

### Comparing `twilio-9.0.5/twilio/rest/accounts/AccountsBase.py` & `twilio-9.1.0/twilio/rest/accounts/AccountsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/__init__.py` & `twilio-9.1.0/twilio/rest/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/__init__.py` & `twilio-9.1.0/twilio/rest/accounts/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/auth_token_promotion.py` & `twilio-9.1.0/twilio/rest/accounts/v1/auth_token_promotion.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/credential/__init__.py` & `twilio-9.1.0/twilio/rest/accounts/v1/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/credential/aws.py` & `twilio-9.1.0/twilio/rest/accounts/v1/credential/aws.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/credential/public_key.py` & `twilio-9.1.0/twilio/rest/accounts/v1/credential/public_key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/safelist.py` & `twilio-9.1.0/twilio/rest/accounts/v1/safelist.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/accounts/v1/secondary_auth_token.py` & `twilio-9.1.0/twilio/rest/accounts/v1/secondary_auth_token.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/ApiBase.py` & `twilio-9.1.0/twilio/rest/api/ApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/__init__.py` & `twilio-9.1.0/twilio/rest/api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/address/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/address/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/address/dependent_phone_number.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/address/dependent_phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/application.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/application.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/authorized_connect_app.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/authorized_connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/local.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/local.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/machine_to_machine.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/national.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/national.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/shared_cost.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/available_phone_number_country/voip.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/available_phone_number_country/voip.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/balance.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/balance.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/event.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/notification.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/payment.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/payment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/recording.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/siprec.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/siprec.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/stream.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/stream.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/user_defined_message.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/user_defined_message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/call/user_defined_message_subscription.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/conference/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/conference/participant.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/conference/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/conference/recording.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/conference/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/connect_app.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/connect_app.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/assigned_add_on/assigned_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/local.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/local.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/mobile.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/incoming_phone_number/toll_free.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/key.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/message/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/message/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     :ivar date_updated: The [RFC 2822](https://datatracker.ietf.org/doc/html/rfc2822#section-3.3) timestamp (in GMT) of when the Message resource was last updated
     :ivar price: The amount billed for the message in the currency specified by `price_unit`. The `price` is populated after the message has been sent/received, and may not be immediately availalble. View the [Pricing page](https://www.twilio.com/en-us/pricing) for more details.
     :ivar error_message: The description of the `error_code` if the Message `status` is `failed` or `undelivered`. If no error was encountered, the value is `null`.
     :ivar uri: The URI of the Message resource, relative to `https://api.twilio.com`.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) associated with the Message resource
     :ivar num_media: The number of media files associated with the Message resource.
     :ivar status: 
-    :ivar messaging_service_sid: The SID of the [Messaging Service](https://www.twilio.com/docs/messaging/api/service-resource) associated with the Message resource. The value is `null` if a Messaging Service was not used.
+    :ivar messaging_service_sid: The SID of the [Messaging Service](https://www.twilio.com/docs/messaging/api/service-resource) associated with the Message resource. A unique default value is assigned if a Messaging Service is not used.
     :ivar sid: The unique, Twilio-provided string that identifies the Message resource.
     :ivar date_sent: The [RFC 2822](https://datatracker.ietf.org/doc/html/rfc2822#section-3.3) timestamp (in GMT) of when the Message was sent. For an outgoing message, this is when Twilio sent the message. For an incoming message, this is when Twilio sent the HTTP request to your incoming message webhook URL.
     :ivar date_created: The [RFC 2822](https://datatracker.ietf.org/doc/html/rfc2822#section-3.3) timestamp (in GMT) of when the Message resource was created
     :ivar error_code: The [error code](https://www.twilio.com/docs/api/errors) returned if the Message `status` is `failed` or `undelivered`. If no error was encountered, the value is `null`.
     :ivar price_unit: The currency in which `price` is measured, in [ISO 4127](https://www.iso.org/iso/home/standards/currency_codes.htm) format (e.g. `usd`, `eur`, `jpy`).
     :ivar api_version: The API version used to process the Message
     :ivar subresource_uris: A list of related resources identified by their URIs relative to `https://api.twilio.com`
```

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/message/feedback.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/message/feedback.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/message/media.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/message/media.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/new_key.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/new_key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/new_signing_key.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/new_signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/notification.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/outgoing_caller_id.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/outgoing_caller_id.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/queue/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/queue/member.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/queue/member.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/recording/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/recording/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/recording/add_on_result/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/recording/add_on_result/payload.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/recording/add_on_result/payload.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/recording/transcription.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/recording/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/short_code.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/signing_key.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/signing_key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/credential_list/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/credential_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/credential_list/credential.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/credential_list/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_calls/auth_calls_ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/auth_types/auth_type_registrations/auth_registrations_credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/credential_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/domain/ip_access_control_list_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/sip/ip_access_control_list/ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/token.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/token.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/transcription.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/transcription.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/__init__.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/all_time.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/all_time.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/daily.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/daily.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/last_month.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/last_month.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/monthly.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/monthly.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/this_month.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/this_month.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/today.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/today.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/yearly.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/yearly.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/record/yesterday.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/record/yesterday.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/usage/trigger.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/usage/trigger.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/api/v2010/account/validation_request.py` & `twilio-9.1.0/twilio/rest/api/v2010/account/validation_request.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/autopilot/__init__.py` & `twilio-9.1.0/twilio/rest/autopilot/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/BulkexportsBase.py` & `twilio-9.1.0/twilio/rest/bulkexports/BulkexportsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/__init__.py` & `twilio-9.1.0/twilio/rest/bulkexports/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/__init__.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/export/__init__.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/export/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/export/day.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/export/day.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/export/export_custom_job.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/export/export_custom_job.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/export/job.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/export/job.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/bulkexports/v1/export_configuration.py` & `twilio-9.1.0/twilio/rest/bulkexports/v1/export_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/ChatBase.py` & `twilio-9.1.0/twilio/rest/chat/ChatBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/__init__.py` & `twilio-9.1.0/twilio/rest/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/credential.py` & `twilio-9.1.0/twilio/rest/chat/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/channel/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/channel/invite.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/channel/member.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/channel/message.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/role.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/user/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v1/service/user/user_channel.py` & `twilio-9.1.0/twilio/rest/chat/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/credential.py` & `twilio-9.1.0/twilio/rest/chat/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/binding.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/channel/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/channel/invite.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/channel/member.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/channel/message.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/channel/webhook.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/role.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/user/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/user/user_binding.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v2/service/user/user_channel.py` & `twilio-9.1.0/twilio/rest/chat/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v3/__init__.py` & `twilio-9.1.0/twilio/rest/chat/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/chat/v3/channel.py` & `twilio-9.1.0/twilio/rest/chat/v3/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/ContentBase.py` & `twilio-9.1.0/twilio/rest/video/VideoBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,36 +9,36 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.content.v1 import V1
+from twilio.rest.video.v1 import V1
 
 
-class ContentBase(Domain):
+class VideoBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the Content Domain
+        Initialize the Video Domain
 
-        :returns: Domain for Content
+        :returns: Domain for Video
         """
-        super().__init__(twilio, "https://content.twilio.com")
+        super().__init__(twilio, "https://video.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Content
+        :returns: Versions v1 of Video
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Content>"
+        return "<Twilio.Video>"
```

### Comparing `twilio-9.0.5/twilio/rest/content/__init__.py` & `twilio-9.1.0/twilio/rest/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/__init__.py` & `twilio-9.1.0/twilio/rest/content/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/content/__init__.py` & `twilio-9.1.0/twilio/rest/content/v1/content/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/content/approval_create.py` & `twilio-9.1.0/twilio/rest/content/v1/content/approval_create.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/content/approval_fetch.py` & `twilio-9.1.0/twilio/rest/content/v1/content/approval_fetch.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/content_and_approvals.py` & `twilio-9.1.0/twilio/rest/content/v1/content_and_approvals.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/content/v1/legacy_content.py` & `twilio-9.1.0/twilio/rest/content/v1/legacy_content.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/ConversationsBase.py` & `twilio-9.1.0/twilio/rest/conversations/ConversationsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/address_configuration.py` & `twilio-9.1.0/twilio/rest/conversations/v1/address_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/configuration/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/configuration/webhook.py` & `twilio-9.1.0/twilio/rest/conversations/v1/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/conversation/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/conversation/message/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py` & `twilio-9.1.0/twilio/rest/conversations/v1/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/conversation/participant.py` & `twilio-9.1.0/twilio/rest/conversations/v1/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/conversation/webhook.py` & `twilio-9.1.0/twilio/rest/conversations/v1/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/credential.py` & `twilio-9.1.0/twilio/rest/conversations/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/participant_conversation.py` & `twilio-9.1.0/twilio/rest/conversations/v1/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/role.py` & `twilio-9.1.0/twilio/rest/conversations/v1/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/binding.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/notification.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/configuration/webhook.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/configuration/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/message/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/message/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/message/delivery_receipt.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/participant.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/conversation/webhook.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/conversation/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/participant_conversation.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/participant_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/role.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/user/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/service/user/user_conversation.py` & `twilio-9.1.0/twilio/rest/conversations/v1/service/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/user/__init__.py` & `twilio-9.1.0/twilio/rest/conversations/v1/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/conversations/v1/user/user_conversation.py` & `twilio-9.1.0/twilio/rest/conversations/v1/user/user_conversation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/EventsBase.py` & `twilio-9.1.0/twilio/rest/events/EventsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/__init__.py` & `twilio-9.1.0/twilio/rest/events/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/__init__.py` & `twilio-9.1.0/twilio/rest/events/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/event_type.py` & `twilio-9.1.0/twilio/rest/events/v1/event_type.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/schema/__init__.py` & `twilio-9.1.0/twilio/rest/events/v1/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/schema/schema_version.py` & `twilio-9.1.0/twilio/rest/events/v1/schema/schema_version.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/sink/__init__.py` & `twilio-9.1.0/twilio/rest/events/v1/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/sink/sink_test.py` & `twilio-9.1.0/twilio/rest/events/v1/sink/sink_test.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/sink/sink_validate.py` & `twilio-9.1.0/twilio/rest/events/v1/sink/sink_validate.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/subscription/__init__.py` & `twilio-9.1.0/twilio/rest/events/v1/subscription/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/events/v1/subscription/subscribed_event.py` & `twilio-9.1.0/twilio/rest/events/v1/subscription/subscribed_event.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/FlexApiBase.py` & `twilio-9.1.0/twilio/rest/flex_api/FlexApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/assessments.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/assessments.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/channel.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/configuration.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/flex_flow.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/flex_flow.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_assessments_comment.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_assessments_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_conversations.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_conversations.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires_category.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires_category.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_questionnaires_question.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_questionnaires_question.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_segments.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_segments.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_session.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_session.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_settings_answer_sets.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_settings_answer_sets.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_settings_comment.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_settings_comment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/insights_user_roles.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/insights_user_roles.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/interaction/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/interaction/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         super().__init__(version)
 
         self._uri = "/Interactions"
 
     def create(
         self,
         channel: object,
-        routing: object,
+        routing: Union[object, object] = values.unset,
         interaction_context_sid: Union[str, object] = values.unset,
     ) -> InteractionInstance:
         """
         Create the InteractionInstance
 
         :param channel: The Interaction's channel.
         :param routing: The Interaction's routing logic.
@@ -226,15 +226,15 @@
         )
 
         return InteractionInstance(self._version, payload)
 
     async def create_async(
         self,
         channel: object,
-        routing: object,
+        routing: Union[object, object] = values.unset,
         interaction_context_sid: Union[str, object] = values.unset,
     ) -> InteractionInstance:
         """
         Asynchronously create the InteractionInstance
 
         :param channel: The Interaction's channel.
         :param routing: The Interaction's routing logic.
```

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_invite.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/interaction/interaction_channel/interaction_channel_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin/plugin_versions.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin/plugin_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,17 @@
     """
     :ivar sid: The unique string that we created to identify the Flex Plugin Version resource.
     :ivar plugin_sid: The SID of the Flex Plugin resource this Flex Plugin Version belongs to.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Flex Plugin Version resource and owns this resource.
     :ivar version: The unique version of this Flex Plugin Version.
     :ivar plugin_url: The URL of where the Flex Plugin Version JavaScript bundle is hosted on.
     :ivar changelog: A changelog that describes the changes this Flex Plugin Version brings.
-    :ivar private: Whether to inject credentials while accessing this Plugin Version. The default value is false.
+    :ivar private: Whether the Flex Plugin Version is validated. The default value is false.
     :ivar archived: Whether the Flex Plugin Version is archived. The default value is false.
+    :ivar validated:
     :ivar date_created: The date and time in GMT when the Flex Plugin Version was created specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     :ivar url: The absolute URL of the Flex Plugin Version resource.
     """
 
     def __init__(
         self,
         version: Version,
@@ -49,14 +50,15 @@
         self.plugin_sid: Optional[str] = payload.get("plugin_sid")
         self.account_sid: Optional[str] = payload.get("account_sid")
         self.version: Optional[str] = payload.get("version")
         self.plugin_url: Optional[str] = payload.get("plugin_url")
         self.changelog: Optional[str] = payload.get("changelog")
         self.private: Optional[bool] = payload.get("private")
         self.archived: Optional[bool] = payload.get("archived")
+        self.validated: Optional[bool] = payload.get("validated")
         self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_created")
         )
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
             "plugin_sid": plugin_sid,
```

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_archive.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_archive.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration/configured_plugin.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration/configured_plugin.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_configuration_archive.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_configuration_archive.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_release.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_release.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/plugin_version_archive.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/plugin_version_archive.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/provisioning_status.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/provisioning_status.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v1/web_channel.py` & `twilio-9.1.0/twilio/rest/flex_api/v1/web_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v2/__init__.py` & `twilio-9.1.0/twilio/rest/flex_api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v2/flex_user.py` & `twilio-9.1.0/twilio/rest/flex_api/v2/flex_user.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/flex_api/v2/web_channels.py` & `twilio-9.1.0/twilio/rest/flex_api/v2/web_channels.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/frontline_api/FrontlineApiBase.py` & `twilio-9.1.0/twilio/rest/frontline_api/FrontlineApiBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/frontline_api/v1/__init__.py` & `twilio-9.1.0/twilio/rest/frontline_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/frontline_api/v1/user.py` & `twilio-9.1.0/twilio/rest/frontline_api/v1/user.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/InsightsBase.py` & `twilio-9.1.0/twilio/rest/insights/InsightsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/__init__.py` & `twilio-9.1.0/twilio/rest/insights/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/__init__.py` & `twilio-9.1.0/twilio/rest/insights/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call/__init__.py` & `twilio-9.1.0/twilio/rest/insights/v1/call/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call/annotation.py` & `twilio-9.1.0/twilio/rest/insights/v1/call/annotation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call/call_summary.py` & `twilio-9.1.0/twilio/rest/insights/v1/call/call_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call/event.py` & `twilio-9.1.0/twilio/rest/insights/v1/call/event.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call/metric.py` & `twilio-9.1.0/twilio/rest/insights/v1/call/metric.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/call_summaries.py` & `twilio-9.1.0/twilio/rest/insights/v1/call_summaries.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/conference/__init__.py` & `twilio-9.1.0/twilio/rest/insights/v1/conference/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/conference/conference_participant.py` & `twilio-9.1.0/twilio/rest/insights/v1/conference/conference_participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/room/__init__.py` & `twilio-9.1.0/twilio/rest/insights/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/room/participant.py` & `twilio-9.1.0/twilio/rest/insights/v1/room/participant.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/insights/v1/setting.py` & `twilio-9.1.0/twilio/rest/insights/v1/setting.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/intelligence/IntelligenceBase.py` & `twilio-9.1.0/twilio/rest/intelligence/IntelligenceBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/__init__.py` & `twilio-9.1.0/twilio/rest/notify/v1/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Intelligence
+    Twilio - Notify
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from typing import Optional
 from twilio.base.version import Version
 from twilio.base.domain import Domain
-from twilio.rest.intelligence.v2.service import ServiceList
-from twilio.rest.intelligence.v2.transcript import TranscriptList
+from twilio.rest.notify.v1.credential import CredentialList
+from twilio.rest.notify.v1.service import ServiceList
 
 
-class V2(Version):
+class V1(Version):
 
     def __init__(self, domain: Domain):
         """
-        Initialize the V2 version of Intelligence
+        Initialize the V1 version of Notify
 
-        :param domain: The Twilio.intelligence domain
+        :param domain: The Twilio.notify domain
         """
-        super().__init__(domain, "v2")
+        super().__init__(domain, "v1")
+        self._credentials: Optional[CredentialList] = None
         self._services: Optional[ServiceList] = None
-        self._transcripts: Optional[TranscriptList] = None
+
+    @property
+    def credentials(self) -> CredentialList:
+        if self._credentials is None:
+            self._credentials = CredentialList(self)
+        return self._credentials
 
     @property
     def services(self) -> ServiceList:
         if self._services is None:
             self._services = ServiceList(self)
         return self._services
 
-    @property
-    def transcripts(self) -> TranscriptList:
-        if self._transcripts is None:
-            self._transcripts = TranscriptList(self)
-        return self._transcripts
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Intelligence.V2>"
+        return "<Twilio.Notify.V1>"
```

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/service.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,20 +34,21 @@
     :ivar auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
     :ivar media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
     :ivar auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
     :ivar data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
     :ivar date_created: The date that this Service was created, given in ISO 8601 format.
     :ivar date_updated: The date that this Service was updated, given in ISO 8601 format.
     :ivar friendly_name: A human readable description of this resource, up to 64 characters.
-    :ivar language_code: The default language code of the audio.
+    :ivar language_code: The language code set during Service creation determines the Transcription language for all call recordings processed by that Service. The default is en-US if no language code is set. A Service can only support one language code, and it cannot be updated once it's set.
     :ivar sid: A 34 character string that uniquely identifies this Service.
     :ivar unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
     :ivar url: The URL of this resource.
     :ivar webhook_url: The URL Twilio will request when executing the Webhook.
     :ivar webhook_http_method: 
+    :ivar read_only_attached_operator_sids: Operator sids attached to this service, read only
     :ivar version: The version number of this Service.
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
@@ -68,14 +69,17 @@
         self.sid: Optional[str] = payload.get("sid")
         self.unique_name: Optional[str] = payload.get("unique_name")
         self.url: Optional[str] = payload.get("url")
         self.webhook_url: Optional[str] = payload.get("webhook_url")
         self.webhook_http_method: Optional["ServiceInstance.HttpMethod"] = payload.get(
             "webhook_http_method"
         )
+        self.read_only_attached_operator_sids: Optional[List[str]] = payload.get(
+            "read_only_attached_operator_sids"
+        )
         self.version: Optional[int] = deserialize.integer(payload.get("version"))
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[ServiceContext] = None
 
@@ -132,85 +136,79 @@
 
     def update(
         self,
         if_match: Union[str, object] = values.unset,
         auto_transcribe: Union[bool, object] = values.unset,
         data_logging: Union[bool, object] = values.unset,
         friendly_name: Union[str, object] = values.unset,
-        language_code: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
         auto_redaction: Union[bool, object] = values.unset,
         media_redaction: Union[bool, object] = values.unset,
         webhook_url: Union[str, object] = values.unset,
         webhook_http_method: Union["ServiceInstance.HttpMethod", object] = values.unset,
     ) -> "ServiceInstance":
         """
         Update the ServiceInstance
 
         :param if_match: The If-Match HTTP request header
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The updated ServiceInstance
         """
         return self._proxy.update(
             if_match=if_match,
             auto_transcribe=auto_transcribe,
             data_logging=data_logging,
             friendly_name=friendly_name,
-            language_code=language_code,
             unique_name=unique_name,
             auto_redaction=auto_redaction,
             media_redaction=media_redaction,
             webhook_url=webhook_url,
             webhook_http_method=webhook_http_method,
         )
 
     async def update_async(
         self,
         if_match: Union[str, object] = values.unset,
         auto_transcribe: Union[bool, object] = values.unset,
         data_logging: Union[bool, object] = values.unset,
         friendly_name: Union[str, object] = values.unset,
-        language_code: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
         auto_redaction: Union[bool, object] = values.unset,
         media_redaction: Union[bool, object] = values.unset,
         webhook_url: Union[str, object] = values.unset,
         webhook_http_method: Union["ServiceInstance.HttpMethod", object] = values.unset,
     ) -> "ServiceInstance":
         """
         Asynchronous coroutine to update the ServiceInstance
 
         :param if_match: The If-Match HTTP request header
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The updated ServiceInstance
         """
         return await self._proxy.update_async(
             if_match=if_match,
             auto_transcribe=auto_transcribe,
             data_logging=data_logging,
             friendly_name=friendly_name,
-            language_code=language_code,
             unique_name=unique_name,
             auto_redaction=auto_redaction,
             media_redaction=media_redaction,
             webhook_url=webhook_url,
             webhook_http_method=webhook_http_method,
         )
 
@@ -305,43 +303,40 @@
 
     def update(
         self,
         if_match: Union[str, object] = values.unset,
         auto_transcribe: Union[bool, object] = values.unset,
         data_logging: Union[bool, object] = values.unset,
         friendly_name: Union[str, object] = values.unset,
-        language_code: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
         auto_redaction: Union[bool, object] = values.unset,
         media_redaction: Union[bool, object] = values.unset,
         webhook_url: Union[str, object] = values.unset,
         webhook_http_method: Union["ServiceInstance.HttpMethod", object] = values.unset,
     ) -> ServiceInstance:
         """
         Update the ServiceInstance
 
         :param if_match: The If-Match HTTP request header
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The updated ServiceInstance
         """
         data = values.of(
             {
                 "AutoTranscribe": serialize.boolean_to_string(auto_transcribe),
                 "DataLogging": serialize.boolean_to_string(data_logging),
                 "FriendlyName": friendly_name,
-                "LanguageCode": language_code,
                 "UniqueName": unique_name,
                 "AutoRedaction": serialize.boolean_to_string(auto_redaction),
                 "MediaRedaction": serialize.boolean_to_string(media_redaction),
                 "WebhookUrl": webhook_url,
                 "WebhookHttpMethod": webhook_http_method,
             }
         )
@@ -359,43 +354,40 @@
 
     async def update_async(
         self,
         if_match: Union[str, object] = values.unset,
         auto_transcribe: Union[bool, object] = values.unset,
         data_logging: Union[bool, object] = values.unset,
         friendly_name: Union[str, object] = values.unset,
-        language_code: Union[str, object] = values.unset,
         unique_name: Union[str, object] = values.unset,
         auto_redaction: Union[bool, object] = values.unset,
         media_redaction: Union[bool, object] = values.unset,
         webhook_url: Union[str, object] = values.unset,
         webhook_http_method: Union["ServiceInstance.HttpMethod", object] = values.unset,
     ) -> ServiceInstance:
         """
         Asynchronous coroutine to update the ServiceInstance
 
         :param if_match: The If-Match HTTP request header
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The updated ServiceInstance
         """
         data = values.of(
             {
                 "AutoTranscribe": serialize.boolean_to_string(auto_transcribe),
                 "DataLogging": serialize.boolean_to_string(data_logging),
                 "FriendlyName": friendly_name,
-                "LanguageCode": language_code,
                 "UniqueName": unique_name,
                 "AutoRedaction": serialize.boolean_to_string(auto_redaction),
                 "MediaRedaction": serialize.boolean_to_string(media_redaction),
                 "WebhookUrl": webhook_url,
                 "WebhookHttpMethod": webhook_http_method,
             }
         )
@@ -468,15 +460,15 @@
         """
         Create the ServiceInstance
 
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
+        :param language_code: The language code set during Service creation determines the Transcription language for all call recordings processed by that Service. The default is en-US if no language code is set. A Service can only support one language code, and it cannot be updated once it's set.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The created ServiceInstance
         """
@@ -518,15 +510,15 @@
         """
         Asynchronously create the ServiceInstance
 
         :param unique_name: Provides a unique and addressable name to be assigned to this Service, assigned by the developer, to be optionally used in addition to SID.
         :param auto_transcribe: Instructs the Speech Recognition service to automatically transcribe all recordings made on the account.
         :param data_logging: Data logging allows Twilio to improve the quality of the speech recognition & language understanding services through using customer data to refine, fine tune and evaluate machine learning models. Note: Data logging cannot be activated via API, only via www.twilio.com, as it requires additional consent.
         :param friendly_name: A human readable description of this resource, up to 64 characters.
-        :param language_code: The default language code of the audio.
+        :param language_code: The language code set during Service creation determines the Transcription language for all call recordings processed by that Service. The default is en-US if no language code is set. A Service can only support one language code, and it cannot be updated once it's set.
         :param auto_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts made on this service.
         :param media_redaction: Instructs the Speech Recognition service to automatically redact PII from all transcripts media made on this service. The auto_redaction flag must be enabled, results in error otherwise.
         :param webhook_url: The URL Twilio will request when executing the Webhook.
         :param webhook_http_method:
 
         :returns: The created ServiceInstance
         """
```

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/transcript/__init__.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/transcript/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/transcript/media.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/transcript/media.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/transcript/operator_result.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/transcript/operator_result.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/intelligence/v2/transcript/sentence.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/transcript/sentence.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/IpMessagingBase.py` & `twilio-9.1.0/twilio/rest/ip_messaging/IpMessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/credential.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/invite.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/member.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/channel/message.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/role.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/user/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v1/service/user/user_channel.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v1/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/credential.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/binding.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/invite.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/invite.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/member.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/member.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/message.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/channel/webhook.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/channel/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/role.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/role.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/__init__.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/user_binding.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/user_binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/ip_messaging/v2/service/user/user_channel.py` & `twilio-9.1.0/twilio/rest/ip_messaging/v2/service/user/user_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/lookups/LookupsBase.py` & `twilio-9.1.0/twilio/rest/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/lookups/v1/__init__.py` & `twilio-9.1.0/twilio/rest/lookups/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/lookups/v1/phone_number.py` & `twilio-9.1.0/twilio/rest/lookups/v1/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/lookups/v2/__init__.py` & `twilio-9.1.0/twilio/rest/lookups/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/lookups/v2/phone_number.py` & `twilio-9.1.0/twilio/rest/lookups/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/media/__init__.py` & `twilio-9.1.0/twilio/rest/media/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/MessagingBase.py` & `twilio-9.1.0/twilio/rest/messaging/MessagingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/__init__.py` & `twilio-9.1.0/twilio/rest/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/__init__.py` & `twilio-9.1.0/twilio/rest/messaging/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/__init__.py` & `twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py` & `twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/brand_registration_otp.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/brand_registration/brand_vetting.py` & `twilio-9.1.0/twilio/rest/messaging/v1/brand_registration/brand_vetting.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/deactivations.py` & `twilio-9.1.0/twilio/rest/messaging/v1/deactivations.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/domain_certs.py` & `twilio-9.1.0/twilio/rest/messaging/v1/domain_certs.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/domain_config.py` & `twilio-9.1.0/twilio/rest/messaging/v1/domain_config.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/domain_config_messaging_service.py` & `twilio-9.1.0/twilio/rest/messaging/v1/domain_config_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/external_campaign.py` & `twilio-9.1.0/twilio/rest/messaging/v1/external_campaign.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/linkshortening_messaging_service.py` & `twilio-9.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py` & `twilio-9.1.0/twilio/rest/messaging/v1/linkshortening_messaging_service_domain_association.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     :ivar synchronous_validation: Reserved.
     :ivar validity_period: How long, in seconds, messages sent from the Service are valid. Can be an integer from `1` to `14,400`.
     :ivar url: The absolute URL of the Service resource.
     :ivar links: The absolute URLs of related resources.
     :ivar usecase: A string that describes the scenario in which the Messaging Service will be used. Possible values are `notifications`, `marketing`, `verification`, `discussion`, `poll`, `undeclared`.
     :ivar us_app_to_person_registered: Whether US A2P campaign is registered for this Service.
     :ivar use_inbound_webhook_on_number: A boolean value that indicates either the webhook url configured on the phone number will be used or `inbound_request_url`/`fallback_url` url will be called when a message is received from the phone number. If this field is enabled then the webhook url defined on the phone number will override the `inbound_request_url`/`fallback_url` defined for the Messaging Service.
-    :ivar sending_windows: A list of Sending Windows, which indicate defined time ranges in which a message can be sent, in the UTC time zone. Each window is defined by two strings, labeled \"start_time\" and \"end_time\".
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
@@ -104,17 +103,14 @@
         self.usecase: Optional[str] = payload.get("usecase")
         self.us_app_to_person_registered: Optional[bool] = payload.get(
             "us_app_to_person_registered"
         )
         self.use_inbound_webhook_on_number: Optional[bool] = payload.get(
             "use_inbound_webhook_on_number"
         )
-        self.sending_windows: Optional[Dict[str, object]] = payload.get(
-            "sending_windows"
-        )
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[ServiceContext] = None
 
     @property
```

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/alpha_sender.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/alpha_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/channel_sender.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/channel_sender.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/phone_number.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/short_code.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/us_app_to_person.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/us_app_to_person.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py` & `twilio-9.1.0/twilio/rest/messaging/v1/service/us_app_to_person_usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/tollfree_verification.py` & `twilio-9.1.0/twilio/rest/messaging/v1/tollfree_verification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/messaging/v1/usecase.py` & `twilio-9.1.0/twilio/rest/messaging/v1/usecase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/MicrovisorBase.py` & `twilio-9.1.0/twilio/rest/microvisor/MicrovisorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/__init__.py` & `twilio-9.1.0/twilio/rest/microvisor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/__init__.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/account_config.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/account_config.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/account_secret.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/account_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/app/__init__.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/app/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/app/app_manifest.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/app/app_manifest.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/device/__init__.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/device/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/device/device_config.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/device/device_config.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/microvisor/v1/device/device_secret.py` & `twilio-9.1.0/twilio/rest/microvisor/v1/device/device_secret.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/monitor/MonitorBase.py` & `twilio-9.1.0/twilio/rest/monitor/MonitorBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/monitor/__init__.py` & `twilio-9.1.0/twilio/rest/monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/monitor/v1/__init__.py` & `twilio-9.1.0/twilio/rest/monitor/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/monitor/v1/alert.py` & `twilio-9.1.0/twilio/rest/monitor/v1/alert.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/monitor/v1/event.py` & `twilio-9.1.0/twilio/rest/monitor/v1/event.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/NotifyBase.py` & `twilio-9.1.0/twilio/rest/notify/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/__init__.py` & `twilio-9.1.0/twilio/rest/notify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/v1/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,43 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Notify
+    Twilio - Serverless
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from typing import Optional
 from twilio.base.version import Version
 from twilio.base.domain import Domain
-from twilio.rest.notify.v1.credential import CredentialList
-from twilio.rest.notify.v1.service import ServiceList
+from twilio.rest.serverless.v1.service import ServiceList
 
 
 class V1(Version):
 
     def __init__(self, domain: Domain):
         """
-        Initialize the V1 version of Notify
+        Initialize the V1 version of Serverless
 
-        :param domain: The Twilio.notify domain
+        :param domain: The Twilio.serverless domain
         """
         super().__init__(domain, "v1")
-        self._credentials: Optional[CredentialList] = None
         self._services: Optional[ServiceList] = None
 
     @property
-    def credentials(self) -> CredentialList:
-        if self._credentials is None:
-            self._credentials = CredentialList(self)
-        return self._credentials
-
-    @property
     def services(self) -> ServiceList:
         if self._services is None:
             self._services = ServiceList(self)
         return self._services
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Notify.V1>"
+        return "<Twilio.Serverless.V1>"
```

### Comparing `twilio-9.0.5/twilio/rest/notify/v1/credential.py` & `twilio-9.1.0/twilio/rest/notify/v1/credential.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/notify/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/v1/service/binding.py` & `twilio-9.1.0/twilio/rest/notify/v1/service/binding.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/notify/v1/service/notification.py` & `twilio-9.1.0/twilio/rest/notify/v1/service/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/NumbersBase.py` & `twilio-9.1.0/twilio/rest/numbers/NumbersBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/__init__.py` & `twilio-9.1.0/twilio/rest/numbers/v1/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,83 +13,111 @@
 """
 
 from typing import Optional
 from twilio.base.version import Version
 from twilio.base.domain import Domain
 from twilio.rest.numbers.v1.bulk_eligibility import BulkEligibilityList
 from twilio.rest.numbers.v1.eligibility import EligibilityList
-from twilio.rest.numbers.v1.porting_bulk_portability import PortingBulkPortabilityList
 from twilio.rest.numbers.v1.porting_port_in import PortingPortInList
-from twilio.rest.numbers.v1.porting_port_in_fetch import PortingPortInFetchList
 from twilio.rest.numbers.v1.porting_port_in_phone_number import (
     PortingPortInPhoneNumberList,
 )
 from twilio.rest.numbers.v1.porting_portability import PortingPortabilityList
+from twilio.rest.numbers.v1.porting_webhook_configuration import (
+    PortingWebhookConfigurationList,
+)
+from twilio.rest.numbers.v1.porting_webhook_configuration_delete import (
+    PortingWebhookConfigurationDeleteList,
+)
+from twilio.rest.numbers.v1.porting_webhook_configuration_fetch import (
+    PortingWebhookConfigurationFetchList,
+)
 
 
 class V1(Version):
 
     def __init__(self, domain: Domain):
         """
         Initialize the V1 version of Numbers
 
         :param domain: The Twilio.numbers domain
         """
         super().__init__(domain, "v1")
         self._bulk_eligibilities: Optional[BulkEligibilityList] = None
         self._eligibilities: Optional[EligibilityList] = None
-        self._porting_bulk_portabilities: Optional[PortingBulkPortabilityList] = None
         self._porting_port_ins: Optional[PortingPortInList] = None
-        self._porting_port_ins_fetch: Optional[PortingPortInFetchList] = None
         self._porting_port_in_phone_number: Optional[PortingPortInPhoneNumberList] = (
             None
         )
         self._porting_portabilities: Optional[PortingPortabilityList] = None
+        self._porting_webhook_configurations: Optional[
+            PortingWebhookConfigurationList
+        ] = None
+        self._porting_webhook_configurations_delete: Optional[
+            PortingWebhookConfigurationDeleteList
+        ] = None
+        self._porting_webhook_configuration_fetch: Optional[
+            PortingWebhookConfigurationFetchList
+        ] = None
 
     @property
     def bulk_eligibilities(self) -> BulkEligibilityList:
         if self._bulk_eligibilities is None:
             self._bulk_eligibilities = BulkEligibilityList(self)
         return self._bulk_eligibilities
 
     @property
     def eligibilities(self) -> EligibilityList:
         if self._eligibilities is None:
             self._eligibilities = EligibilityList(self)
         return self._eligibilities
 
     @property
-    def porting_bulk_portabilities(self) -> PortingBulkPortabilityList:
-        if self._porting_bulk_portabilities is None:
-            self._porting_bulk_portabilities = PortingBulkPortabilityList(self)
-        return self._porting_bulk_portabilities
-
-    @property
     def porting_port_ins(self) -> PortingPortInList:
         if self._porting_port_ins is None:
             self._porting_port_ins = PortingPortInList(self)
         return self._porting_port_ins
 
     @property
-    def porting_port_ins_fetch(self) -> PortingPortInFetchList:
-        if self._porting_port_ins_fetch is None:
-            self._porting_port_ins_fetch = PortingPortInFetchList(self)
-        return self._porting_port_ins_fetch
-
-    @property
     def porting_port_in_phone_number(self) -> PortingPortInPhoneNumberList:
         if self._porting_port_in_phone_number is None:
             self._porting_port_in_phone_number = PortingPortInPhoneNumberList(self)
         return self._porting_port_in_phone_number
 
     @property
     def porting_portabilities(self) -> PortingPortabilityList:
         if self._porting_portabilities is None:
             self._porting_portabilities = PortingPortabilityList(self)
         return self._porting_portabilities
 
+    @property
+    def porting_webhook_configurations(self) -> PortingWebhookConfigurationList:
+        if self._porting_webhook_configurations is None:
+            self._porting_webhook_configurations = PortingWebhookConfigurationList(self)
+        return self._porting_webhook_configurations
+
+    @property
+    def porting_webhook_configurations_delete(
+        self,
+    ) -> PortingWebhookConfigurationDeleteList:
+        if self._porting_webhook_configurations_delete is None:
+            self._porting_webhook_configurations_delete = (
+                PortingWebhookConfigurationDeleteList(self)
+            )
+        return self._porting_webhook_configurations_delete
+
+    @property
+    def porting_webhook_configuration_fetch(
+        self,
+    ) -> PortingWebhookConfigurationFetchList:
+        if self._porting_webhook_configuration_fetch is None:
+            self._porting_webhook_configuration_fetch = (
+                PortingWebhookConfigurationFetchList(self)
+            )
+        return self._porting_webhook_configuration_fetch
+
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
         return "<Twilio.Numbers.V1>"
```

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/bulk_eligibility.py` & `twilio-9.1.0/twilio/rest/numbers/v1/bulk_eligibility.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/eligibility.py` & `twilio-9.1.0/twilio/rest/numbers/v1/eligibility.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/porting_bulk_portability.py` & `twilio-9.1.0/twilio/rest/numbers/v1/porting_portability.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,245 +8,236 @@
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from datetime import datetime
-from typing import Any, Dict, List, Optional
-from twilio.base import deserialize, serialize, values
+from typing import Any, Dict, Optional, Union
+from twilio.base import deserialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class PortingBulkPortabilityInstance(InstanceResource):
+class PortingPortabilityInstance(InstanceResource):
 
-    class Status(object):
-        IN_PROGRESS = "in-progress"
-        COMPLETED = "completed"
-        EXPIRED = "expired"
+    class NumberType(object):
+        LOCAL = "LOCAL"
+        UNKNOWN = "UNKNOWN"
+        MOBILE = "MOBILE"
+        TOLL_FREE = "TOLL-FREE"
 
     """
-    :ivar sid: A 34 character string that uniquely identifies this Portability check.
-    :ivar status: 
-    :ivar datetime_created: The date that the Portability check was created, given in ISO 8601 format.
-    :ivar phone_numbers: Contains a list with all the information of the requested phone numbers. Each phone number contains the following properties: `phone_number`: The phone number which portability is to be checked. `portable`: Boolean flag specifying if phone number is portable or not. `not_portable_reason`: Reason why the phone number cannot be ported into Twilio, `null` otherwise. `not_portable_reason_code`: The Portability Reason Code for the phone number if it cannot be ported in Twilio, `null` otherwise. `pin_and_account_number_required`: Boolean flag specifying if PIN and account number is required for the phone number. `number_type`: The type of the requested phone number. `country` Country the phone number belongs to. `messaging_carrier` Current messaging carrier of the phone number. `voice_carrier` Current voice carrier of the phone number.
+    :ivar phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
+    :ivar account_sid: The target account sid to which the number will be ported
+    :ivar portable: Boolean flag specifying if phone number is portable or not.
+    :ivar pin_and_account_number_required: Boolean flag specifying if PIN and account number is required for the phone number.
+    :ivar not_portable_reason: Reason why the phone number cannot be ported into Twilio, `null` otherwise.
+    :ivar not_portable_reason_code: The Portability Reason Code for the phone number if it cannot be ported into Twilio, `null` otherwise. One of `22131`, `22132`, `22130`, `22133`, `22102` or `22135`.
+    :ivar number_type: 
+    :ivar country: Country the phone number belongs to.
+    :ivar messaging_carrier: Current messaging carrier of the phone number
+    :ivar voice_carrier: Current voice carrier of the phone number
     :ivar url: This is the url of the request that you're trying to reach out to locate the resource.
     """
 
     def __init__(
-        self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
+        self,
+        version: Version,
+        payload: Dict[str, Any],
+        phone_number: Optional[str] = None,
     ):
         super().__init__(version)
 
-        self.sid: Optional[str] = payload.get("sid")
-        self.status: Optional["PortingBulkPortabilityInstance.Status"] = payload.get(
-            "status"
-        )
-        self.datetime_created: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("datetime_created")
-        )
-        self.phone_numbers: Optional[List[Dict[str, object]]] = payload.get(
-            "phone_numbers"
-        )
+        self.phone_number: Optional[str] = payload.get("phone_number")
+        self.account_sid: Optional[str] = payload.get("account_sid")
+        self.portable: Optional[bool] = payload.get("portable")
+        self.pin_and_account_number_required: Optional[bool] = payload.get(
+            "pin_and_account_number_required"
+        )
+        self.not_portable_reason: Optional[str] = payload.get("not_portable_reason")
+        self.not_portable_reason_code: Optional[int] = deserialize.integer(
+            payload.get("not_portable_reason_code")
+        )
+        self.number_type: Optional["PortingPortabilityInstance.NumberType"] = (
+            payload.get("number_type")
+        )
+        self.country: Optional[str] = payload.get("country")
+        self.messaging_carrier: Optional[str] = payload.get("messaging_carrier")
+        self.voice_carrier: Optional[str] = payload.get("voice_carrier")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "sid": sid or self.sid,
+            "phone_number": phone_number or self.phone_number,
         }
-        self._context: Optional[PortingBulkPortabilityContext] = None
+        self._context: Optional[PortingPortabilityContext] = None
 
     @property
-    def _proxy(self) -> "PortingBulkPortabilityContext":
+    def _proxy(self) -> "PortingPortabilityContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: PortingBulkPortabilityContext for this PortingBulkPortabilityInstance
+        :returns: PortingPortabilityContext for this PortingPortabilityInstance
         """
         if self._context is None:
-            self._context = PortingBulkPortabilityContext(
+            self._context = PortingPortabilityContext(
                 self._version,
-                sid=self._solution["sid"],
+                phone_number=self._solution["phone_number"],
             )
         return self._context
 
-    def fetch(self) -> "PortingBulkPortabilityInstance":
+    def fetch(
+        self, target_account_sid: Union[str, object] = values.unset
+    ) -> "PortingPortabilityInstance":
         """
-        Fetch the PortingBulkPortabilityInstance
+        Fetch the PortingPortabilityInstance
 
+        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingBulkPortabilityInstance
+        :returns: The fetched PortingPortabilityInstance
         """
-        return self._proxy.fetch()
+        return self._proxy.fetch(
+            target_account_sid=target_account_sid,
+        )
 
-    async def fetch_async(self) -> "PortingBulkPortabilityInstance":
+    async def fetch_async(
+        self, target_account_sid: Union[str, object] = values.unset
+    ) -> "PortingPortabilityInstance":
         """
-        Asynchronous coroutine to fetch the PortingBulkPortabilityInstance
+        Asynchronous coroutine to fetch the PortingPortabilityInstance
 
+        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingBulkPortabilityInstance
+        :returns: The fetched PortingPortabilityInstance
         """
-        return await self._proxy.fetch_async()
+        return await self._proxy.fetch_async(
+            target_account_sid=target_account_sid,
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingBulkPortabilityInstance {}>".format(context)
+        return "<Twilio.Numbers.V1.PortingPortabilityInstance {}>".format(context)
 
 
-class PortingBulkPortabilityContext(InstanceContext):
+class PortingPortabilityContext(InstanceContext):
 
-    def __init__(self, version: Version, sid: str):
+    def __init__(self, version: Version, phone_number: str):
         """
-        Initialize the PortingBulkPortabilityContext
+        Initialize the PortingPortabilityContext
 
         :param version: Version that contains the resource
-        :param sid: A 34 character string that uniquely identifies the Portability check.
+        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "sid": sid,
+            "phone_number": phone_number,
         }
-        self._uri = "/Porting/Portability/{sid}".format(**self._solution)
+        self._uri = "/Porting/Portability/PhoneNumber/{phone_number}".format(
+            **self._solution
+        )
 
-    def fetch(self) -> PortingBulkPortabilityInstance:
+    def fetch(
+        self, target_account_sid: Union[str, object] = values.unset
+    ) -> PortingPortabilityInstance:
         """
-        Fetch the PortingBulkPortabilityInstance
+        Fetch the PortingPortabilityInstance
 
+        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingBulkPortabilityInstance
+        :returns: The fetched PortingPortabilityInstance
         """
 
-        payload = self._version.fetch(
-            method="GET",
-            uri=self._uri,
+        data = values.of(
+            {
+                "TargetAccountSid": target_account_sid,
+            }
         )
 
-        return PortingBulkPortabilityInstance(
+        payload = self._version.fetch(method="GET", uri=self._uri, params=data)
+
+        return PortingPortabilityInstance(
             self._version,
             payload,
-            sid=self._solution["sid"],
+            phone_number=self._solution["phone_number"],
         )
 
-    async def fetch_async(self) -> PortingBulkPortabilityInstance:
+    async def fetch_async(
+        self, target_account_sid: Union[str, object] = values.unset
+    ) -> PortingPortabilityInstance:
         """
-        Asynchronous coroutine to fetch the PortingBulkPortabilityInstance
+        Asynchronous coroutine to fetch the PortingPortabilityInstance
 
+        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingBulkPortabilityInstance
+        :returns: The fetched PortingPortabilityInstance
         """
 
+        data = values.of(
+            {
+                "TargetAccountSid": target_account_sid,
+            }
+        )
+
         payload = await self._version.fetch_async(
-            method="GET",
-            uri=self._uri,
+            method="GET", uri=self._uri, params=data
         )
 
-        return PortingBulkPortabilityInstance(
+        return PortingPortabilityInstance(
             self._version,
             payload,
-            sid=self._solution["sid"],
+            phone_number=self._solution["phone_number"],
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingBulkPortabilityContext {}>".format(context)
+        return "<Twilio.Numbers.V1.PortingPortabilityContext {}>".format(context)
 
 
-class PortingBulkPortabilityList(ListResource):
+class PortingPortabilityList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the PortingBulkPortabilityList
+        Initialize the PortingPortabilityList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Porting/Portability"
-
-    def create(self, phone_numbers: List[str]) -> PortingBulkPortabilityInstance:
-        """
-        Create the PortingBulkPortabilityInstance
-
-        :param phone_numbers: The phone numbers which portability is to be checked. This should be a list of strings. Phone numbers are in E.164 format (e.g. +16175551212). .
-
-        :returns: The created PortingBulkPortabilityInstance
-        """
-
-        data = values.of(
-            {
-                "PhoneNumbers": serialize.map(phone_numbers, lambda e: e),
-            }
-        )
-
-        payload = self._version.create(
-            method="POST",
-            uri=self._uri,
-            data=data,
-        )
-
-        return PortingBulkPortabilityInstance(self._version, payload)
-
-    async def create_async(
-        self, phone_numbers: List[str]
-    ) -> PortingBulkPortabilityInstance:
-        """
-        Asynchronously create the PortingBulkPortabilityInstance
-
-        :param phone_numbers: The phone numbers which portability is to be checked. This should be a list of strings. Phone numbers are in E.164 format (e.g. +16175551212). .
-
-        :returns: The created PortingBulkPortabilityInstance
-        """
-
-        data = values.of(
-            {
-                "PhoneNumbers": serialize.map(phone_numbers, lambda e: e),
-            }
-        )
-
-        payload = await self._version.create_async(
-            method="POST",
-            uri=self._uri,
-            data=data,
-        )
-
-        return PortingBulkPortabilityInstance(self._version, payload)
-
-    def get(self, sid: str) -> PortingBulkPortabilityContext:
+    def get(self, phone_number: str) -> PortingPortabilityContext:
         """
-        Constructs a PortingBulkPortabilityContext
+        Constructs a PortingPortabilityContext
 
-        :param sid: A 34 character string that uniquely identifies the Portability check.
+        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
         """
-        return PortingBulkPortabilityContext(self._version, sid=sid)
+        return PortingPortabilityContext(self._version, phone_number=phone_number)
 
-    def __call__(self, sid: str) -> PortingBulkPortabilityContext:
+    def __call__(self, phone_number: str) -> PortingPortabilityContext:
         """
-        Constructs a PortingBulkPortabilityContext
+        Constructs a PortingPortabilityContext
 
-        :param sid: A 34 character string that uniquely identifies the Portability check.
+        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
         """
-        return PortingBulkPortabilityContext(self._version, sid=sid)
+        return PortingPortabilityContext(self._version, phone_number=phone_number)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers.V1.PortingBulkPortabilityList>"
+        return "<Twilio.Numbers.V1.PortingPortabilityList>"
```

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/porting_port_in.py` & `twilio-9.1.0/twilio/rest/pricing/v1/voice/number.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,218 +1,192 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Numbers
+    Twilio - Pricing
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from typing import Any, Dict, Optional, Union
-from twilio.base import values
+from typing import Any, Dict, Optional
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class PortingPortInInstance(InstanceResource):
+class NumberInstance(InstanceResource):
     """
-    :ivar port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
-    :ivar url:
+    :ivar number: The phone number.
+    :ivar country: The name of the country.
+    :ivar iso_country: The [ISO country code](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
+    :ivar outbound_call_price:
+    :ivar inbound_call_price:
+    :ivar price_unit: The currency in which prices are measured, specified in [ISO 4127](http://www.iso.org/iso/home/standards/currency_codes.htm) format (e.g. `usd`, `eur`, `jpy`).
+    :ivar url: The absolute URL of the resource.
     """
 
     def __init__(
-        self,
-        version: Version,
-        payload: Dict[str, Any],
-        port_in_request_sid: Optional[str] = None,
+        self, version: Version, payload: Dict[str, Any], number: Optional[str] = None
     ):
         super().__init__(version)
 
-        self.port_in_request_sid: Optional[str] = payload.get("port_in_request_sid")
+        self.number: Optional[str] = payload.get("number")
+        self.country: Optional[str] = payload.get("country")
+        self.iso_country: Optional[str] = payload.get("iso_country")
+        self.outbound_call_price: Optional[str] = payload.get("outbound_call_price")
+        self.inbound_call_price: Optional[str] = payload.get("inbound_call_price")
+        self.price_unit: Optional[str] = payload.get("price_unit")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "port_in_request_sid": port_in_request_sid or self.port_in_request_sid,
+            "number": number or self.number,
         }
-        self._context: Optional[PortingPortInContext] = None
+        self._context: Optional[NumberContext] = None
 
     @property
-    def _proxy(self) -> "PortingPortInContext":
+    def _proxy(self) -> "NumberContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: PortingPortInContext for this PortingPortInInstance
+        :returns: NumberContext for this NumberInstance
         """
         if self._context is None:
-            self._context = PortingPortInContext(
+            self._context = NumberContext(
                 self._version,
-                port_in_request_sid=self._solution["port_in_request_sid"],
+                number=self._solution["number"],
             )
         return self._context
 
-    def delete(self) -> bool:
+    def fetch(self) -> "NumberInstance":
         """
-        Deletes the PortingPortInInstance
+        Fetch the NumberInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched NumberInstance
         """
-        return self._proxy.delete()
+        return self._proxy.fetch()
 
-    async def delete_async(self) -> bool:
+    async def fetch_async(self) -> "NumberInstance":
         """
-        Asynchronous coroutine that deletes the PortingPortInInstance
+        Asynchronous coroutine to fetch the NumberInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched NumberInstance
         """
-        return await self._proxy.delete_async()
+        return await self._proxy.fetch_async()
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortInInstance {}>".format(context)
+        return "<Twilio.Pricing.V1.NumberInstance {}>".format(context)
 
 
-class PortingPortInContext(InstanceContext):
+class NumberContext(InstanceContext):
 
-    def __init__(self, version: Version, port_in_request_sid: str):
+    def __init__(self, version: Version, number: str):
         """
-        Initialize the PortingPortInContext
+        Initialize the NumberContext
 
         :param version: Version that contains the resource
-        :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
+        :param number: The phone number to fetch.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "port_in_request_sid": port_in_request_sid,
+            "number": number,
         }
-        self._uri = "/Porting/PortIn/{port_in_request_sid}".format(**self._solution)
+        self._uri = "/Voice/Numbers/{number}".format(**self._solution)
 
-    def delete(self) -> bool:
+    def fetch(self) -> NumberInstance:
         """
-        Deletes the PortingPortInInstance
+        Fetch the NumberInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched NumberInstance
         """
-        return self._version.delete(
-            method="DELETE",
+
+        payload = self._version.fetch(
+            method="GET",
             uri=self._uri,
         )
 
-    async def delete_async(self) -> bool:
+        return NumberInstance(
+            self._version,
+            payload,
+            number=self._solution["number"],
+        )
+
+    async def fetch_async(self) -> NumberInstance:
         """
-        Asynchronous coroutine that deletes the PortingPortInInstance
+        Asynchronous coroutine to fetch the NumberInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched NumberInstance
         """
-        return await self._version.delete_async(
-            method="DELETE",
+
+        payload = await self._version.fetch_async(
+            method="GET",
             uri=self._uri,
         )
 
+        return NumberInstance(
+            self._version,
+            payload,
+            number=self._solution["number"],
+        )
+
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortInContext {}>".format(context)
+        return "<Twilio.Pricing.V1.NumberContext {}>".format(context)
 
 
-class PortingPortInList(ListResource):
+class NumberList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the PortingPortInList
+        Initialize the NumberList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Porting/PortIn"
-
-    def create(
-        self, body: Union[object, object] = values.unset
-    ) -> PortingPortInInstance:
+    def get(self, number: str) -> NumberContext:
         """
-        Create the PortingPortInInstance
+        Constructs a NumberContext
 
-        :param body:
-
-        :returns: The created PortingPortInInstance
+        :param number: The phone number to fetch.
         """
-        data = body.to_dict()
-
-        headers = {"Content-Type": "application/json"}
-
-        payload = self._version.create(
-            method="POST", uri=self._uri, data=data, headers=headers
-        )
+        return NumberContext(self._version, number=number)
 
-        return PortingPortInInstance(self._version, payload)
-
-    async def create_async(
-        self, body: Union[object, object] = values.unset
-    ) -> PortingPortInInstance:
+    def __call__(self, number: str) -> NumberContext:
         """
-        Asynchronously create the PortingPortInInstance
-
-        :param body:
+        Constructs a NumberContext
 
-        :returns: The created PortingPortInInstance
+        :param number: The phone number to fetch.
         """
-        data = body.to_dict()
-
-        headers = {"Content-Type": "application/json"}
-
-        payload = await self._version.create_async(
-            method="POST", uri=self._uri, data=data, headers=headers
-        )
-
-        return PortingPortInInstance(self._version, payload)
-
-    def get(self, port_in_request_sid: str) -> PortingPortInContext:
-        """
-        Constructs a PortingPortInContext
-
-        :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
-        """
-        return PortingPortInContext(
-            self._version, port_in_request_sid=port_in_request_sid
-        )
-
-    def __call__(self, port_in_request_sid: str) -> PortingPortInContext:
-        """
-        Constructs a PortingPortInContext
-
-        :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
-        """
-        return PortingPortInContext(
-            self._version, port_in_request_sid=port_in_request_sid
-        )
+        return NumberContext(self._version, number=number)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers.V1.PortingPortInList>"
+        return "<Twilio.Pricing.V1.NumberList>"
```

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/porting_port_in_fetch.py` & `twilio-9.1.0/twilio/rest/numbers/v1/porting_port_in.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from datetime import date
-from typing import Any, Dict, List, Optional
-from twilio.base import deserialize
+from typing import Any, Dict, List, Optional, Union
+from twilio.base import deserialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class PortingPortInFetchInstance(InstanceResource):
+class PortingPortInInstance(InstanceResource):
     """
     :ivar port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
     :ivar url: The URL of this Port In request
     :ivar account_sid: The Account SID that the numbers will be added to after they are ported into Twilio.
     :ivar notification_emails: List of emails for getting notifications about the LOA signing process. Allowed Max 10 emails.
     :ivar target_port_in_date: Minimum number of days in the future (at least 2 days) needs to be established with the Ops team for validation.
     :ivar target_port_in_time_range_start: Minimum hour in the future needs to be established with the Ops team for validation.
@@ -69,155 +69,239 @@
             "phone_numbers"
         )
         self.documents: Optional[List[str]] = payload.get("documents")
 
         self._solution = {
             "port_in_request_sid": port_in_request_sid or self.port_in_request_sid,
         }
-        self._context: Optional[PortingPortInFetchContext] = None
+        self._context: Optional[PortingPortInContext] = None
 
     @property
-    def _proxy(self) -> "PortingPortInFetchContext":
+    def _proxy(self) -> "PortingPortInContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: PortingPortInFetchContext for this PortingPortInFetchInstance
+        :returns: PortingPortInContext for this PortingPortInInstance
         """
         if self._context is None:
-            self._context = PortingPortInFetchContext(
+            self._context = PortingPortInContext(
                 self._version,
                 port_in_request_sid=self._solution["port_in_request_sid"],
             )
         return self._context
 
-    def fetch(self) -> "PortingPortInFetchInstance":
+    def delete(self) -> bool:
         """
-        Fetch the PortingPortInFetchInstance
+        Deletes the PortingPortInInstance
 
 
-        :returns: The fetched PortingPortInFetchInstance
+        :returns: True if delete succeeds, False otherwise
+        """
+        return self._proxy.delete()
+
+    async def delete_async(self) -> bool:
+        """
+        Asynchronous coroutine that deletes the PortingPortInInstance
+
+
+        :returns: True if delete succeeds, False otherwise
+        """
+        return await self._proxy.delete_async()
+
+    def fetch(self) -> "PortingPortInInstance":
+        """
+        Fetch the PortingPortInInstance
+
+
+        :returns: The fetched PortingPortInInstance
         """
         return self._proxy.fetch()
 
-    async def fetch_async(self) -> "PortingPortInFetchInstance":
+    async def fetch_async(self) -> "PortingPortInInstance":
         """
-        Asynchronous coroutine to fetch the PortingPortInFetchInstance
+        Asynchronous coroutine to fetch the PortingPortInInstance
 
 
-        :returns: The fetched PortingPortInFetchInstance
+        :returns: The fetched PortingPortInInstance
         """
         return await self._proxy.fetch_async()
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortInFetchInstance {}>".format(context)
+        return "<Twilio.Numbers.V1.PortingPortInInstance {}>".format(context)
 
 
-class PortingPortInFetchContext(InstanceContext):
+class PortingPortInContext(InstanceContext):
 
     def __init__(self, version: Version, port_in_request_sid: str):
         """
-        Initialize the PortingPortInFetchContext
+        Initialize the PortingPortInContext
 
         :param version: Version that contains the resource
         :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
             "port_in_request_sid": port_in_request_sid,
         }
         self._uri = "/Porting/PortIn/{port_in_request_sid}".format(**self._solution)
 
-    def fetch(self) -> PortingPortInFetchInstance:
+    def delete(self) -> bool:
+        """
+        Deletes the PortingPortInInstance
+
+
+        :returns: True if delete succeeds, False otherwise
+        """
+        return self._version.delete(
+            method="DELETE",
+            uri=self._uri,
+        )
+
+    async def delete_async(self) -> bool:
         """
-        Fetch the PortingPortInFetchInstance
+        Asynchronous coroutine that deletes the PortingPortInInstance
 
 
-        :returns: The fetched PortingPortInFetchInstance
+        :returns: True if delete succeeds, False otherwise
+        """
+        return await self._version.delete_async(
+            method="DELETE",
+            uri=self._uri,
+        )
+
+    def fetch(self) -> PortingPortInInstance:
+        """
+        Fetch the PortingPortInInstance
+
+
+        :returns: The fetched PortingPortInInstance
         """
 
         payload = self._version.fetch(
             method="GET",
             uri=self._uri,
         )
 
-        return PortingPortInFetchInstance(
+        return PortingPortInInstance(
             self._version,
             payload,
             port_in_request_sid=self._solution["port_in_request_sid"],
         )
 
-    async def fetch_async(self) -> PortingPortInFetchInstance:
+    async def fetch_async(self) -> PortingPortInInstance:
         """
-        Asynchronous coroutine to fetch the PortingPortInFetchInstance
+        Asynchronous coroutine to fetch the PortingPortInInstance
 
 
-        :returns: The fetched PortingPortInFetchInstance
+        :returns: The fetched PortingPortInInstance
         """
 
         payload = await self._version.fetch_async(
             method="GET",
             uri=self._uri,
         )
 
-        return PortingPortInFetchInstance(
+        return PortingPortInInstance(
             self._version,
             payload,
             port_in_request_sid=self._solution["port_in_request_sid"],
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortInFetchContext {}>".format(context)
+        return "<Twilio.Numbers.V1.PortingPortInContext {}>".format(context)
 
 
-class PortingPortInFetchList(ListResource):
+class PortingPortInList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the PortingPortInFetchList
+        Initialize the PortingPortInList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-    def get(self, port_in_request_sid: str) -> PortingPortInFetchContext:
+        self._uri = "/Porting/PortIn"
+
+    def create(
+        self, body: Union[object, object] = values.unset
+    ) -> PortingPortInInstance:
+        """
+        Create the PortingPortInInstance
+
+        :param body:
+
+        :returns: The created PortingPortInInstance
+        """
+        data = body.to_dict()
+
+        headers = {"Content-Type": "application/json"}
+
+        payload = self._version.create(
+            method="POST", uri=self._uri, data=data, headers=headers
+        )
+
+        return PortingPortInInstance(self._version, payload)
+
+    async def create_async(
+        self, body: Union[object, object] = values.unset
+    ) -> PortingPortInInstance:
+        """
+        Asynchronously create the PortingPortInInstance
+
+        :param body:
+
+        :returns: The created PortingPortInInstance
+        """
+        data = body.to_dict()
+
+        headers = {"Content-Type": "application/json"}
+
+        payload = await self._version.create_async(
+            method="POST", uri=self._uri, data=data, headers=headers
+        )
+
+        return PortingPortInInstance(self._version, payload)
+
+    def get(self, port_in_request_sid: str) -> PortingPortInContext:
         """
-        Constructs a PortingPortInFetchContext
+        Constructs a PortingPortInContext
 
         :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
         """
-        return PortingPortInFetchContext(
+        return PortingPortInContext(
             self._version, port_in_request_sid=port_in_request_sid
         )
 
-    def __call__(self, port_in_request_sid: str) -> PortingPortInFetchContext:
+    def __call__(self, port_in_request_sid: str) -> PortingPortInContext:
         """
-        Constructs a PortingPortInFetchContext
+        Constructs a PortingPortInContext
 
         :param port_in_request_sid: The SID of the Port In request. This is a unique identifier of the port in request.
         """
-        return PortingPortInFetchContext(
+        return PortingPortInContext(
             self._version, port_in_request_sid=port_in_request_sid
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers.V1.PortingPortInFetchList>"
+        return "<Twilio.Numbers.V1.PortingPortInList>"
```

### Comparing `twilio-9.0.5/twilio/rest/numbers/v1/porting_portability.py` & `twilio-9.1.0/twilio/rest/verify/v2/safelist.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,243 +1,278 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Numbers
+    Twilio - Verify
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from typing import Any, Dict, Optional, Union
-from twilio.base import deserialize, values
+from typing import Any, Dict, Optional
+from twilio.base import values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class PortingPortabilityInstance(InstanceResource):
-
-    class NumberType(object):
-        LOCAL = "LOCAL"
-        UNKNOWN = "UNKNOWN"
-        MOBILE = "MOBILE"
-        TOLL_FREE = "TOLL-FREE"
-
+class SafelistInstance(InstanceResource):
     """
-    :ivar phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
-    :ivar account_sid: The target account sid to which the number will be ported
-    :ivar portable: Boolean flag specifying if phone number is portable or not.
-    :ivar pin_and_account_number_required: Boolean flag specifying if PIN and account number is required for the phone number.
-    :ivar not_portable_reason: Reason why the phone number cannot be ported into Twilio, `null` otherwise.
-    :ivar not_portable_reason_code: The Portability Reason Code for the phone number if it cannot be ported into Twilio, `null` otherwise. One of `22131`, `22132`, `22130`, `22133`, `22102` or `22135`.
-    :ivar number_type: 
-    :ivar country: Country the phone number belongs to.
-    :ivar messaging_carrier: Current messaging carrier of the phone number
-    :ivar voice_carrier: Current voice carrier of the phone number
-    :ivar url: This is the url of the request that you're trying to reach out to locate the resource.
+    :ivar sid: The unique string that we created to identify the SafeList resource.
+    :ivar phone_number: The phone number in SafeList.
+    :ivar url: The absolute URL of the SafeList resource.
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
         phone_number: Optional[str] = None,
     ):
         super().__init__(version)
 
+        self.sid: Optional[str] = payload.get("sid")
         self.phone_number: Optional[str] = payload.get("phone_number")
-        self.account_sid: Optional[str] = payload.get("account_sid")
-        self.portable: Optional[bool] = payload.get("portable")
-        self.pin_and_account_number_required: Optional[bool] = payload.get(
-            "pin_and_account_number_required"
-        )
-        self.not_portable_reason: Optional[str] = payload.get("not_portable_reason")
-        self.not_portable_reason_code: Optional[int] = deserialize.integer(
-            payload.get("not_portable_reason_code")
-        )
-        self.number_type: Optional["PortingPortabilityInstance.NumberType"] = (
-            payload.get("number_type")
-        )
-        self.country: Optional[str] = payload.get("country")
-        self.messaging_carrier: Optional[str] = payload.get("messaging_carrier")
-        self.voice_carrier: Optional[str] = payload.get("voice_carrier")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
             "phone_number": phone_number or self.phone_number,
         }
-        self._context: Optional[PortingPortabilityContext] = None
+        self._context: Optional[SafelistContext] = None
 
     @property
-    def _proxy(self) -> "PortingPortabilityContext":
+    def _proxy(self) -> "SafelistContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: PortingPortabilityContext for this PortingPortabilityInstance
+        :returns: SafelistContext for this SafelistInstance
         """
         if self._context is None:
-            self._context = PortingPortabilityContext(
+            self._context = SafelistContext(
                 self._version,
                 phone_number=self._solution["phone_number"],
             )
         return self._context
 
-    def fetch(
-        self, target_account_sid: Union[str, object] = values.unset
-    ) -> "PortingPortabilityInstance":
+    def delete(self) -> bool:
         """
-        Fetch the PortingPortabilityInstance
+        Deletes the SafelistInstance
 
-        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingPortabilityInstance
+        :returns: True if delete succeeds, False otherwise
         """
-        return self._proxy.fetch(
-            target_account_sid=target_account_sid,
-        )
+        return self._proxy.delete()
 
-    async def fetch_async(
-        self, target_account_sid: Union[str, object] = values.unset
-    ) -> "PortingPortabilityInstance":
+    async def delete_async(self) -> bool:
         """
-        Asynchronous coroutine to fetch the PortingPortabilityInstance
+        Asynchronous coroutine that deletes the SafelistInstance
 
-        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingPortabilityInstance
+        :returns: True if delete succeeds, False otherwise
         """
-        return await self._proxy.fetch_async(
-            target_account_sid=target_account_sid,
-        )
+        return await self._proxy.delete_async()
+
+    def fetch(self) -> "SafelistInstance":
+        """
+        Fetch the SafelistInstance
+
+
+        :returns: The fetched SafelistInstance
+        """
+        return self._proxy.fetch()
+
+    async def fetch_async(self) -> "SafelistInstance":
+        """
+        Asynchronous coroutine to fetch the SafelistInstance
+
+
+        :returns: The fetched SafelistInstance
+        """
+        return await self._proxy.fetch_async()
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortabilityInstance {}>".format(context)
+        return "<Twilio.Verify.V2.SafelistInstance {}>".format(context)
 
 
-class PortingPortabilityContext(InstanceContext):
+class SafelistContext(InstanceContext):
 
     def __init__(self, version: Version, phone_number: str):
         """
-        Initialize the PortingPortabilityContext
+        Initialize the SafelistContext
 
         :param version: Version that contains the resource
-        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
+        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
             "phone_number": phone_number,
         }
-        self._uri = "/Porting/Portability/PhoneNumber/{phone_number}".format(
-            **self._solution
-        )
+        self._uri = "/SafeList/Numbers/{phone_number}".format(**self._solution)
 
-    def fetch(
-        self, target_account_sid: Union[str, object] = values.unset
-    ) -> PortingPortabilityInstance:
+    def delete(self) -> bool:
         """
-        Fetch the PortingPortabilityInstance
+        Deletes the SafelistInstance
 
-        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingPortabilityInstance
+        :returns: True if delete succeeds, False otherwise
         """
+        return self._version.delete(
+            method="DELETE",
+            uri=self._uri,
+        )
 
-        data = values.of(
-            {
-                "TargetAccountSid": target_account_sid,
-            }
+    async def delete_async(self) -> bool:
+        """
+        Asynchronous coroutine that deletes the SafelistInstance
+
+
+        :returns: True if delete succeeds, False otherwise
+        """
+        return await self._version.delete_async(
+            method="DELETE",
+            uri=self._uri,
         )
 
-        payload = self._version.fetch(method="GET", uri=self._uri, params=data)
+    def fetch(self) -> SafelistInstance:
+        """
+        Fetch the SafelistInstance
 
-        return PortingPortabilityInstance(
+
+        :returns: The fetched SafelistInstance
+        """
+
+        payload = self._version.fetch(
+            method="GET",
+            uri=self._uri,
+        )
+
+        return SafelistInstance(
             self._version,
             payload,
             phone_number=self._solution["phone_number"],
         )
 
-    async def fetch_async(
-        self, target_account_sid: Union[str, object] = values.unset
-    ) -> PortingPortabilityInstance:
+    async def fetch_async(self) -> SafelistInstance:
         """
-        Asynchronous coroutine to fetch the PortingPortabilityInstance
+        Asynchronous coroutine to fetch the SafelistInstance
 
-        :param target_account_sid: The SID of the account where the phone number(s) will be ported.
 
-        :returns: The fetched PortingPortabilityInstance
+        :returns: The fetched SafelistInstance
         """
 
-        data = values.of(
-            {
-                "TargetAccountSid": target_account_sid,
-            }
-        )
-
         payload = await self._version.fetch_async(
-            method="GET", uri=self._uri, params=data
+            method="GET",
+            uri=self._uri,
         )
 
-        return PortingPortabilityInstance(
+        return SafelistInstance(
             self._version,
             payload,
             phone_number=self._solution["phone_number"],
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Numbers.V1.PortingPortabilityContext {}>".format(context)
+        return "<Twilio.Verify.V2.SafelistContext {}>".format(context)
 
 
-class PortingPortabilityList(ListResource):
+class SafelistList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the PortingPortabilityList
+        Initialize the SafelistList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-    def get(self, phone_number: str) -> PortingPortabilityContext:
+        self._uri = "/SafeList/Numbers"
+
+    def create(self, phone_number: str) -> SafelistInstance:
+        """
+        Create the SafelistInstance
+
+        :param phone_number: The phone number to be added in SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
+
+        :returns: The created SafelistInstance
+        """
+
+        data = values.of(
+            {
+                "PhoneNumber": phone_number,
+            }
+        )
+
+        payload = self._version.create(
+            method="POST",
+            uri=self._uri,
+            data=data,
+        )
+
+        return SafelistInstance(self._version, payload)
+
+    async def create_async(self, phone_number: str) -> SafelistInstance:
+        """
+        Asynchronously create the SafelistInstance
+
+        :param phone_number: The phone number to be added in SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
+
+        :returns: The created SafelistInstance
+        """
+
+        data = values.of(
+            {
+                "PhoneNumber": phone_number,
+            }
+        )
+
+        payload = await self._version.create_async(
+            method="POST",
+            uri=self._uri,
+            data=data,
+        )
+
+        return SafelistInstance(self._version, payload)
+
+    def get(self, phone_number: str) -> SafelistContext:
         """
-        Constructs a PortingPortabilityContext
+        Constructs a SafelistContext
 
-        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
+        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
-        return PortingPortabilityContext(self._version, phone_number=phone_number)
+        return SafelistContext(self._version, phone_number=phone_number)
 
-    def __call__(self, phone_number: str) -> PortingPortabilityContext:
+    def __call__(self, phone_number: str) -> SafelistContext:
         """
-        Constructs a PortingPortabilityContext
+        Constructs a SafelistContext
 
-        :param phone_number: The phone number which portability is to be checked. Phone numbers are in E.164 format (e.g. +16175551212).
+        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
-        return PortingPortabilityContext(self._version, phone_number=phone_number)
+        return SafelistContext(self._version, phone_number=phone_number)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Numbers.V1.PortingPortabilityList>"
+        return "<Twilio.Verify.V2.SafelistList>"
```

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/__init__.py` & `twilio-9.1.0/twilio/rest/numbers/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/authorization_document/__init__.py` & `twilio-9.1.0/twilio/rest/numbers/v2/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py` & `twilio-9.1.0/twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/bulk_hosted_number_order.py` & `twilio-9.1.0/twilio/rest/numbers/v2/bulk_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/hosted_number_order.py` & `twilio-9.1.0/twilio/rest/numbers/v2/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/__init__.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/bundle_copy.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/evaluation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/item_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/bundle/replace_items.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/end_user.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/regulation.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/regulation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py` & `twilio-9.1.0/twilio/rest/numbers/v2/regulatory_compliance/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/oauth/OauthBase.py` & `twilio-9.1.0/twilio/rest/oauth/OauthBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/oauth/__init__.py` & `twilio-9.1.0/twilio/rest/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/oauth/v1/__init__.py` & `twilio-9.1.0/twilio/rest/oauth/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/oauth/v1/authorize.py` & `twilio-9.1.0/twilio/rest/oauth/v1/authorize.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/oauth/v1/token.py` & `twilio-9.1.0/twilio/rest/oauth/v1/token.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/PreviewBase.py` & `twilio-9.1.0/twilio/rest/preview/PreviewBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/__init__.py` & `twilio-9.1.0/twilio/rest/preview/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/__init__.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/__init__.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/certificate.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/certificate.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/deployment.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/device.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/device.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/deployed_devices/fleet/key.py` & `twilio-9.1.0/twilio/rest/preview/deployed_devices/fleet/key.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/hosted_numbers/__init__.py` & `twilio-9.1.0/twilio/rest/preview/hosted_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py` & `twilio-9.1.0/twilio/rest/preview/hosted_numbers/authorization_document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py` & `twilio-9.1.0/twilio/rest/preview/hosted_numbers/authorization_document/dependent_hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/hosted_numbers/hosted_number_order.py` & `twilio-9.1.0/twilio/rest/preview/hosted_numbers/hosted_number_order.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/marketplace/__init__.py` & `twilio-9.1.0/twilio/rest/preview/marketplace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/marketplace/available_add_on/__init__.py` & `twilio-9.1.0/twilio/rest/preview/marketplace/available_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py` & `twilio-9.1.0/twilio/rest/preview/marketplace/available_add_on/available_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/marketplace/installed_add_on/__init__.py` & `twilio-9.1.0/twilio/rest/preview/marketplace/installed_add_on/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py` & `twilio-9.1.0/twilio/rest/preview/marketplace/installed_add_on/installed_add_on_extension.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/__init__.py` & `twilio-9.1.0/twilio/rest/preview/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/__init__.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/document/__init__.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/document/document_permission.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/__init__.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/sync_list_item.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/__init__.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/sync_map_item.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py` & `twilio-9.1.0/twilio/rest/preview/sync/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/wireless/__init__.py` & `twilio-9.1.0/twilio/rest/preview/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/wireless/command.py` & `twilio-9.1.0/twilio/rest/preview/wireless/command.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/wireless/rate_plan.py` & `twilio-9.1.0/twilio/rest/preview/wireless/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/wireless/sim/__init__.py` & `twilio-9.1.0/twilio/rest/preview/wireless/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview/wireless/sim/usage.py` & `twilio-9.1.0/twilio/rest/preview/wireless/sim/usage.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/preview_messaging/PreviewMessagingBase.py` & `twilio-9.1.0/twilio/rest/sync/SyncBase.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,36 +9,36 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.preview_messaging.v1 import V1
+from twilio.rest.sync.v1 import V1
 
 
-class PreviewMessagingBase(Domain):
+class SyncBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the PreviewMessaging Domain
+        Initialize the Sync Domain
 
-        :returns: Domain for PreviewMessaging
+        :returns: Domain for Sync
         """
-        super().__init__(twilio, "https://preview.messaging.twilio.com")
+        super().__init__(twilio, "https://sync.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of PreviewMessaging
+        :returns: Versions v1 of Sync
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.PreviewMessaging>"
+        return "<Twilio.Sync>"
```

### Comparing `twilio-9.0.5/twilio/rest/preview_messaging/v1/broadcast.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow_validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,125 +1,137 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Bulk Messaging and Broadcast
-    Bulk Sending is a public Twilio REST API for 1:Many Message creation up to 100 recipients. Broadcast is a public Twilio REST API for 1:Many Message creation up to 10,000 recipients via file upload.
+    Twilio - Studio
+    This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from datetime import datetime
 from typing import Any, Dict, Optional, Union
-from twilio.base import deserialize, values
+from twilio.base import serialize, values
 
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class BroadcastInstance(InstanceResource):
+class FlowValidateInstance(InstanceResource):
+
+    class Status(object):
+        DRAFT = "draft"
+        PUBLISHED = "published"
+
     """
-    :ivar broadcast_sid: Numeric ID indentifying individual Broadcast requests
-    :ivar created_date: Timestamp of when the Broadcast was created
-    :ivar updated_date: Timestamp of when the Broadcast was last updated
-    :ivar broadcast_status: Status of the Broadcast request. Valid values are None, Pending-Upload, Uploaded, Queued, Executing, Execution-Failure, Execution-Completed, Cancelation-Requested, and Canceled
-    :ivar execution_details:
-    :ivar results_file: Path to a file detailing successful requests and errors from Broadcast execution
+    :ivar valid: Boolean if the flow definition is valid.
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
-        self.broadcast_sid: Optional[str] = payload.get("broadcast_sid")
-        self.created_date: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("created_date")
-        )
-        self.updated_date: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("updated_date")
-        )
-        self.broadcast_status: Optional[str] = payload.get("broadcast_status")
-        self.execution_details: Optional[str] = payload.get("execution_details")
-        self.results_file: Optional[str] = payload.get("results_file")
+        self.valid: Optional[bool] = payload.get("valid")
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
 
-        return "<Twilio.PreviewMessaging.V1.BroadcastInstance>"
+        return "<Twilio.Studio.V2.FlowValidateInstance>"
 
 
-class BroadcastList(ListResource):
+class FlowValidateList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the BroadcastList
+        Initialize the FlowValidateList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Broadcasts"
+        self._uri = "/Flows/Validate"
 
-    def create(
-        self, x_twilio_request_key: Union[str, object] = values.unset
-    ) -> BroadcastInstance:
+    def update(
+        self,
+        friendly_name: str,
+        status: "FlowValidateInstance.Status",
+        definition: object,
+        commit_message: Union[str, object] = values.unset,
+    ) -> FlowValidateInstance:
         """
-        Create the BroadcastInstance
+        Update the FlowValidateInstance
 
-        :param x_twilio_request_key: Idempotency key provided by the client
+        :param friendly_name: The string that you assigned to describe the Flow.
+        :param status:
+        :param definition: JSON representation of flow definition.
+        :param commit_message: Description of change made in the revision.
 
-        :returns: The created BroadcastInstance
+        :returns: The created FlowValidateInstance
         """
 
-        data = values.of({})
-        headers = values.of(
+        data = values.of(
             {
-                "X-Twilio-Request-Key": x_twilio_request_key,
+                "FriendlyName": friendly_name,
+                "Status": status,
+                "Definition": serialize.object(definition),
+                "CommitMessage": commit_message,
             }
         )
 
-        payload = self._version.create(
-            method="POST", uri=self._uri, data=data, headers=headers
+        payload = self._version.update(
+            method="POST",
+            uri=self._uri,
+            data=data,
         )
 
-        return BroadcastInstance(self._version, payload)
+        return FlowValidateInstance(self._version, payload)
 
-    async def create_async(
-        self, x_twilio_request_key: Union[str, object] = values.unset
-    ) -> BroadcastInstance:
+    async def update_async(
+        self,
+        friendly_name: str,
+        status: "FlowValidateInstance.Status",
+        definition: object,
+        commit_message: Union[str, object] = values.unset,
+    ) -> FlowValidateInstance:
         """
-        Asynchronously create the BroadcastInstance
+        Asynchronously update the FlowValidateInstance
 
-        :param x_twilio_request_key: Idempotency key provided by the client
+        :param friendly_name: The string that you assigned to describe the Flow.
+        :param status:
+        :param definition: JSON representation of flow definition.
+        :param commit_message: Description of change made in the revision.
 
-        :returns: The created BroadcastInstance
+        :returns: The created FlowValidateInstance
         """
 
-        data = values.of({})
-        headers = values.of(
+        data = values.of(
             {
-                "X-Twilio-Request-Key": x_twilio_request_key,
+                "FriendlyName": friendly_name,
+                "Status": status,
+                "Definition": serialize.object(definition),
+                "CommitMessage": commit_message,
             }
         )
 
-        payload = await self._version.create_async(
-            method="POST", uri=self._uri, data=data, headers=headers
+        payload = await self._version.update_async(
+            method="POST",
+            uri=self._uri,
+            data=data,
         )
 
-        return BroadcastInstance(self._version, payload)
+        return FlowValidateInstance(self._version, payload)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.PreviewMessaging.V1.BroadcastList>"
+        return "<Twilio.Studio.V2.FlowValidateList>"
```

### Comparing `twilio-9.0.5/twilio/rest/preview_messaging/v1/message.py` & `twilio-9.1.0/twilio/rest/supersim/v1/sim/billing_period.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,204 +1,306 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Bulk Messaging and Broadcast
-    Bulk Sending is a public Twilio REST API for 1:Many Message creation up to 100 recipients. Broadcast is a public Twilio REST API for 1:Many Message creation up to 10,000 recipients via file upload.
+    Twilio - Supersim
+    This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from typing import Any, Dict, List, Optional
-from twilio.base import deserialize
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
+from twilio.base import deserialize, values
 
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
+from twilio.base.page import Page
 
 
-class MessageInstance(InstanceResource):
+class BillingPeriodInstance(InstanceResource):
+
+    class BpType(object):
+        READY = "ready"
+        ACTIVE = "active"
+
     """
-    :ivar total_message_count: The number of Messages processed in the request, equal to the sum of success_count and error_count.
-    :ivar success_count: The number of Messages successfully created.
-    :ivar error_count: The number of Messages unsuccessfully processed in the request.
-    :ivar message_receipts:
-    :ivar failed_message_receipts:
+    :ivar sid: The SID of the Billing Period.
+    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) the Super SIM belongs to.
+    :ivar sim_sid: The SID of the Super SIM the Billing Period belongs to.
+    :ivar start_time: The start time of the Billing Period specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    :ivar end_time: The end time of the Billing Period specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    :ivar period_type: 
+    :ivar date_created: The date and time in GMT when the resource was created specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    :ivar date_updated: The date and time in GMT when the resource was last updated specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     """
 
-    def __init__(self, version: Version, payload: Dict[str, Any]):
+    def __init__(self, version: Version, payload: Dict[str, Any], sim_sid: str):
         super().__init__(version)
 
-        self.total_message_count: Optional[int] = deserialize.integer(
-            payload.get("total_message_count")
+        self.sid: Optional[str] = payload.get("sid")
+        self.account_sid: Optional[str] = payload.get("account_sid")
+        self.sim_sid: Optional[str] = payload.get("sim_sid")
+        self.start_time: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("start_time")
         )
-        self.success_count: Optional[int] = deserialize.integer(
-            payload.get("success_count")
+        self.end_time: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("end_time")
         )
-        self.error_count: Optional[int] = deserialize.integer(
-            payload.get("error_count")
+        self.period_type: Optional["BillingPeriodInstance.BpType"] = payload.get(
+            "period_type"
         )
-        self.message_receipts: Optional[List[str]] = payload.get("message_receipts")
-        self.failed_message_receipts: Optional[List[str]] = payload.get(
-            "failed_message_receipts"
+        self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("date_created")
         )
+        self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("date_updated")
+        )
+
+        self._solution = {
+            "sim_sid": sim_sid,
+        }
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
+        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
+        return "<Twilio.Supersim.V1.BillingPeriodInstance {}>".format(context)
 
-        return "<Twilio.PreviewMessaging.V1.MessageInstance>"
 
+class BillingPeriodPage(Page):
 
-class MessageList(ListResource):
-
-    class CreateMessagesRequest(object):
-        """
-        :ivar messages:
-        :ivar from_: A Twilio phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format, an [alphanumeric sender ID](https://www.twilio.com/docs/sms/send-messages#use-an-alphanumeric-sender-id), or a [Channel Endpoint address](https://www.twilio.com/docs/sms/channels#channel-addresses) that is enabled for the type of message you want to send. Phone numbers or [short codes](https://www.twilio.com/docs/sms/api/short-code) purchased from Twilio also work here. You cannot, for example, spoof messages from a private cell phone number. If you are using `messaging_service_sid`, this parameter must be empty.
-        :ivar messaging_service_sid: The SID of the [Messaging Service](https://www.twilio.com/docs/sms/services#send-a-message-with-copilot) you want to associate with the Message. Set this parameter to use the [Messaging Service Settings and Copilot Features](https://www.twilio.com/console/sms/services) you have configured and leave the `from` parameter empty. When only this parameter is set, Twilio will use your enabled Copilot Features to select the `from` phone number for delivery.
-        :ivar body: The text of the message you want to send. Can be up to 1,600 characters in length.
-        :ivar content_sid: The SID of the preconfigured [Content Template](https://www.twilio.com/docs/content-api/create-and-send-your-first-content-api-template#create-a-template) you want to associate with the Message. Must be used in conjuction with a preconfigured [Messaging Service Settings and Copilot Features](https://www.twilio.com/console/sms/services) When this parameter is set, Twilio will use your configured content template and the provided `ContentVariables`. This Twilio product is currently in Private Beta.
-        :ivar media_url: The URL of the media to send with the message. The media can be of type `gif`, `png`, and `jpeg` and will be formatted correctly on the recipient's device. The media size limit is 5MB for supported file types (JPEG, PNG, GIF) and 500KB for [other types](https://www.twilio.com/docs/sms/accepted-mime-types) of accepted media. To send more than one image in the message body, provide multiple `media_url` parameters in the POST request. You can include up to 10 `media_url` parameters per message. You can send images in an SMS message in only the US and Canada.
-        :ivar status_callback: The URL we should call using the \"status_callback_method\" to send status information to your application. If specified, we POST these message status changes to the URL - queued, failed, sent, delivered, or undelivered. Twilio will POST its [standard request parameters](https://www.twilio.com/docs/messaging/twiml#request-parameters) as well as some additional parameters including \"MessageSid\", \"MessageStatus\", and \"ErrorCode\". If you include this parameter with the \"messaging_service_sid\", we use this URL instead of the Status Callback URL of the [Messaging Service](https://www.twilio.com/docs/messaging/services/api). URLs must contain a valid hostname and underscores are not allowed.
-        :ivar validity_period: How long in seconds the message can remain in our outgoing message queue. After this period elapses, the message fails and we call your status callback. Can be between 1 and the default value of 14,400 seconds. After a message has been accepted by a carrier, however, we cannot guarantee that the message will not be queued after this period. We recommend that this value be at least 5 seconds.
-        :ivar send_at: The time at which Twilio will send the message. This parameter can be used to schedule a message to be sent at a particular time. Must be in ISO 8601 format.
-        :ivar schedule_type: This parameter indicates your intent to schedule a message. Pass the value `fixed` to schedule a message at a fixed time. This parameter works in conjuction with the `SendAt` parameter.
-        :ivar shorten_urls: Determines the usage of Click Tracking. Setting it to `true` will instruct Twilio to replace all links in the Message with a shortened version based on the associated Domain Sid and track clicks on them. If this parameter is not set on an API call, we will use the value set on the Messaging Service. If this parameter is not set and the value is not configured on the Messaging Service used this will default to `false`.
-        :ivar send_as_mms: If set to True, Twilio will deliver the message as a single MMS message, regardless of the presence of media.
-        :ivar max_price: The maximum total price in US dollars that you will pay for the message to be delivered. Can be a decimal value that has up to 4 decimal places. All messages are queued for delivery and the message cost is checked before the message is sent. If the cost exceeds max_price, the message will fail and a status of Failed is sent to the status callback. If MaxPrice is not set, the message cost is not checked.
-        :ivar attempt: Total number of attempts made ( including this ) to send out the message regardless of the provider used
-        :ivar smart_encoded: This parameter indicates whether to detect Unicode characters that have a similar GSM-7 character and replace them. Can be true or false.
-        :ivar force_delivery: This parameter allows Twilio to send SMS traffic to carriers without checking/caring whether the destination number is a mobile or a landline.
-        :ivar application_sid: The SID of the application that should receive message status. We POST a message_sid parameter and a message_status parameter with a value of sent or failed to the application's message_status_callback. If a status_callback parameter is also passed, it will be ignored and the application's message_status_callback parameter will be used.
+    def get_instance(self, payload: Dict[str, Any]) -> BillingPeriodInstance:
         """
+        Build an instance of BillingPeriodInstance
 
-        def __init__(self, payload: Dict[str, Any]):
-
-            self.messages: Optional[List[MessageList.MessagingV1Message]] = payload.get(
-                "messages"
-            )
-            self.from_: Optional[str] = payload.get("from_")
-            self.messaging_service_sid: Optional[str] = payload.get(
-                "messaging_service_sid"
-            )
-            self.body: Optional[str] = payload.get("body")
-            self.content_sid: Optional[str] = payload.get("content_sid")
-            self.media_url: Optional[List[str]] = payload.get("media_url")
-            self.status_callback: Optional[str] = payload.get("status_callback")
-            self.validity_period: Optional[int] = payload.get("validity_period")
-            self.send_at: Optional[str] = payload.get("send_at")
-            self.schedule_type: Optional[str] = payload.get("schedule_type")
-            self.shorten_urls: Optional[bool] = payload.get("shorten_urls")
-            self.send_as_mms: Optional[bool] = payload.get("send_as_mms")
-            self.max_price: Optional[float] = payload.get("max_price")
-            self.attempt: Optional[int] = payload.get("attempt")
-            self.smart_encoded: Optional[bool] = payload.get("smart_encoded")
-            self.force_delivery: Optional[bool] = payload.get("force_delivery")
-            self.application_sid: Optional[str] = payload.get("application_sid")
-
-        def to_dict(self):
-            return {
-                "messages": [messages.to_dict() for messages in self.messages],
-                "from": self.from_,
-                "messaging_service_sid": self.messaging_service_sid,
-                "body": self.body,
-                "content_sid": self.content_sid,
-                "media_url": self.media_url,
-                "status_callback": self.status_callback,
-                "validity_period": self.validity_period,
-                "send_at": self.send_at,
-                "schedule_type": self.schedule_type,
-                "shorten_urls": self.shorten_urls,
-                "send_as_mms": self.send_as_mms,
-                "max_price": self.max_price,
-                "attempt": self.attempt,
-                "smart_encoded": self.smart_encoded,
-                "force_delivery": self.force_delivery,
-                "application_sid": self.application_sid,
-            }
-
-    class MessagingV1Message(object):
+        :param payload: Payload response from the API
         """
-        :ivar to: The destination phone number in [E.164](https://www.twilio.com/docs/glossary/what-e164) format for SMS/MMS or [Channel user address](https://www.twilio.com/docs/sms/channels#channel-addresses) for other 3rd-party channels.
-        :ivar body: The text of the message you want to send. Can be up to 1,600 characters in length. Overrides the request-level body and content template if provided.
-        :ivar content_variables: Key-value pairs of variable names to substitution values. Refer to the [Twilio Content API Resources](https://www.twilio.com/docs/content-api/content-api-resources#send-a-message-with-preconfigured-content) for more details.
+        return BillingPeriodInstance(
+            self._version, payload, sim_sid=self._solution["sim_sid"]
+        )
+
+    def __repr__(self) -> str:
         """
+        Provide a friendly representation
 
-        def __init__(self, payload: Dict[str, Any]):
+        :returns: Machine friendly representation
+        """
+        return "<Twilio.Supersim.V1.BillingPeriodPage>"
 
-            self.to: Optional[str] = payload.get("to")
-            self.body: Optional[str] = payload.get("body")
-            self.content_variables: Optional[dict[str, str]] = payload.get(
-                "content_variables"
-            )
 
-        def to_dict(self):
-            return {
-                "to": self.to,
-                "body": self.body,
-                "content_variables": self.content_variables,
-            }
+class BillingPeriodList(ListResource):
 
-    def __init__(self, version: Version):
+    def __init__(self, version: Version, sim_sid: str):
         """
-        Initialize the MessageList
+        Initialize the BillingPeriodList
 
         :param version: Version that contains the resource
+        :param sim_sid: The SID of the Super SIM to list Billing Periods for.
 
         """
         super().__init__(version)
 
-        self._uri = "/Messages"
-
-    def create(self, create_messages_request: CreateMessagesRequest) -> MessageInstance:
-        """
-        Create the MessageInstance
+        # Path Solution
+        self._solution = {
+            "sim_sid": sim_sid,
+        }
+        self._uri = "/Sims/{sim_sid}/BillingPeriods".format(**self._solution)
+
+    def stream(
+        self,
+        limit: Optional[int] = None,
+        page_size: Optional[int] = None,
+    ) -> Iterator[BillingPeriodInstance]:
+        """
+        Streams BillingPeriodInstance records from the API as a generator stream.
+        This operation lazily loads records as efficiently as possible until the limit
+        is reached.
+        The results are returned as a generator, so this operation is memory efficient.
+
+        :param limit: Upper limit for the number of records to return. stream()
+                      guarantees to never return more than limit.  Default is no limit
+        :param page_size: Number of records to fetch per request, when not set will use
+                          the default value of 50 records.  If no page_size is defined
+                          but a limit is defined, stream() will attempt to read the
+                          limit with the most efficient page size, i.e. min(limit, 1000)
+
+        :returns: Generator that will yield up to limit results
+        """
+        limits = self._version.read_limits(limit, page_size)
+        page = self.page(page_size=limits["page_size"])
+
+        return self._version.stream(page, limits["limit"])
+
+    async def stream_async(
+        self,
+        limit: Optional[int] = None,
+        page_size: Optional[int] = None,
+    ) -> AsyncIterator[BillingPeriodInstance]:
+        """
+        Asynchronously streams BillingPeriodInstance records from the API as a generator stream.
+        This operation lazily loads records as efficiently as possible until the limit
+        is reached.
+        The results are returned as a generator, so this operation is memory efficient.
+
+        :param limit: Upper limit for the number of records to return. stream()
+                      guarantees to never return more than limit.  Default is no limit
+        :param page_size: Number of records to fetch per request, when not set will use
+                          the default value of 50 records.  If no page_size is defined
+                          but a limit is defined, stream() will attempt to read the
+                          limit with the most efficient page size, i.e. min(limit, 1000)
+
+        :returns: Generator that will yield up to limit results
+        """
+        limits = self._version.read_limits(limit, page_size)
+        page = await self.page_async(page_size=limits["page_size"])
+
+        return self._version.stream_async(page, limits["limit"])
+
+    def list(
+        self,
+        limit: Optional[int] = None,
+        page_size: Optional[int] = None,
+    ) -> List[BillingPeriodInstance]:
+        """
+        Lists BillingPeriodInstance records from the API as a list.
+        Unlike stream(), this operation is eager and will load `limit` records into
+        memory before returning.
+
+        :param limit: Upper limit for the number of records to return. list() guarantees
+                      never to return more than limit.  Default is no limit
+        :param page_size: Number of records to fetch per request, when not set will use
+                          the default value of 50 records.  If no page_size is defined
+                          but a limit is defined, list() will attempt to read the limit
+                          with the most efficient page size, i.e. min(limit, 1000)
+
+        :returns: list that will contain up to limit results
+        """
+        return list(
+            self.stream(
+                limit=limit,
+                page_size=page_size,
+            )
+        )
 
-        :param create_messages_request:
+    async def list_async(
+        self,
+        limit: Optional[int] = None,
+        page_size: Optional[int] = None,
+    ) -> List[BillingPeriodInstance]:
+        """
+        Asynchronously lists BillingPeriodInstance records from the API as a list.
+        Unlike stream(), this operation is eager and will load `limit` records into
+        memory before returning.
+
+        :param limit: Upper limit for the number of records to return. list() guarantees
+                      never to return more than limit.  Default is no limit
+        :param page_size: Number of records to fetch per request, when not set will use
+                          the default value of 50 records.  If no page_size is defined
+                          but a limit is defined, list() will attempt to read the limit
+                          with the most efficient page size, i.e. min(limit, 1000)
+
+        :returns: list that will contain up to limit results
+        """
+        return [
+            record
+            async for record in await self.stream_async(
+                limit=limit,
+                page_size=page_size,
+            )
+        ]
 
-        :returns: The created MessageInstance
-        """
-        data = create_messages_request.to_dict()
+    def page(
+        self,
+        page_token: Union[str, object] = values.unset,
+        page_number: Union[int, object] = values.unset,
+        page_size: Union[int, object] = values.unset,
+    ) -> BillingPeriodPage:
+        """
+        Retrieve a single page of BillingPeriodInstance records from the API.
+        Request is executed immediately
+
+        :param page_token: PageToken provided by the API
+        :param page_number: Page Number, this value is simply for client state
+        :param page_size: Number of records to return, defaults to 50
+
+        :returns: Page of BillingPeriodInstance
+        """
+        data = values.of(
+            {
+                "PageToken": page_token,
+                "Page": page_number,
+                "PageSize": page_size,
+            }
+        )
 
-        headers = {"Content-Type": "application/json"}
+        response = self._version.page(method="GET", uri=self._uri, params=data)
+        return BillingPeriodPage(self._version, response, self._solution)
 
-        payload = self._version.create(
-            method="POST", uri=self._uri, data=data, headers=headers
+    async def page_async(
+        self,
+        page_token: Union[str, object] = values.unset,
+        page_number: Union[int, object] = values.unset,
+        page_size: Union[int, object] = values.unset,
+    ) -> BillingPeriodPage:
+        """
+        Asynchronously retrieve a single page of BillingPeriodInstance records from the API.
+        Request is executed immediately
+
+        :param page_token: PageToken provided by the API
+        :param page_number: Page Number, this value is simply for client state
+        :param page_size: Number of records to return, defaults to 50
+
+        :returns: Page of BillingPeriodInstance
+        """
+        data = values.of(
+            {
+                "PageToken": page_token,
+                "Page": page_number,
+                "PageSize": page_size,
+            }
         )
 
-        return MessageInstance(self._version, payload)
+        response = await self._version.page_async(
+            method="GET", uri=self._uri, params=data
+        )
+        return BillingPeriodPage(self._version, response, self._solution)
 
-    async def create_async(
-        self, create_messages_request: CreateMessagesRequest
-    ) -> MessageInstance:
+    def get_page(self, target_url: str) -> BillingPeriodPage:
         """
-        Asynchronously create the MessageInstance
+        Retrieve a specific page of BillingPeriodInstance records from the API.
+        Request is executed immediately
 
-        :param create_messages_request:
+        :param target_url: API-generated URL for the requested results page
 
-        :returns: The created MessageInstance
+        :returns: Page of BillingPeriodInstance
         """
-        data = create_messages_request.to_dict()
+        response = self._version.domain.twilio.request("GET", target_url)
+        return BillingPeriodPage(self._version, response, self._solution)
 
-        headers = {"Content-Type": "application/json"}
+    async def get_page_async(self, target_url: str) -> BillingPeriodPage:
+        """
+        Asynchronously retrieve a specific page of BillingPeriodInstance records from the API.
+        Request is executed immediately
 
-        payload = await self._version.create_async(
-            method="POST", uri=self._uri, data=data, headers=headers
-        )
+        :param target_url: API-generated URL for the requested results page
 
-        return MessageInstance(self._version, payload)
+        :returns: Page of BillingPeriodInstance
+        """
+        response = await self._version.domain.twilio.request_async("GET", target_url)
+        return BillingPeriodPage(self._version, response, self._solution)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.PreviewMessaging.V1.MessageList>"
+        return "<Twilio.Supersim.V1.BillingPeriodList>"
```

### Comparing `twilio-9.0.5/twilio/rest/pricing/PricingBase.py` & `twilio-9.1.0/twilio/rest/pricing/PricingBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/messaging/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v1/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/messaging/country.py` & `twilio-9.1.0/twilio/rest/pricing/v1/messaging/country.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/phone_number/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v1/phone_number/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/phone_number/country.py` & `twilio-9.1.0/twilio/rest/pricing/v1/phone_number/country.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/voice/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v1/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/voice/country.py` & `twilio-9.1.0/twilio/rest/pricing/v1/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v1/voice/number.py` & `twilio-9.1.0/twilio/rest/verify/v2/form.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,192 +1,193 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Pricing
+    Twilio - Verify
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from typing import Any, Dict, Optional
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class NumberInstance(InstanceResource):
+class FormInstance(InstanceResource):
+
+    class FormTypes(object):
+        FORM_PUSH = "form-push"
+
     """
-    :ivar number: The phone number.
-    :ivar country: The name of the country.
-    :ivar iso_country: The [ISO country code](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2).
-    :ivar outbound_call_price:
-    :ivar inbound_call_price:
-    :ivar price_unit: The currency in which prices are measured, specified in [ISO 4127](http://www.iso.org/iso/home/standards/currency_codes.htm) format (e.g. `usd`, `eur`, `jpy`).
-    :ivar url: The absolute URL of the resource.
+    :ivar form_type: 
+    :ivar forms: Object that contains the available forms for this type. This available forms are given in the standard [JSON Schema](https://json-schema.org/) format
+    :ivar form_meta: Additional information for the available forms for this type. E.g. The separator string used for `binding` in a Factor push.
+    :ivar url: The URL to access the forms for this type.
     """
 
     def __init__(
-        self, version: Version, payload: Dict[str, Any], number: Optional[str] = None
+        self,
+        version: Version,
+        payload: Dict[str, Any],
+        form_type: Optional[FormTypes] = None,
     ):
         super().__init__(version)
 
-        self.number: Optional[str] = payload.get("number")
-        self.country: Optional[str] = payload.get("country")
-        self.iso_country: Optional[str] = payload.get("iso_country")
-        self.outbound_call_price: Optional[str] = payload.get("outbound_call_price")
-        self.inbound_call_price: Optional[str] = payload.get("inbound_call_price")
-        self.price_unit: Optional[str] = payload.get("price_unit")
+        self.form_type: Optional["FormInstance.FormTypes"] = payload.get("form_type")
+        self.forms: Optional[Dict[str, object]] = payload.get("forms")
+        self.form_meta: Optional[Dict[str, object]] = payload.get("form_meta")
         self.url: Optional[str] = payload.get("url")
 
         self._solution = {
-            "number": number or self.number,
+            "form_type": form_type or self.form_type,
         }
-        self._context: Optional[NumberContext] = None
+        self._context: Optional[FormContext] = None
 
     @property
-    def _proxy(self) -> "NumberContext":
+    def _proxy(self) -> "FormContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: NumberContext for this NumberInstance
+        :returns: FormContext for this FormInstance
         """
         if self._context is None:
-            self._context = NumberContext(
+            self._context = FormContext(
                 self._version,
-                number=self._solution["number"],
+                form_type=self._solution["form_type"],
             )
         return self._context
 
-    def fetch(self) -> "NumberInstance":
+    def fetch(self) -> "FormInstance":
         """
-        Fetch the NumberInstance
+        Fetch the FormInstance
 
 
-        :returns: The fetched NumberInstance
+        :returns: The fetched FormInstance
         """
         return self._proxy.fetch()
 
-    async def fetch_async(self) -> "NumberInstance":
+    async def fetch_async(self) -> "FormInstance":
         """
-        Asynchronous coroutine to fetch the NumberInstance
+        Asynchronous coroutine to fetch the FormInstance
 
 
-        :returns: The fetched NumberInstance
+        :returns: The fetched FormInstance
         """
         return await self._proxy.fetch_async()
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Pricing.V1.NumberInstance {}>".format(context)
+        return "<Twilio.Verify.V2.FormInstance {}>".format(context)
 
 
-class NumberContext(InstanceContext):
+class FormContext(InstanceContext):
 
-    def __init__(self, version: Version, number: str):
+    def __init__(self, version: Version, form_type: "FormInstance.FormTypes"):
         """
-        Initialize the NumberContext
+        Initialize the FormContext
 
         :param version: Version that contains the resource
-        :param number: The phone number to fetch.
+        :param form_type: The Type of this Form. Currently only `form-push` is supported.
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
-            "number": number,
+            "form_type": form_type,
         }
-        self._uri = "/Voice/Numbers/{number}".format(**self._solution)
+        self._uri = "/Forms/{form_type}".format(**self._solution)
 
-    def fetch(self) -> NumberInstance:
+    def fetch(self) -> FormInstance:
         """
-        Fetch the NumberInstance
+        Fetch the FormInstance
 
 
-        :returns: The fetched NumberInstance
+        :returns: The fetched FormInstance
         """
 
         payload = self._version.fetch(
             method="GET",
             uri=self._uri,
         )
 
-        return NumberInstance(
+        return FormInstance(
             self._version,
             payload,
-            number=self._solution["number"],
+            form_type=self._solution["form_type"],
         )
 
-    async def fetch_async(self) -> NumberInstance:
+    async def fetch_async(self) -> FormInstance:
         """
-        Asynchronous coroutine to fetch the NumberInstance
+        Asynchronous coroutine to fetch the FormInstance
 
 
-        :returns: The fetched NumberInstance
+        :returns: The fetched FormInstance
         """
 
         payload = await self._version.fetch_async(
             method="GET",
             uri=self._uri,
         )
 
-        return NumberInstance(
+        return FormInstance(
             self._version,
             payload,
-            number=self._solution["number"],
+            form_type=self._solution["form_type"],
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Pricing.V1.NumberContext {}>".format(context)
+        return "<Twilio.Verify.V2.FormContext {}>".format(context)
 
 
-class NumberList(ListResource):
+class FormList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the NumberList
+        Initialize the FormList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-    def get(self, number: str) -> NumberContext:
+    def get(self, form_type: "FormInstance.FormTypes") -> FormContext:
         """
-        Constructs a NumberContext
+        Constructs a FormContext
 
-        :param number: The phone number to fetch.
+        :param form_type: The Type of this Form. Currently only `form-push` is supported.
         """
-        return NumberContext(self._version, number=number)
+        return FormContext(self._version, form_type=form_type)
 
-    def __call__(self, number: str) -> NumberContext:
+    def __call__(self, form_type: "FormInstance.FormTypes") -> FormContext:
         """
-        Constructs a NumberContext
+        Constructs a FormContext
 
-        :param number: The phone number to fetch.
+        :param form_type: The Type of this Form. Currently only `form-push` is supported.
         """
-        return NumberContext(self._version, number=number)
+        return FormContext(self._version, form_type=form_type)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Pricing.V1.NumberList>"
+        return "<Twilio.Verify.V2.FormList>"
```

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/country.py` & `twilio-9.1.0/twilio/rest/pricing/v2/country.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/number.py` & `twilio-9.1.0/twilio/rest/pricing/v2/number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/voice/__init__.py` & `twilio-9.1.0/twilio/rest/pricing/v2/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/voice/country.py` & `twilio-9.1.0/twilio/rest/pricing/v2/voice/country.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/pricing/v2/voice/number.py` & `twilio-9.1.0/twilio/rest/pricing/v2/voice/number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/ProxyBase.py` & `twilio-9.1.0/twilio/rest/proxy/ProxyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/__init__.py` & `twilio-9.1.0/twilio/rest/proxy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/phone_number.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/session/__init__.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/session/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/session/interaction.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/session/interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/session/participant/__init__.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/session/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/session/participant/message_interaction.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/session/participant/message_interaction.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/proxy/v1/service/short_code.py` & `twilio-9.1.0/twilio/rest/proxy/v1/service/short_code.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/RoutesBase.py` & `twilio-9.1.0/twilio/rest/routes/RoutesBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/__init__.py` & `twilio-9.1.0/twilio/rest/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/v2/__init__.py` & `twilio-9.1.0/twilio/rest/routes/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/v2/phone_number.py` & `twilio-9.1.0/twilio/rest/routes/v2/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/v2/sip_domain.py` & `twilio-9.1.0/twilio/rest/routes/v2/sip_domain.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/routes/v2/trunk.py` & `twilio-9.1.0/twilio/rest/routes/v2/trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/ServerlessBase.py` & `twilio-9.1.0/twilio/rest/serverless/ServerlessBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/__init__.py` & `twilio-9.1.0/twilio/rest/trusthub/TrusthubBase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 r"""
-    This code was generated by
-   ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
-    |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
-    |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
-
-    Twilio - Serverless
-    This is the public Twilio REST API.
-
-    NOTE: This class is auto generated by OpenAPI Generator.
-    https://openapi-generator.tech
-    Do not edit the class manually.
+  This code was generated by
+  ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
+   |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
+   |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
+
+  NOTE: This class is auto generated by OpenAPI Generator.
+  https://openapi-generator.tech
+  Do not edit the class manually.
 """
 
 from typing import Optional
-from twilio.base.version import Version
+
 from twilio.base.domain import Domain
-from twilio.rest.serverless.v1.service import ServiceList
+from twilio.rest import Client
+from twilio.rest.trusthub.v1 import V1
 
 
-class V1(Version):
+class TrusthubBase(Domain):
 
-    def __init__(self, domain: Domain):
+    def __init__(self, twilio: Client):
         """
-        Initialize the V1 version of Serverless
+        Initialize the Trusthub Domain
 
-        :param domain: The Twilio.serverless domain
+        :returns: Domain for Trusthub
         """
-        super().__init__(domain, "v1")
-        self._services: Optional[ServiceList] = None
+        super().__init__(twilio, "https://trusthub.twilio.com")
+        self._v1: Optional[V1] = None
 
     @property
-    def services(self) -> ServiceList:
-        if self._services is None:
-            self._services = ServiceList(self)
-        return self._services
+    def v1(self) -> V1:
+        """
+        :returns: Versions v1 of Trusthub
+        """
+        if self._v1 is None:
+            self._v1 = V1(self)
+        return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Serverless.V1>"
+        return "<Twilio.Trusthub>"
```

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/asset/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/asset/asset_version.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/asset/asset_version.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/build/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/build/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/build/build_status.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/build/build_status.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/environment/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/environment/deployment.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/environment/deployment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/environment/log.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/environment/log.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/environment/variable.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/environment/variable.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/function/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/function/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/function/function_version/__init__.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/function/function_version/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py` & `twilio-9.1.0/twilio/rest/serverless/v1/service/function/function_version/function_version_content.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/StudioBase.py` & `twilio-9.1.0/twilio/rest/studio/StudioBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/__init__.py` & `twilio-9.1.0/twilio/rest/studio/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/engagement_context.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/engagement_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/step/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/engagement/step/step_context.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/engagement/step/step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/execution/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_context.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py` & `twilio-9.1.0/twilio/rest/studio/v1/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/execution/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_context.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_step/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/execution/execution_step/execution_step_context.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/flow_revision.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/flow_revision.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow/flow_test_user.py` & `twilio-9.1.0/twilio/rest/studio/v2/flow/flow_test_user.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/studio/v2/flow_validate.py` & `twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/bulk_country_update.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,137 +1,112 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Studio
+    Twilio - Voice
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from typing import Any, Dict, Optional, Union
-from twilio.base import serialize, values
+from typing import Any, Dict, Optional
+from twilio.base import deserialize, values
 
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class FlowValidateInstance(InstanceResource):
-
-    class Status(object):
-        DRAFT = "draft"
-        PUBLISHED = "published"
-
+class BulkCountryUpdateInstance(InstanceResource):
     """
-    :ivar valid: Boolean if the flow definition is valid.
+    :ivar update_count: The number of countries updated
+    :ivar update_request: A bulk update request to change voice dialing country permissions stored as a URL-encoded, JSON array of update objects. For example : `[ { \"iso_code\": \"GB\", \"low_risk_numbers_enabled\": \"true\", \"high_risk_special_numbers_enabled\":\"true\", \"high_risk_tollfraud_numbers_enabled\": \"false\" } ]`
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
-        self.valid: Optional[bool] = payload.get("valid")
+        self.update_count: Optional[int] = deserialize.integer(
+            payload.get("update_count")
+        )
+        self.update_request: Optional[str] = payload.get("update_request")
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
 
-        return "<Twilio.Studio.V2.FlowValidateInstance>"
+        return "<Twilio.Voice.V1.BulkCountryUpdateInstance>"
 
 
-class FlowValidateList(ListResource):
+class BulkCountryUpdateList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the FlowValidateList
+        Initialize the BulkCountryUpdateList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/Flows/Validate"
+        self._uri = "/DialingPermissions/BulkCountryUpdates"
 
-    def update(
-        self,
-        friendly_name: str,
-        status: "FlowValidateInstance.Status",
-        definition: object,
-        commit_message: Union[str, object] = values.unset,
-    ) -> FlowValidateInstance:
-        """
-        Update the FlowValidateInstance
-
-        :param friendly_name: The string that you assigned to describe the Flow.
-        :param status:
-        :param definition: JSON representation of flow definition.
-        :param commit_message: Description of change made in the revision.
+    def create(self, update_request: str) -> BulkCountryUpdateInstance:
+        """
+        Create the BulkCountryUpdateInstance
 
-        :returns: The created FlowValidateInstance
+        :param update_request: URL encoded JSON array of update objects. example : `[ { \\\"iso_code\\\": \\\"GB\\\", \\\"low_risk_numbers_enabled\\\": \\\"true\\\", \\\"high_risk_special_numbers_enabled\\\":\\\"true\\\", \\\"high_risk_tollfraud_numbers_enabled\\\": \\\"false\\\" } ]`
+
+        :returns: The created BulkCountryUpdateInstance
         """
 
         data = values.of(
             {
-                "FriendlyName": friendly_name,
-                "Status": status,
-                "Definition": serialize.object(definition),
-                "CommitMessage": commit_message,
+                "UpdateRequest": update_request,
             }
         )
 
-        payload = self._version.update(
+        payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return FlowValidateInstance(self._version, payload)
+        return BulkCountryUpdateInstance(self._version, payload)
+
+    async def create_async(self, update_request: str) -> BulkCountryUpdateInstance:
+        """
+        Asynchronously create the BulkCountryUpdateInstance
 
-    async def update_async(
-        self,
-        friendly_name: str,
-        status: "FlowValidateInstance.Status",
-        definition: object,
-        commit_message: Union[str, object] = values.unset,
-    ) -> FlowValidateInstance:
-        """
-        Asynchronously update the FlowValidateInstance
-
-        :param friendly_name: The string that you assigned to describe the Flow.
-        :param status:
-        :param definition: JSON representation of flow definition.
-        :param commit_message: Description of change made in the revision.
+        :param update_request: URL encoded JSON array of update objects. example : `[ { \\\"iso_code\\\": \\\"GB\\\", \\\"low_risk_numbers_enabled\\\": \\\"true\\\", \\\"high_risk_special_numbers_enabled\\\":\\\"true\\\", \\\"high_risk_tollfraud_numbers_enabled\\\": \\\"false\\\" } ]`
 
-        :returns: The created FlowValidateInstance
+        :returns: The created BulkCountryUpdateInstance
         """
 
         data = values.of(
             {
-                "FriendlyName": friendly_name,
-                "Status": status,
-                "Definition": serialize.object(definition),
-                "CommitMessage": commit_message,
+                "UpdateRequest": update_request,
             }
         )
 
-        payload = await self._version.update_async(
+        payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return FlowValidateInstance(self._version, payload)
+        return BulkCountryUpdateInstance(self._version, payload)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Studio.V2.FlowValidateList>"
+        return "<Twilio.Voice.V1.BulkCountryUpdateList>"
```

### Comparing `twilio-9.0.5/twilio/rest/supersim/SupersimBase.py` & `twilio-9.1.0/twilio/rest/supersim/SupersimBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/__init__.py` & `twilio-9.1.0/twilio/rest/supersim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/__init__.py` & `twilio-9.1.0/twilio/rest/supersim/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/esim_profile.py` & `twilio-9.1.0/twilio/rest/supersim/v1/esim_profile.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/fleet.py` & `twilio-9.1.0/twilio/rest/supersim/v1/fleet.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/ip_command.py` & `twilio-9.1.0/twilio/rest/supersim/v1/ip_command.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/network.py` & `twilio-9.1.0/twilio/rest/supersim/v1/network.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/network_access_profile/__init__.py` & `twilio-9.1.0/twilio/rest/supersim/v1/network_access_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py` & `twilio-9.1.0/twilio/rest/supersim/v1/network_access_profile/network_access_profile_network.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/settings_update.py` & `twilio-9.1.0/twilio/rest/supersim/v1/settings_update.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/sim/__init__.py` & `twilio-9.1.0/twilio/rest/supersim/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/sim/billing_period.py` & `twilio-9.1.0/twilio/rest/wireless/v1/sim/data_session.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Supersim
+    Twilio - Wireless
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
@@ -18,113 +18,124 @@
 
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
 
 
-class BillingPeriodInstance(InstanceResource):
-
-    class BpType(object):
-        READY = "ready"
-        ACTIVE = "active"
-
+class DataSessionInstance(InstanceResource):
     """
-    :ivar sid: The SID of the Billing Period.
-    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) the Super SIM belongs to.
-    :ivar sim_sid: The SID of the Super SIM the Billing Period belongs to.
-    :ivar start_time: The start time of the Billing Period specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
-    :ivar end_time: The end time of the Billing Period specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
-    :ivar period_type: 
-    :ivar date_created: The date and time in GMT when the resource was created specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
-    :ivar date_updated: The date and time in GMT when the resource was last updated specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    :ivar sid: The unique string that we created to identify the DataSession resource.
+    :ivar sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) that the Data Session is for.
+    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the DataSession resource.
+    :ivar radio_link: The generation of wireless technology that the device was using.
+    :ivar operator_mcc: The 'mobile country code' is the unique ID of the home country where the Data Session took place. See: [MCC/MNC lookup](http://mcc-mnc.com/).
+    :ivar operator_mnc: The 'mobile network code' is the unique ID specific to the mobile operator network where the Data Session took place.
+    :ivar operator_country: The three letter country code representing where the device's Data Session took place. This is determined by looking up the `operator_mcc`.
+    :ivar operator_name: The friendly name of the mobile operator network that the [SIM](https://www.twilio.com/docs/iot/wireless/api/sim-resource)-connected device is attached to. This is determined by looking up the `operator_mnc`.
+    :ivar cell_id: The unique ID of the cellular tower that the device was attached to at the moment when the Data Session was last updated.
+    :ivar cell_location_estimate: An object that describes the estimated location in latitude and longitude where the device's Data Session took place. The location is derived from the `cell_id` when the Data Session was last updated. See [Cell Location Estimate Object](https://www.twilio.com/docs/iot/wireless/api/datasession-resource#cell-location-estimate-object).
+    :ivar packets_uploaded: The number of packets uploaded by the device between the `start` time and when the Data Session was last updated.
+    :ivar packets_downloaded: The number of packets downloaded by the device between the `start` time and when the Data Session was last updated.
+    :ivar last_updated: The date that the resource was last updated, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
+    :ivar start: The date that the Data Session started, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
+    :ivar end: The date that the record ended, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
+    :ivar imei: The 'international mobile equipment identity' is the unique ID of the device using the SIM to connect. An IMEI is a 15-digit string: 14 digits for the device identifier plus a check digit calculated using the Luhn formula.
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any], sim_sid: str):
         super().__init__(version)
 
         self.sid: Optional[str] = payload.get("sid")
-        self.account_sid: Optional[str] = payload.get("account_sid")
         self.sim_sid: Optional[str] = payload.get("sim_sid")
-        self.start_time: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("start_time")
+        self.account_sid: Optional[str] = payload.get("account_sid")
+        self.radio_link: Optional[str] = payload.get("radio_link")
+        self.operator_mcc: Optional[str] = payload.get("operator_mcc")
+        self.operator_mnc: Optional[str] = payload.get("operator_mnc")
+        self.operator_country: Optional[str] = payload.get("operator_country")
+        self.operator_name: Optional[str] = payload.get("operator_name")
+        self.cell_id: Optional[str] = payload.get("cell_id")
+        self.cell_location_estimate: Optional[Dict[str, object]] = payload.get(
+            "cell_location_estimate"
         )
-        self.end_time: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("end_time")
+        self.packets_uploaded: Optional[int] = deserialize.integer(
+            payload.get("packets_uploaded")
         )
-        self.period_type: Optional["BillingPeriodInstance.BpType"] = payload.get(
-            "period_type"
+        self.packets_downloaded: Optional[int] = deserialize.integer(
+            payload.get("packets_downloaded")
         )
-        self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("date_created")
+        self.last_updated: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("last_updated")
         )
-        self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("date_updated")
+        self.start: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("start")
         )
+        self.end: Optional[datetime] = deserialize.iso8601_datetime(payload.get("end"))
+        self.imei: Optional[str] = payload.get("imei")
 
         self._solution = {
             "sim_sid": sim_sid,
         }
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Supersim.V1.BillingPeriodInstance {}>".format(context)
+        return "<Twilio.Wireless.V1.DataSessionInstance {}>".format(context)
 
 
-class BillingPeriodPage(Page):
+class DataSessionPage(Page):
 
-    def get_instance(self, payload: Dict[str, Any]) -> BillingPeriodInstance:
+    def get_instance(self, payload: Dict[str, Any]) -> DataSessionInstance:
         """
-        Build an instance of BillingPeriodInstance
+        Build an instance of DataSessionInstance
 
         :param payload: Payload response from the API
         """
-        return BillingPeriodInstance(
+        return DataSessionInstance(
             self._version, payload, sim_sid=self._solution["sim_sid"]
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Supersim.V1.BillingPeriodPage>"
+        return "<Twilio.Wireless.V1.DataSessionPage>"
 
 
-class BillingPeriodList(ListResource):
+class DataSessionList(ListResource):
 
     def __init__(self, version: Version, sim_sid: str):
         """
-        Initialize the BillingPeriodList
+        Initialize the DataSessionList
 
         :param version: Version that contains the resource
-        :param sim_sid: The SID of the Super SIM to list Billing Periods for.
+        :param sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) with the Data Sessions to read.
 
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
             "sim_sid": sim_sid,
         }
-        self._uri = "/Sims/{sim_sid}/BillingPeriods".format(**self._solution)
+        self._uri = "/Sims/{sim_sid}/DataSessions".format(**self._solution)
 
     def stream(
         self,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> Iterator[BillingPeriodInstance]:
+    ) -> Iterator[DataSessionInstance]:
         """
-        Streams BillingPeriodInstance records from the API as a generator stream.
+        Streams DataSessionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
@@ -139,17 +150,17 @@
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> AsyncIterator[BillingPeriodInstance]:
+    ) -> AsyncIterator[DataSessionInstance]:
         """
-        Asynchronously streams BillingPeriodInstance records from the API as a generator stream.
+        Asynchronously streams DataSessionInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
@@ -164,17 +175,17 @@
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[BillingPeriodInstance]:
+    ) -> List[DataSessionInstance]:
         """
-        Lists BillingPeriodInstance records from the API as a list.
+        Lists DataSessionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
@@ -190,17 +201,17 @@
             )
         )
 
     async def list_async(
         self,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[BillingPeriodInstance]:
+    ) -> List[DataSessionInstance]:
         """
-        Asynchronously lists BillingPeriodInstance records from the API as a list.
+        Asynchronously lists DataSessionInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
@@ -218,89 +229,89 @@
         ]
 
     def page(
         self,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> BillingPeriodPage:
+    ) -> DataSessionPage:
         """
-        Retrieve a single page of BillingPeriodInstance records from the API.
+        Retrieve a single page of DataSessionInstance records from the API.
         Request is executed immediately
 
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of BillingPeriodInstance
+        :returns: Page of DataSessionInstance
         """
         data = values.of(
             {
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return BillingPeriodPage(self._version, response, self._solution)
+        return DataSessionPage(self._version, response, self._solution)
 
     async def page_async(
         self,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> BillingPeriodPage:
+    ) -> DataSessionPage:
         """
-        Asynchronously retrieve a single page of BillingPeriodInstance records from the API.
+        Asynchronously retrieve a single page of DataSessionInstance records from the API.
         Request is executed immediately
 
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of BillingPeriodInstance
+        :returns: Page of DataSessionInstance
         """
         data = values.of(
             {
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return BillingPeriodPage(self._version, response, self._solution)
+        return DataSessionPage(self._version, response, self._solution)
 
-    def get_page(self, target_url: str) -> BillingPeriodPage:
+    def get_page(self, target_url: str) -> DataSessionPage:
         """
-        Retrieve a specific page of BillingPeriodInstance records from the API.
+        Retrieve a specific page of DataSessionInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of BillingPeriodInstance
+        :returns: Page of DataSessionInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return BillingPeriodPage(self._version, response, self._solution)
+        return DataSessionPage(self._version, response, self._solution)
 
-    async def get_page_async(self, target_url: str) -> BillingPeriodPage:
+    async def get_page_async(self, target_url: str) -> DataSessionPage:
         """
-        Asynchronously retrieve a specific page of BillingPeriodInstance records from the API.
+        Asynchronously retrieve a specific page of DataSessionInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of BillingPeriodInstance
+        :returns: Page of DataSessionInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return BillingPeriodPage(self._version, response, self._solution)
+        return DataSessionPage(self._version, response, self._solution)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Supersim.V1.BillingPeriodList>"
+        return "<Twilio.Wireless.V1.DataSessionList>"
```

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/sim/sim_ip_address.py` & `twilio-9.1.0/twilio/rest/supersim/v1/sim/sim_ip_address.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/sms_command.py` & `twilio-9.1.0/twilio/rest/supersim/v1/sms_command.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/supersim/v1/usage_record.py` & `twilio-9.1.0/twilio/rest/supersim/v1/usage_record.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/SyncBase.py` & `twilio-9.1.0/twilio/rest/trunking/TrunkingBase.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,36 +9,36 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.sync.v1 import V1
+from twilio.rest.trunking.v1 import V1
 
 
-class SyncBase(Domain):
+class TrunkingBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the Sync Domain
+        Initialize the Trunking Domain
 
-        :returns: Domain for Sync
+        :returns: Domain for Trunking
         """
-        super().__init__(twilio, "https://sync.twilio.com")
+        super().__init__(twilio, "https://trunking.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Sync
+        :returns: Versions v1 of Trunking
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Sync>"
+        return "<Twilio.Trunking>"
```

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/document/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/document/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/document/document_permission.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/document/document_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/sync_list_item.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_item.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_list/sync_list_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/sync_map_item.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_item.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_map/sync_map_permission.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_stream/__init__.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_stream/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/sync/v1/service/sync_stream/stream_message.py` & `twilio-9.1.0/twilio/rest/sync/v1/service/sync_stream/stream_message.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/TaskrouterBase.py` & `twilio-9.1.0/twilio/rest/taskrouter/TaskrouterBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/activity.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/activity.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/event.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/event.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     :ivar timeout: The amount of time in seconds that the Task can live before being assigned.
     :ivar workflow_sid: The SID of the Workflow that is controlling the Task.
     :ivar workflow_friendly_name: The friendly name of the Workflow that is controlling the Task.
     :ivar workspace_sid: The SID of the Workspace that contains the Task.
     :ivar url: The absolute URL of the Task resource.
     :ivar links: The URLs of related resources.
     :ivar virtual_start_time: The date and time in GMT indicating the ordering for routing of the Task specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
+    :ivar ignore_capacity: A boolean indicating if a new task should respect a worker's capacity during assignment
+    :ivar routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
     """
 
     def __init__(
         self,
         version: Version,
         payload: Dict[str, Any],
         workspace_sid: str,
@@ -101,14 +103,16 @@
         )
         self.workspace_sid: Optional[str] = payload.get("workspace_sid")
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
         self.virtual_start_time: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("virtual_start_time")
         )
+        self.ignore_capacity: Optional[bool] = payload.get("ignore_capacity")
+        self.routing_target: Optional[str] = payload.get("routing_target")
 
         self._solution = {
             "workspace_sid": workspace_sid,
             "sid": sid or self.sid,
         }
         self._context: Optional[TaskContext] = None
 
@@ -514,36 +518,45 @@
         self,
         timeout: Union[int, object] = values.unset,
         priority: Union[int, object] = values.unset,
         task_channel: Union[str, object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         attributes: Union[str, object] = values.unset,
         virtual_start_time: Union[datetime, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
+        ignore_capacity: Union[str, object] = values.unset,
+        task_queue_sid: Union[str, object] = values.unset,
     ) -> TaskInstance:
         """
         Create the TaskInstance
 
         :param timeout: The amount of time in seconds the new task can live before being assigned. Can be up to a maximum of 2 weeks (1,209,600 seconds). The default value is 24 hours (86,400 seconds). On timeout, the `task.canceled` event will fire with description `Task TTL Exceeded`.
         :param priority: The priority to assign the new task and override the default. When supplied, the new Task will have this priority unless it matches a Workflow Target with a Priority set. When not supplied, the new Task will have the priority of the matching Workflow Target. Value can be 0 to 2^31^ (2,147,483,647).
         :param task_channel: When MultiTasking is enabled, specify the TaskChannel by passing either its `unique_name` or `sid`. Default value is `default`.
         :param workflow_sid: The SID of the Workflow that you would like to handle routing for the new Task. If there is only one Workflow defined for the Workspace that you are posting the new task to, this parameter is optional.
         :param attributes: A URL-encoded JSON string with the attributes of the new task. This value is passed to the Workflow's `assignment_callback_url` when the Task is assigned to a Worker. For example: `{ \\\"task_type\\\": \\\"call\\\", \\\"twilio_call_sid\\\": \\\"CAxxx\\\", \\\"customer_ticket_number\\\": \\\"12345\\\" }`.
         :param virtual_start_time: The virtual start time to assign the new task and override the default. When supplied, the new task will have this virtual start time. When not supplied, the new task will have the virtual start time equal to `date_created`. Value can't be in the future.
+        :param routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
+        :param ignore_capacity: A boolean indicating if a new task should respect a worker's capacity during assignment
+        :param task_queue_sid: The SID of the TaskQueue in which the Task belongs
 
         :returns: The created TaskInstance
         """
 
         data = values.of(
             {
                 "Timeout": timeout,
                 "Priority": priority,
                 "TaskChannel": task_channel,
                 "WorkflowSid": workflow_sid,
                 "Attributes": attributes,
                 "VirtualStartTime": serialize.iso8601_datetime(virtual_start_time),
+                "RoutingTarget": routing_target,
+                "IgnoreCapacity": ignore_capacity,
+                "TaskQueueSid": task_queue_sid,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
@@ -557,36 +570,45 @@
         self,
         timeout: Union[int, object] = values.unset,
         priority: Union[int, object] = values.unset,
         task_channel: Union[str, object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         attributes: Union[str, object] = values.unset,
         virtual_start_time: Union[datetime, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
+        ignore_capacity: Union[str, object] = values.unset,
+        task_queue_sid: Union[str, object] = values.unset,
     ) -> TaskInstance:
         """
         Asynchronously create the TaskInstance
 
         :param timeout: The amount of time in seconds the new task can live before being assigned. Can be up to a maximum of 2 weeks (1,209,600 seconds). The default value is 24 hours (86,400 seconds). On timeout, the `task.canceled` event will fire with description `Task TTL Exceeded`.
         :param priority: The priority to assign the new task and override the default. When supplied, the new Task will have this priority unless it matches a Workflow Target with a Priority set. When not supplied, the new Task will have the priority of the matching Workflow Target. Value can be 0 to 2^31^ (2,147,483,647).
         :param task_channel: When MultiTasking is enabled, specify the TaskChannel by passing either its `unique_name` or `sid`. Default value is `default`.
         :param workflow_sid: The SID of the Workflow that you would like to handle routing for the new Task. If there is only one Workflow defined for the Workspace that you are posting the new task to, this parameter is optional.
         :param attributes: A URL-encoded JSON string with the attributes of the new task. This value is passed to the Workflow's `assignment_callback_url` when the Task is assigned to a Worker. For example: `{ \\\"task_type\\\": \\\"call\\\", \\\"twilio_call_sid\\\": \\\"CAxxx\\\", \\\"customer_ticket_number\\\": \\\"12345\\\" }`.
         :param virtual_start_time: The virtual start time to assign the new task and override the default. When supplied, the new task will have this virtual start time. When not supplied, the new task will have the virtual start time equal to `date_created`. Value can't be in the future.
+        :param routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
+        :param ignore_capacity: A boolean indicating if a new task should respect a worker's capacity during assignment
+        :param task_queue_sid: The SID of the TaskQueue in which the Task belongs
 
         :returns: The created TaskInstance
         """
 
         data = values.of(
             {
                 "Timeout": timeout,
                 "Priority": priority,
                 "TaskChannel": task_channel,
                 "WorkflowSid": workflow_sid,
                 "Attributes": attributes,
                 "VirtualStartTime": serialize.iso8601_datetime(virtual_start_time),
+                "RoutingTarget": routing_target,
+                "IgnoreCapacity": ignore_capacity,
+                "TaskQueueSid": task_queue_sid,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
@@ -601,14 +623,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> Iterator[TaskInstance]:
         """
         Streams TaskInstance records from the API as a generator stream.
@@ -619,14 +642,15 @@
         :param int priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param List[str] assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param str workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param str workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param str task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param str task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param str evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param str routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param str ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param bool has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
@@ -639,14 +663,15 @@
             priority=priority,
             assignment_status=assignment_status,
             workflow_sid=workflow_sid,
             workflow_name=workflow_name,
             task_queue_sid=task_queue_sid,
             task_queue_name=task_queue_name,
             evaluate_task_attributes=evaluate_task_attributes,
+            routing_target=routing_target,
             ordering=ordering,
             has_addons=has_addons,
             page_size=limits["page_size"],
         )
 
         return self._version.stream(page, limits["limit"])
 
@@ -655,14 +680,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> AsyncIterator[TaskInstance]:
         """
         Asynchronously streams TaskInstance records from the API as a generator stream.
@@ -673,14 +699,15 @@
         :param int priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param List[str] assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param str workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param str workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param str task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param str task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param str evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param str routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param str ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param bool has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
@@ -693,14 +720,15 @@
             priority=priority,
             assignment_status=assignment_status,
             workflow_sid=workflow_sid,
             workflow_name=workflow_name,
             task_queue_sid=task_queue_sid,
             task_queue_name=task_queue_name,
             evaluate_task_attributes=evaluate_task_attributes,
+            routing_target=routing_target,
             ordering=ordering,
             has_addons=has_addons,
             page_size=limits["page_size"],
         )
 
         return self._version.stream_async(page, limits["limit"])
 
@@ -709,14 +737,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[TaskInstance]:
         """
         Lists TaskInstance records from the API as a list.
@@ -726,14 +755,15 @@
         :param int priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param List[str] assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param str workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param str workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param str task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param str task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param str evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param str routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param str ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param bool has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
@@ -746,14 +776,15 @@
                 priority=priority,
                 assignment_status=assignment_status,
                 workflow_sid=workflow_sid,
                 workflow_name=workflow_name,
                 task_queue_sid=task_queue_sid,
                 task_queue_name=task_queue_name,
                 evaluate_task_attributes=evaluate_task_attributes,
+                routing_target=routing_target,
                 ordering=ordering,
                 has_addons=has_addons,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
@@ -762,14 +793,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
     ) -> List[TaskInstance]:
         """
         Asynchronously lists TaskInstance records from the API as a list.
@@ -779,14 +811,15 @@
         :param int priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param List[str] assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param str workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param str workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param str task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param str task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param str evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param str routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param str ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param bool has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
@@ -800,14 +833,15 @@
                 priority=priority,
                 assignment_status=assignment_status,
                 workflow_sid=workflow_sid,
                 workflow_name=workflow_name,
                 task_queue_sid=task_queue_sid,
                 task_queue_name=task_queue_name,
                 evaluate_task_attributes=evaluate_task_attributes,
+                routing_target=routing_target,
                 ordering=ordering,
                 has_addons=has_addons,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
@@ -816,14 +850,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> TaskPage:
         """
@@ -833,14 +868,15 @@
         :param priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of TaskInstance
@@ -850,14 +886,15 @@
                 "Priority": priority,
                 "AssignmentStatus": serialize.map(assignment_status, lambda e: e),
                 "WorkflowSid": workflow_sid,
                 "WorkflowName": workflow_name,
                 "TaskQueueSid": task_queue_sid,
                 "TaskQueueName": task_queue_name,
                 "EvaluateTaskAttributes": evaluate_task_attributes,
+                "RoutingTarget": routing_target,
                 "Ordering": ordering,
                 "HasAddons": serialize.boolean_to_string(has_addons),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
@@ -870,14 +907,15 @@
         priority: Union[int, object] = values.unset,
         assignment_status: Union[List[str], object] = values.unset,
         workflow_sid: Union[str, object] = values.unset,
         workflow_name: Union[str, object] = values.unset,
         task_queue_sid: Union[str, object] = values.unset,
         task_queue_name: Union[str, object] = values.unset,
         evaluate_task_attributes: Union[str, object] = values.unset,
+        routing_target: Union[str, object] = values.unset,
         ordering: Union[str, object] = values.unset,
         has_addons: Union[bool, object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> TaskPage:
         """
@@ -887,14 +925,15 @@
         :param priority: The priority value of the Tasks to read. Returns the list of all Tasks in the Workspace with the specified priority.
         :param assignment_status: The `assignment_status` of the Tasks you want to read. Can be: `pending`, `reserved`, `assigned`, `canceled`, `wrapping`, or `completed`. Returns all Tasks in the Workspace with the specified `assignment_status`.
         :param workflow_sid: The SID of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this SID.
         :param workflow_name: The friendly name of the Workflow with the Tasks to read. Returns the Tasks controlled by the Workflow identified by this friendly name.
         :param task_queue_sid: The SID of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this SID.
         :param task_queue_name: The `friendly_name` of the TaskQueue with the Tasks to read. Returns the Tasks waiting in the TaskQueue identified by this friendly name.
         :param evaluate_task_attributes: The attributes of the Tasks to read. Returns the Tasks that match the attributes specified in this parameter.
+        :param routing_target: A SID of a Worker, Queue, or Workflow to route a Task to
         :param ordering: How to order the returned Task resources. By default, Tasks are sorted by ascending DateCreated. This value is specified as: `Attribute:Order`, where `Attribute` can be either `DateCreated`, `Priority`, or `VirtualStartTime` and `Order` can be either `asc` or `desc`. For example, `Priority:desc` returns Tasks ordered in descending order of their Priority. Pairings of sort orders can be specified in a comma-separated list such as `Priority:desc,DateCreated:asc`, which returns the Tasks in descending Priority order and ascending DateCreated Order. The only ordering pairing not allowed is DateCreated and VirtualStartTime.
         :param has_addons: Whether to read Tasks with Add-ons. If `true`, returns only Tasks with Add-ons. If `false`, returns only Tasks without Add-ons.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of TaskInstance
@@ -904,14 +943,15 @@
                 "Priority": priority,
                 "AssignmentStatus": serialize.map(assignment_status, lambda e: e),
                 "WorkflowSid": workflow_sid,
                 "WorkflowName": workflow_name,
                 "TaskQueueSid": task_queue_sid,
                 "TaskQueueName": task_queue_name,
                 "EvaluateTaskAttributes": evaluate_task_attributes,
+                "RoutingTarget": routing_target,
                 "Ordering": ordering,
                 "HasAddons": serialize.boolean_to_string(has_addons),
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
```

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task/reservation.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_channel.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_bulk_real_time_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_bulk_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queue_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/task_queue/task_queues_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/reservation.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/reservation.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_channel.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/worker_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/worker/workers_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workflow/workflow_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_cumulative_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_real_time_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py` & `twilio-9.1.0/twilio/rest/taskrouter/v1/workspace/workspace_statistics.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/TrunkingBase.py` & `twilio-9.1.0/twilio/rest/voice/VoiceBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,36 +9,36 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.trunking.v1 import V1
+from twilio.rest.voice.v1 import V1
 
 
-class TrunkingBase(Domain):
+class VoiceBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the Trunking Domain
+        Initialize the Voice Domain
 
-        :returns: Domain for Trunking
+        :returns: Domain for Voice
         """
-        super().__init__(twilio, "https://trunking.twilio.com")
+        super().__init__(twilio, "https://voice.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Trunking
+        :returns: Versions v1 of Voice
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Trunking>"
+        return "<Twilio.Voice>"
```

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/__init__.py` & `twilio-9.1.0/twilio/rest/trunking/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/__init__.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/credential_list.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/credential_list.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/ip_access_control_list.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/ip_access_control_list.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/origination_url.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/origination_url.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/phone_number.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/phone_number.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trunking/v1/trunk/recording.py` & `twilio-9.1.0/twilio/rest/trunking/v1/trunk/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/TrusthubBase.py` & `twilio-9.1.0/twilio/rest/wireless/WirelessBase.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,36 +9,36 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.trusthub.v1 import V1
+from twilio.rest.wireless.v1 import V1
 
 
-class TrusthubBase(Domain):
+class WirelessBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the Trusthub Domain
+        Initialize the Wireless Domain
 
-        :returns: Domain for Trusthub
+        :returns: Domain for Wireless
         """
-        super().__init__(twilio, "https://trusthub.twilio.com")
+        super().__init__(twilio, "https://wireless.twilio.com")
         self._v1: Optional[V1] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Trusthub
+        :returns: Versions v1 of Wireless
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Trusthub>"
+        return "<Twilio.Wireless>"
```

### Comparing `twilio-9.0.5/twilio/rest/trusthub/__init__.py` & `twilio-9.1.0/twilio/rest/trusthub/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/__init__.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/compliance_inquiries.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/compliance_inquiries.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/compliance_registration_inquiries.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/compliance_registration_inquiries.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/compliance_tollfree_inquiries.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/compliance_tollfree_inquiries.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         business_postal_code: Union[str, object] = values.unset,
         business_country: Union[str, object] = values.unset,
         additional_information: Union[str, object] = values.unset,
         business_contact_first_name: Union[str, object] = values.unset,
         business_contact_last_name: Union[str, object] = values.unset,
         business_contact_email: Union[str, object] = values.unset,
         business_contact_phone: Union[str, object] = values.unset,
+        theme_set_id: Union[str, object] = values.unset,
     ) -> ComplianceTollfreeInquiriesInstance:
         """
         Create the ComplianceTollfreeInquiriesInstance
 
         :param tollfree_phone_number: The Tollfree phone number to be verified
         :param notification_email: The email address to receive the notification about the verification result.
         :param business_name: The name of the business or organization using the Tollfree number.
@@ -113,14 +114,15 @@
         :param business_postal_code: The postal code of the business or organization using the Tollfree number.
         :param business_country: The country of the business or organization using the Tollfree number.
         :param additional_information: Additional information to be provided for verification.
         :param business_contact_first_name: The first name of the contact for the business or organization using the Tollfree number.
         :param business_contact_last_name: The last name of the contact for the business or organization using the Tollfree number.
         :param business_contact_email: The email address of the contact for the business or organization using the Tollfree number.
         :param business_contact_phone: The phone number of the contact for the business or organization using the Tollfree number.
+        :param theme_set_id: Theme id for styling the inquiry form.
 
         :returns: The created ComplianceTollfreeInquiriesInstance
         """
 
         data = values.of(
             {
                 "TollfreePhoneNumber": tollfree_phone_number,
@@ -140,14 +142,15 @@
                 "BusinessPostalCode": business_postal_code,
                 "BusinessCountry": business_country,
                 "AdditionalInformation": additional_information,
                 "BusinessContactFirstName": business_contact_first_name,
                 "BusinessContactLastName": business_contact_last_name,
                 "BusinessContactEmail": business_contact_email,
                 "BusinessContactPhone": business_contact_phone,
+                "ThemeSetId": theme_set_id,
             }
         )
 
         payload = self._version.create(
             method="POST",
             uri=self._uri,
             data=data,
@@ -176,14 +179,15 @@
         business_postal_code: Union[str, object] = values.unset,
         business_country: Union[str, object] = values.unset,
         additional_information: Union[str, object] = values.unset,
         business_contact_first_name: Union[str, object] = values.unset,
         business_contact_last_name: Union[str, object] = values.unset,
         business_contact_email: Union[str, object] = values.unset,
         business_contact_phone: Union[str, object] = values.unset,
+        theme_set_id: Union[str, object] = values.unset,
     ) -> ComplianceTollfreeInquiriesInstance:
         """
         Asynchronously create the ComplianceTollfreeInquiriesInstance
 
         :param tollfree_phone_number: The Tollfree phone number to be verified
         :param notification_email: The email address to receive the notification about the verification result.
         :param business_name: The name of the business or organization using the Tollfree number.
@@ -201,14 +205,15 @@
         :param business_postal_code: The postal code of the business or organization using the Tollfree number.
         :param business_country: The country of the business or organization using the Tollfree number.
         :param additional_information: Additional information to be provided for verification.
         :param business_contact_first_name: The first name of the contact for the business or organization using the Tollfree number.
         :param business_contact_last_name: The last name of the contact for the business or organization using the Tollfree number.
         :param business_contact_email: The email address of the contact for the business or organization using the Tollfree number.
         :param business_contact_phone: The phone number of the contact for the business or organization using the Tollfree number.
+        :param theme_set_id: Theme id for styling the inquiry form.
 
         :returns: The created ComplianceTollfreeInquiriesInstance
         """
 
         data = values.of(
             {
                 "TollfreePhoneNumber": tollfree_phone_number,
@@ -228,14 +233,15 @@
                 "BusinessPostalCode": business_postal_code,
                 "BusinessCountry": business_country,
                 "AdditionalInformation": additional_information,
                 "BusinessContactFirstName": business_contact_first_name,
                 "BusinessContactLastName": business_contact_last_name,
                 "BusinessContactEmail": business_contact_email,
                 "BusinessContactPhone": business_contact_phone,
+                "ThemeSetId": theme_set_id,
             }
         )
 
         payload = await self._version.create_async(
             method="POST",
             uri=self._uri,
             data=data,
```

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/__init__.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     :ivar valid_until: The date and time in GMT in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format when the resource will be valid until.
     :ivar email: The email address that will receive updates when the Customer-Profile resource changes status.
     :ivar status_callback: The URL we call to inform your application of status changes.
     :ivar date_created: The date and time in GMT when the resource was created specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     :ivar date_updated: The date and time in GMT when the resource was last updated specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     :ivar url: The absolute URL of the Customer-Profile resource.
     :ivar links: The URLs of the Assigned Items of the Customer-Profile resource.
+    :ivar errors: The error codes associated with the rejection of the Customer-Profile.
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
@@ -74,14 +75,15 @@
             payload.get("date_created")
         )
         self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_updated")
         )
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
+        self.errors: Optional[List[Dict[str, object]]] = payload.get("errors")
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[CustomerProfilesContext] = None
 
     @property
```

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/customer_profiles/customer_profiles_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/end_user.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/end_user.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/end_user_type.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/end_user_type.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/policies.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/policies.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/supporting_document.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/supporting_document.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/supporting_document_type.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/supporting_document_type.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/__init__.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     :ivar valid_until: The date and time in GMT in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format until which the resource will be valid.
     :ivar email: The email address that will receive updates when the Trust Product resource changes status.
     :ivar status_callback: The URL we call to inform your application of status changes.
     :ivar date_created: The date and time in GMT when the resource was created specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     :ivar date_updated: The date and time in GMT when the resource was last updated specified in [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) format.
     :ivar url: The absolute URL of the Trust Product resource.
     :ivar links: The URLs of the Assigned Items of the Trust Product resource.
+    :ivar errors: The error codes associated with the rejection of the Trust Product.
     """
 
     def __init__(
         self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
     ):
         super().__init__(version)
 
@@ -74,14 +75,15 @@
             payload.get("date_created")
         )
         self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
             payload.get("date_updated")
         )
         self.url: Optional[str] = payload.get("url")
         self.links: Optional[Dict[str, object]] = payload.get("links")
+        self.errors: Optional[List[Dict[str, object]]] = payload.get("errors")
 
         self._solution = {
             "sid": sid or self.sid,
         }
         self._context: Optional[TrustProductsContext] = None
 
     @property
```

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_channel_endpoint_assignment.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_entity_assignments.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py` & `twilio-9.1.0/twilio/rest/trusthub/v1/trust_products/trust_products_evaluations.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/VerifyBase.py` & `twilio-9.1.0/twilio/rest/verify/VerifyBase.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/__init__.py` & `twilio-9.1.0/twilio/rest/verify/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/__init__.py` & `twilio-9.1.0/twilio/rest/verify/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/safelist.py` & `twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/settings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,278 +1,250 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Verify
+    Twilio - Voice
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
-from typing import Any, Dict, Optional
-from twilio.base import values
+from typing import Any, Dict, Optional, Union
+from twilio.base import serialize, values
 from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 
 
-class SafelistInstance(InstanceResource):
+class SettingsInstance(InstanceResource):
     """
-    :ivar sid: The unique string that we created to identify the SafeList resource.
-    :ivar phone_number: The phone number in SafeList.
-    :ivar url: The absolute URL of the SafeList resource.
+    :ivar dialing_permissions_inheritance: `true` if the sub-account will inherit voice dialing permissions from the Master Project; otherwise `false`.
+    :ivar url: The absolute URL of this resource.
     """
 
-    def __init__(
-        self,
-        version: Version,
-        payload: Dict[str, Any],
-        phone_number: Optional[str] = None,
-    ):
+    def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
-        self.sid: Optional[str] = payload.get("sid")
-        self.phone_number: Optional[str] = payload.get("phone_number")
+        self.dialing_permissions_inheritance: Optional[bool] = payload.get(
+            "dialing_permissions_inheritance"
+        )
         self.url: Optional[str] = payload.get("url")
 
-        self._solution = {
-            "phone_number": phone_number or self.phone_number,
-        }
-        self._context: Optional[SafelistContext] = None
+        self._context: Optional[SettingsContext] = None
 
     @property
-    def _proxy(self) -> "SafelistContext":
+    def _proxy(self) -> "SettingsContext":
         """
         Generate an instance context for the instance, the context is capable of
         performing various actions. All instance actions are proxied to the context
 
-        :returns: SafelistContext for this SafelistInstance
+        :returns: SettingsContext for this SettingsInstance
         """
         if self._context is None:
-            self._context = SafelistContext(
+            self._context = SettingsContext(
                 self._version,
-                phone_number=self._solution["phone_number"],
             )
         return self._context
 
-    def delete(self) -> bool:
+    def fetch(self) -> "SettingsInstance":
         """
-        Deletes the SafelistInstance
+        Fetch the SettingsInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched SettingsInstance
         """
-        return self._proxy.delete()
+        return self._proxy.fetch()
 
-    async def delete_async(self) -> bool:
+    async def fetch_async(self) -> "SettingsInstance":
         """
-        Asynchronous coroutine that deletes the SafelistInstance
+        Asynchronous coroutine to fetch the SettingsInstance
 
 
-        :returns: True if delete succeeds, False otherwise
+        :returns: The fetched SettingsInstance
         """
-        return await self._proxy.delete_async()
+        return await self._proxy.fetch_async()
 
-    def fetch(self) -> "SafelistInstance":
+    def update(
+        self, dialing_permissions_inheritance: Union[bool, object] = values.unset
+    ) -> "SettingsInstance":
         """
-        Fetch the SafelistInstance
+        Update the SettingsInstance
 
+        :param dialing_permissions_inheritance: `true` for the sub-account to inherit voice dialing permissions from the Master Project; otherwise `false`.
 
-        :returns: The fetched SafelistInstance
+        :returns: The updated SettingsInstance
         """
-        return self._proxy.fetch()
+        return self._proxy.update(
+            dialing_permissions_inheritance=dialing_permissions_inheritance,
+        )
 
-    async def fetch_async(self) -> "SafelistInstance":
+    async def update_async(
+        self, dialing_permissions_inheritance: Union[bool, object] = values.unset
+    ) -> "SettingsInstance":
         """
-        Asynchronous coroutine to fetch the SafelistInstance
+        Asynchronous coroutine to update the SettingsInstance
 
+        :param dialing_permissions_inheritance: `true` for the sub-account to inherit voice dialing permissions from the Master Project; otherwise `false`.
 
-        :returns: The fetched SafelistInstance
+        :returns: The updated SettingsInstance
         """
-        return await self._proxy.fetch_async()
+        return await self._proxy.update_async(
+            dialing_permissions_inheritance=dialing_permissions_inheritance,
+        )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Verify.V2.SafelistInstance {}>".format(context)
+
+        return "<Twilio.Voice.V1.SettingsInstance>"
 
 
-class SafelistContext(InstanceContext):
+class SettingsContext(InstanceContext):
 
-    def __init__(self, version: Version, phone_number: str):
+    def __init__(self, version: Version):
         """
-        Initialize the SafelistContext
+        Initialize the SettingsContext
 
         :param version: Version that contains the resource
-        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
         super().__init__(version)
 
-        # Path Solution
-        self._solution = {
-            "phone_number": phone_number,
-        }
-        self._uri = "/SafeList/Numbers/{phone_number}".format(**self._solution)
+        self._uri = "/Settings"
 
-    def delete(self) -> bool:
+    def fetch(self) -> SettingsInstance:
         """
-        Deletes the SafelistInstance
-
+        Fetch the SettingsInstance
 
-        :returns: True if delete succeeds, False otherwise
-        """
-        return self._version.delete(
-            method="DELETE",
-            uri=self._uri,
-        )
 
-    async def delete_async(self) -> bool:
-        """
-        Asynchronous coroutine that deletes the SafelistInstance
-
-
-        :returns: True if delete succeeds, False otherwise
-        """
-        return await self._version.delete_async(
-            method="DELETE",
-            uri=self._uri,
-        )
-
-    def fetch(self) -> SafelistInstance:
-        """
-        Fetch the SafelistInstance
-
-
-        :returns: The fetched SafelistInstance
+        :returns: The fetched SettingsInstance
         """
 
         payload = self._version.fetch(
             method="GET",
             uri=self._uri,
         )
 
-        return SafelistInstance(
+        return SettingsInstance(
             self._version,
             payload,
-            phone_number=self._solution["phone_number"],
         )
 
-    async def fetch_async(self) -> SafelistInstance:
+    async def fetch_async(self) -> SettingsInstance:
         """
-        Asynchronous coroutine to fetch the SafelistInstance
+        Asynchronous coroutine to fetch the SettingsInstance
 
 
-        :returns: The fetched SafelistInstance
+        :returns: The fetched SettingsInstance
         """
 
         payload = await self._version.fetch_async(
             method="GET",
             uri=self._uri,
         )
 
-        return SafelistInstance(
+        return SettingsInstance(
             self._version,
             payload,
-            phone_number=self._solution["phone_number"],
         )
 
-    def __repr__(self) -> str:
+    def update(
+        self, dialing_permissions_inheritance: Union[bool, object] = values.unset
+    ) -> SettingsInstance:
         """
-        Provide a friendly representation
-
-        :returns: Machine friendly representation
-        """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Verify.V2.SafelistContext {}>".format(context)
+        Update the SettingsInstance
 
+        :param dialing_permissions_inheritance: `true` for the sub-account to inherit voice dialing permissions from the Master Project; otherwise `false`.
 
-class SafelistList(ListResource):
-
-    def __init__(self, version: Version):
+        :returns: The updated SettingsInstance
         """
-        Initialize the SafelistList
-
-        :param version: Version that contains the resource
-
-        """
-        super().__init__(version)
-
-        self._uri = "/SafeList/Numbers"
-
-    def create(self, phone_number: str) -> SafelistInstance:
-        """
-        Create the SafelistInstance
-
-        :param phone_number: The phone number to be added in SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
-
-        :returns: The created SafelistInstance
-        """
-
         data = values.of(
             {
-                "PhoneNumber": phone_number,
+                "DialingPermissionsInheritance": serialize.boolean_to_string(
+                    dialing_permissions_inheritance
+                ),
             }
         )
 
-        payload = self._version.create(
+        payload = self._version.update(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return SafelistInstance(self._version, payload)
+        return SettingsInstance(self._version, payload)
 
-    async def create_async(self, phone_number: str) -> SafelistInstance:
+    async def update_async(
+        self, dialing_permissions_inheritance: Union[bool, object] = values.unset
+    ) -> SettingsInstance:
         """
-        Asynchronously create the SafelistInstance
+        Asynchronous coroutine to update the SettingsInstance
 
-        :param phone_number: The phone number to be added in SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
+        :param dialing_permissions_inheritance: `true` for the sub-account to inherit voice dialing permissions from the Master Project; otherwise `false`.
 
-        :returns: The created SafelistInstance
+        :returns: The updated SettingsInstance
         """
-
         data = values.of(
             {
-                "PhoneNumber": phone_number,
+                "DialingPermissionsInheritance": serialize.boolean_to_string(
+                    dialing_permissions_inheritance
+                ),
             }
         )
 
-        payload = await self._version.create_async(
+        payload = await self._version.update_async(
             method="POST",
             uri=self._uri,
             data=data,
         )
 
-        return SafelistInstance(self._version, payload)
+        return SettingsInstance(self._version, payload)
+
+    def __repr__(self) -> str:
+        """
+        Provide a friendly representation
+
+        :returns: Machine friendly representation
+        """
+
+        return "<Twilio.Voice.V1.SettingsContext>"
+
+
+class SettingsList(ListResource):
+
+    def __init__(self, version: Version):
+        """
+        Initialize the SettingsList
+
+        :param version: Version that contains the resource
+
+        """
+        super().__init__(version)
 
-    def get(self, phone_number: str) -> SafelistContext:
+    def get(self) -> SettingsContext:
         """
-        Constructs a SafelistContext
+        Constructs a SettingsContext
 
-        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
-        return SafelistContext(self._version, phone_number=phone_number)
+        return SettingsContext(self._version)
 
-    def __call__(self, phone_number: str) -> SafelistContext:
+    def __call__(self) -> SettingsContext:
         """
-        Constructs a SafelistContext
+        Constructs a SettingsContext
 
-        :param phone_number: The phone number to be fetched from SafeList. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
         """
-        return SafelistContext(self._version, phone_number=phone_number)
+        return SettingsContext(self._version)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Verify.V2.SafelistList>"
+        return "<Twilio.Voice.V1.SettingsList>"
```

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/__init__.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from twilio.rest.verify.v2.service.webhook import WebhookList
 
 
 class ServiceInstance(InstanceResource):
     """
     :ivar sid: The unique string that we created to identify the Service resource.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Service resource.
-    :ivar friendly_name: The string that you assigned to describe the verification service. It can be up to 32 characters long. **This value should not contain PII.**
+    :ivar friendly_name: The name that appears in the body of your verification messages. It can be up to 30 characters long and can include letters, numbers, spaces, dashes, underscores. Phone numbers, special characters or links are NOT allowed. **This value should not contain PII.**
     :ivar code_length: The length of the verification code to generate.
     :ivar lookup_enabled: Whether to perform a lookup with each verification started and return info about the phone number.
     :ivar psd2_enabled: Whether to pass PSD2 transaction parameters when starting a verification.
     :ivar skip_sms_to_landlines: Whether to skip sending SMS verifications to landlines. Requires `lookup_enabled`.
     :ivar dtmf_input_required: Whether to ask the user to press a number before delivering the verify code in a phone call.
     :ivar tts_name: The name of an alternative text-to-speech service to use in phone calls. Applies only to TTS languages.
     :ivar do_not_share_warning_enabled: Whether to add a security warning at the end of an SMS verification body. Disabled by default and applies only to SMS. Example SMS body: `Your AppName verification code is: 1234. Don’t share this code with anyone; our employees will never ask for the code`
```

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/access_token.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/access_token.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/entity/__init__.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/entity/challenge/__init__.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/entity/challenge/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/entity/challenge/notification.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/entity/challenge/notification.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/entity/factor.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/entity/factor.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/entity/new_factor.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/entity/new_factor.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/messaging_configuration.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/messaging_configuration.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/rate_limit/__init__.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/rate_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/rate_limit/bucket.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/rate_limit/bucket.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/verification.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     """
     :ivar sid: The unique string that we created to identify the Verification resource.
     :ivar service_sid: The SID of the [Service](https://www.twilio.com/docs/verify/api/service) the resource is associated with.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the Verification resource.
     :ivar to: The phone number or [email](https://www.twilio.com/docs/verify/email) being verified. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
     :ivar channel: 
-    :ivar status: The status of the verification. One of: `pending`, `approved`, or `canceled`
+    :ivar status: The status of the verification. Can be: `pending`, `approved`, `canceled`, `max_attempts_reached`, `deleted`, `failed` or `expired`.
     :ivar valid: Use \"status\" instead. Legacy property indicating whether the verification was successful.
     :ivar lookup: Information about the phone number being verified.
     :ivar amount: The amount of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
     :ivar payee: The payee of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
     :ivar send_code_attempts: An array of verification attempt objects containing the channel attempted and the channel-specific transaction SID.
     :ivar date_created: The date and time in GMT when the resource was created specified in [RFC 2822](https://www.ietf.org/rfc/rfc2822.txt) format.
     :ivar date_updated: The date and time in GMT when the resource was last updated specified in [RFC 2822](https://www.ietf.org/rfc/rfc2822.txt) format.
```

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/verification_check.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/verification_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     """
     :ivar sid: The unique string that we created to identify the VerificationCheck resource.
     :ivar service_sid: The SID of the [Service](https://www.twilio.com/docs/verify/api/service) the resource is associated with.
     :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the VerificationCheck resource.
     :ivar to: The phone number or [email](https://www.twilio.com/docs/verify/email) being verified. Phone numbers must be in [E.164 format](https://www.twilio.com/docs/glossary/what-e164).
     :ivar channel: 
-    :ivar status: The status of the verification. Can be: `pending`, `approved`, or `canceled`.
+    :ivar status: The status of the verification. Can be: `pending`, `approved`, `canceled`, `max_attempts_reached`, `deleted`, `failed` or `expired`.
     :ivar valid: Use \"status\" instead. Legacy property indicating whether the verification was successful.
     :ivar amount: The amount of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
     :ivar payee: The payee of the associated PSD2 compliant transaction. Requires the PSD2 Service flag enabled.
     :ivar date_created: The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time in GMT when the Verification Check resource was created.
     :ivar date_updated: The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time in GMT when the Verification Check resource was last updated.
     :ivar sna_attempts_error_codes: List of error codes as a result of attempting a verification using the `sna` channel. The error codes are chronologically ordered, from the first attempt to the latest attempt. This will be an empty list if no errors occured or `null` if the last channel used wasn't `sna`.
     """
```

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/service/webhook.py` & `twilio-9.1.0/twilio/rest/verify/v2/service/webhook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/template.py` & `twilio-9.1.0/twilio/rest/verify/v2/template.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/verification_attempt.py` & `twilio-9.1.0/twilio/rest/verify/v2/verification_attempt.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/verify/v2/verification_attempts_summary.py` & `twilio-9.1.0/twilio/rest/verify/v2/verification_attempts_summary.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/VideoBase.py` & `twilio-9.1.0/twilio/rest/content/ContentBase.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,36 +9,47 @@
   Do not edit the class manually.
 """
 
 from typing import Optional
 
 from twilio.base.domain import Domain
 from twilio.rest import Client
-from twilio.rest.video.v1 import V1
+from twilio.rest.content.v1 import V1
+from twilio.rest.content.v2 import V2
 
 
-class VideoBase(Domain):
+class ContentBase(Domain):
 
     def __init__(self, twilio: Client):
         """
-        Initialize the Video Domain
+        Initialize the Content Domain
 
-        :returns: Domain for Video
+        :returns: Domain for Content
         """
-        super().__init__(twilio, "https://video.twilio.com")
+        super().__init__(twilio, "https://content.twilio.com")
         self._v1: Optional[V1] = None
+        self._v2: Optional[V2] = None
 
     @property
     def v1(self) -> V1:
         """
-        :returns: Versions v1 of Video
+        :returns: Versions v1 of Content
         """
         if self._v1 is None:
             self._v1 = V1(self)
         return self._v1
 
+    @property
+    def v2(self) -> V2:
+        """
+        :returns: Versions v2 of Content
+        """
+        if self._v2 is None:
+            self._v2 = V2(self)
+        return self._v2
+
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Video>"
+        return "<Twilio.Content>"
```

### Comparing `twilio-9.0.5/twilio/rest/video/__init__.py` & `twilio-9.1.0/twilio/rest/video/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/__init__.py` & `twilio-9.1.0/twilio/rest/video/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/composition.py` & `twilio-9.1.0/twilio/rest/video/v1/composition.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/composition_hook.py` & `twilio-9.1.0/twilio/rest/video/v1/composition_hook.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/composition_settings.py` & `twilio-9.1.0/twilio/rest/video/v1/composition_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/recording.py` & `twilio-9.1.0/twilio/rest/video/v1/recording.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/recording_settings.py` & `twilio-9.1.0/twilio/rest/video/v1/recording_settings.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/__init__.py` & `twilio-9.1.0/twilio/rest/video/v1/room/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/participant/__init__.py` & `twilio-9.1.0/twilio/rest/video/v1/room/participant/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/participant/anonymize.py` & `twilio-9.1.0/twilio/rest/video/v1/room/participant/anonymize.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/participant/published_track.py` & `twilio-9.1.0/twilio/rest/video/v1/room/participant/published_track.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/participant/subscribe_rules.py` & `twilio-9.1.0/twilio/rest/video/v1/room/participant/subscribe_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/participant/subscribed_track.py` & `twilio-9.1.0/twilio/rest/video/v1/room/participant/subscribed_track.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/recording_rules.py` & `twilio-9.1.0/twilio/rest/video/v1/room/recording_rules.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/video/v1/room/room_recording.py` & `twilio-9.1.0/twilio/rest/video/v1/room/room_recording.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/VoiceBase.py` & `twilio-9.1.0/twilio/rest/content/v2/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,51 @@
 r"""
-  This code was generated by
-  ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
-   |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
-   |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
-
-  NOTE: This class is auto generated by OpenAPI Generator.
-  https://openapi-generator.tech
-  Do not edit the class manually.
+    This code was generated by
+   ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
+    |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
+    |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
+
+    Twilio - Content
+    This is the public Twilio REST API.
+
+    NOTE: This class is auto generated by OpenAPI Generator.
+    https://openapi-generator.tech
+    Do not edit the class manually.
 """
 
 from typing import Optional
-
+from twilio.base.version import Version
 from twilio.base.domain import Domain
-from twilio.rest import Client
-from twilio.rest.voice.v1 import V1
+from twilio.rest.content.v2.content import ContentList
+from twilio.rest.content.v2.content_and_approvals import ContentAndApprovalsList
 
 
-class VoiceBase(Domain):
+class V2(Version):
 
-    def __init__(self, twilio: Client):
+    def __init__(self, domain: Domain):
         """
-        Initialize the Voice Domain
+        Initialize the V2 version of Content
 
-        :returns: Domain for Voice
+        :param domain: The Twilio.content domain
         """
-        super().__init__(twilio, "https://voice.twilio.com")
-        self._v1: Optional[V1] = None
+        super().__init__(domain, "v2")
+        self._contents: Optional[ContentList] = None
+        self._content_and_approvals: Optional[ContentAndApprovalsList] = None
 
     @property
-    def v1(self) -> V1:
-        """
-        :returns: Versions v1 of Voice
-        """
-        if self._v1 is None:
-            self._v1 = V1(self)
-        return self._v1
+    def contents(self) -> ContentList:
+        if self._contents is None:
+            self._contents = ContentList(self)
+        return self._contents
+
+    @property
+    def content_and_approvals(self) -> ContentAndApprovalsList:
+        if self._content_and_approvals is None:
+            self._content_and_approvals = ContentAndApprovalsList(self)
+        return self._content_and_approvals
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
         :returns: Machine friendly representation
         """
-        return "<Twilio.Voice>"
+        return "<Twilio.Content.V2>"
```

### Comparing `twilio-9.0.5/twilio/rest/voice/__init__.py` & `twilio-9.1.0/twilio/rest/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/__init__.py` & `twilio-9.1.0/twilio/rest/voice/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/archived_call.py` & `twilio-9.1.0/twilio/rest/voice/v1/archived_call.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/byoc_trunk.py` & `twilio-9.1.0/twilio/rest/voice/v1/byoc_trunk.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/connection_policy/__init__.py` & `twilio-9.1.0/twilio/rest/voice/v1/connection_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/connection_policy/connection_policy_target.py` & `twilio-9.1.0/twilio/rest/voice/v1/connection_policy/connection_policy_target.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/__init__.py` & `twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/country/__init__.py` & `twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/country/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py` & `twilio-9.1.0/twilio/rest/voice/v1/dialing_permissions/country/highrisk_special_prefix.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/ip_record.py` & `twilio-9.1.0/twilio/rest/voice/v1/ip_record.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/voice/v1/source_ip_mapping.py` & `twilio-9.1.0/twilio/rest/voice/v1/source_ip_mapping.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/__init__.py` & `twilio-9.1.0/twilio/rest/wireless/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/__init__.py` & `twilio-9.1.0/twilio/rest/wireless/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/command.py` & `twilio-9.1.0/twilio/rest/wireless/v1/command.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/rate_plan.py` & `twilio-9.1.0/twilio/rest/wireless/v1/rate_plan.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/sim/__init__.py` & `twilio-9.1.0/twilio/rest/wireless/v1/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/sim/data_session.py` & `twilio-9.1.0/twilio/rest/wireless/v1/sim/usage_record.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,308 +10,334 @@
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
-from twilio.base import deserialize, values
+from twilio.base import serialize, values
 
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
 
 
-class DataSessionInstance(InstanceResource):
+class UsageRecordInstance(InstanceResource):
+
+    class Granularity(object):
+        HOURLY = "hourly"
+        DAILY = "daily"
+        ALL = "all"
+
     """
-    :ivar sid: The unique string that we created to identify the DataSession resource.
-    :ivar sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) that the Data Session is for.
-    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the DataSession resource.
-    :ivar radio_link: The generation of wireless technology that the device was using.
-    :ivar operator_mcc: The 'mobile country code' is the unique ID of the home country where the Data Session took place. See: [MCC/MNC lookup](http://mcc-mnc.com/).
-    :ivar operator_mnc: The 'mobile network code' is the unique ID specific to the mobile operator network where the Data Session took place.
-    :ivar operator_country: The three letter country code representing where the device's Data Session took place. This is determined by looking up the `operator_mcc`.
-    :ivar operator_name: The friendly name of the mobile operator network that the [SIM](https://www.twilio.com/docs/iot/wireless/api/sim-resource)-connected device is attached to. This is determined by looking up the `operator_mnc`.
-    :ivar cell_id: The unique ID of the cellular tower that the device was attached to at the moment when the Data Session was last updated.
-    :ivar cell_location_estimate: An object that describes the estimated location in latitude and longitude where the device's Data Session took place. The location is derived from the `cell_id` when the Data Session was last updated. See [Cell Location Estimate Object](https://www.twilio.com/docs/iot/wireless/api/datasession-resource#cell-location-estimate-object).
-    :ivar packets_uploaded: The number of packets uploaded by the device between the `start` time and when the Data Session was last updated.
-    :ivar packets_downloaded: The number of packets downloaded by the device between the `start` time and when the Data Session was last updated.
-    :ivar last_updated: The date that the resource was last updated, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
-    :ivar start: The date that the Data Session started, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
-    :ivar end: The date that the record ended, given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
-    :ivar imei: The 'international mobile equipment identity' is the unique ID of the device using the SIM to connect. An IMEI is a 15-digit string: 14 digits for the device identifier plus a check digit calculated using the Luhn formula.
+    :ivar sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) that this Usage Record is for.
+    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the UsageRecord resource.
+    :ivar period: The time period for which the usage is reported. Contains `start` and `end` datetime values given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
+    :ivar commands: An object that describes the SIM's usage of Commands during the specified period. See [Commands Usage Object](https://www.twilio.com/docs/iot/wireless/api/sim-usagerecord-resource#commands-usage-object).
+    :ivar data: An object that describes the SIM's data usage during the specified period. See [Data Usage Object](https://www.twilio.com/docs/iot/wireless/api/sim-usagerecord-resource#data-usage-object).
     """
 
     def __init__(self, version: Version, payload: Dict[str, Any], sim_sid: str):
         super().__init__(version)
 
-        self.sid: Optional[str] = payload.get("sid")
         self.sim_sid: Optional[str] = payload.get("sim_sid")
         self.account_sid: Optional[str] = payload.get("account_sid")
-        self.radio_link: Optional[str] = payload.get("radio_link")
-        self.operator_mcc: Optional[str] = payload.get("operator_mcc")
-        self.operator_mnc: Optional[str] = payload.get("operator_mnc")
-        self.operator_country: Optional[str] = payload.get("operator_country")
-        self.operator_name: Optional[str] = payload.get("operator_name")
-        self.cell_id: Optional[str] = payload.get("cell_id")
-        self.cell_location_estimate: Optional[Dict[str, object]] = payload.get(
-            "cell_location_estimate"
-        )
-        self.packets_uploaded: Optional[int] = deserialize.integer(
-            payload.get("packets_uploaded")
-        )
-        self.packets_downloaded: Optional[int] = deserialize.integer(
-            payload.get("packets_downloaded")
-        )
-        self.last_updated: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("last_updated")
-        )
-        self.start: Optional[datetime] = deserialize.iso8601_datetime(
-            payload.get("start")
-        )
-        self.end: Optional[datetime] = deserialize.iso8601_datetime(payload.get("end"))
-        self.imei: Optional[str] = payload.get("imei")
+        self.period: Optional[Dict[str, object]] = payload.get("period")
+        self.commands: Optional[Dict[str, object]] = payload.get("commands")
+        self.data: Optional[Dict[str, object]] = payload.get("data")
 
         self._solution = {
             "sim_sid": sim_sid,
         }
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Wireless.V1.DataSessionInstance {}>".format(context)
+        return "<Twilio.Wireless.V1.UsageRecordInstance {}>".format(context)
 
 
-class DataSessionPage(Page):
+class UsageRecordPage(Page):
 
-    def get_instance(self, payload: Dict[str, Any]) -> DataSessionInstance:
+    def get_instance(self, payload: Dict[str, Any]) -> UsageRecordInstance:
         """
-        Build an instance of DataSessionInstance
+        Build an instance of UsageRecordInstance
 
         :param payload: Payload response from the API
         """
-        return DataSessionInstance(
+        return UsageRecordInstance(
             self._version, payload, sim_sid=self._solution["sim_sid"]
         )
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Wireless.V1.DataSessionPage>"
+        return "<Twilio.Wireless.V1.UsageRecordPage>"
 
 
-class DataSessionList(ListResource):
+class UsageRecordList(ListResource):
 
     def __init__(self, version: Version, sim_sid: str):
         """
-        Initialize the DataSessionList
+        Initialize the UsageRecordList
 
         :param version: Version that contains the resource
-        :param sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) with the Data Sessions to read.
+        :param sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource)  to read the usage from.
 
         """
         super().__init__(version)
 
         # Path Solution
         self._solution = {
             "sim_sid": sim_sid,
         }
-        self._uri = "/Sims/{sim_sid}/DataSessions".format(**self._solution)
+        self._uri = "/Sims/{sim_sid}/UsageRecords".format(**self._solution)
 
     def stream(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> Iterator[DataSessionInstance]:
+    ) -> Iterator[UsageRecordInstance]:
         """
-        Streams DataSessionInstance records from the API as a generator stream.
+        Streams UsageRecordInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(page_size=limits["page_size"])
+        page = self.page(
+            end=end, start=start, granularity=granularity, page_size=limits["page_size"]
+        )
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> AsyncIterator[DataSessionInstance]:
+    ) -> AsyncIterator[UsageRecordInstance]:
         """
-        Asynchronously streams DataSessionInstance records from the API as a generator stream.
+        Asynchronously streams UsageRecordInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
+        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(page_size=limits["page_size"])
+        page = await self.page_async(
+            end=end, start=start, granularity=granularity, page_size=limits["page_size"]
+        )
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[DataSessionInstance]:
+    ) -> List[UsageRecordInstance]:
         """
-        Lists DataSessionInstance records from the API as a list.
+        Lists UsageRecordInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
+                end=end,
+                start=start,
+                granularity=granularity,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[DataSessionInstance]:
+    ) -> List[UsageRecordInstance]:
         """
-        Asynchronously lists DataSessionInstance records from the API as a list.
+        Asynchronously lists UsageRecordInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
+        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
+                end=end,
+                start=start,
+                granularity=granularity,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> DataSessionPage:
+    ) -> UsageRecordPage:
         """
-        Retrieve a single page of DataSessionInstance records from the API.
+        Retrieve a single page of UsageRecordInstance records from the API.
         Request is executed immediately
 
+        :param end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of DataSessionInstance
+        :returns: Page of UsageRecordInstance
         """
         data = values.of(
             {
+                "End": serialize.iso8601_datetime(end),
+                "Start": serialize.iso8601_datetime(start),
+                "Granularity": granularity,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return DataSessionPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response, self._solution)
 
     async def page_async(
         self,
+        end: Union[datetime, object] = values.unset,
+        start: Union[datetime, object] = values.unset,
+        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> DataSessionPage:
+    ) -> UsageRecordPage:
         """
-        Asynchronously retrieve a single page of DataSessionInstance records from the API.
+        Asynchronously retrieve a single page of UsageRecordInstance records from the API.
         Request is executed immediately
 
+        :param end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
+        :param start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
+        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of DataSessionInstance
+        :returns: Page of UsageRecordInstance
         """
         data = values.of(
             {
+                "End": serialize.iso8601_datetime(end),
+                "Start": serialize.iso8601_datetime(start),
+                "Granularity": granularity,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return DataSessionPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response, self._solution)
 
-    def get_page(self, target_url: str) -> DataSessionPage:
+    def get_page(self, target_url: str) -> UsageRecordPage:
         """
-        Retrieve a specific page of DataSessionInstance records from the API.
+        Retrieve a specific page of UsageRecordInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of DataSessionInstance
+        :returns: Page of UsageRecordInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return DataSessionPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response, self._solution)
 
-    async def get_page_async(self, target_url: str) -> DataSessionPage:
+    async def get_page_async(self, target_url: str) -> UsageRecordPage:
         """
-        Asynchronously retrieve a specific page of DataSessionInstance records from the API.
+        Asynchronously retrieve a specific page of UsageRecordInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of DataSessionInstance
+        :returns: Page of UsageRecordInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return DataSessionPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response, self._solution)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Wireless.V1.DataSessionList>"
+        return "<Twilio.Wireless.V1.UsageRecordList>"
```

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/sim/usage_record.py` & `twilio-9.1.0/twilio/rest/wireless/v1/usage_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,82 +26,69 @@
 
     class Granularity(object):
         HOURLY = "hourly"
         DAILY = "daily"
         ALL = "all"
 
     """
-    :ivar sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource) that this Usage Record is for.
-    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the UsageRecord resource.
-    :ivar period: The time period for which the usage is reported. Contains `start` and `end` datetime values given as GMT in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
-    :ivar commands: An object that describes the SIM's usage of Commands during the specified period. See [Commands Usage Object](https://www.twilio.com/docs/iot/wireless/api/sim-usagerecord-resource#commands-usage-object).
-    :ivar data: An object that describes the SIM's data usage during the specified period. See [Data Usage Object](https://www.twilio.com/docs/iot/wireless/api/sim-usagerecord-resource#data-usage-object).
+    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the AccountUsageRecord resource.
+    :ivar period: The time period for which usage is reported. Contains `start` and `end` properties that describe the period using GMT date-time values specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
+    :ivar commands: An object that describes the aggregated Commands usage for all SIMs during the specified period. See [Commands Usage Object](https://www.twilio.com/docs/iot/wireless/api/account-usagerecord-resource#commands-usage-object).
+    :ivar data: An object that describes the aggregated Data usage for all SIMs over the period. See [Data Usage Object](https://www.twilio.com/docs/iot/wireless/api/account-usagerecord-resource#data-usage-object).
     """
 
-    def __init__(self, version: Version, payload: Dict[str, Any], sim_sid: str):
+    def __init__(self, version: Version, payload: Dict[str, Any]):
         super().__init__(version)
 
-        self.sim_sid: Optional[str] = payload.get("sim_sid")
         self.account_sid: Optional[str] = payload.get("account_sid")
         self.period: Optional[Dict[str, object]] = payload.get("period")
         self.commands: Optional[Dict[str, object]] = payload.get("commands")
         self.data: Optional[Dict[str, object]] = payload.get("data")
 
-        self._solution = {
-            "sim_sid": sim_sid,
-        }
-
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
-        return "<Twilio.Wireless.V1.UsageRecordInstance {}>".format(context)
+
+        return "<Twilio.Wireless.V1.UsageRecordInstance>"
 
 
 class UsageRecordPage(Page):
 
     def get_instance(self, payload: Dict[str, Any]) -> UsageRecordInstance:
         """
         Build an instance of UsageRecordInstance
 
         :param payload: Payload response from the API
         """
-        return UsageRecordInstance(
-            self._version, payload, sim_sid=self._solution["sim_sid"]
-        )
+        return UsageRecordInstance(self._version, payload)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
         return "<Twilio.Wireless.V1.UsageRecordPage>"
 
 
 class UsageRecordList(ListResource):
 
-    def __init__(self, version: Version, sim_sid: str):
+    def __init__(self, version: Version):
         """
         Initialize the UsageRecordList
 
         :param version: Version that contains the resource
-        :param sim_sid: The SID of the [Sim resource](https://www.twilio.com/docs/iot/wireless/api/sim-resource)  to read the usage from.
 
         """
         super().__init__(version)
 
-        # Path Solution
-        self._solution = {
-            "sim_sid": sim_sid,
-        }
-        self._uri = "/Sims/{sim_sid}/UsageRecords".format(**self._solution)
+        self._uri = "/UsageRecords"
 
     def stream(
         self,
         end: Union[datetime, object] = values.unset,
         start: Union[datetime, object] = values.unset,
         granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
@@ -109,17 +96,17 @@
     ) -> Iterator[UsageRecordInstance]:
         """
         Streams UsageRecordInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -142,17 +129,17 @@
     ) -> AsyncIterator[UsageRecordInstance]:
         """
         Asynchronously streams UsageRecordInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
@@ -174,17 +161,17 @@
         page_size: Optional[int] = None,
     ) -> List[UsageRecordInstance]:
         """
         Lists UsageRecordInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -209,17 +196,17 @@
         page_size: Optional[int] = None,
     ) -> List[UsageRecordInstance]:
         """
         Asynchronously lists UsageRecordInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param datetime end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param datetime start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
@@ -245,17 +232,17 @@
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> UsageRecordPage:
         """
         Retrieve a single page of UsageRecordInstance records from the API.
         Request is executed immediately
 
-        :param end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of UsageRecordInstance
         """
         data = values.of(
@@ -266,32 +253,32 @@
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return UsageRecordPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response)
 
     async def page_async(
         self,
         end: Union[datetime, object] = values.unset,
         start: Union[datetime, object] = values.unset,
         granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
     ) -> UsageRecordPage:
         """
         Asynchronously retrieve a single page of UsageRecordInstance records from the API.
         Request is executed immediately
 
-        :param end: Only include usage that occurred on or before this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is the current time.
-        :param start: Only include usage that has occurred on or after this date, specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html). The default is one month before the `end` parameter value.
-        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. The default is `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
+        :param end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
+        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
         :returns: Page of UsageRecordInstance
         """
         data = values.of(
@@ -304,39 +291,39 @@
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return UsageRecordPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response)
 
     def get_page(self, target_url: str) -> UsageRecordPage:
         """
         Retrieve a specific page of UsageRecordInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of UsageRecordInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return UsageRecordPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response)
 
     async def get_page_async(self, target_url: str) -> UsageRecordPage:
         """
         Asynchronously retrieve a specific page of UsageRecordInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
         :returns: Page of UsageRecordInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return UsageRecordPage(self._version, response, self._solution)
+        return UsageRecordPage(self._version, response)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
```

### Comparing `twilio-9.0.5/twilio/rest/wireless/v1/usage_record.py` & `twilio-9.1.0/twilio/rest/intelligence/v2/operator_type.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,330 +1,443 @@
 r"""
     This code was generated by
    ___ _ _ _ _ _    _ ____    ____ ____ _    ____ ____ _  _ ____ ____ ____ ___ __   __
     |  | | | | |    | |  | __ |  | |__| | __ | __ |___ |\ | |___ |__/ |__|  | |  | |__/
     |  |_|_| | |___ | |__|    |__| |  | |    |__] |___ | \| |___ |  \ |  |  | |__| |  \
 
-    Twilio - Wireless
+    Twilio - Intelligence
     This is the public Twilio REST API.
 
     NOTE: This class is auto generated by OpenAPI Generator.
     https://openapi-generator.tech
     Do not edit the class manually.
 """
 
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union, Iterator, AsyncIterator
-from twilio.base import serialize, values
-
+from twilio.base import deserialize, values
+from twilio.base.instance_context import InstanceContext
 from twilio.base.instance_resource import InstanceResource
 from twilio.base.list_resource import ListResource
 from twilio.base.version import Version
 from twilio.base.page import Page
 
 
-class UsageRecordInstance(InstanceResource):
+class OperatorTypeInstance(InstanceResource):
 
-    class Granularity(object):
-        HOURLY = "hourly"
-        DAILY = "daily"
-        ALL = "all"
+    class Availability(object):
+        INTERNAL = "internal"
+        BETA = "beta"
+        PUBLIC = "public"
+        RETIRED = "retired"
+
+    class OutputType(object):
+        TEXT_CLASSIFICATION = "text-classification"
+        TEXT_EXTRACTION = "text-extraction"
+        TEXT_EXTRACTION_NORMALIZED = "text-extraction-normalized"
+        TEXT_GENERATION = "text-generation"
+
+    class Provider(object):
+        TWILIO = "twilio"
+        AMAZON = "amazon"
+        OPENAI = "openai"
 
     """
-    :ivar account_sid: The SID of the [Account](https://www.twilio.com/docs/iam/api/account) that created the AccountUsageRecord resource.
-    :ivar period: The time period for which usage is reported. Contains `start` and `end` properties that describe the period using GMT date-time values specified in [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html) format.
-    :ivar commands: An object that describes the aggregated Commands usage for all SIMs during the specified period. See [Commands Usage Object](https://www.twilio.com/docs/iot/wireless/api/account-usagerecord-resource#commands-usage-object).
-    :ivar data: An object that describes the aggregated Data usage for all SIMs over the period. See [Data Usage Object](https://www.twilio.com/docs/iot/wireless/api/account-usagerecord-resource#data-usage-object).
+    :ivar name: A unique name that references an Operator's Operator Type.
+    :ivar sid: A 34 character string that uniquely identifies this Operator Type.
+    :ivar friendly_name: A human-readable name of this resource, up to 64 characters.
+    :ivar description: A human-readable description of this resource, longer than the friendly name.
+    :ivar docs_link: Additional documentation for the Operator Type.
+    :ivar output_type: 
+    :ivar supported_languages: List of languages this Operator Type supports.
+    :ivar provider: 
+    :ivar availability: 
+    :ivar configurable: Operators can be created from configurable Operator Types.
+    :ivar config_schema: JSON Schema for configuring an Operator with this Operator Type. Following https://json-schema.org/
+    :ivar date_created: The date that this Operator Type was created, given in ISO 8601 format.
+    :ivar date_updated: The date that this Operator Type was updated, given in ISO 8601 format.
+    :ivar url: The URL of this resource.
     """
 
-    def __init__(self, version: Version, payload: Dict[str, Any]):
+    def __init__(
+        self, version: Version, payload: Dict[str, Any], sid: Optional[str] = None
+    ):
         super().__init__(version)
 
-        self.account_sid: Optional[str] = payload.get("account_sid")
-        self.period: Optional[Dict[str, object]] = payload.get("period")
-        self.commands: Optional[Dict[str, object]] = payload.get("commands")
-        self.data: Optional[Dict[str, object]] = payload.get("data")
+        self.name: Optional[str] = payload.get("name")
+        self.sid: Optional[str] = payload.get("sid")
+        self.friendly_name: Optional[str] = payload.get("friendly_name")
+        self.description: Optional[str] = payload.get("description")
+        self.docs_link: Optional[str] = payload.get("docs_link")
+        self.output_type: Optional["OperatorTypeInstance.OutputType"] = payload.get(
+            "output_type"
+        )
+        self.supported_languages: Optional[List[str]] = payload.get(
+            "supported_languages"
+        )
+        self.provider: Optional["OperatorTypeInstance.Provider"] = payload.get(
+            "provider"
+        )
+        self.availability: Optional["OperatorTypeInstance.Availability"] = payload.get(
+            "availability"
+        )
+        self.configurable: Optional[bool] = payload.get("configurable")
+        self.config_schema: Optional[Dict[str, object]] = payload.get("config_schema")
+        self.date_created: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("date_created")
+        )
+        self.date_updated: Optional[datetime] = deserialize.iso8601_datetime(
+            payload.get("date_updated")
+        )
+        self.url: Optional[str] = payload.get("url")
+
+        self._solution = {
+            "sid": sid or self.sid,
+        }
+        self._context: Optional[OperatorTypeContext] = None
+
+    @property
+    def _proxy(self) -> "OperatorTypeContext":
+        """
+        Generate an instance context for the instance, the context is capable of
+        performing various actions. All instance actions are proxied to the context
+
+        :returns: OperatorTypeContext for this OperatorTypeInstance
+        """
+        if self._context is None:
+            self._context = OperatorTypeContext(
+                self._version,
+                sid=self._solution["sid"],
+            )
+        return self._context
+
+    def fetch(self) -> "OperatorTypeInstance":
+        """
+        Fetch the OperatorTypeInstance
+
+
+        :returns: The fetched OperatorTypeInstance
+        """
+        return self._proxy.fetch()
+
+    async def fetch_async(self) -> "OperatorTypeInstance":
+        """
+        Asynchronous coroutine to fetch the OperatorTypeInstance
+
+
+        :returns: The fetched OperatorTypeInstance
+        """
+        return await self._proxy.fetch_async()
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
+        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
+        return "<Twilio.Intelligence.V2.OperatorTypeInstance {}>".format(context)
+
+
+class OperatorTypeContext(InstanceContext):
+
+    def __init__(self, version: Version, sid: str):
+        """
+        Initialize the OperatorTypeContext
+
+        :param version: Version that contains the resource
+        :param sid: A 34 character string that uniquely identifies this Operator Type.
+        """
+        super().__init__(version)
+
+        # Path Solution
+        self._solution = {
+            "sid": sid,
+        }
+        self._uri = "/OperatorTypes/{sid}".format(**self._solution)
+
+    def fetch(self) -> OperatorTypeInstance:
+        """
+        Fetch the OperatorTypeInstance
 
-        return "<Twilio.Wireless.V1.UsageRecordInstance>"
 
+        :returns: The fetched OperatorTypeInstance
+        """
 
-class UsageRecordPage(Page):
+        payload = self._version.fetch(
+            method="GET",
+            uri=self._uri,
+        )
+
+        return OperatorTypeInstance(
+            self._version,
+            payload,
+            sid=self._solution["sid"],
+        )
 
-    def get_instance(self, payload: Dict[str, Any]) -> UsageRecordInstance:
+    async def fetch_async(self) -> OperatorTypeInstance:
         """
-        Build an instance of UsageRecordInstance
+        Asynchronous coroutine to fetch the OperatorTypeInstance
+
+
+        :returns: The fetched OperatorTypeInstance
+        """
+
+        payload = await self._version.fetch_async(
+            method="GET",
+            uri=self._uri,
+        )
+
+        return OperatorTypeInstance(
+            self._version,
+            payload,
+            sid=self._solution["sid"],
+        )
+
+    def __repr__(self) -> str:
+        """
+        Provide a friendly representation
+
+        :returns: Machine friendly representation
+        """
+        context = " ".join("{}={}".format(k, v) for k, v in self._solution.items())
+        return "<Twilio.Intelligence.V2.OperatorTypeContext {}>".format(context)
+
+
+class OperatorTypePage(Page):
+
+    def get_instance(self, payload: Dict[str, Any]) -> OperatorTypeInstance:
+        """
+        Build an instance of OperatorTypeInstance
 
         :param payload: Payload response from the API
         """
-        return UsageRecordInstance(self._version, payload)
+        return OperatorTypeInstance(self._version, payload)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Wireless.V1.UsageRecordPage>"
+        return "<Twilio.Intelligence.V2.OperatorTypePage>"
 
 
-class UsageRecordList(ListResource):
+class OperatorTypeList(ListResource):
 
     def __init__(self, version: Version):
         """
-        Initialize the UsageRecordList
+        Initialize the OperatorTypeList
 
         :param version: Version that contains the resource
 
         """
         super().__init__(version)
 
-        self._uri = "/UsageRecords"
+        self._uri = "/OperatorTypes"
 
     def stream(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> Iterator[UsageRecordInstance]:
+    ) -> Iterator[OperatorTypeInstance]:
         """
-        Streams UsageRecordInstance records from the API as a generator stream.
+        Streams OperatorTypeInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = self.page(
-            end=end, start=start, granularity=granularity, page_size=limits["page_size"]
-        )
+        page = self.page(page_size=limits["page_size"])
 
         return self._version.stream(page, limits["limit"])
 
     async def stream_async(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> AsyncIterator[UsageRecordInstance]:
+    ) -> AsyncIterator[OperatorTypeInstance]:
         """
-        Asynchronously streams UsageRecordInstance records from the API as a generator stream.
+        Asynchronously streams OperatorTypeInstance records from the API as a generator stream.
         This operation lazily loads records as efficiently as possible until the limit
         is reached.
         The results are returned as a generator, so this operation is memory efficient.
 
-        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. stream()
                       guarantees to never return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, stream() will attempt to read the
                           limit with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: Generator that will yield up to limit results
         """
         limits = self._version.read_limits(limit, page_size)
-        page = await self.page_async(
-            end=end, start=start, granularity=granularity, page_size=limits["page_size"]
-        )
+        page = await self.page_async(page_size=limits["page_size"])
 
         return self._version.stream_async(page, limits["limit"])
 
     def list(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[UsageRecordInstance]:
+    ) -> List[OperatorTypeInstance]:
         """
-        Lists UsageRecordInstance records from the API as a list.
+        Lists OperatorTypeInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return list(
             self.stream(
-                end=end,
-                start=start,
-                granularity=granularity,
                 limit=limit,
                 page_size=page_size,
             )
         )
 
     async def list_async(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         limit: Optional[int] = None,
         page_size: Optional[int] = None,
-    ) -> List[UsageRecordInstance]:
+    ) -> List[OperatorTypeInstance]:
         """
-        Asynchronously lists UsageRecordInstance records from the API as a list.
+        Asynchronously lists OperatorTypeInstance records from the API as a list.
         Unlike stream(), this operation is eager and will load `limit` records into
         memory before returning.
 
-        :param datetime end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param datetime start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param &quot;UsageRecordInstance.Granularity&quot; granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param limit: Upper limit for the number of records to return. list() guarantees
                       never to return more than limit.  Default is no limit
         :param page_size: Number of records to fetch per request, when not set will use
                           the default value of 50 records.  If no page_size is defined
                           but a limit is defined, list() will attempt to read the limit
                           with the most efficient page size, i.e. min(limit, 1000)
 
         :returns: list that will contain up to limit results
         """
         return [
             record
             async for record in await self.stream_async(
-                end=end,
-                start=start,
-                granularity=granularity,
                 limit=limit,
                 page_size=page_size,
             )
         ]
 
     def page(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> UsageRecordPage:
+    ) -> OperatorTypePage:
         """
-        Retrieve a single page of UsageRecordInstance records from the API.
+        Retrieve a single page of OperatorTypeInstance records from the API.
         Request is executed immediately
 
-        :param end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of UsageRecordInstance
+        :returns: Page of OperatorTypeInstance
         """
         data = values.of(
             {
-                "End": serialize.iso8601_datetime(end),
-                "Start": serialize.iso8601_datetime(start),
-                "Granularity": granularity,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = self._version.page(method="GET", uri=self._uri, params=data)
-        return UsageRecordPage(self._version, response)
+        return OperatorTypePage(self._version, response)
 
     async def page_async(
         self,
-        end: Union[datetime, object] = values.unset,
-        start: Union[datetime, object] = values.unset,
-        granularity: Union["UsageRecordInstance.Granularity", object] = values.unset,
         page_token: Union[str, object] = values.unset,
         page_number: Union[int, object] = values.unset,
         page_size: Union[int, object] = values.unset,
-    ) -> UsageRecordPage:
+    ) -> OperatorTypePage:
         """
-        Asynchronously retrieve a single page of UsageRecordInstance records from the API.
+        Asynchronously retrieve a single page of OperatorTypeInstance records from the API.
         Request is executed immediately
 
-        :param end: Only include usage that has occurred on or before this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param start: Only include usage that has occurred on or after this date. Format is [ISO 8601](https://www.iso.org/iso-8601-date-and-time-format.html).
-        :param granularity: How to summarize the usage by time. Can be: `daily`, `hourly`, or `all`. A value of `all` returns one Usage Record that describes the usage for the entire period.
         :param page_token: PageToken provided by the API
         :param page_number: Page Number, this value is simply for client state
         :param page_size: Number of records to return, defaults to 50
 
-        :returns: Page of UsageRecordInstance
+        :returns: Page of OperatorTypeInstance
         """
         data = values.of(
             {
-                "End": serialize.iso8601_datetime(end),
-                "Start": serialize.iso8601_datetime(start),
-                "Granularity": granularity,
                 "PageToken": page_token,
                 "Page": page_number,
                 "PageSize": page_size,
             }
         )
 
         response = await self._version.page_async(
             method="GET", uri=self._uri, params=data
         )
-        return UsageRecordPage(self._version, response)
+        return OperatorTypePage(self._version, response)
 
-    def get_page(self, target_url: str) -> UsageRecordPage:
+    def get_page(self, target_url: str) -> OperatorTypePage:
         """
-        Retrieve a specific page of UsageRecordInstance records from the API.
+        Retrieve a specific page of OperatorTypeInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of UsageRecordInstance
+        :returns: Page of OperatorTypeInstance
         """
         response = self._version.domain.twilio.request("GET", target_url)
-        return UsageRecordPage(self._version, response)
+        return OperatorTypePage(self._version, response)
 
-    async def get_page_async(self, target_url: str) -> UsageRecordPage:
+    async def get_page_async(self, target_url: str) -> OperatorTypePage:
         """
-        Asynchronously retrieve a specific page of UsageRecordInstance records from the API.
+        Asynchronously retrieve a specific page of OperatorTypeInstance records from the API.
         Request is executed immediately
 
         :param target_url: API-generated URL for the requested results page
 
-        :returns: Page of UsageRecordInstance
+        :returns: Page of OperatorTypeInstance
         """
         response = await self._version.domain.twilio.request_async("GET", target_url)
-        return UsageRecordPage(self._version, response)
+        return OperatorTypePage(self._version, response)
+
+    def get(self, sid: str) -> OperatorTypeContext:
+        """
+        Constructs a OperatorTypeContext
+
+        :param sid: A 34 character string that uniquely identifies this Operator Type.
+        """
+        return OperatorTypeContext(self._version, sid=sid)
+
+    def __call__(self, sid: str) -> OperatorTypeContext:
+        """
+        Constructs a OperatorTypeContext
+
+        :param sid: A 34 character string that uniquely identifies this Operator Type.
+        """
+        return OperatorTypeContext(self._version, sid=sid)
 
     def __repr__(self) -> str:
         """
         Provide a friendly representation
 
         :returns: Machine friendly representation
         """
-        return "<Twilio.Wireless.V1.UsageRecordList>"
+        return "<Twilio.Intelligence.V2.OperatorTypeList>"
```

### Comparing `twilio-9.0.5/twilio/twiml/__init__.py` & `twilio-9.1.0/twilio/twiml/__init__.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/twiml/fax_response.py` & `twilio-9.1.0/twilio/twiml/fax_response.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/twiml/messaging_response.py` & `twilio-9.1.0/twilio/twiml/messaging_response.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio/twiml/voice_response.py` & `twilio-9.1.0/twilio/twiml/voice_response.py`

 * *Files identical despite different names*

### Comparing `twilio-9.0.5/twilio.egg-info/PKG-INFO` & `twilio-9.1.0/twilio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twilio
-Version: 9.0.5
+Version: 9.1.0
 Summary: Twilio API client and TwiML generator
 Home-page: https://github.com/twilio/twilio-python/
 Author: Twilio
 Keywords: twilio,twiml
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `twilio-9.0.5/twilio.egg-info/SOURCES.txt` & `twilio-9.1.0/twilio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -167,14 +167,17 @@
 twilio/rest/content/__init__.py
 twilio/rest/content/v1/__init__.py
 twilio/rest/content/v1/content_and_approvals.py
 twilio/rest/content/v1/legacy_content.py
 twilio/rest/content/v1/content/__init__.py
 twilio/rest/content/v1/content/approval_create.py
 twilio/rest/content/v1/content/approval_fetch.py
+twilio/rest/content/v2/__init__.py
+twilio/rest/content/v2/content.py
+twilio/rest/content/v2/content_and_approvals.py
 twilio/rest/conversations/ConversationsBase.py
 twilio/rest/conversations/__init__.py
 twilio/rest/conversations/v1/__init__.py
 twilio/rest/conversations/v1/address_configuration.py
 twilio/rest/conversations/v1/credential.py
 twilio/rest/conversations/v1/participant_conversation.py
 twilio/rest/conversations/v1/role.py
@@ -263,14 +266,20 @@
 twilio/rest/insights/v1/conference/__init__.py
 twilio/rest/insights/v1/conference/conference_participant.py
 twilio/rest/insights/v1/room/__init__.py
 twilio/rest/insights/v1/room/participant.py
 twilio/rest/intelligence/IntelligenceBase.py
 twilio/rest/intelligence/__init__.py
 twilio/rest/intelligence/v2/__init__.py
+twilio/rest/intelligence/v2/custom_operator.py
+twilio/rest/intelligence/v2/operator.py
+twilio/rest/intelligence/v2/operator_attachment.py
+twilio/rest/intelligence/v2/operator_attachments.py
+twilio/rest/intelligence/v2/operator_type.py
+twilio/rest/intelligence/v2/prebuilt_operator.py
 twilio/rest/intelligence/v2/service.py
 twilio/rest/intelligence/v2/transcript/__init__.py
 twilio/rest/intelligence/v2/transcript/media.py
 twilio/rest/intelligence/v2/transcript/operator_result.py
 twilio/rest/intelligence/v2/transcript/sentence.py
 twilio/rest/ip_messaging/IpMessagingBase.py
 twilio/rest/ip_messaging/__init__.py
@@ -349,19 +358,20 @@
 twilio/rest/notify/v1/service/binding.py
 twilio/rest/notify/v1/service/notification.py
 twilio/rest/numbers/NumbersBase.py
 twilio/rest/numbers/__init__.py
 twilio/rest/numbers/v1/__init__.py
 twilio/rest/numbers/v1/bulk_eligibility.py
 twilio/rest/numbers/v1/eligibility.py
-twilio/rest/numbers/v1/porting_bulk_portability.py
 twilio/rest/numbers/v1/porting_port_in.py
-twilio/rest/numbers/v1/porting_port_in_fetch.py
 twilio/rest/numbers/v1/porting_port_in_phone_number.py
 twilio/rest/numbers/v1/porting_portability.py
+twilio/rest/numbers/v1/porting_webhook_configuration.py
+twilio/rest/numbers/v1/porting_webhook_configuration_delete.py
+twilio/rest/numbers/v1/porting_webhook_configuration_fetch.py
 twilio/rest/numbers/v2/__init__.py
 twilio/rest/numbers/v2/bulk_hosted_number_order.py
 twilio/rest/numbers/v2/hosted_number_order.py
 twilio/rest/numbers/v2/authorization_document/__init__.py
 twilio/rest/numbers/v2/authorization_document/dependent_hosted_number_order.py
 twilio/rest/numbers/v2/regulatory_compliance/__init__.py
 twilio/rest/numbers/v2/regulatory_compliance/end_user.py
@@ -407,19 +417,15 @@
 twilio/rest/preview/sync/service/sync_map/sync_map_item.py
 twilio/rest/preview/sync/service/sync_map/sync_map_permission.py
 twilio/rest/preview/wireless/__init__.py
 twilio/rest/preview/wireless/command.py
 twilio/rest/preview/wireless/rate_plan.py
 twilio/rest/preview/wireless/sim/__init__.py
 twilio/rest/preview/wireless/sim/usage.py
-twilio/rest/preview_messaging/PreviewMessagingBase.py
 twilio/rest/preview_messaging/__init__.py
-twilio/rest/preview_messaging/v1/__init__.py
-twilio/rest/preview_messaging/v1/broadcast.py
-twilio/rest/preview_messaging/v1/message.py
 twilio/rest/pricing/PricingBase.py
 twilio/rest/pricing/__init__.py
 twilio/rest/pricing/v1/__init__.py
 twilio/rest/pricing/v1/messaging/__init__.py
 twilio/rest/pricing/v1/messaging/country.py
 twilio/rest/pricing/v1/phone_number/__init__.py
 twilio/rest/pricing/v1/phone_number/country.py
```

