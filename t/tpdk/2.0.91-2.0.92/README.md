# Comparing `tmp/tpdk-2.0.91.tar.gz` & `tmp/tpdk-2.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpdk-2.0.91.tar", last modified: Thu Oct 19 12:57:14 2023, max compression
+gzip compressed data, was "tpdk-2.0.92.tar", last modified: Thu Oct 19 14:15:27 2023, max compression
```

## Comparing `tpdk-2.0.91.tar` & `tpdk-2.0.92.tar`

### file list

```diff
@@ -1,213 +1,213 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.043391 tpdk-2.0.91/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-19 12:57:14.043391 tpdk-2.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21297 2023-10-19 12:56:52.000000 tpdk-2.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-19 12:56:52.000000 tpdk-2.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-19 12:57:14.047391 tpdk-2.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-10-19 12:56:52.000000 tpdk-2.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.031391 tpdk-2.0.91/test/
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_address_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_address_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_address_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_api_client_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_api_client_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_api_client_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_branding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     9497 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    10244 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     9220 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_evidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_media_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_media_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_media_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_media_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_notification_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_notification_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_offer_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_organization_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_parcel_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_auth_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_external_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_token_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_persona_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     7089 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_transaction_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_invite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_user_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    12896 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_webhook_subscription_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_workflow_event_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-10-19 12:56:52.000000 tpdk-2.0.91/test/test_workflow_event_read.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.035391 tpdk-2.0.91/tpdk/
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.035391 tpdk-2.0.91/tpdk/api/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33393 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/branding_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30277 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13739 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/organization_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    51069 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/persona_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   104908 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/resolution_center_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   155933 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/safe_checkout_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    90795 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/user_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41796 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api/webhook_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    30394 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16244 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5561 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.043391 tpdk-2.0.91/tpdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/address_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/address_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/address_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/address_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/api_client_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/api_client_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/api_client_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    14112 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    23395 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    23230 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)    11791 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/dispute_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/evaluation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/evaluation_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/evidence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/evidence_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/evidence_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/media_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/media_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/media_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/media_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/metadata_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/notification_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/notification_update.py
--rw-r--r--   0 runner    (1001) docker     (127)    12593 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_post_creation_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/offer_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     7448 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/organization_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/parcel_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/parcel_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/parcel_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/parcel_write.py
--rw-r--r--   0 runner    (1001) docker     (127)    12658 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_auth_return.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_external_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_post_auth_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     8818 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_token_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/persona_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/transaction_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/transaction_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/transaction_independent_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/transaction_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/unprocessable_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/unprocessable_entity_violations_inner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_authenticated_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_email_validation_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_invite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_post_register_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/user_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook_history_collection_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook_history_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook_subscription_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/webhook_subscription_write.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/workflow_event_dispute_read.py
--rw-r--r--   0 runner    (1001) docker     (127)     4669 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/models/workflow_event_read.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13049 2023-10-19 12:56:52.000000 tpdk-2.0.91/tpdk/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 12:57:14.035391 tpdk-2.0.91/tpdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-19 12:57:14.000000 tpdk-2.0.91/tpdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6414 2023-10-19 12:57:14.000000 tpdk-2.0.91/tpdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 12:57:14.000000 tpdk-2.0.91/tpdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-19 12:57:14.000000 tpdk-2.0.91/tpdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 12:57:14.000000 tpdk-2.0.91/tpdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.966109 tpdk-2.0.92/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-19 14:15:27.966109 tpdk-2.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21297 2023-10-19 14:15:17.000000 tpdk-2.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-19 14:15:17.000000 tpdk-2.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-10-19 14:15:27.966109 tpdk-2.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2023-10-19 14:15:17.000000 tpdk-2.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.950109 tpdk-2.0.92/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_address_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_address_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_address_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_api_client_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_api_client_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_api_client_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9497 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10244 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9220 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_evidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_media_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_media_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_media_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_media_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4079 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_parcel_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3240 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_token_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7089 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_transaction_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10634 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_user_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12896 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_webhook_subscription_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_workflow_event_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1853 2023-10-19 14:15:17.000000 tpdk-2.0.92/test/test_workflow_event_read.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.950109 tpdk-2.0.92/tpdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.954109 tpdk-2.0.92/tpdk/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33393 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/branding_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30277 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13739 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/organization_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51069 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/persona_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104908 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/resolution_center_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   155933 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/safe_checkout_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90795 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/user_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41796 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api/webhook_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30394 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16244 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5561 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.966109 tpdk-2.0.92/tpdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/address_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/address_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/address_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4470 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/address_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/api_client_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/api_client_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/api_client_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14112 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23395 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11791 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/dispute_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/evaluation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/evaluation_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5001 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/evidence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/evidence_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/evidence_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/media_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/media_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/media_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/media_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/metadata_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/notification_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/notification_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12593 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_post_creation_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/offer_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5091 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6077 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7448 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/organization_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5387 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/parcel_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/parcel_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/parcel_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/parcel_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_auth_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3852 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_external_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_post_auth_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8818 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_token_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/persona_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/transaction_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/transaction_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/transaction_independent_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/transaction_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/unprocessable_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/unprocessable_entity_violations_inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_authenticated_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_email_validation_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_invite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_post_register_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/user_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3979 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook_history_collection_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook_history_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5411 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook_subscription_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/webhook_subscription_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/workflow_event_dispute_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4669 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/models/workflow_event_read.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13049 2023-10-19 14:15:17.000000 tpdk-2.0.92/tpdk/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-19 14:15:27.950109 tpdk-2.0.92/tpdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2023-10-19 14:15:27.000000 tpdk-2.0.92/tpdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6414 2023-10-19 14:15:27.000000 tpdk-2.0.92/tpdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-19 14:15:27.000000 tpdk-2.0.92/tpdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-19 14:15:27.000000 tpdk-2.0.92/tpdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-19 14:15:27.000000 tpdk-2.0.92/tpdk.egg-info/top_level.txt
```

### Comparing `tpdk-2.0.91/PKG-INFO` & `tpdk-2.0.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpdk
-Version: 2.0.91
+Version: 2.0.92
 Summary: Tripartie
 Home-page: https://pypi.org/project/tpdk
 Author: Tripartie SAS
 Author-email: noc@tripartie.com
 Keywords: OpenAPI,OpenAPI-Generator,Tripartie
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `tpdk-2.0.91/README.md` & `tpdk-2.0.92/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # tpdk
 Our API suite for the **Resolution Center** and the **Safe Checkout** features.
 Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 2.0.91
-- Package version: 2.0.91
+- API version: 2.0.92
+- Package version: 2.0.92
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://tripartie.com](https://tripartie.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `tpdk-2.0.91/pyproject.toml` & `tpdk-2.0.92/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tpdk"
-version = "2.0.91"
+version = "2.0.92"
 description = "Tripartie"
 authors = ["Tripartie SAS <noc@tripartie.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/tripartie/tpdk"
 keywords = ["OpenAPI", "OpenAPI-Generator", "Tripartie"]
 include = ["tpdk/py.typed"]
```

### Comparing `tpdk-2.0.91/setup.py` & `tpdk-2.0.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "tpdk"
-VERSION = "2.0.91"
+VERSION = "2.0.92"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3, < 2.1.0",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `tpdk-2.0.91/test/test_address.py` & `tpdk-2.0.92/test/test_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_address_independent_write.py` & `tpdk-2.0.92/test/test_address_independent_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_address_read.py` & `tpdk-2.0.92/test/test_address_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_address_update.py` & `tpdk-2.0.92/test/test_address_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_address_write.py` & `tpdk-2.0.92/test/test_address_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_api_client_post_creation_read.py` & `tpdk-2.0.92/test/test_api_client_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_api_client_read.py` & `tpdk-2.0.92/test/test_api_client_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_api_client_write.py` & `tpdk-2.0.92/test/test_api_client_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_branding_api.py` & `tpdk-2.0.92/test/test_branding_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_collection_read.py` & `tpdk-2.0.92/test/test_dispute_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_dispute_read.py` & `tpdk-2.0.92/test/test_dispute_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_independent_write.py` & `tpdk-2.0.92/test/test_dispute_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_post_creation_read.py` & `tpdk-2.0.92/test/test_dispute_post_creation_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_read.py` & `tpdk-2.0.92/test/test_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_update.py` & `tpdk-2.0.92/test/test_dispute_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_dispute_write.py` & `tpdk-2.0.92/test/test_dispute_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_evaluation_read.py` & `tpdk-2.0.92/test/test_evaluation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_evaluation_write.py` & `tpdk-2.0.92/test/test_evaluation_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_evidence.py` & `tpdk-2.0.92/test/test_evidence.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -40,15 +40,16 @@
                 id = 56,
                 dispute = '',
                 owner = '',
                 status = 'SUBMITTED',
                 media = '',
                 additional_information = 'The motherboard I received have a minor scratch at the bottom, here is the proof.',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                publisher = 'BUYER'
             )
         else:
             return Evidence(
                 status = 'SUBMITTED',
         )
         """
```

### Comparing `tpdk-2.0.91/test/test_evidence_read.py` & `tpdk-2.0.92/test/test_evidence_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -39,15 +39,16 @@
             return EvidenceRead(
                 id = 56,
                 status = 'SUBMITTED',
                 media = tpdk.models.media_read.Media-Read(
                     public_url = 'https://cdn.tripartie.app/b15e64db-fbd2-442b-afee-69ee45e2959b.jpg', ),
                 additional_information = 'The motherboard I received have a minor scratch at the bottom, here is the proof.',
                 created_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
-                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f')
+                updated_at = datetime.datetime.strptime('2013-10-20 19:20:30.00', '%Y-%m-%d %H:%M:%S.%f'),
+                publisher = 'BUYER'
             )
         else:
             return EvidenceRead(
                 status = 'SUBMITTED',
         )
         """
```

### Comparing `tpdk-2.0.91/test/test_evidence_write.py` & `tpdk-2.0.92/test/test_evidence_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_media.py` & `tpdk-2.0.92/test/test_media.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_media_authenticated_read.py` & `tpdk-2.0.92/test/test_media_authenticated_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_media_collection_read.py` & `tpdk-2.0.92/test/test_media_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_media_dispute_read.py` & `tpdk-2.0.92/test/test_media_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_media_read.py` & `tpdk-2.0.92/test/test_media_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata.py` & `tpdk-2.0.92/test/test_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata_dispute_read.py` & `tpdk-2.0.92/test/test_metadata_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata_independent_write.py` & `tpdk-2.0.92/test/test_metadata_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata_read.py` & `tpdk-2.0.92/test/test_metadata_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata_update.py` & `tpdk-2.0.92/test/test_metadata_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_metadata_write.py` & `tpdk-2.0.92/test/test_metadata_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_notification_api.py` & `tpdk-2.0.92/test/test_notification_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_notification_read.py` & `tpdk-2.0.92/test/test_notification_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_notification_update.py` & `tpdk-2.0.92/test/test_notification_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer.py` & `tpdk-2.0.92/test/test_offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_collection_read.py` & `tpdk-2.0.92/test/test_offer_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_dispute_read.py` & `tpdk-2.0.92/test/test_offer_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_independent_write.py` & `tpdk-2.0.92/test/test_offer_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_post_creation_read.py` & `tpdk-2.0.92/test/test_offer_post_creation_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_read.py` & `tpdk-2.0.92/test/test_offer_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_update.py` & `tpdk-2.0.92/test/test_offer_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_offer_write.py` & `tpdk-2.0.92/test/test_offer_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_api.py` & `tpdk-2.0.92/test/test_organization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_authenticated_read.py` & `tpdk-2.0.92/test/test_organization_authenticated_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_collection_read.py` & `tpdk-2.0.92/test/test_organization_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_dispute_read.py` & `tpdk-2.0.92/test/test_organization_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_read.py` & `tpdk-2.0.92/test/test_organization_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_update.py` & `tpdk-2.0.92/test/test_organization_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_organization_write.py` & `tpdk-2.0.92/test/test_organization_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_parcel.py` & `tpdk-2.0.92/test/test_parcel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_parcel_dispute_read.py` & `tpdk-2.0.92/test/test_parcel_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_parcel_independent_write.py` & `tpdk-2.0.92/test/test_parcel_independent_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_parcel_read.py` & `tpdk-2.0.92/test/test_parcel_read.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_parcel_write.py` & `tpdk-2.0.92/test/test_parcel_write.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona.py` & `tpdk-2.0.92/test/test_persona.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_api.py` & `tpdk-2.0.92/test/test_persona_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_auth_return.py` & `tpdk-2.0.92/test/test_persona_auth_return.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_collection_read.py` & `tpdk-2.0.92/test/test_persona_collection_read.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_external_auth.py` & `tpdk-2.0.92/test/test_persona_external_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_independent_write.py` & `tpdk-2.0.92/test/test_persona_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_post_auth_read.py` & `tpdk-2.0.92/test/test_persona_post_auth_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_read.py` & `tpdk-2.0.92/test/test_persona_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_register.py` & `tpdk-2.0.92/test/test_persona_register.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_token_write.py` & `tpdk-2.0.92/test/test_persona_token_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_update.py` & `tpdk-2.0.92/test/test_persona_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_persona_write.py` & `tpdk-2.0.92/test/test_persona_write.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_resolution_center_api.py` & `tpdk-2.0.92/test/test_resolution_center_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_safe_checkout_api.py` & `tpdk-2.0.92/test/test_safe_checkout_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_transaction_collection_read.py` & `tpdk-2.0.92/test/test_transaction_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_transaction_dispute_read.py` & `tpdk-2.0.92/test/test_transaction_dispute_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_transaction_independent_write.py` & `tpdk-2.0.92/test/test_transaction_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_transaction_read.py` & `tpdk-2.0.92/test/test_transaction_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_unprocessable_entity.py` & `tpdk-2.0.92/test/test_unprocessable_entity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_unprocessable_entity_violations_inner.py` & `tpdk-2.0.92/test/test_unprocessable_entity_violations_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user.py` & `tpdk-2.0.92/test/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_api.py` & `tpdk-2.0.92/test/test_user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_authenticated_read.py` & `tpdk-2.0.92/test/test_user_authenticated_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_collection_read.py` & `tpdk-2.0.92/test/test_user_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_email_validation_write.py` & `tpdk-2.0.92/test/test_user_email_validation_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_invite.py` & `tpdk-2.0.92/test/test_user_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_post_register_read.py` & `tpdk-2.0.92/test/test_user_post_register_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_update.py` & `tpdk-2.0.92/test/test_user_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_user_write.py` & `tpdk-2.0.92/test/test_user_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_view.py` & `tpdk-2.0.92/test/test_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook.py` & `tpdk-2.0.92/test/test_webhook.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_api.py` & `tpdk-2.0.92/test/test_webhook_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_history_collection_read.py` & `tpdk-2.0.92/test/test_webhook_history_collection_read.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_history_read.py` & `tpdk-2.0.92/test/test_webhook_history_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_object.py` & `tpdk-2.0.92/test/test_webhook_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_subscription_read.py` & `tpdk-2.0.92/test/test_webhook_subscription_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_webhook_subscription_write.py` & `tpdk-2.0.92/test/test_webhook_subscription_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_workflow_event_dispute_read.py` & `tpdk-2.0.92/test/test_workflow_event_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/test/test_workflow_event_read.py` & `tpdk-2.0.92/test/test_workflow_event_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/__init__.py` & `tpdk-2.0.92/tpdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
-__version__ = "2.0.91"
+__version__ = "2.0.92"
 
 # import apis into sdk package
 from tpdk.api.branding_api import BrandingApi
 from tpdk.api.notification_api import NotificationApi
 from tpdk.api.organization_api import OrganizationApi
 from tpdk.api.persona_api import PersonaApi
 from tpdk.api.resolution_center_api import ResolutionCenterApi
```

### Comparing `tpdk-2.0.91/tpdk/api/branding_api.py` & `tpdk-2.0.92/tpdk/api/branding_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/notification_api.py` & `tpdk-2.0.92/tpdk/api/notification_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/organization_api.py` & `tpdk-2.0.92/tpdk/api/organization_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/persona_api.py` & `tpdk-2.0.92/tpdk/api/persona_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/resolution_center_api.py` & `tpdk-2.0.92/tpdk/api/resolution_center_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/safe_checkout_api.py` & `tpdk-2.0.92/tpdk/api/safe_checkout_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/user_api.py` & `tpdk-2.0.92/tpdk/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api/webhook_api.py` & `tpdk-2.0.92/tpdk/api/webhook_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/api_client.py` & `tpdk-2.0.92/tpdk/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/2.0.91/python'
+        self.user_agent = 'OpenAPI-Generator/2.0.92/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `tpdk-2.0.91/tpdk/api_response.py` & `tpdk-2.0.92/tpdk/api_response.py`

 * *Files identical despite different names*

### Comparing `tpdk-2.0.91/tpdk/configuration.py` & `tpdk-2.0.92/tpdk/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -409,16 +409,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.0.91\n"\
-               "SDK Package Version: 2.0.91".\
+               "Version of the API: 2.0.92\n"\
+               "SDK Package Version: 2.0.92".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `tpdk-2.0.91/tpdk/exceptions.py` & `tpdk-2.0.92/tpdk/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/__init__.py` & `tpdk-2.0.92/tpdk/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/address.py` & `tpdk-2.0.92/tpdk/models/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/address_independent_write.py` & `tpdk-2.0.92/tpdk/models/address_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/address_read.py` & `tpdk-2.0.92/tpdk/models/address_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/address_update.py` & `tpdk-2.0.92/tpdk/models/address_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/address_write.py` & `tpdk-2.0.92/tpdk/models/address_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/api_client_post_creation_read.py` & `tpdk-2.0.92/tpdk/models/api_client_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/api_client_read.py` & `tpdk-2.0.92/tpdk/models/api_client_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/api_client_write.py` & `tpdk-2.0.92/tpdk/models/api_client_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_collection_read.py` & `tpdk-2.0.92/tpdk/models/dispute_collection_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_dispute_read.py` & `tpdk-2.0.92/tpdk/models/dispute_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_independent_write.py` & `tpdk-2.0.92/tpdk/models/dispute_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_post_creation_read.py` & `tpdk-2.0.92/tpdk/models/dispute_post_creation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_read.py` & `tpdk-2.0.92/tpdk/models/dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_update.py` & `tpdk-2.0.92/tpdk/models/dispute_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/dispute_write.py` & `tpdk-2.0.92/tpdk/models/dispute_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/evaluation_read.py` & `tpdk-2.0.92/tpdk/models/evaluation_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/evaluation_write.py` & `tpdk-2.0.92/tpdk/models/evaluation_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/evidence.py` & `tpdk-2.0.92/tpdk/models/evidence.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -30,23 +30,34 @@
     dispute: Optional[StrictStr] = None
     owner: Optional[StrictStr] = None
     status: StrictStr = Field(...)
     media: Optional[StrictStr] = None
     additional_information: Optional[StrictStr] = Field(None, alias="additionalInformation", description="Description of what the evidence actually is.")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
     updated_at: Optional[datetime] = Field(None, alias="updatedAt")
-    __properties = ["id", "dispute", "owner", "status", "media", "additionalInformation", "createdAt", "updatedAt"]
+    publisher: Optional[StrictStr] = Field(None, description="Shortcut to whomever sent the evidence")
+    __properties = ["id", "dispute", "owner", "status", "media", "additionalInformation", "createdAt", "updatedAt", "publisher"]
 
     @validator('status')
     def status_validate_enum(cls, value):
         """Validates the enum"""
         if value not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
             raise ValueError("must be one of enum values ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED')")
         return value
 
+    @validator('publisher')
+    def publisher_validate_enum(cls, value):
+        """Validates the enum"""
+        if value is None:
+            return value
+
+        if value not in ('BUYER', 'PLATFORM', 'SELLER'):
+            raise ValueError("must be one of enum values ('BUYER', 'PLATFORM', 'SELLER')")
+        return value
+
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
@@ -64,14 +75,15 @@
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                             "id",
                             "created_at",
                             "updated_at",
+                            "publisher",
                           },
                           exclude_none=True)
         # set to None if dispute (nullable) is None
         # and __fields_set__ contains the field
         if self.dispute is None and "dispute" in self.__fields_set__:
             _dict['dispute'] = None
 
@@ -86,14 +98,19 @@
             _dict['media'] = None
 
         # set to None if updated_at (nullable) is None
         # and __fields_set__ contains the field
         if self.updated_at is None and "updated_at" in self.__fields_set__:
             _dict['updatedAt'] = None
 
+        # set to None if publisher (nullable) is None
+        # and __fields_set__ contains the field
+        if self.publisher is None and "publisher" in self.__fields_set__:
+            _dict['publisher'] = None
+
         return _dict
 
     @classmethod
     def from_dict(cls, obj: dict) -> Evidence:
         """Create an instance of Evidence from a dict"""
         if obj is None:
             return None
@@ -105,12 +122,13 @@
             "id": obj.get("id"),
             "dispute": obj.get("dispute"),
             "owner": obj.get("owner"),
             "status": obj.get("status") if obj.get("status") is not None else 'SUBMITTED',
             "media": obj.get("media"),
             "additional_information": obj.get("additionalInformation"),
             "created_at": obj.get("createdAt"),
-            "updated_at": obj.get("updatedAt")
+            "updated_at": obj.get("updatedAt"),
+            "publisher": obj.get("publisher")
         })
         return _obj
```

### Comparing `tpdk-2.0.91/tpdk/models/evidence_read.py` & `tpdk-2.0.92/tpdk/models/view.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 from datetime import datetime
 from typing import Optional
-from pydantic import BaseModel, Field, StrictInt, StrictStr, validator
-from tpdk.models.media_read import MediaRead
+from pydantic import BaseModel, Field, StrictInt, StrictStr
 
-class EvidenceRead(BaseModel):
+class View(BaseModel):
     """
       # noqa: E501
     """
     id: Optional[StrictInt] = None
-    status: StrictStr = Field(...)
-    media: Optional[MediaRead] = None
-    additional_information: Optional[StrictStr] = Field(None, alias="additionalInformation", description="Description of what the evidence actually is.")
+    ip_address: StrictStr = Field(..., alias="ipAddress")
+    offer: Optional[StrictStr] = None
+    dispute: Optional[StrictStr] = None
+    persona: Optional[StrictStr] = None
+    user: Optional[StrictStr] = None
+    hit_count: StrictInt = Field(..., alias="hitCount")
     created_at: Optional[datetime] = Field(None, alias="createdAt")
-    updated_at: Optional[datetime] = Field(None, alias="updatedAt")
-    __properties = ["id", "status", "media", "additionalInformation", "createdAt", "updatedAt"]
-
-    @validator('status')
-    def status_validate_enum(cls, value):
-        """Validates the enum"""
-        if value not in ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED'):
-            raise ValueError("must be one of enum values ('SUBMITTED', 'CORRELATED', 'UNRELATED', 'PENDING', 'TEMPERED', 'REJECTED')")
-        return value
+    __properties = ["id", "ipAddress", "offer", "dispute", "persona", "user", "hitCount", "createdAt"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -52,55 +46,63 @@
         return pprint.pformat(self.dict(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return json.dumps(self.to_dict())
 
     @classmethod
-    def from_json(cls, json_str: str) -> EvidenceRead:
-        """Create an instance of EvidenceRead from a JSON string"""
+    def from_json(cls, json_str: str) -> View:
+        """Create an instance of View from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self):
         """Returns the dictionary representation of the model using alias"""
         _dict = self.dict(by_alias=True,
                           exclude={
                             "id",
                             "created_at",
-                            "updated_at",
                           },
                           exclude_none=True)
-        # override the default output from pydantic by calling `to_dict()` of media
-        if self.media:
-            _dict['media'] = self.media.to_dict()
-        # set to None if media (nullable) is None
+        # set to None if offer (nullable) is None
+        # and __fields_set__ contains the field
+        if self.offer is None and "offer" in self.__fields_set__:
+            _dict['offer'] = None
+
+        # set to None if dispute (nullable) is None
+        # and __fields_set__ contains the field
+        if self.dispute is None and "dispute" in self.__fields_set__:
+            _dict['dispute'] = None
+
+        # set to None if persona (nullable) is None
         # and __fields_set__ contains the field
-        if self.media is None and "media" in self.__fields_set__:
-            _dict['media'] = None
+        if self.persona is None and "persona" in self.__fields_set__:
+            _dict['persona'] = None
 
-        # set to None if updated_at (nullable) is None
+        # set to None if user (nullable) is None
         # and __fields_set__ contains the field
-        if self.updated_at is None and "updated_at" in self.__fields_set__:
-            _dict['updatedAt'] = None
+        if self.user is None and "user" in self.__fields_set__:
+            _dict['user'] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> EvidenceRead:
-        """Create an instance of EvidenceRead from a dict"""
+    def from_dict(cls, obj: dict) -> View:
+        """Create an instance of View from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
-            return EvidenceRead.parse_obj(obj)
+            return View.parse_obj(obj)
 
-        _obj = EvidenceRead.parse_obj({
+        _obj = View.parse_obj({
             "id": obj.get("id"),
-            "status": obj.get("status") if obj.get("status") is not None else 'SUBMITTED',
-            "media": MediaRead.from_dict(obj.get("media")) if obj.get("media") is not None else None,
-            "additional_information": obj.get("additionalInformation"),
-            "created_at": obj.get("createdAt"),
-            "updated_at": obj.get("updatedAt")
+            "ip_address": obj.get("ipAddress"),
+            "offer": obj.get("offer"),
+            "dispute": obj.get("dispute"),
+            "persona": obj.get("persona"),
+            "user": obj.get("user"),
+            "hit_count": obj.get("hitCount") if obj.get("hitCount") is not None else 1,
+            "created_at": obj.get("createdAt")
         })
         return _obj
```

### Comparing `tpdk-2.0.91/tpdk/models/evidence_write.py` & `tpdk-2.0.92/tpdk/models/evidence_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -22,15 +22,15 @@
 
 from pydantic import BaseModel, Field, constr
 
 class EvidenceWrite(BaseModel):
     """
       # noqa: E501
     """
-    additional_information: constr(strict=True, max_length=500) = Field(..., alias="additionalInformation", description="Description of what the evidence actually is.")
+    additional_information: constr(strict=True, max_length=500, min_length=10) = Field(..., alias="additionalInformation", description="Description of what the evidence actually is.")
     __properties = ["additionalInformation"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
```

### Comparing `tpdk-2.0.91/tpdk/models/media.py` & `tpdk-2.0.92/tpdk/models/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/media_authenticated_read.py` & `tpdk-2.0.92/tpdk/models/media_authenticated_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/media_collection_read.py` & `tpdk-2.0.92/tpdk/models/media_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/media_dispute_read.py` & `tpdk-2.0.92/tpdk/models/media_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/media_read.py` & `tpdk-2.0.92/tpdk/models/media_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata.py` & `tpdk-2.0.92/tpdk/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata_dispute_read.py` & `tpdk-2.0.92/tpdk/models/metadata_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata_independent_write.py` & `tpdk-2.0.92/tpdk/models/metadata_independent_write.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata_read.py` & `tpdk-2.0.92/tpdk/models/metadata_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata_update.py` & `tpdk-2.0.92/tpdk/models/metadata_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/metadata_write.py` & `tpdk-2.0.92/tpdk/models/metadata_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/notification_read.py` & `tpdk-2.0.92/tpdk/models/notification_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/notification_update.py` & `tpdk-2.0.92/tpdk/models/notification_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer.py` & `tpdk-2.0.92/tpdk/models/offer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_collection_read.py` & `tpdk-2.0.92/tpdk/models/offer_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_dispute_read.py` & `tpdk-2.0.92/tpdk/models/offer_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_independent_write.py` & `tpdk-2.0.92/tpdk/models/offer_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_post_creation_read.py` & `tpdk-2.0.92/tpdk/models/offer_post_creation_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_read.py` & `tpdk-2.0.92/tpdk/models/offer_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_update.py` & `tpdk-2.0.92/tpdk/models/offer_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/offer_write.py` & `tpdk-2.0.92/tpdk/models/offer_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_authenticated_read.py` & `tpdk-2.0.92/tpdk/models/organization_authenticated_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_collection_read.py` & `tpdk-2.0.92/tpdk/models/organization_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_dispute_read.py` & `tpdk-2.0.92/tpdk/models/organization_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_read.py` & `tpdk-2.0.92/tpdk/models/organization_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_update.py` & `tpdk-2.0.92/tpdk/models/organization_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/organization_write.py` & `tpdk-2.0.92/tpdk/models/organization_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/parcel.py` & `tpdk-2.0.92/tpdk/models/parcel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/parcel_dispute_read.py` & `tpdk-2.0.92/tpdk/models/parcel_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/parcel_independent_write.py` & `tpdk-2.0.92/tpdk/models/parcel_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/parcel_read.py` & `tpdk-2.0.92/tpdk/models/parcel_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/parcel_write.py` & `tpdk-2.0.92/tpdk/models/parcel_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona.py` & `tpdk-2.0.92/tpdk/models/persona.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_auth_return.py` & `tpdk-2.0.92/tpdk/models/persona_auth_return.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_collection_read.py` & `tpdk-2.0.92/tpdk/models/persona_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_external_auth.py` & `tpdk-2.0.92/tpdk/models/persona_external_auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_independent_write.py` & `tpdk-2.0.92/tpdk/models/persona_independent_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_post_auth_read.py` & `tpdk-2.0.92/tpdk/models/persona_post_auth_read.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_read.py` & `tpdk-2.0.92/tpdk/models/persona_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_register.py` & `tpdk-2.0.92/tpdk/models/persona_register.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_token_write.py` & `tpdk-2.0.92/tpdk/models/persona_token_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_update.py` & `tpdk-2.0.92/tpdk/models/persona_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/persona_write.py` & `tpdk-2.0.92/tpdk/models/persona_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/transaction_collection_read.py` & `tpdk-2.0.92/tpdk/models/transaction_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/transaction_dispute_read.py` & `tpdk-2.0.92/tpdk/models/transaction_dispute_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/transaction_independent_write.py` & `tpdk-2.0.92/tpdk/models/transaction_independent_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/transaction_read.py` & `tpdk-2.0.92/tpdk/models/transaction_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/unprocessable_entity.py` & `tpdk-2.0.92/tpdk/models/unprocessable_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/unprocessable_entity_violations_inner.py` & `tpdk-2.0.92/tpdk/models/unprocessable_entity_violations_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user.py` & `tpdk-2.0.92/tpdk/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_authenticated_read.py` & `tpdk-2.0.92/tpdk/models/user_authenticated_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_collection_read.py` & `tpdk-2.0.92/tpdk/models/user_collection_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_email_validation_write.py` & `tpdk-2.0.92/tpdk/models/user_email_validation_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_invite.py` & `tpdk-2.0.92/tpdk/models/user_invite.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_post_register_read.py` & `tpdk-2.0.92/tpdk/models/user_post_register_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_update.py` & `tpdk-2.0.92/tpdk/models/user_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/user_write.py` & `tpdk-2.0.92/tpdk/models/user_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook.py` & `tpdk-2.0.92/tpdk/models/webhook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook_history_collection_read.py` & `tpdk-2.0.92/tpdk/models/webhook_history_collection_read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook_history_read.py` & `tpdk-2.0.92/tpdk/models/webhook_history_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook_object.py` & `tpdk-2.0.92/tpdk/models/webhook_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook_subscription_read.py` & `tpdk-2.0.92/tpdk/models/webhook_subscription_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/webhook_subscription_write.py` & `tpdk-2.0.92/tpdk/models/webhook_subscription_write.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/workflow_event_dispute_read.py` & `tpdk-2.0.92/tpdk/models/workflow_event_dispute_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/models/workflow_event_read.py` & `tpdk-2.0.92/tpdk/models/workflow_event_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk/rest.py` & `tpdk-2.0.92/tpdk/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Tripartie
 
     Our API suite for the **Resolution Center** and the **Safe Checkout** features. Simple, yet elegant web interfaces for your convenience. One request away from your first automated resolution or safe-checkout.
 
-    The version of the OpenAPI document: 2.0.91
+    The version of the OpenAPI document: 2.0.92
     Contact: noc@tripartie.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `tpdk-2.0.91/tpdk.egg-info/PKG-INFO` & `tpdk-2.0.92/tpdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpdk
-Version: 2.0.91
+Version: 2.0.92
 Summary: Tripartie
 Home-page: https://pypi.org/project/tpdk
 Author: Tripartie SAS
 Author-email: noc@tripartie.com
 Keywords: OpenAPI,OpenAPI-Generator,Tripartie
 Description-Content-Type: text/markdown
 Requires-Dist: urllib3<2.1.0,>=1.25.3
```

### Comparing `tpdk-2.0.91/tpdk.egg-info/SOURCES.txt` & `tpdk-2.0.92/tpdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

