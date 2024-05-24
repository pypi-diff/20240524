# Comparing `tmp/mistapi-0.47.5.tar.gz` & `tmp/mistapi-0.48.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistapi-0.47.5.tar", last modified: Tue May 14 11:12:49 2024, max compression
+gzip compressed data, was "mistapi-0.48.0.tar", last modified: Fri May 24 08:32:23 2024, max compression
```

## Comparing `mistapi-0.47.5.tar` & `mistapi-0.48.0.tar`

### file list

```diff
@@ -1,251 +1,255 @@
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.327151 mistapi-0.47.5/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.47.5/LICENSE
--rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-14 11:12:49.326999 mistapi-0.47.5/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.47.5/README.md
--rw-r--r--   0 tmunzer    (502) staff       (20)      977 2024-05-14 11:12:44.000000 mistapi-0.47.5/pyproject.toml
--rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-05-14 11:12:49.328731 mistapi-0.47.5/setup.cfg
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.265611 mistapi-0.47.5/src/
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.270341 mistapi-0.47.5/src/mistapi/
--rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.47.5/src/mistapi/__api_request.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.47.5/src/mistapi/__api_response.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    34436 2024-05-14 11:10:23.000000 mistapi-0.47.5/src/mistapi/__api_session.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.47.5/src/mistapi/__logger.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.271508 mistapi-0.47.5/src/mistapi/__models/
--rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.47.5/src/mistapi/__models/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.47.5/src/mistapi/__models/privilege.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.47.5/src/mistapi/__pagination.py
--rw-r--r--   0 tmunzer    (502) staff       (20)       74 2023-10-10 14:55:37.000000 mistapi-0.47.5/src/mistapi/__version.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.271679 mistapi-0.47.5/src/mistapi/api/
--rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.271829 mistapi-0.47.5/src/mistapi/api/v1/
--rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.274651 mistapi-0.47.5/src/mistapi/api/v1/const/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1341 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/alarm_defs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/ap_channels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/ap_led_status.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/client_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/countries.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1412 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/default_gateway_config.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/device_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/device_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/gateway_applications.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/insight_metrics.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/languages.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/license_types.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/mxedge_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/mxedge_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1779 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/nac_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1835 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/otherdevice_events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1825 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/otherdevice_models.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/const/traffic_types.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.274798 mistapi-0.47.5/src/mistapi/api/v1/installer/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/__init__.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.276117 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)      798 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7099 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8000 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/sites.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.276492 mistapi-0.47.5/src/mistapi/api/v1/installer/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/installer/sites/optimize.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.276808 mistapi-0.47.5/src/mistapi/api/v1/invite/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/invite/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/invite/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.277524 mistapi-0.47.5/src/mistapi/api/v1/login/
--rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/login/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/login/login.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/login/lookup.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/login/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/login/two_factor.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.277843 mistapi-0.47.5/src/mistapi/api/v1/logout/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/logout/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/logout/logout.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.278142 mistapi-0.47.5/src/mistapi/api/v1/mobile/
--rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/mobile/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/mobile/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.281425 mistapi-0.47.5/src/mistapi/api/v1/msps/
--rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1683 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/logo.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4542 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/msps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/orggroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6691 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1674 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/search.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7398 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/suggestion.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/msps/tickets.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.294215 mistapi-0.47.5/src/mistapi/api/v1/orgs/
--rw-r--r--   0 tmunzer    (502) staff       (20)     3378 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/admins.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8412 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/alarmtemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5245 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6580 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2337 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/cert.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/claim.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12343 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/clone.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/crl.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19522 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5295 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/idpprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2959 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6616 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/inventory.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/invites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/jsi.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5309 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/mist_nac.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5237 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/mxclusters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    24910 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12704 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/nacrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5101 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/nactags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5355 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1417 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/ocdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/orgs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9689 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2365 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/pma.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    10543 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/pskportals.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sdkclients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sdkinvites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sdktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5204 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/secpolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5308 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    19166 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5185 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sitegroups.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9353 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5271 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/ssoroles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8754 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/ssos.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5758 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    32781 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5940 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/templates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7361 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/tickets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1764 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/troubleshoot.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/vars.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5024 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1374 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4985 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7229 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3722 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7464 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5729 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6385 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/orgs/wxtunnels.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.294654 mistapi-0.47.5/src/mistapi/api/v1/recover/
--rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/recover/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/recover/recover.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/recover/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.295236 mistapi-0.47.5/src/mistapi/api/v1/register/
--rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/register/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/register/recaptcha.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/register/register.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/register/verify.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.297222 mistapi-0.47.5/src/mistapi/api/v1/self/
--rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4317 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/apitokens.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/logs.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/oauth.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/self.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1953 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/two_factor.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/self/update.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.325056 mistapi-0.47.5/src/mistapi/api/v1/sites/
--rw-r--r--   0 tmunzer    (502) staff       (20)     2876 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8779 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/alarms.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/anomaly.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/apps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/aptemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5280 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/assetfilters.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6629 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/assets.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5142 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/beacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2349 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/call.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    18402 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2418 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/count.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2356 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/deviceprofiles.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    65592 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/devices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4040 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/events.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     4114 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/evpn_topologies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/gatewaytemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7121 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/guests.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/insights.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/licenses.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7146 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/location.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    16638 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/maps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     9250 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/mxedges.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/mxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    12392 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/nac_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2314 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/networks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1373 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/networktemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5875 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/otherdevices.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5899 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/pcaps.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/psks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/rfdiags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1358 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/rftemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5809 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/rogues.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3862 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/rrm.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/rssizones.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2363 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/servicepolicies.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6185 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/services.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/setting.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/sites.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1364 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/sitetemplates.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3886 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/skyatp.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    20772 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/sle.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/ssr.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    66094 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/stats.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/subscriptions.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1928 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/synthetic_test.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5425 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/uisettings.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5166 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/vbeacons.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2308 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/visits.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/vpns.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1380 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wan_client.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5003 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wan_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     7212 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/webhooks.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     3986 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wired_clients.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     8790 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wlans.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5772 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wxrules.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     6434 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wxtags.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/wxtunnels.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     5082 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/sites/zones.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.326298 mistapi-0.47.5/src/mistapi/api/v1/utils/
--rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/utils/__init__.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/utils/test_telstra.py
--rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-05-14 11:12:44.000000 mistapi-0.47.5/src/mistapi/api/v1/utils/test_twilio.py
--rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.47.5/src/mistapi/cli.py
-drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-14 11:12:49.326548 mistapi-0.47.5/src/mistapi.egg-info/
--rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-14 11:12:49.000000 mistapi-0.47.5/src/mistapi.egg-info/PKG-INFO
--rw-r--r--   0 tmunzer    (502) staff       (20)     8339 2024-05-14 11:12:49.000000 mistapi-0.47.5/src/mistapi.egg-info/SOURCES.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-05-14 11:12:49.000000 mistapi-0.47.5/src/mistapi.egg-info/dependency_links.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-05-14 11:12:49.000000 mistapi-0.47.5/src/mistapi.egg-info/requires.txt
--rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-05-14 11:12:49.000000 mistapi-0.47.5/src/mistapi.egg-info/top_level.txt
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.119171 mistapi-0.48.0/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2023-01-13 07:55:51.000000 mistapi-0.48.0/LICENSE
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-24 08:32:23.119036 mistapi-0.48.0/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10541 2023-10-05 14:00:29.000000 mistapi-0.48.0/README.md
+-rw-r--r--   0 tmunzer    (502) staff       (20)      977 2024-05-24 08:32:05.000000 mistapi-0.48.0/pyproject.toml
+-rw-r--r--   0 tmunzer    (502) staff       (20)      125 2024-05-24 08:32:23.119412 mistapi-0.48.0/setup.cfg
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.066983 mistapi-0.48.0/src/
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.072439 mistapi-0.48.0/src/mistapi/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    15410 2023-10-10 06:25:01.000000 mistapi-0.48.0/src/mistapi/__api_request.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3275 2023-10-10 08:14:00.000000 mistapi-0.48.0/src/mistapi/__api_response.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    34436 2024-05-14 11:10:23.000000 mistapi-0.48.0/src/mistapi/__api_session.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      615 2024-05-24 08:32:05.000000 mistapi-0.48.0/src/mistapi/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2297 2023-10-19 16:39:16.000000 mistapi-0.48.0/src/mistapi/__logger.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.073783 mistapi-0.48.0/src/mistapi/__models/
+-rw-r--r--   0 tmunzer    (502) staff       (20)        0 2023-02-21 08:35:01.000000 mistapi-0.48.0/src/mistapi/__models/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1530 2023-05-30 09:43:55.000000 mistapi-0.48.0/src/mistapi/__models/privilege.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2079 2023-10-10 06:34:01.000000 mistapi-0.48.0/src/mistapi/__pagination.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)       74 2023-10-10 14:55:37.000000 mistapi-0.48.0/src/mistapi/__version.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.074023 mistapi-0.48.0/src/mistapi/api/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      446 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.074151 mistapi-0.48.0/src/mistapi/api/v1/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      869 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.078155 mistapi-0.48.0/src/mistapi/api/v1/const/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1490 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/alarm_defs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2047 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/ap_channels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1760 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/ap_led_status.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1797 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/app_categories.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1818 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/app_subcategories.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1743 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/client_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1737 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/countries.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1274 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/default_gateway_config.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/device_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/device_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1794 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/gateway_applications.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1759 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/insight_metrics.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1742 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/languages.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1070 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/license_types.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/mxedge_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/mxedge_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1779 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/nac_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1835 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/otherdevice_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1825 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/otherdevice_models.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1800 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/system_events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1745 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/const/traffic_types.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.078293 mistapi-0.48.0/src/mistapi/api/v1/installer/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/__init__.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.079490 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      798 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1988 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2304 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11082 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1992 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1967 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1960 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8000 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/sites.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.079812 mistapi-0.48.0/src/mistapi/api/v1/installer/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      471 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1178 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/installer/sites/optimize.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.080089 mistapi-0.48.0/src/mistapi/api/v1/invite/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/invite/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1109 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/invite/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.080742 mistapi-0.48.0/src/mistapi/api/v1/login/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      584 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/login/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1154 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/login/login.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1163 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/login/lookup.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2656 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/login/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1173 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/login/two_factor.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.080993 mistapi-0.48.0/src/mistapi/api/v1/logout/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/logout/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)      999 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/logout/logout.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.081328 mistapi-0.48.0/src/mistapi/api/v1/mobile/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      460 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/mobile/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1270 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/mobile/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.084758 mistapi-0.48.0/src/mistapi/api/v1/msps/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1104 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3925 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1625 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1210 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2653 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1851 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/logo.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4392 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3032 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/msps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/orggroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6589 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1662 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/search.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4048 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7398 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3709 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1518 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/suggestion.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3269 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/msps/tickets.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.101917 mistapi-0.48.0/src/mistapi/api/v1/orgs/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3465 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3288 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/admins.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6526 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8412 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/alarmtemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4725 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5245 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6580 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1729 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/cert.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1263 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/claim.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11110 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1249 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/clone.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1869 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/crl.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7161 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18238 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5295 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5353 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6601 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/idpprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2878 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6362 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/inventory.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2693 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/invites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7004 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/jsi.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2536 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5172 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1931 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1293 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/mist_nac.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5237 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/mxclusters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    22922 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10477 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9109 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/nacportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/nacrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5385 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/nactags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5355 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1323 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/ocdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3018 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/orgs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9487 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4820 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2365 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/pma.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10500 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/pskportals.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8448 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5213 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1324 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sdkclients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6964 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sdkinvites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4770 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sdktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5204 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/secpolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5308 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    19138 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5185 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sitegroups.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8775 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5271 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5129 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/ssoroles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8754 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/ssos.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5758 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    29814 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1767 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5940 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/templates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7361 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/tickets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1592 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/troubleshoot.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4636 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/usermacs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1611 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/vars.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5024 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1780 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4604 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7352 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3553 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7464 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5729 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6385 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5157 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/orgs/wxtunnels.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.102376 mistapi-0.48.0/src/mistapi/api/v1/recover/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      505 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/recover/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1176 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/recover/recover.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1120 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/recover/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.102982 mistapi-0.48.0/src/mistapi/api/v1/register/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      555 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/register/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1308 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/register/recaptcha.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1179 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/register/register.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1113 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/register/verify.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.104391 mistapi-0.48.0/src/mistapi/api/v1/self/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      707 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4317 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/apitokens.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2654 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/logs.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2033 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/oauth.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2157 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/self.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1773 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1890 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/two_factor.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1784 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/self/update.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.117821 mistapi-0.48.0/src/mistapi/api/v1/sites/
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2837 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8111 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/alarms.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2660 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/anomaly.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1881 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/apps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/aptemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5280 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/assetfilters.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6629 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/assets.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5142 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/beacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    17220 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2286 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/count.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2272 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/deviceprofiles.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    66075 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/devices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3933 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/events.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4900 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/evpn_topologies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/gatewaytemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8945 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/guests.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     9228 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/insights.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1167 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/licenses.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6914 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/location.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    16638 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/maps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8710 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/mxedges.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1189 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/mxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    10279 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/nac_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2230 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/networks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1331 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/networktemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5708 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/otherdevices.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5831 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/pcaps.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7696 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/psks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5817 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/rfdiags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1316 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/rftemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5113 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/rogues.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4765 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/rrm.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/rssizones.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2279 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/servicepolicies.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6105 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/services.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6746 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/setting.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2437 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/sites.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1322 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/sitetemplates.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3624 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/skyatp.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    18950 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/sle.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1983 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/ssr.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    63607 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/stats.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1751 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/subscriptions.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3150 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/synthetic_test.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5425 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/uisettings.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5166 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/vbeacons.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2176 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/visits.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     2202 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/vpns.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1786 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wan_client.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     4622 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wan_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     7212 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/webhooks.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     3770 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wired_clients.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8668 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wlans.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5772 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wxrules.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     6434 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wxtags.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5194 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/wxtunnels.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     5082 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/sites/zones.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.118390 mistapi-0.48.0/src/mistapi/api/v1/utils/
+-rw-r--r--   0 tmunzer    (502) staff       (20)      511 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/utils/__init__.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1205 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/utils/test_telstra.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)     1202 2024-05-24 08:32:08.000000 mistapi-0.48.0/src/mistapi/api/v1/utils/test_twilio.py
+-rw-r--r--   0 tmunzer    (502) staff       (20)    13223 2023-10-11 11:11:09.000000 mistapi-0.48.0/src/mistapi/cli.py
+drwxr-xr-x   0 tmunzer    (502) staff       (20)        0 2024-05-24 08:32:23.118655 mistapi-0.48.0/src/mistapi.egg-info/
+-rw-r--r--   0 tmunzer    (502) staff       (20)    11444 2024-05-24 08:32:23.000000 mistapi-0.48.0/src/mistapi.egg-info/PKG-INFO
+-rw-r--r--   0 tmunzer    (502) staff       (20)     8512 2024-05-24 08:32:23.000000 mistapi-0.48.0/src/mistapi.egg-info/SOURCES.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        1 2024-05-24 08:32:23.000000 mistapi-0.48.0/src/mistapi.egg-info/dependency_links.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)       66 2024-05-24 08:32:23.000000 mistapi-0.48.0/src/mistapi.egg-info/requires.txt
+-rw-r--r--   0 tmunzer    (502) staff       (20)        8 2024-05-24 08:32:23.000000 mistapi-0.48.0/src/mistapi.egg-info/top_level.txt
```

### Comparing `mistapi-0.47.5/LICENSE` & `mistapi-0.48.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/PKG-INFO` & `mistapi-0.48.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.47.5
+Version: 0.48.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.47.5/README.md` & `mistapi-0.48.0/README.md`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/pyproject.toml` & `mistapi-0.48.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mistapi"
-version = "0.47.5"
+version = "0.48.0"
 authors = [{name="Thomas Munzer", email="tmunzer@juniper.net"}]
 description = "Python package to simplify the Mist System APIs usage"
 keywords = ["Mist", "Juniper", "API"]
 license = {text =  "MIT"}
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `mistapi-0.47.5/src/mistapi/__api_request.py` & `mistapi-0.48.0/src/mistapi/__api_request.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__api_response.py` & `mistapi-0.48.0/src/mistapi/__api_response.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__api_session.py` & `mistapi-0.48.0/src/mistapi/__api_session.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__init__.py` & `mistapi-0.48.0/src/mistapi/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__logger.py` & `mistapi-0.48.0/src/mistapi/__logger.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__models/privilege.py` & `mistapi-0.48.0/src/mistapi/__models/privilege.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/__pagination.py` & `mistapi-0.48.0/src/mistapi/__pagination.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 --------------------------------------------------------------------------------
 '''
 
 from mistapi.api.v1.const import alarm_defs
 from mistapi.api.v1.const import ap_channels
 from mistapi.api.v1.const import ap_led_status
+from mistapi.api.v1.const import app_categories
+from mistapi.api.v1.const import app_subcategories
 from mistapi.api.v1.const import applications
 from mistapi.api.v1.const import client_events
 from mistapi.api.v1.const import countries
 from mistapi.api.v1.const import default_gateway_config
 from mistapi.api.v1.const import device_events
 from mistapi.api.v1.const import device_models
 from mistapi.api.v1.const import gateway_applications
@@ -24,8 +26,9 @@
 from mistapi.api.v1.const import languages
 from mistapi.api.v1.const import license_types
 from mistapi.api.v1.const import mxedge_events
 from mistapi.api.v1.const import mxedge_models
 from mistapi.api.v1.const import nac_events
 from mistapi.api.v1.const import otherdevice_events
 from mistapi.api.v1.const import otherdevice_models
+from mistapi.api.v1.const import system_events
 from mistapi.api.v1.const import traffic_types
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/alarm_defs.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/alarm_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listAlarmDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listAlarmDefinitions")  
 def getAlarmDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/ap_channels.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/ap_channels.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listApChannels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listApChannels")  
 def getApChannels(mist_session:_APISession, country_code:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApChannels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/ap_led_status.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/ap_led_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listApLedDefinition")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listApLedDefinition")  
 def getApLedDefinition(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApLedDefinition
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/applications.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listApplications")  
 def getApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/client_events.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/client_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listClientEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listClientEventsDefinitions")  
 def getClientEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listClientEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/countries.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/countries.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listCountryCodes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listCountryCodes")  
 def getCountryCodes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listCountryCodes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/default_gateway_config.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/sitetemplates.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getGatawayDefaultConfig(mist_session:_APISession, model:str, ha:str=None) -> _APIResponse:
+def getSiteSiteTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getGatawayDefaultConfig
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSiteTemplateDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
     QUERY PARAMS
     ------------
-    model : str
-      model the default gateway config is intended (as the default LAN/WAN port can differ)
-    ha : str
-      whether the config is intended for HA        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/const/default_gateway_config"
+    uri = f"/api/v1/sites/{site_id}/sitetemplates/derived"
     query_params={}
-    if model: query_params["model"]=model
-    if ha: query_params["ha"]=ha
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/device_events.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/device_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listDeviceEventsDefinitions")  
 def getDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/device_models.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/device_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listDeviceModels")  
 def getDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/gateway_applications.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/gateway_applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listGatewayApplications")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listGatewayApplications")  
 def getGatewayApplications(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listGatewayApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/insight_metrics.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/insight_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInsightMetrics")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInsightMetrics")  
 def getInsightMetrics(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInsightMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/languages.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/languages.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteLanguages")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteLanguages")  
 def getSiteLanguages(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteLanguages
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/license_types.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/license_types.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/mxedge_events.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/mxedge_events.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMxEdgeEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMxEdgeEventsDefinitions")  
 def getMxEdgeEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/mxedge_models.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/mxedge_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMxEdgeModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMxEdgeModels")  
 def getMxEdgeModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMxEdgeModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/nac_events.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/nac_events.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listNacEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listNacEventsDefinitions")  
 def getNacEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listNacEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/otherdevice_events.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/otherdevice_events.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOtherDeviceEventsDefinitions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOtherDeviceEventsDefinitions")  
 def getOtherDeviceEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOtherDeviceEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/otherdevice_models.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/otherdevice_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSupportedOtherDeviceModels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSupportedOtherDeviceModels")  
 def getSupportedOtherDeviceModels(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSupportedOtherDeviceModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/const/traffic_types.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/traffic_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listTrafficTypes")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listTrafficTypes")  
 def getTrafficTypes(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listTrafficTypes
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/alarmtemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerAlarmTemplates")  
 def getInstallerAlarmTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/deviceprofiles.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/secpolicies.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerDeviceProfiles")  
-def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerSecPolicies")  
+def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +29,22 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/deviceprofiles"
+    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listInstallerDeviceProfiles(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,12 +52,12 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/deviceprofiles"
+    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/devices.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/assets.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,64 +10,78 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerListOfRenctlyClaimedDevices")  
-def getInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAssets")  
+def getOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
+    QUERY PARAMS
+    ------------
+    page : int, default: 1
+    limit : int, default: 100        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/assets"
+    query_params={}
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listInstallerListOfRenctlyClaimedDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerListOfRenctlyClaimedDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
+    QUERY PARAMS
+    ------------
+    page : int, default: 1
+    limit : int, default: 100        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices"
-    query_params={}
+    uri = f"/api/v1/orgs/{org_id}/assets"
+    query_params={}
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def claimInstallerDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgAsset(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/claimInstallerDevices
+    API doc: https://doc.mist-lab.fr/#operation/createOrgAsset
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -80,159 +94,144 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices"
+    uri = f"/api/v1/orgs/{org_id}/assets"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def unassignInstallerRecentlyClaimedDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def importOrgAssetsFile(mist_session:_APISession, org_id:str, file:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unassignInstallerRecentlyClaimedDevice
+    API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    device_mac : str        
+    org_id : str        
+    
+    BODY PARAMS
+    -----------
+    file : str
+        path to the file to upload. CSV file
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    multipart_form_data = {
+        "file":file,
+    }
+    uri = f"/api/v1/orgs/{org_id}/assets/import"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
-    
-def provisionInstallerDevices(mist_session:_APISession, org_id:str, device_mac:str, body:object) -> _APIResponse:
+
+def importOrgAssets(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/provisionInstallerDevices
+    API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    device_mac : str        
+    org_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def startInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/startInstallerLocateDevice
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    device_mac : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/locate"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}/assets/import"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def stopInstallerLocateDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
+def getOrgAsset(mist_session:_APISession, org_id:str, asset_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/stopInstallerLocateDevice
+    API doc: https://doc.mist-lab.fr/#operation/getOrgAsset
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    device_mac : str        
+    asset_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/unlocate"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteInstallerDeviceImage(mist_session:_APISession, org_id:str, image_name:str, device_mac:str) -> _APIResponse:
+def deleteOrgAsset(mist_session:_APISession, org_id:str, asset_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteInstallerDeviceImage
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgAsset
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    image_name : str
-    device_mac : str        
+    asset_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
+    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addInstallerDeviceImageFile(mist_session:_APISession, org_id:str, image_name:str, device_mac:str) -> _APIResponse:
+def updateOrgAsset(mist_session:_APISession, org_id:str, asset_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addInstallerDeviceImage
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgAsset
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    image_name : str
-    device_mac : str        
+    asset_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    multipart_form_data = {
-    }
-    uri = f"/api/v1/installer/orgs/{org_id}/devices/{device_mac}/{image_name}"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
+
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/rftemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerRfTemplatesNames")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerRfTemplatesNames")  
 def getInstallerRfTemplatesNames(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerRfTemplatesNames
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/secpolicies.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/licenses.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,18 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerSecPolicies")  
-def getInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -29,22 +28,49 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
+    uri = f"/api/v1/orgs/{org_id}/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listInstallerSecPolicies(mist_session:_APISession, org_id:str) -> _APIResponse:
+def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listInstallerSecPolicies
+    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    org_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/orgs/{org_id}/licenses"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
+    
+def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -52,12 +78,12 @@
     org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/installer/orgs/{org_id}/secpolicies"
+    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/sitegroups.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/sitegroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerSiteGroups")  
 def getInstallerSiteGroups(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/orgs/sites.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/sites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerSites")  
 def getInstallerSites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -85,15 +85,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/installer/orgs/{org_id}/sites/{site_name}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listInstallerMaps")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerMaps")  
 def getInstallerMaps(mist_session:_APISession, org_id:str, site_name:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listInstallerMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/installer/sites/optimize.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/sites/optimize.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/invite/verify.py` & `mistapi-0.48.0/src/mistapi/api/v1/invite/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/login/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/login/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/login/login.py` & `mistapi-0.48.0/src/mistapi/api/v1/login/login.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/login/lookup.py` & `mistapi-0.48.0/src/mistapi/api/v1/login/lookup.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/login/oauth.py` & `mistapi-0.48.0/src/mistapi/api/v1/login/oauth.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOAuth2AuthorizationUrlForLogin(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
+def getOauth2AuthorizationUrlForLogin(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOAuth2AuthorizationUrlForLogin
+    API doc: https://doc.mist-lab.fr/#operation/getOauth2AuthorizationUrlForLogin
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -38,17 +38,17 @@
     """
     uri = f"/api/v1/login/oauth/{provider}"
     query_params={}
     if forward: query_params["forward"]=forward
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def unlinkOAuth2Provider(mist_session:_APISession, provider:str) -> _APIResponse:
+def unlinkOauth2Provider(mist_session:_APISession, provider:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unlinkOAuth2Provider
+    API doc: https://doc.mist-lab.fr/#operation/unlinkOauth2Provider
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -61,17 +61,17 @@
         response from the API call
     """
     uri = f"/api/v1/login/oauth/{provider}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def loginOAuth2(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
+def loginOauth2(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/loginOAuth2
+    API doc: https://doc.mist-lab.fr/#operation/loginOauth2
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/login/two_factor.py` & `mistapi-0.48.0/src/mistapi/api/v1/login/two_factor.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/logout/logout.py` & `mistapi-0.48.0/src/mistapi/api/v1/logout/logout.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/mobile/verify.py` & `mistapi-0.48.0/src/mistapi/api/v1/mobile/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/admins.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/admins.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspAdmins")  
 def getMspAdmins(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/claim.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/insights.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/insights.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     -----------
     msp_id : str
     metric : str        
     
     QUERY PARAMS
     ------------
     sle : str
-      see /api/v1/const/insight_metrics for more details
     duration : str, default: 1d
     interval : str
     start : int
     end : int        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/inventory.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/inventory.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/invites.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/licenses.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/licenses.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspLicenses")  
 def getMspLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/logo.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/logo.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/logs.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/logs.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspLogs")  
 def getMspLogs(mist_session:_APISession, msp_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -27,21 +27,17 @@
     PATH PARAMS
     -----------
     msp_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      site id
     admin_name : str
-      admin name or email
     message : str
-      message
     sort : str{'timestamp', '-timestamp', 'site_id', 'admin_id'}
-      sort order
     start : int
     end : int
     limit : int, default: 100
     page : int, default: 1
     duration : str, default: 1d        
     
     RETURN
@@ -75,21 +71,17 @@
     PATH PARAMS
     -----------
     msp_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      site id
     admin_name : str
-      admin name or email
     message : str
-      message
     sort : str{'timestamp', '-timestamp', 'site_id', 'admin_id'}
-      sort order
     start : int
     end : int
     limit : int, default: 100
     page : int, default: 1
     duration : str, default: 1d        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/msps.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/msps.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/orggroups.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/orggroups.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspOrgGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspOrgGroups")  
 def getMspOrgGroups(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/orgs.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/orgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspOrgs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspOrgs")  
 def getMspOrgs(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -128,19 +128,16 @@
     -----------
     msp_id : str        
     
     QUERY PARAMS
     ------------
     name : str
     org_id : str
-      org id
     sub_insufficient : bool
-      if this org has sufficient subscription
     trial_enabled : bool
-      if this org is under trial period
     usage_types : list
       a list of types that enabled by usage
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/search.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     PATH PARAMS
     -----------
     msp_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'orgs'}
-      orgs
     q : str
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/ssoroles.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspSsoRoles")  
 def getMspSsoRoles(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/ssos.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/ssos.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspSsos")  
 def getMspSsos(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -160,15 +160,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspSsoLatestFailures")  
 def getMspSsoLatestFailures(mist_session:_APISession, msp_id:str, sso_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/stats.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspOrgLicenses")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspOrgLicenses")  
 def getMspOrgLicenses(mist_session:_APISession, msp_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgLicenses
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/msps/{msp_id}/stats/licenses"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspOrgStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspOrgStats")  
 def getMspOrgStats(mist_session:_APISession, msp_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspOrgStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/suggestion.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/suggestion.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/msps/tickets.py` & `mistapi-0.48.0/src/mistapi/api/v1/msps/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listMspTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listMspTickets")  
 def getMspTickets(mist_session:_APISession, msp_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listMspTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from mistapi.api.v1.orgs import admins
 from mistapi.api.v1.orgs import alarms
 from mistapi.api.v1.orgs import alarmtemplates
 from mistapi.api.v1.orgs import apitokens
 from mistapi.api.v1.orgs import aptemplates
 from mistapi.api.v1.orgs import assetfilters
 from mistapi.api.v1.orgs import assets
-from mistapi.api.v1.orgs import call
 from mistapi.api.v1.orgs import cert
 from mistapi.api.v1.orgs import claim
 from mistapi.api.v1.orgs import clients
 from mistapi.api.v1.orgs import clone
 from mistapi.api.v1.orgs import crl
 from mistapi.api.v1.orgs import deviceprofiles
 from mistapi.api.v1.orgs import devices
@@ -39,20 +38,22 @@
 from mistapi.api.v1.orgs import logs
 from mistapi.api.v1.orgs import maps
 from mistapi.api.v1.orgs import mist_nac
 from mistapi.api.v1.orgs import mxclusters
 from mistapi.api.v1.orgs import mxedges
 from mistapi.api.v1.orgs import mxtunnels
 from mistapi.api.v1.orgs import nac_clients
+from mistapi.api.v1.orgs import nacportals
 from mistapi.api.v1.orgs import nacrules
 from mistapi.api.v1.orgs import nactags
 from mistapi.api.v1.orgs import networks
 from mistapi.api.v1.orgs import networktemplates
 from mistapi.api.v1.orgs import ocdevices
 from mistapi.api.v1.orgs import otherdevices
+from mistapi.api.v1.orgs import pcaps
 from mistapi.api.v1.orgs import pma
 from mistapi.api.v1.orgs import pskportals
 from mistapi.api.v1.orgs import psks
 from mistapi.api.v1.orgs import rftemplates
 from mistapi.api.v1.orgs import sdkclients
 from mistapi.api.v1.orgs import sdkinvites
 from mistapi.api.v1.orgs import sdktemplates
@@ -66,14 +67,15 @@
 from mistapi.api.v1.orgs import ssoroles
 from mistapi.api.v1.orgs import ssos
 from mistapi.api.v1.orgs import stats
 from mistapi.api.v1.orgs import subscriptions
 from mistapi.api.v1.orgs import templates
 from mistapi.api.v1.orgs import tickets
 from mistapi.api.v1.orgs import troubleshoot
+from mistapi.api.v1.orgs import usermacs
 from mistapi.api.v1.orgs import vars
 from mistapi.api.v1.orgs import vpns
 from mistapi.api.v1.orgs import wan_client
 from mistapi.api.v1.orgs import wan_clients
 from mistapi.api.v1.orgs import webhooks
 from mistapi.api.v1.orgs import wired_clients
 from mistapi.api.v1.orgs import wlans
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/admins.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/admins.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAdmins")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAdmins")  
 def getOrgAdmins(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAdmins
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/alarms.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/alarms.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/alarmtemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/alarmtemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAlarmTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAlarmTemplates")  
 def getOrgAlarmTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAlarmTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/alarmtemplates"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSuppressedAlarms")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSuppressedAlarms")  
 def getOrgSuppressedAlarms(mist_session:_APISession, org_id:str, scope:str="site") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSuppressedAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/apitokens.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgApiTokens")  
 def getOrgApiTokens(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/aptemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/aptemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAptemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAptemplates")  
 def getOrgAptemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAptemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/assetfilters.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/assetfilters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAssetFilters")  
 def getOrgAssetFilters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/assets.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/inventory.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,78 +10,90 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAssets")  
-def getOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def getOrgInventory(mist_session:_APISession, org_id:str, serial:str=None, model:str=None, type:str="ap", mac:str=None, site_id:str=None, vc_mac:str=None, vc:str=None, unassigned:bool=None, limit:int=100, page:int=1) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
+    API doc: https://doc.mist-lab.fr/#operation/getOrgInventory
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    serial : str
+    model : str
+    type : str{'ap', 'switch', 'gateway'}, default: ap
+    mac : str
+    site_id : str
+    vc_mac : str
+    vc : str
+    unassigned : bool
+    limit : int, default: 100
+    page : int, default: 1        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets"
+    uri = f"/api/v1/orgs/{org_id}/inventory"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if serial: query_params["serial"]=serial
+    if model: query_params["model"]=model
+    if type: query_params["type"]=type
+    if mac: query_params["mac"]=mac
+    if site_id: query_params["site_id"]=site_id
+    if vc_mac: query_params["vc_mac"]=vc_mac
+    if vc: query_params["vc"]=vc
+    if unassigned: query_params["unassigned"]=unassigned
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgAssets(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def addOrgInventory(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgAssets
+    API doc: https://doc.mist-lab.fr/#operation/addOrgInventory
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    QUERY PARAMS
-    ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets"
-    query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/inventory"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def createOrgAsset(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def updateOrgInventoryAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgAsset
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgInventoryAssignment
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,51 +106,48 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/inventory"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def importOrgAssetsFile(mist_session:_APISession, org_id:str, file:str=None) -> _APIResponse:
+def createOrgGatewayHaCluster(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
+    API doc: https://doc.mist-lab.fr/#operation/createOrgGatewayHaCluster
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     BODY PARAMS
     -----------
-    file : str
-        path to the file to upload. CSV file
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    multipart_form_data = {
-        "file":file,
-    }
-    uri = f"/api/v1/orgs/{org_id}/assets/import"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    uri = f"/api/v1/orgs/{org_id}/inventory/create_ha_cluster"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
-
-def importOrgAssets(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+    
+def deleteOrgGatewayHaCluster(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importOrgAssets
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgGatewayHaCluster
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -151,87 +160,60 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets/import"
+    uri = f"/api/v1/orgs/{org_id}/inventory/delete_ha_cluster"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgAsset(mist_session:_APISession, org_id:str, asset_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgAsset
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    asset_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteOrgAsset(mist_session:_APISession, org_id:str, asset_id:str) -> _APIResponse:
+def reevaluateOrgAutoAssignment(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgAsset
+    API doc: https://doc.mist-lab.fr/#operation/reevaluateOrgAutoAssignment
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    asset_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/inventory/reevaluate_auto_assignment"
+    resp = mist_session.mist_post(uri=uri)
     return resp
     
-def updateOrgAsset(mist_session:_APISession, org_id:str, asset_id:str, body:object) -> _APIResponse:
+def replaceOrgDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgAsset
+    API doc: https://doc.mist-lab.fr/#operation/replaceOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    asset_id : str        
+    org_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/assets/{asset_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/inventory/replace"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/call.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wan_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,70 +10,45 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countOrgCallEvents(mist_session:_APISession, org_id:str, distinct:str=None) -> _APIResponse:
+def countOrgWanClientEvents(mist_session:_APISession, org_id:str, distinct:str="type", type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgCallEvents
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
-    QUERY PARAMS
-    ------------
-    distinct : str{'type', 'app'}        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/call/events/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def searchOrgCallEvents(mist_session:_APISession, org_id:str, type:str=None, ap:str=None, mac:str=None, app:str=None) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgCallEvents
+    API doc: https://doc.mist-lab.fr/#operation/countOrgWanClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
+    distinct : str{'type', 'hostname', 'ip', 'mfg', 'mac'}, default: type
     type : str
-      Event Type. See [listCallEventsDefinitions](/#operation/listCallEventsDefinitions)
-    ap : str
-    mac : str
-    app : str        
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/call/events/search"
+    uri = f"/api/v1/orgs/{org_id}/wan_client/events/count"
     query_params={}
+    if distinct: query_params["distinct"]=distinct
     if type: query_params["type"]=type
-    if ap: query_params["ap"]=ap
-    if mac: query_params["mac"]=mac
-    if app: query_params["app"]=app
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/cert.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/cert.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/claim.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/claim.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/clients.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,29 +27,21 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'mac', 'hostname', 'device', 'os', 'model', 'ap', 'vlan', 'ssid', 'ip'}, default: device
     mac : str
-      partial / full MAC address
     hostname : str
-      partial / full hostname
     device : str
-      device type, e.g. Mac, Nvidia, iPhone
     os : str
-      os, e.g. Sierra, Yosemite, Windows 10
     model : str
-      model, e.g. “MBP 15 late 2013”, 6, 6s, “8+ GSM”
     ap : str
-      AP mac where the client has connected to
     vlan : str
-      vlan
     ssid : str
-      SSID
     ip_address : str
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
@@ -90,29 +82,23 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      event type, e.g. MARVIS_EVENT_CLIENT_FBT_FAILURE
     reason_code : int
-      for assoc/disassoc events
     ssid : str
-      SSID Name
     ap : str
-      AP MAC
-    proto : str{'b', 'g', 'n', 'ac', 'ax', 'a'}
-      802.11 standard
-    band : str{'24', '5'}
-      24 / 5
+    proto : str{'a', 'b', 'g', 'n', 'ac', 'ax'}
+      a / b / g / n / ac / ax
+    band : str{'24', '5', '6'}
+      802.11 Band
     wlan_id : str
-      wlan_id
     nacrule_id : str
-      nacrule_id
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -148,37 +134,26 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      Site ID
     mac : str
-      partial / full MAC address
     ip_address : str
     hostname : str
-      partial / full hostname
     device : str
-      device type, e.g. Mac, Nvidia, iPhone
     os : str
-      os, e.g. Sierra, Yosemite, Windows 10
     model : str
-      model, e.g. “MBP 15 late 2013”, 6, 6s, “8+ GSM”
     ap : str
-      AP mac where the client has connected to
     psk_id : str
     psk_name : str
-      PSK Name
     vlan : str
-      vlan
     ssid : str
-      SSID
     text : str
-      partial / full MAC address, hostname, username, psk_name or ip
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -203,15 +178,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgWirelessClientsSessions(mist_session:_APISession, org_id:str, distinct:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgWirelessClientsSessions(mist_session:_APISession, org_id:str, distinct:str="device", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgWirelessClientsSessions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -220,29 +195,22 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'ssid', 'ap', 'ip', 'vlan', 'hostname', 'os', 'model', 'device'}, default: device
     ap : str
-      AP MAC
-    band : str{'24', '5'}
-      5 / 24
+    band : str{'24', '5', '6'}
+      802.11 Band
     client_family : str
-      E.g. “Mac”, “iPhone”, “Apple watch”
     client_manufacture : str
-      E.g. “Apple”
     client_model : str
-      E.g. “8+”, “XS”
     client_os : str
-      E.g. “Mojave”, “Windows 10”, “Linux”
     ssid : str
-      SSID
     wlan_id : str
-      wlan_id
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -281,34 +249,25 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     ap : str
-      AP MAC
-    band : str{'24', '5'}
-      5 / 24
+    band : str{'24', '5', '6'}
+      802.11 Band
     client_family : str
-      E.g. “Mac”, “iPhone”, “Apple watch”
     client_manufacture : str
-      E.g. “Apple”
     client_model : str
-      E.g. “8+”, “XS”
     client_username : str
-      Username
     client_os : str
-      E.g. “Mojave”, “Windows 10”, “Linux”
     ssid : str
-      SSID
     wlan_id : str
-      wlan_id
     psk_id : str
     psk_name : str
-      PSK Name
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/clone.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/clone.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/crl.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/crl.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/deviceprofiles.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/deviceprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgDeviceProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgDeviceProfiles")  
 def getOrgDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/devices.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgDevices")  
 def getOrgDevices(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -57,15 +57,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgDevices(mist_session:_APISession, org_id:str, distinct:str, hostname:str=None, site_id:str=None, model:str=None, mac:str=None, version:str=None, ip_address:str=None, mxtunnel_status:str=None, mxedge_id:str=None, lldp_system_name:str=None, lldp_system_desc:str=None, lldp_port_id:str=None, lldp_mgmt_addr:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgDevices(mist_session:_APISession, org_id:str, distinct:str="model", hostname:str=None, site_id:str=None, model:str=None, mac:str=None, version:str=None, ip_address:str=None, mxtunnel_status:str=None, mxedge_id:str=None, lldp_system_name:str=None, lldp_system_desc:str=None, lldp_port_id:str=None, lldp_mgmt_addr:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -74,36 +74,25 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'hostname', 'site_id', 'model', 'mac', 'version', 'ip', 'mxtunnel_status', 'mxedge_id', 'lldp_system_name', 'lldp_system_desc', 'lldp_port_id', 'lldp_mgmt_addr'}, default: model
     hostname : str
-      partial / full hostname
     site_id : str
-      site id
     model : str
-      device model
     mac : str
-      AP mac
     version : str
-      version
     ip_address : str
     mxtunnel_status : str{'up', 'down'}
-      MxTunnel status, up / down
     mxedge_id : str
-      Mist Edge id, if AP is connecting to a Mist Edge
     lldp_system_name : str
-      LLDP system name
     lldp_system_desc : str
-      LLDP system description
     lldp_port_id : str
-      LLDP port id
     lldp_mgmt_addr : str
-      LLDP management ip address
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -130,15 +119,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgDeviceEvents(mist_session:_APISession, org_id:str, distinct:str, site_id:str=None, ap:str=None, apfw:str=None, model:str=None, text:str=None, timestamp:str=None, type:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgDeviceEvents(mist_session:_APISession, org_id:str, distinct:str="model", site_id:str=None, ap:str=None, apfw:str=None, model:str=None, text:str=None, timestamp:str=None, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -147,28 +136,20 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'org_id', 'site_id', 'ap', 'apfw', 'model', 'text', 'timestamp', 'type'}, default: model
     site_id : str
-      site id
     ap : str
-      AP mac
     apfw : str
-      AP Firmware
     model : str
-      device model
     text : str
-      event message
     timestamp : str
-      event time
     type : str
-      Events Type
-    page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -181,15 +162,14 @@
     if site_id: query_params["site_id"]=site_id
     if ap: query_params["ap"]=ap
     if apfw: query_params["apfw"]=apfw
     if model: query_params["model"]=model
     if text: query_params["text"]=text
     if timestamp: query_params["timestamp"]=timestamp
     if type: query_params["type"]=type
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
@@ -205,27 +185,20 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      device mac
     model : str
-      device model
     device_type : str{'ap', 'switch', 'gateway'}, default: ap
-      device type
     text : str
-      event message
     timestamp : str
-      event time
     type : str
-      see [listDeviceEventsDefinitions](/#operation/listDeviceEventsDefinitions)
     last_by : str
-      Return last/recent event for passed in field
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -244,66 +217,66 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgDeviceLastConfigs(mist_session:_APISession, org_id:str, device_type:str="ap", distinct:str=None, start:int=None, end:int=None, limit:int=100) -> _APIResponse:
+def countOrgDeviceLastConfigs(mist_session:_APISession, org_id:str, type:str="ap", distinct:str=None, start:int=None, end:int=None, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgDeviceLastConfigs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
-    device_type : str{'ap', 'switch', 'gateway'}, default: ap
+    type : str{'ap', 'switch', 'gateway'}, default: ap
     distinct : str{'mac', 'version', 'name', 'site_id'}
     start : int
     end : int
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/last_config/count"
     query_params={}
-    if device_type: query_params["device_type"]=device_type
+    if type: query_params["type"]=type
     if distinct: query_params["distinct"]=distinct
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgDeviceLastConfigs(mist_session:_APISession, org_id:str, device_type:str="ap", mac:str=None, name:str=None, version:str=None, start:int=None, end:int=None, limit:int=100, duration:str="1d") -> _APIResponse:
+def searchOrgDeviceLastConfigs(mist_session:_APISession, org_id:str, type:str="ap", mac:str=None, name:str=None, version:str=None, start:int=None, end:int=None, limit:int=100, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgDeviceLastConfigs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
-    device_type : str{'ap', 'switch', 'gateway'}, default: ap
+    type : str{'ap', 'switch', 'gateway'}, default: ap
     mac : str
     name : str
     version : str
     start : int
     end : int
     limit : int, default: 100
     duration : str, default: 1d        
@@ -311,26 +284,26 @@
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/devices/last_config/search"
     query_params={}
-    if device_type: query_params["device_type"]=device_type
+    if type: query_params["type"]=type
     if mac: query_params["mac"]=mac
     if name: query_params["name"]=name
     if version: query_params["version"]=version
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgApsMacs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgApsMacs")  
 def getOrgApsMacs(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgApsMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -399,52 +372,33 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     hostname : str
-      partial / full hostname
     site_id : str
-      site id
     model : str
-      device model
     mac : str
-      AP mac
     version : str
-      version
     power_constrained : bool
-      power_constrained
     ip_address : str
     mxtunnel_status : str{'up', 'down'}
-      MxTunnel status, up / down
     mxedge_id : str
-      Mist Edge id, if AP is connecting to a Mist Edge
     lldp_system_name : str
-      LLDP system name
     lldp_system_desc : str
-      LLDP system description
     lldp_port_id : str
-      LLDP port id
     lldp_mgmt_addr : str
-      LLDP management ip address
     band_24_bandwith : int
-      Bandwith of band_24
     band_5_bandwith : int
-      Bandwith of band_5
     band_6_bandwith : int
-      Bandwith of band_6
     band_24_channel : int
-      Channel of band_24
     band_5_channel : int
-      Channel of band_5
     band_6_channel : int
-      Channel of band_6
     eth0_port_speed : int
-      Port speed of eth0
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -476,15 +430,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMultiSitesDevicesUpgrades")  
 def getOrgMultiSitesDevicesUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMultiSitesDevicesUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/evpn_topologies.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/evpn_topologies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgEvpnTopologies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgEvpnTopologies")  
 def getOrgEvpnTopologies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/gatewaytemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/gatewaytemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgGatewayTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgGatewayTemplates")  
 def getOrgGatewayTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGatewayTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/guests.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/guests.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgGuestAuthorizations")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgGuestAuthorizations")  
 def getOrgGuestAuthorizations(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgGuestAuthorizations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/idpprofiles.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/idpprofiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgIdpProfiles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgIdpProfiles")  
 def getOrgIdpProfiles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgIdpProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/insights.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/insights.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     -----------
     org_id : str
     metric : str        
     
     QUERY PARAMS
     ------------
     sle : str
-      see [listInsightMetrics](/#operation/listInsightMetrics) for more details
     duration : str, default: 1d
     interval : str
     start : int
     end : int        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/inventory.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/ssr.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,121 +10,87 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrgInventory(mist_session:_APISession, org_id:str, serial:str=None, model:str=None, type:str=None, mac:str=None, site_id:str=None, vc_mac:str=None, vc:str=None, unassigned:bool=None, limit:int=100, page:int=1) -> _APIResponse:
+def getOrg128TRegistrationCommands(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgInventory
+    API doc: https://doc.mist-lab.fr/#operation/getOrg128TRegistrationCommands
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    QUERY PARAMS
-    ------------
-    serial : str
-      device serial
-    model : str
-      device model
-    type : str{'ap', 'switch', 'gateway'}
-    mac : str
-      MAC address
-    site_id : str
-      site id if assigned, null if not assigned
-    vc_mac : str
-    vc : str
-    unassigned : bool
-    limit : int, default: 100
-    page : int, default: 1        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
-    query_params={}
-    if serial: query_params["serial"]=serial
-    if model: query_params["model"]=model
-    if type: query_params["type"]=type
-    if mac: query_params["mac"]=mac
-    if site_id: query_params["site_id"]=site_id
-    if vc_mac: query_params["vc_mac"]=vc_mac
-    if vc: query_params["vc"]=vc
-    if unassigned: query_params["unassigned"]=unassigned
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def addOrgInventory(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSsrUpgrades")  
+def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addOrgInventory
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def updateOrgInventoryAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def listOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgInventoryAssignment
+    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgGatewayHaCluster(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def upgradeOrgSsrs(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgGatewayHaCluster
+    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgSsrs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -137,92 +103,96 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/create_ha_cluster"
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def deleteOrgGatewayHaCluster(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def cancelOrgSsrUpgrade(mist_session:_APISession, org_id:str, upgrade_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgGatewayHaCluster
+    API doc: https://doc.mist-lab.fr/#operation/cancelOrgSsrUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    org_id : str
+    upgrade_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/delete_ha_cluster"
+    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def reevaluateOrgAutoAssignment(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAvailableSsrVersions")  
+def getOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/reevaluateOrgAutoAssignment
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    channel : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/reevaluate_auto_assignment"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
+    query_params={}
+    if channel: query_params["channel"]=channel
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def replaceOrgDevices(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def listOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/replaceOrgDevices
+    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    channel : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/inventory/replace"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
+    query_params={}
+    if channel: query_params["channel"]=channel
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/invites.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/invites.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/jsi.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/jsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgJsiDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgJsiDevices")  
 def getOrgJsiDevices(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None, mac:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -157,15 +157,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/jsi/devices/{device_mac}/upgrade"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgJsiPastPurchases")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgJsiPastPurchases")  
 def getOrgJsiPastPurchases(mist_session:_APISession, org_id:str, limit:int=100, page:int=1, model:str=None, serial:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgJsiPastPurchases
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/licenses.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/oauth.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,80 +10,62 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrgLicencesSummary(mist_session:_APISession, org_id:str) -> _APIResponse:
+def getOauth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesSummary
+    API doc: https://doc.mist-lab.fr/#operation/getOauth2UrlForLinking
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    provider : str        
+    
+    QUERY PARAMS
+    ------------
+    forward : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
-    query_params={}
+    uri = f"/api/v1/self/oauth/{provider}"
+    query_params={}
+    if forward: query_params["forward"]=forward
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def moveOrDeleteOrgLicenseToAnotherOrg(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def linkOauth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/moveOrDeleteOrgLicenseToAnotherOrg
+    API doc: https://doc.mist-lab.fr/#operation/linkOauth2MistAccount
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    provider : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/licenses"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def getOrgLicencesBySite(mist_session:_APISession, org_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgLicencesBySite
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/licenses/usages"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/oauth/{provider}"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/logs.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgLogs")  
 def getOrgLogs(mist_session:_APISession, org_id:str, site_id:str=None, admin_name:str=None, message:str=None, sort:str=None, start:int=None, end:int=None, limit:int=100, page:int=1, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -27,21 +27,17 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      site id
     admin_name : str
-      admin name or email
     message : str
-      message
     sort : str{'timestamp', '-timestamp', 'site_id', 'admin_id'}
-      sort order
     start : int
     end : int
     limit : int, default: 100
     page : int, default: 1
     duration : str, default: 1d        
     
     RETURN
@@ -75,21 +71,17 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      site id
     admin_name : str
-      admin name or email
     message : str
-      message
     sort : str{'timestamp', '-timestamp', 'site_id', 'admin_id'}
-      sort order
     start : int
     end : int
     limit : int, default: 100
     page : int, default: 1
     duration : str, default: 1d        
     
     RETURN
@@ -107,15 +99,15 @@
     if end: query_params["end"]=end
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgLogs(mist_session:_APISession, org_id:str, distinct:str, admin_id:str=None, admin_name:str=None, site_id:str=None, message:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countOrgLogs(mist_session:_APISession, org_id:str, distinct:str="admin_name", admin_id:str=None, admin_name:str=None, site_id:str=None, message:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/maps.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/maps.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         path to the file to upload. csv file for ap name mapping, optional
     file : str
         path to the file to upload. ekahau or ibwave file
     json : dict
         import_all_floorplans : bool
         import_height : bool, default: True
         import_orientation : bool, default: True
-        site_id : str
+        site_id : any
         vendor_name : {'ekahau', 'ibwave'}
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/mist_nac.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/mist_nac.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/mxclusters.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/mxclusters.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMxEdgeClusters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMxEdgeClusters")  
 def getOrgMxEdgeClusters(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeClusters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/mxedges.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/mxedges.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMxEdges")  
 def getOrgMxEdges(mist_session:_APISession, org_id:str, for_sites:str="any", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -27,15 +27,14 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     for_sites : str{'any', 'true', 'false'}, default: any
-      filter for site level mist edges
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
@@ -60,15 +59,14 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     for_sites : str{'any', 'true', 'false'}, default: any
-      filter for site level mist edges
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
@@ -175,29 +173,21 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'model', 'mxcluster_id', 'distro', 'tunterm_version', 'site_id'}, default: model
     mxedge_id : str
-      mist edge id
     site_id : str
-      mist edge site id
     mxcluster_id : str
-      mist edge cluster id
     model : str
-      model name
     distro : str
-      debian code name(buster, bullseye)
     tunterm_version : str
-      tunterm version
     sort : str
-      sort options, -prefix represents DESC order, default is -last_seen
     stats : bool
-      whether to return device stats, default is false
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
@@ -220,15 +210,15 @@
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgSiteMxEdgeEvents(mist_session:_APISession, org_id:str, distinct:str="mxedge_id", mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", page:int=1, limit:int=100) -> _APIResponse:
+def countOrgSiteMxEdgeEvents(mist_session:_APISession, org_id:str, distinct:str="mxedge_id", mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgSiteMxEdgeEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -237,25 +227,20 @@
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'mxedge_id', 'type', 'mxcluster_id', 'package'}, default: mxedge_id
     mxedge_id : str
-      mist edge id
     mxcluster_id : str
-      mist edge cluster id
     type : str
-      mist edge event type [Supported Events](/#operation/listGatewayApplications)
     service : str
-      service running on mist edge(mxagent, tunterm etc)
     start : int
     end : int
     duration : str, default: 1d
-    page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
@@ -265,20 +250,19 @@
     if mxedge_id: query_params["mxedge_id"]=mxedge_id
     if mxcluster_id: query_params["mxcluster_id"]=mxcluster_id
     if type: query_params["type"]=type
     if service: query_params["service"]=service
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgMistEdgeEvents(mist_session:_APISession, org_id:str, mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", page:int=1, limit:int=100) -> _APIResponse:
+def searchOrgMistEdgeEvents(mist_session:_APISession, org_id:str, mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgMistEdgeEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -286,25 +270,20 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mxedge_id : str
-      mist edge id
     mxcluster_id : str
-      mist edge cluster id
     type : str
-      mist edge event type [Supported Events](/#operation/listGatewayApplications)
     service : str
-      service running on mist edge(mxagent, tunterm etc)
     start : int
     end : int
     duration : str, default: 1d
-    page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
@@ -313,15 +292,14 @@
     if mxedge_id: query_params["mxedge_id"]=mxedge_id
     if mxcluster_id: query_params["mxcluster_id"]=mxcluster_id
     if type: query_params["type"]=type
     if service: query_params["service"]=service
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def searchOrgMxEdges(mist_session:_APISession, org_id:str, mxedge_id:str=None, site_id:str=None, mxcluster_id:str=None, model:str=None, distro:str=None, tunterm_version:str=None, sort:str=None, stats:bool=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgMxEdges
@@ -334,29 +312,21 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mxedge_id : str
-      mist edge id
     site_id : str
-      mist edge site id
     mxcluster_id : str
-      mist edge cluster id
     model : str
-      model name
     distro : str
-      debian code name(buster, bullseye)
     tunterm_version : str
-      tunterm version
     sort : str
-      sort options, -prefix represents DESC order, default is -last_seen
     stats : bool
-      whether to return device stats, default is false
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
@@ -405,15 +375,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/unassign"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMxEdgeUpgrades")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMxEdgeUpgrades")  
 def getOrgMxEdgeUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgeUpgrades
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -518,16 +488,15 @@
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
-    channel : str{'stable', 'beta', 'alpha'}, default: stable
-      upgrade channel to follow, stable (default) / beta / alpha        
+    channel : str{'stable', 'beta', 'alpha'}, default: stable        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/version"
@@ -608,65 +577,65 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:float) -> _APIResponse:
+def deleteOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:int) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/deleteOrgMxEdgeImage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     mxedge_id : str
-    image_number : float        
+    image_number : int        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}//image{image_number}"
+    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/image/{image_number}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def addOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:float, body:object) -> _APIResponse:
+def addOrgMxEdgeImage(mist_session:_APISession, org_id:str, mxedge_id:str, image_number:int, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/addOrgMxEdgeImage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     mxedge_id : str
-    image_number : float        
+    image_number : int        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}//image{image_number}"
+    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/image/{image_number}"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
 def restartOrgMxEdge(mist_session:_APISession, org_id:str, mxedge_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/restartOrgMxEdge
     
@@ -726,17 +695,16 @@
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
     mxedge_id : str
-    name : str
-    action : str
-      restart or start or stop        
+    name : str{'tunterm', 'radsecproxy', 'mxagent', 'mxocproxy', 'mxdas'}
+    action : str{'restart', 'start', 'stop'}        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/services/{name}/{action}"
@@ -784,36 +752,8 @@
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/unregister"
     resp = mist_session.mist_post(uri=uri)
     return resp
-    
-def upgradeOrgMxEdge(mist_session:_APISession, org_id:str, mxedge_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgMxEdge
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    mxedge_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/mxedges/{mxedge_id}/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/mxtunnels.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/mxtunnels.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMxTunnels")  
 def getOrgMxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/nac_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/clients.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,309 +10,505 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countOrgNacClients(mist_session:_APISession, org_id:str, distinct:str="type", last_nacrule_id:str=None, nacrule_matched:bool=None, auth_type:str=None, last_vlan_id:str=None, last_nas_vendor:str=None, idp_id:str=None, last_ssid:str=None, last_username:str=None, timestamp:float=None, site_id:str=None, last_ap:str=None, mac:str=None, last_status:str=None, type:str=None, mdm_compliance_status:str=None, mdm_provider:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def countSiteWirelessClients(mist_session:_APISession, site_id:str, distinct:str="device", ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgNacClients
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
-    distinct : str{'type', 'last_nacrule_id', 'auth_type', 'last_vlan_id', 'last_nas_vendor', 'last_username', 'last_ap', 'mac', 'last_ssid', 'last_status', 'mdm_compliance_status', 'mdm_provider'}, default: type
-      NAC Policy Rule ID, if matched
-    last_nacrule_id : str
-      NAC Policy Rule ID, if matched
-    nacrule_matched : bool
-      NAC Policy Rule Matched
-    auth_type : str
-      authentication type, e.g. “eap-tls”, “eap-ttls”, “eap-teap”, “mab”, “device-auth”
-    last_vlan_id : str
-      Vlan ID
-    last_nas_vendor : str
-      vendor of NAS device
-    idp_id : str
-      SSO ID, if present and used
-    last_ssid : str
-      SSID
-    last_username : str
-      Username presented by the client
-    timestamp : float
-      start time, in epoch
-    site_id : str
-      site id if assigned, null if not assigned
-    last_ap : str
-      AP MAC connected to by client
-    mac : str
-      MAC address
-    last_status : str
-      Connection status of client i.e “permitted”, “denied, “session_ended”
-    type : str
-      Client type i.e. “wireless”, “wired” etc.
-    mdm_compliance_status : str
-      MDM compliancy of client i.e “compliant”, “not compliant”
-    mdm_provider : str
-      MDM provider of client’s organisation eg “intune”, “jamf”
+    distinct : str{'ssid', 'ap', 'ip', 'vlan', 'hostname', 'os', 'model', 'device'}, default: device
+    ssid : str
+    ap : str
+    ip_address : str
+    vlan : str
+    hostname : str
+    os : str
+    model : str
+    device : str
+    page : int, default: 1
+    limit : int, default: 100
     start : int
     end : int
-    duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nac_clients/count"
+    uri = f"/api/v1/sites/{site_id}/clients/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
-    if last_nacrule_id: query_params["last_nacrule_id"]=last_nacrule_id
-    if nacrule_matched: query_params["nacrule_matched"]=nacrule_matched
-    if auth_type: query_params["auth_type"]=auth_type
-    if last_vlan_id: query_params["last_vlan_id"]=last_vlan_id
-    if last_nas_vendor: query_params["last_nas_vendor"]=last_nas_vendor
-    if idp_id: query_params["idp_id"]=idp_id
-    if last_ssid: query_params["last_ssid"]=last_ssid
-    if last_username: query_params["last_username"]=last_username
-    if timestamp: query_params["timestamp"]=timestamp
-    if site_id: query_params["site_id"]=site_id
-    if last_ap: query_params["last_ap"]=last_ap
-    if mac: query_params["mac"]=mac
-    if last_status: query_params["last_status"]=last_status
-    if type: query_params["type"]=type
-    if mdm_compliance_status: query_params["mdm_compliance_status"]=mdm_compliance_status
-    if mdm_provider: query_params["mdm_provider"]=mdm_provider
+    if ssid: query_params["ssid"]=ssid
+    if ap: query_params["ap"]=ap
+    if ip_address: query_params["ip_address"]=ip_address
+    if vlan: query_params["vlan"]=vlan
+    if hostname: query_params["hostname"]=hostname
+    if os: query_params["os"]=os
+    if model: query_params["model"]=model
+    if device: query_params["device"]=device
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgNacClientEvents(mist_session:_APISession, org_id:str, distinct:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def disconnectSiteMultipleClients(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteMultipleClients
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/disconnect"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def countSiteWirelessClientEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgNacClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
-    distinct : str{'type', 'nacrule_id', 'dryrun_nacrule_id', 'auth_type', 'vlan', 'nas_vendor', 'username', 'ap', 'mac', 'ssid'}
+    distinct : str{'type', 'proto', 'band', 'channel', 'wlan_id', 'ssid'}
+    type : str
+    reason_code : int
+    ssid : str
+    ap : str
+    proto : str{'a', 'b', 'g', 'n', 'ac', 'ax'}
+      a / b / g / n / ac / ax
+    band : str{'24', '5', '6'}
+      802.11 Band
+    wlan_id : str
+    limit : int, default: 100
     start : int
     end : int
-    duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nac_clients/events/count"
+    uri = f"/api/v1/sites/{site_id}/clients/events/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
+    if reason_code: query_params["reason_code"]=reason_code
+    if ssid: query_params["ssid"]=ssid
+    if ap: query_params["ap"]=ap
+    if proto: query_params["proto"]=proto
+    if band: query_params["band"]=band
+    if wlan_id: query_params["wlan_id"]=wlan_id
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgNacClientEvents(mist_session:_APISession, org_id:str, type:str=None, nacrule_id:str=None, nacrule_matched:bool=None, dryrun_nacrule_id:str=None, dryrun_nacrule_matched:bool=None, auth_type:str=None, vlan:int=None, nas_vendor:str=None, bssid:str=None, idp_id:str=None, idp_role:str=None, resp_attrs:list=None, ssid:str=None, username:str=None, site_id:str=None, ap:str=None, random_mac:bool=None, mac:str=None, timestamp:float=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchSiteWirelessClientEvents(mist_session:_APISession, site_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, nacrule_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgNacClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      event type, e.g. NAC_CLIENT_PERMIT
-    nacrule_id : str
-      NAC Policy Rule ID, if matched
-    nacrule_matched : bool
-      NAC Policy Rule Matched
-    dryrun_nacrule_id : str
-      NAC Policy Dry Run Rule ID, if present and matched
-    dryrun_nacrule_matched : bool
-      True - if dryrun rule present and matched with priority, False - if not matched or not present
-    auth_type : str
-      authentication type, e.g. “802.1X”, “MAB”, “DeviceAuth”
-    vlan : int
-      Vlan ID
-    nas_vendor : str
-      vendor of NAS device
-    bssid : str
-      SSID
-    idp_id : str
-      SSO ID, if present and used
-    idp_role : str
-      IDP returned roles/groups for the user
-    resp_attrs : list
-      Radius attributes returned by NAC to NAS Devive
+    reason_code : int
     ssid : str
-      SSID
-    username : str
-      Username presented by the client
-    site_id : str
-      site id
     ap : str
-      AP MAC
-    random_mac : bool
-      AP random macMAC
-    mac : str
-      MAC address
-    timestamp : float
-      start time, in epoch
+    proto : str{'a', 'b', 'g', 'n', 'ac', 'ax'}
+      a / b / g / n / ac / ax
+    band : str{'24', '5', '6'}
+      802.11 Band
+    wlan_id : str
+    nacrule_id : str
+    limit : int, default: 100
     start : int
     end : int
-    duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nac_clients/events/search"
+    uri = f"/api/v1/sites/{site_id}/clients/events/search"
     query_params={}
     if type: query_params["type"]=type
-    if nacrule_id: query_params["nacrule_id"]=nacrule_id
-    if nacrule_matched: query_params["nacrule_matched"]=nacrule_matched
-    if dryrun_nacrule_id: query_params["dryrun_nacrule_id"]=dryrun_nacrule_id
-    if dryrun_nacrule_matched: query_params["dryrun_nacrule_matched"]=dryrun_nacrule_matched
-    if auth_type: query_params["auth_type"]=auth_type
-    if vlan: query_params["vlan"]=vlan
-    if nas_vendor: query_params["nas_vendor"]=nas_vendor
-    if bssid: query_params["bssid"]=bssid
-    if idp_id: query_params["idp_id"]=idp_id
-    if idp_role: query_params["idp_role"]=idp_role
-    if resp_attrs: query_params["resp_attrs"]=resp_attrs
+    if reason_code: query_params["reason_code"]=reason_code
     if ssid: query_params["ssid"]=ssid
-    if username: query_params["username"]=username
-    if site_id: query_params["site_id"]=site_id
     if ap: query_params["ap"]=ap
-    if random_mac: query_params["random_mac"]=random_mac
+    if proto: query_params["proto"]=proto
+    if band: query_params["band"]=band
+    if wlan_id: query_params["wlan_id"]=wlan_id
+    if nacrule_id: query_params["nacrule_id"]=nacrule_id
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def searchSiteWirelessClients(mist_session:_APISession, site_id:str, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, ssid:str=None, text:str=None, nacrule_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClients
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    mac : str
+    ip_address : str
+    hostname : str
+    device : str
+    os : str
+    model : str
+    ap : str
+    ssid : str
+    text : str
+    nacrule_id : str
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/search"
+    query_params={}
     if mac: query_params["mac"]=mac
-    if timestamp: query_params["timestamp"]=timestamp
+    if ip_address: query_params["ip_address"]=ip_address
+    if hostname: query_params["hostname"]=hostname
+    if device: query_params["device"]=device
+    if os: query_params["os"]=os
+    if model: query_params["model"]=model
+    if ap: query_params["ap"]=ap
+    if ssid: query_params["ssid"]=ssid
+    if text: query_params["text"]=text
+    if nacrule_id: query_params["nacrule_id"]=nacrule_id
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if duration: query_params["duration"]=duration
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def countSiteWirelessClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientSessions
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    distinct : str{'ssid', 'wlan_id', 'ap', 'mac', 'client_family', 'client_manufacture', 'client_model', 'client_os'}, default: mac
+    ap : str
+    band : str{'24', '5', '6'}
+      802.11 Band
+    client_family : str
+    client_manufacture : str
+    client_model : str
+    client_os : str
+    ssid : str
+    wlan_id : str
+    page : int, default: 1
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/sessions/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    if ap: query_params["ap"]=ap
+    if band: query_params["band"]=band
+    if client_family: query_params["client_family"]=client_family
+    if client_manufacture: query_params["client_manufacture"]=client_manufacture
+    if client_model: query_params["client_model"]=client_model
+    if client_os: query_params["client_os"]=client_os
+    if ssid: query_params["ssid"]=ssid
+    if wlan_id: query_params["wlan_id"]=wlan_id
+    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgNacClients(mist_session:_APISession, org_id:str, last_nacrule_id:str=None, nacrule_matched:bool=None, auth_type:str=None, last_vlan_id:str=None, last_nas_vendor:str=None, idp_id:str=None, last_ssid:str=None, last_username:str=None, timestamp:float=None, site_id:str=None, last_ap:str=None, mac:str=None, last_status:str=None, type:str=None, mdm_compliance_status:str=None, mdm_provider:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchSiteWirelessClientSessions(mist_session:_APISession, site_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchOrgNacClients
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientSessions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
     QUERY PARAMS
     ------------
-    last_nacrule_id : str
-      NAC Policy Rule ID, if matched
-    nacrule_matched : bool
-      NAC Policy Rule Matched
-    auth_type : str
-      authentication type, e.g. “eap-tls”, “eap-ttls”, “eap-teap”, “mab”, “device-auth”
-    last_vlan_id : str
-      Vlan ID
-    last_nas_vendor : str
-      vendor of NAS device
-    idp_id : str
-      SSO ID, if present and used
-    last_ssid : str
-      SSID
-    last_username : str
-      Username presented by the client
-    timestamp : float
-      start time, in epoch
+    ap : str
+    band : str{'24', '5', '6'}
+      802.11 Band
+    client_family : str
+    client_manufacture : str
+    client_model : str
+    client_username : str
+    client_os : str
+    ssid : str
+    wlan_id : str
+    psk_id : str
+    psk_name : str
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/sessions/search"
+    query_params={}
+    if ap: query_params["ap"]=ap
+    if band: query_params["band"]=band
+    if client_family: query_params["client_family"]=client_family
+    if client_manufacture: query_params["client_manufacture"]=client_manufacture
+    if client_model: query_params["client_model"]=client_model
+    if client_username: query_params["client_username"]=client_username
+    if client_os: query_params["client_os"]=client_os
+    if ssid: query_params["ssid"]=ssid
+    if wlan_id: query_params["wlan_id"]=wlan_id
+    if psk_id: query_params["psk_id"]=psk_id
+    if psk_name: query_params["psk_name"]=psk_name
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def unauthorizeSiteMultipleClients(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteMultipleClients
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/unauthorize"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def reauthSiteDot1xWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/reauthSiteDot1xWirelessClient
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
     site_id : str
-      site id if assigned, null if not assigned
-    last_ap : str
-      AP MAC connected to by client
-    mac : str
-      MAC address
-    last_status : str
-      Connection status of client i.e “permitted”, “denied, “session_ended”
+    client_mac : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/coa"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
+    
+def disconnectSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteWirelessClient
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    client_mac : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/disconnect"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
+    
+def getSiteEventsForClient(mist_session:_APISession, site_id:str, client_mac:str, type:str=None, proto:str=None, band:str=None, channel:str=None, wlan_id:str=None, ssid:str=None, start:int=None, end:int=None, page:int=1, limit:int=100, duration:str="1d") -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteEventsForClient
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    client_mac : str        
+    
+    QUERY PARAMS
+    ------------
     type : str
-      Client type i.e. “wireless”, “wired” etc.
-    mdm_compliance_status : str
-      MDM compliancy of client i.e “compliant”, “not compliant”
-    mdm_provider : str
-      MDM provider of client’s organisation eg “intune”, “jamf”
+    proto : str{'a', 'b', 'g', 'n', 'ac', 'ax'}
+      a / b / g / n / ac / ax
+    band : str{'24', '5', '6'}
+      802.11 Band
+    channel : str
+    wlan_id : str
+    ssid : str
     start : int
     end : int
-    duration : str, default: 1d
+    page : int, default: 1
     limit : int, default: 100
-    page : int, default: 1        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nac_clients/search"
+    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/events"
     query_params={}
-    if last_nacrule_id: query_params["last_nacrule_id"]=last_nacrule_id
-    if nacrule_matched: query_params["nacrule_matched"]=nacrule_matched
-    if auth_type: query_params["auth_type"]=auth_type
-    if last_vlan_id: query_params["last_vlan_id"]=last_vlan_id
-    if last_nas_vendor: query_params["last_nas_vendor"]=last_nas_vendor
-    if idp_id: query_params["idp_id"]=idp_id
-    if last_ssid: query_params["last_ssid"]=last_ssid
-    if last_username: query_params["last_username"]=last_username
-    if timestamp: query_params["timestamp"]=timestamp
-    if site_id: query_params["site_id"]=site_id
-    if last_ap: query_params["last_ap"]=last_ap
-    if mac: query_params["mac"]=mac
-    if last_status: query_params["last_status"]=last_status
     if type: query_params["type"]=type
-    if mdm_compliance_status: query_params["mdm_compliance_status"]=mdm_compliance_status
-    if mdm_provider: query_params["mdm_provider"]=mdm_provider
+    if proto: query_params["proto"]=proto
+    if band: query_params["band"]=band
+    if channel: query_params["channel"]=channel
+    if wlan_id: query_params["wlan_id"]=wlan_id
+    if ssid: query_params["ssid"]=ssid
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
+    
+def unauthorizeSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteWirelessClient
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    client_mac : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/unauthorize"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/nacrules.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/nacrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgNacRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgNacRules")  
 def getOrgNacRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNacRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/nactags.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/vpns.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgNacTags")  
-def getOrgNacTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgsVpns")  
+def getOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
+    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgNacTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgNacTags
+    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgNacTag(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgVpns(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgNacTag
+    API doc: https://doc.mist-lab.fr/#operation/createOrgVpns
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,87 +94,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags"
+    uri = f"/api/v1/orgs/{org_id}/vpns"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgNacTag(mist_session:_APISession, org_id:str, nactag_id:str) -> _APIResponse:
+def getOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgNacTag
+    API doc: https://doc.mist-lab.fr/#operation/getOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    nactag_id : str        
+    vpn_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags/{nactag_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgNacTag(mist_session:_APISession, org_id:str, nactag_id:str) -> _APIResponse:
+def deleteOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgNacTag
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    nactag_id : str        
+    vpn_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags/{nactag_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateOrgNacTag(mist_session:_APISession, org_id:str, nactag_id:str, body:object) -> _APIResponse:
+def updateOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgNacTag
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgVpn
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    nactag_id : str        
+    vpn_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/nactags/{nactag_id}"
+    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/networks.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgNetworks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgNetworks")  
 def getOrgNetworks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/networktemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/networktemplates.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgNetworkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgNetworkTemplates")  
 def getOrgNetworkTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgNetworkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/ocdevices.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/apps.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,36 +10,54 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrgJuniperDevicesCommand(mist_session:_APISession, org_id:str, site_id:str=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteApps")  
+def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgJuniperDevicesCommand
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
     
-    QUERY PARAMS
-    ------------
-    site_id : str
-      site_id would be used for proxy config check of the site and automatic site assignment        
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ocdevices/outbound_ssh_cmd"
-    query_params={}
-    if site_id: query_params["site_id"]=site_id
+    uri = f"/api/v1/sites/{site_id}/apps"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/orgs.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/orgs.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/otherdevices.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/otherdevices.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgOtherDevices")  
 def getOrgOtherDevices(mist_session:_APISession, org_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -118,15 +118,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/otherdevices"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def countOrgOtherDeviceEvents(mist_session:_APISession, org_id:str, distinct:str="mac", start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def countOrgOtherDeviceEvents(mist_session:_APISession, org_id:str, distinct:str="mac", type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgOtherDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -134,37 +134,37 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'mac', 'type', 'vendor', 'site_id'}, default: mac
+    type : str
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/otherdevices/events/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgOtherDeviceEvents(mist_session:_APISession, org_id:str, site_id:str=None, mac:str=None, device_mac:str=None, model:str=None, vendor:str=None, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchOrgOtherDeviceEvents(mist_session:_APISession, org_id:str, site_id:str=None, mac:str=None, device_mac:str=None, model:str=None, vendor:str=None, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgOtherDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -172,30 +172,23 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      site id
     mac : str
-      mac
     device_mac : str
-      mac of attached device
     model : str
-      device model
     vendor : str
-      vendor name
     type : str
-      event type
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/otherdevices/events/search"
@@ -205,16 +198,15 @@
     if device_mac: query_params["device_mac"]=device_mac
     if model: query_params["model"]=model
     if vendor: query_params["vendor"]=vendor
     if type: query_params["type"]=type
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def getOrgOtherDevice(mist_session:_APISession, org_id:str, device_mac:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getOrgOtherDevice
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/pma.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/pma.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgPmaDashboards")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgPmaDashboards")  
 def getOrgPmaDashboards(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPmaDashboards
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/pskportals.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/pskportals.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgPskPortals")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgPskPortals")  
 def getOrgPskPortals(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortals
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/pskportals"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgPskPortalLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgPskPortalLogs")  
 def getOrgPskPortalLogs(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPskPortalLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -233,19 +233,17 @@
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1
     psk_name : str
     psk_id : str
     pskportal_id : str
     id : str
-      audit_id
     admin_name : str
     admin_id : str
-    name_id : str
-      name_id used in SSO        
+    name_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/pskportals/logs/search"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/psks.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgPsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgPsks")  
 def getOrgPsks(mist_session:_APISession, org_id:str, name:str=None, ssid:str=None, role:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgPsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/rftemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/rftemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgRfTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgRfTemplates")  
 def getOrgRfTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgRfTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sdkclients.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sdkclients.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sdkinvites.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sdkinvites.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSdkInvites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSdkInvites")  
 def getSdkInvites(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkInvites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sdktemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sdktemplates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSdkTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSdkTemplates")  
 def getSdkTemplates(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSdkTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/secpolicies.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/secpolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSecPolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSecPolicies")  
 def getOrgSecPolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSecPolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/servicepolicies.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/servicepolicies.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgServicePolicies")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgServicePolicies")  
 def getOrgServicePolicies(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServicePolicies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/services.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/services.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgServices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgServices")  
 def getOrgServices(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgServices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/setting.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -574,109 +574,105 @@
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    app_name : str
-      OAuth application name        
+    app_name : str{'zoom', 'teams', 'intune', 'jamf', 'vmware'}        
     
     QUERY PARAMS
     ------------
-    forward : str
-      Mist portal url to which backend needs to redirect after succesful OAuth authorization. **Required** to get the `authorization_url`        
+    forward : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
     query_params={}
     if forward: query_params["forward"]=forward
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteOrgOauthAppAuthorization(mist_session:_APISession, org_id:str, app_name:str) -> _APIResponse:
+def addOrgOauthAppAccounts(mist_session:_APISession, org_id:str, app_name:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgOauthAppAuthorization
+    API doc: https://doc.mist-lab.fr/#operation/addOrgOauthAppAccounts
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    app_name : str
-      OAuth application name        
+    app_name : str{'zoom', 'teams', 'intune', 'jamf', 'vmware'}        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def addOrgOauthAppAccounts(mist_session:_APISession, org_id:str, app_name:str, body:object) -> _APIResponse:
+def updateOrgOauthAppAccounts(mist_session:_APISession, org_id:str, app_name:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addOrgOauthAppAccounts
+    API doc: https://doc.mist-lab.fr/#operation/updateOrgOauthAppAccounts
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    app_name : str
-      OAuth application name        
+    app_name : str{'zoom', 'teams', 'intune', 'jamf', 'vmware'}        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def updateOrgOauthAppAccounts(mist_session:_APISession, org_id:str, app_name:str, body:object) -> _APIResponse:
+def deleteOrgOauthAppAuthorization(mist_session:_APISession, org_id:str, app_name:str, account_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgOauthAppAccounts
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgOauthAppAuthorization
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str
-    app_name : str
-      OAuth application name        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    app_name : str{'zoom', 'teams', 'intune', 'jamf', 'vmware'}
+    account_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/orgs/{org_id}/setting/{app_name}/link_accounts/{account_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sitegroups.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sitegroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSiteGroups")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSiteGroups")  
 def getOrgSiteGroups(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteGroups
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sites.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sites.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSites")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSites")  
 def getOrgSites(mist_session:_APISession, org_id:str, limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSites
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -152,45 +152,29 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     analytic_enabled : bool
-      if Advanced Analytic feature is enabled
     app_waking : bool
-      if App Waking feature is enabled
     asset_enabled : bool
-      if Asset Tracking is enabled
     auto_upgrade_enabled : bool
-      if Auto Upgrade feature is enabled
     auto_upgrade_version : str
-      if Auto Upgrade feature is enabled
     country_code : str
-      site country code
     honeypot_enabled : bool
-      if Honeypot detection is enabled
     id : str
-      site id
     locate_unconnected : bool
-      if unconnected client are located
     mesh_enabled : bool
-      if Mesh feature is enabled
     name : str
-      site name
     rogue_enabled : bool
-      if Rogue detection is enabled
     remote_syslog_enabled : bool
-      if Remote Syslog is enabled
     rtsa_enabled : bool
-      if managed mobility feature is enabled
     vna_enabled : bool
-      if Virtual Network Assistant is enabled
     wifi_enabled : bool
-      if WIFI feature is enabled
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/sitetemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/sitetemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSiteTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSiteTemplates")  
 def getOrgSiteTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSiteTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/ssoroles.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/ssoroles.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSsoRoles")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSsoRoles")  
 def getOrgSsoRoles(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoRoles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/ssos.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/ssos.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSsos")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSsos")  
 def getOrgSsos(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsos
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -174,15 +174,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/ssos/{sso_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSsoLatestFailures")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgSsoLatestFailures")  
 def getOrgSsoLatestFailures(mist_session:_APISession, org_id:str, sso_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgSsoLatestFailures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/ssr.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wxtags.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,189 +10,218 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOrg128TRegistrationCommands(mist_session:_APISession, org_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWxTags")  
+def getSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrg128TRegistrationCommands
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    page : int, default: 1
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/128routers/register_cmd"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/wxtags"
+    query_params={}
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgSsrUpgrades")  
-def getOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def listSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    page : int, default: 1
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/wxtags"
+    query_params={}
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgSsrUpgrades(mist_session:_APISession, org_id:str) -> _APIResponse:
+def createSiteWxTag(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgSsrUpgrades
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/wxtags"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def upgradeOrgSsrs(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def getSiteApplicationList(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgradeOrgSsrs
+    API doc: https://doc.mist-lab.fr/#operation/getSiteApplicationList
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxtags/apps"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def cancelOrgSsrUpgrade(mist_session:_APISession, org_id:str, upgrade_id:str, body:object) -> _APIResponse:
+def getSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/cancelOrgSsrUpgrade
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    upgrade_id : str        
+    site_id : str
+    wxtag_id : str        
     
-    BODY PARAMS
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def deleteSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTag
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
     -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    site_id : str
+    wxtag_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/upgrade/{upgrade_id}/cancel"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAvailableSsrVersions")  
-def getOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
+def updateSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
+    site_id : str
+    wxtag_id : str        
     
-    QUERY PARAMS
-    ------------
-    channel : str        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
-    query_params={}
-    if channel: query_params["channel"]=channel
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def listOrgAvailableSsrVersions(mist_session:_APISession, org_id:str, channel:str=None) -> _APIResponse:
+def getSiteCurrentMatchingClientsOfAWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgAvailableSsrVersions
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentMatchingClientsOfAWxTag
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str        
-    
-    QUERY PARAMS
-    ------------
-    channel : str        
+    site_id : str
+    wxtag_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/ssr/versions"
-    query_params={}
-    if channel: query_params["channel"]=channel
+    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}/clients"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/stats.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/stats.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgAssetsStats")  
 def getOrgAssetsStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -255,15 +255,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/bgp_peers/search"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgDevicesStats")  
 def getOrgDevicesStats(mist_session:_APISession, org_id:str, type:str="ap", status:str="all", site_id:str=None, mac:str=None, evpntopo_id:str=None, evpn_unused:str=None, fields:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -276,17 +276,15 @@
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway', 'all'}, default: ap
     status : str{'all', 'connected', 'disconnected'}, default: all
     site_id : str
     mac : str
     evpntopo_id : str
-      EVPN Topology ID
     evpn_unused : str
-      if `evpn_unused`==`true`, find EVPN eligible switches which don’t belong to any EVPN Topology yet
     fields : str
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
@@ -328,17 +326,15 @@
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway', 'all'}, default: ap
     status : str{'all', 'connected', 'disconnected'}, default: all
     site_id : str
     mac : str
     evpntopo_id : str
-      EVPN Topology ID
     evpn_unused : str
-      if `evpn_unused`==`true`, find EVPN eligible switches which don’t belong to any EVPN Topology yet
     fields : str
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
@@ -360,15 +356,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgMxEdgesStats")  
 def getOrgMxEdgesStats(mist_session:_APISession, org_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", for_site:str="false") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -381,16 +377,15 @@
     QUERY PARAMS
     ------------
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d
-    for_site : str{'true', 'false', 'any'}, default: false
-      filter for site level mist edges        
+    for_site : str{'true', 'false', 'any'}, default: false        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/mxedges"
@@ -420,16 +415,15 @@
     QUERY PARAMS
     ------------
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d
-    for_site : str{'true', 'false', 'any'}, default: false
-      filter for site level mist edges        
+    for_site : str{'true', 'false', 'any'}, default: false        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/stats/mxedges"
@@ -503,71 +497,42 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_errors : int
-      Output errors
     rx_errors : int
-      Input errors
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     mac_limit : int
-      Limit on number of dynamically learned macs
     mac_count : int
-      Number of mac addresses in the forwarding table
     up : bool
-      indicates if interface is up
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true` && has Authenticator role
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -624,65 +589,39 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'port_id', 'port_mac', 'full_duplex', 'mac', 'neighbor_mac', 'neighbor_port_desc', 'neighbor_system_name', 'poe_disabled', 'poe_mode', 'poe_on', 'speed', 'up'}, default: mac
-      port_id, port_mac, full_duplex, mac, neighbor_macneighbor_port_desc, neighbor_system_name, poe_disabled, poe_mode, poe_on, speed, up
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true`
     up : bool
-      indicates if interface is up
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -722,32 +661,30 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countOrgTunnelsStats(mist_session:_APISession, org_id:str, distinct:str=None, type:str="wxtunnel") -> _APIResponse:
+def countOrgTunnelsStats(mist_session:_APISession, org_id:str, distinct:str="wxtunnel_id", type:str="wxtunnel") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countOrgTunnelsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
-    distinct : str{'auth_algo'}
-      - If `type`==`wxtunnel`: wxtunnel_id / ap / remote_ip / remote_port / state / mxedge_id / mxcluster_id / site_id / peer_mxedge_id; default is wxtunnel_id 
-- If `type`==`wan`: mac / site_id / node / peer_ip / peer_host/ ip / tunnel_name / protocol / auth_algo / encrypt_algo / ike_version / last_event / up
+    distinct : str{'auth_algo', 'wxtunnel_id', 'ap', 'remote_ip', 'remote_port', 'state', 'mxedge_id', 'mxcluster_id', 'site_id', 'peer_mxedge_id', 'mac', 'node', 'peer_ip', 'peer_host', 'ip', 'tunnel_name', 'protocol', 'encrypt_algo', 'ike_version', 'last_event', 'up'}, default: wxtunnel_id
     type : str{'wxtunnel', 'wan'}, default: wxtunnel        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
@@ -770,42 +707,28 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mxcluster_id : str
-      if `type`==`wxtunnel`
     site_id : str
     wxtunnel_id : str
-      if `type`==`wxtunnel`
     ap : str
-      if `type`==`wxtunnel`
     mac : str
-      if `type`==`wan`
     node : str
-      if `type`==`wan`
     peer_ip : str
-      if `type`==`wan`
     peer_host : str
-      if `type`==`wan`
     ip : str
-      if `type`==`wan`
     tunnel_name : str
-      if `type`==`wan`
     protocol : str
-      if `type`==`wan`
     auth_algo : str
-      if `type`==`wan`
     encrypt_algo : str
-      if `type`==`wan`
     ike_version : str
-      if `type`==`wan`
     up : str
-      if `type`==`wan`
     type : str{'wxtunnel', 'wan'}, default: wxtunnel
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/subscriptions.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/subscriptions.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/templates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgTemplates")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgTemplates")  
 def getOrgTemplates(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTemplates
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/tickets.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/tickets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgTickets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgTickets")  
 def getOrgTickets(mist_session:_APISession, org_id:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgTickets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/troubleshoot.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/troubleshoot.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,21 +26,18 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      **required** when troubleshooting device or a client
     site_id : str
-      **required** when troubleshooting site
     start : int
     end : int
-    type : str{'wireless', 'wired', 'wan'}
-      when troubleshooting site, type of network to troubleshoot        
+    type : str{'wireless', 'wired', 'wan'}        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/troubleshoot"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/vars.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/vars.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/vpns.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/usermacs.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,78 +10,86 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgsVpns")  
-def getOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgUserMacs")  
+def getOrgUserMacs(mist_session:_APISession, org_id:str, blacklisted:bool=None, for:bool=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
+    API doc: https://doc.mist-lab.fr/#operation/listOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
+    blacklisted : bool
+    for : bool
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/orgs/{org_id}/usermacs"
     query_params={}
+    if blacklisted: query_params["blacklisted"]=blacklisted
+    if for: query_params["for"]=for
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listOrgsVpns(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listOrgUserMacs(mist_session:_APISession, org_id:str, blacklisted:bool=None, for:bool=None, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listOrgsVpns
+    API doc: https://doc.mist-lab.fr/#operation/listOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
+    blacklisted : bool
+    for : bool
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/orgs/{org_id}/usermacs"
     query_params={}
+    if blacklisted: query_params["blacklisted"]=blacklisted
+    if for: query_params["for"]=for
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createOrgVpns(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
+def createOrgUserMacs(mist_session:_APISession, org_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createOrgVpns
+    API doc: https://doc.mist-lab.fr/#operation/createOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,87 +102,57 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns"
+    uri = f"/api/v1/orgs/{org_id}/usermacs"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
+def deleteOrgUserMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOrgVpn
+    API doc: https://doc.mist-lab.fr/#operation/deleteOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    vpn_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
+    uri = f"/api/v1/orgs/{org_id}/usermacs/delete"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def deleteOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str) -> _APIResponse:
+def importOrgUserMacs(mist_session:_APISession, org_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteOrgVpn
+    API doc: https://doc.mist-lab.fr/#operation/importOrgUserMacs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    org_id : str
-    vpn_id : str        
+    org_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
+    uri = f"/api/v1/orgs/{org_id}/usermacs/import"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
-    
-def updateOrgVpn(mist_session:_APISession, org_id:str, vpn_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateOrgVpn
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    org_id : str
-    vpn_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/orgs/{org_id}/vpns/{vpn_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wan_client.py` & `mistapi-0.48.0/src/mistapi/api/v1/utils/test_telstra.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,35 +10,30 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countOrgWanClientEvents(mist_session:_APISession, org_id:str, distinct:str="type") -> _APIResponse:
+def testSiteWlanTelstraSetup(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countOrgWanClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTelstraSetup
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
+    BODY PARAMS
     -----------
-    org_id : str        
-    
-    QUERY PARAMS
-    ------------
-    distinct : str{'type', 'hostname', 'ip', 'mfg', 'mac'}, default: type        
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/orgs/{org_id}/wan_client/events/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/utils/test_telstra"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wan_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wan_clients.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchOrgWanClientEvents(mist_session:_APISession, org_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, nacrule_id:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchOrgWanClientEvents(mist_session:_APISession, org_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, nacrule_id:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgWanClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -64,30 +64,23 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      Event type, e.g. CLIENT_IP_ASSIGNED, CLIENT_IP_RENEWED, CLIENT_IP_EXPIRED
     mac : str
-      partial / full MAC address
     hostname : str
-      partial / full hostname
     ip : str
-      client IP
     mfg : str
-      Manufacture
     nacrule_id : str
-      nacrule_id
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/wan_clients/events/search"
@@ -97,16 +90,15 @@
     if hostname: query_params["hostname"]=hostname
     if ip: query_params["ip"]=ip
     if mfg: query_params["mfg"]=mfg
     if nacrule_id: query_params["nacrule_id"]=nacrule_id
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def searchOrgWanClients(mist_session:_APISession, org_id:str, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgWanClients
     
@@ -118,21 +110,17 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      partial / full MAC address
     hostname : str
-      partial / full hostname
     ip : str
-      client IP
     mfg : str
-      Manufacture
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/webhooks.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/webhooks.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgWebhooks")  
 def getOrgWebhooks(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -174,15 +174,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def searchOrgWebhooksDeliveries(mist_session:_APISession, org_id:str, webhook_id:str, site_id:str=None, error:str=None, status_code:int=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
+def searchOrgWebhooksDeliveries(mist_session:_APISession, org_id:str, webhook_id:str, site_id:str=None, error:str=None, status_code:int=None, status:str=None, topic:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchOrgWebhooksDeliveries
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -193,15 +193,16 @@
     webhook_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
     error : str
     status_code : int
-    topic : str{'alarms', 'audits', 'device-updowns', 'ping'}
+    status : str{'success', 'failure'}
+    topic : str{'alarms', 'audits', 'device-updowns', 'occupancy-alerts', 'ping'}
       webhook topic
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100        
     
     RETURN
@@ -210,14 +211,15 @@
         response from the API call
     """
     uri = f"/api/v1/orgs/{org_id}/webhooks/{webhook_id}/events/search"
     query_params={}
     if site_id: query_params["site_id"]=site_id
     if error: query_params["error"]=error
     if status_code: query_params["status_code"]=status_code
+    if status: query_params["status"]=status
     if topic: query_params["topic"]=topic
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wired_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wired_clients.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,31 +64,22 @@
     PATH PARAMS
     -----------
     org_id : str        
     
     QUERY PARAMS
     ------------
     site_id : str
-      Site ID
     device_mac : str
-      device mac
     mac : str
-      client mac
     port_id : str
-      port id
     vlan : int
-      vlan
     ip : str
-      ip
     manufacture : str
-      client manufacturer
     text : str
-      single entry of hostname/mac
     nacrule_id : str
-      nacrule_id
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wlans.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wlans.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgWlans")  
 def getOrgWlans(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wxrules.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wxrules.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgWxRules")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgWxRules")  
 def getOrgWxRules(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wxtags.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wxtags.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgWxTags")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgWxTags")  
 def getOrgWxTags(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTags
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/orgs/wxtunnels.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/wxtunnels.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listOrgWxTunnels")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listOrgWxTunnels")  
 def getOrgWxTunnels(mist_session:_APISession, org_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listOrgWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/recover/recover.py` & `mistapi-0.48.0/src/mistapi/api/v1/recover/recover.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/recover/verify.py` & `mistapi-0.48.0/src/mistapi/api/v1/recover/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/register/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/register/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/register/recaptcha.py` & `mistapi-0.48.0/src/mistapi/api/v1/register/recaptcha.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/register/register.py` & `mistapi-0.48.0/src/mistapi/api/v1/register/register.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/register/verify.py` & `mistapi-0.48.0/src/mistapi/api/v1/register/verify.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/__init__.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/apitokens.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/apitokens.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listApiTokens")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listApiTokens")  
 def getApiTokens(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listApiTokens
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/logs.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSelfAuditLogs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSelfAuditLogs")  
 def getSelfAuditLogs(mist_session:_APISession, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSelfAuditLogs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/oauth.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/update.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,62 +10,53 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getOAuth2UrlForLinking(mist_session:_APISession, provider:str, forward:str=None) -> _APIResponse:
+def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getOAuth2UrlForLinking
+    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
+    BODY PARAMS
     -----------
-    provider : str        
-    
-    QUERY PARAMS
-    ------------
-    forward : str        
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
-    query_params={}
-    if forward: query_params["forward"]=forward
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/self/update"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def linkOAuth2MistAccount(mist_session:_APISession, provider:str, body:object) -> _APIResponse:
+def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/linkOAuth2MistAccount
+    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    provider : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    token : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/oauth/{provider}"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/self/update/verify/{token}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/self.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/self.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/subscriptions.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/subscriptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listAlarmSubscriptions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listAlarmSubscriptions")  
 def getAlarmSubscriptions(mist_session:_APISession) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listAlarmSubscriptions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/two_factor.py` & `mistapi-0.48.0/src/mistapi/api/v1/self/two_factor.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     QUERY PARAMS
     ------------
-    by : str{'qrcode'}, default: qrcode
-      if `by`==`qrcode`, returns the secret as a qrcode image        
+    by : str{'qrcode'}, default: qrcode        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/self/two_factor/token"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/self/update.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/sites.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,53 +10,80 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def updateSelfEmail(mist_session:_APISession, body:object) -> _APIResponse:
+def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSelfEmail
+    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    BODY PARAMS
+    PATH PARAMS
     -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/update"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def verifySelfEmail(mist_session:_APISession, token:str) -> _APIResponse:
+def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/verifySelfEmail
+    API doc: https://doc.mist-lab.fr/#operation/deleteSite
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    token : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/self/update/verify/{token}"
+    uri = f"/api/v1/sites/{site_id}"
     query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/__init__.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from mistapi.api.v1.sites import alarms
 from mistapi.api.v1.sites import anomaly
 from mistapi.api.v1.sites import apps
 from mistapi.api.v1.sites import aptemplates
 from mistapi.api.v1.sites import assetfilters
 from mistapi.api.v1.sites import assets
 from mistapi.api.v1.sites import beacons
-from mistapi.api.v1.sites import call
 from mistapi.api.v1.sites import clients
 from mistapi.api.v1.sites import deviceprofiles
 from mistapi.api.v1.sites import devices
 from mistapi.api.v1.sites import events
 from mistapi.api.v1.sites import evpn_topologies
 from mistapi.api.v1.sites import gatewaytemplates
 from mistapi.api.v1.sites import guests
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/alarms.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/alarms.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,24 +80,19 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type', 'acked', 'severity', 'group'}, default: type
-      Group by and count the alarms by some distinct field
     ack_admin_name : str
-      Name of the admins who have acked the alarms; accepts multiple values separated by comma
     acked : bool
     type : str
-      Key-name of the alarms; accepts multiple values separated by comma
     severity : str
-      Alarm severity; accepts multiple values separated by comma
     group : str
-      Alarm group name; accepts multiple values separated by comma
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -133,22 +128,18 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      Key-name of the alarms; accepts multiple values separated by comma
     ack_admin_name : str
-      Name of the admins who have acked the alarms; accepts multiple values separated by comma
     acked : bool
     severity : str
-      Alarm severity; accepts multiple values separated by comma
     group : str
-      Alarm group name; accepts multiple values separated by comma
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/anomaly.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/anomaly.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/apps.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/networks.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,54 +10,64 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteApps")  
-def getSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteNetworksDerived")  
+def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteApps(mist_session:_APISession, site_id:str) -> _APIResponse:
+def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteApps
+    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
+    QUERY PARAMS
+    ------------
+    resolve : bool        
+    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/apps"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    query_params={}
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/aptemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/aptemplates.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/aptemplates/derived"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/assetfilters.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/assetfilters.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteAssetFilters")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteAssetFilters")  
 def getSiteAssetFilters(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetFilters
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/assets.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteAssets")  
 def getSiteAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/beacons.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/beacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteBeacons")  
 def getSiteBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/call.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/deviceprofiles.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,70 +10,64 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteCallEvents(mist_session:_APISession, site_id:str, distinct:str=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteDeviceProfilesDerived")  
+def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteCallEvents
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    distinct : str{'type', 'app'}        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/call/events/count"
+    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
     query_params={}
-    if distinct: query_params["distinct"]=distinct
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteCallEvents(mist_session:_APISession, site_id:str, type:str=None, ap:str=None, mac:str=None, app:str=None) -> _APIResponse:
+def listSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteCallEvents
+    API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    type : str
-      Event Type. See [listCallEventsDefinitions](/#operation/listCallEventsDefinitions)
-    ap : str
-    mac : str
-    app : str        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/call/events/search"
+    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
     query_params={}
-    if type: query_params["type"]=type
-    if ap: query_params["ap"]=ap
-    if mac: query_params["mac"]=mac
-    if app: query_params["app"]=app
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/maps.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,71 +10,78 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteWirelessClients(mist_session:_APISession, site_id:str, distinct:str, ssid:str=None, ap:str=None, ip_address:str=None, vlan:str=None, hostname:str=None, os:str=None, model:str=None, device:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteMaps")  
+def getSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClients
+    API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    distinct : str{'ssid', 'ap', 'ip', 'vlan', 'hostname', 'os', 'model', 'device'}, default: device
-    ssid : str
-    ap : str
-    ip_address : str
-    vlan : str
-    hostname : str
-    os : str
-    model : str
-    device : str
     page : int, default: 1
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/count"
+    uri = f"/api/v1/sites/{site_id}/maps"
     query_params={}
-    if distinct: query_params["distinct"]=distinct
-    if ssid: query_params["ssid"]=ssid
-    if ap: query_params["ap"]=ap
-    if ip_address: query_params["ip_address"]=ip_address
-    if vlan: query_params["vlan"]=vlan
-    if hostname: query_params["hostname"]=hostname
-    if os: query_params["os"]=os
-    if model: query_params["model"]=model
-    if device: query_params["device"]=device
     if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def disconnectSiteMultipleClients(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def listSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteMultipleClients
+    API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    QUERY PARAMS
+    ------------
+    page : int, default: 1
+    limit : int, default: 100        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps"
+    query_params={}
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def createSiteMap(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/createSiteMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -87,467 +94,490 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/disconnect"
+    uri = f"/api/v1/sites/{site_id}/maps"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def countSiteWirelessClientEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def importSiteMapsFile(mist_session:_APISession, site_id:str, auto_deviceprofile_assignment:bool=None, csv:str=None, file:str=None, json:dict=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/importSiteMaps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    distinct : str{'type', 'proto', 'band', 'channel', 'wlan_id', 'ssid'}
-      type / proto / band / channel / wlan_id / ssid
-    type : str
-      event type, e.g. MARVIS_EVENT_CLIENT_FBT_FAILURE
-    reason_code : int
-      for assoc/disassoc events
-    ssid : str
-      SSID Name
-    ap : str
-      AP MAC
-    proto : str{'b', 'g', 'n', 'ac', 'ax', 'a'}
-      802.11 standard
-    band : str{'24', '5'}
-      24 / 5
-    wlan_id : str
-      wlan_id
-    page : int, default: 1
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    BODY PARAMS
+    -----------
+    auto_deviceprofile_assignment : bool
+        whether to auto assign device to deviceprofile by name
+    csv : str
+        path to the file to upload. csv file for ap name mapping, optional
+    file : str
+        path to the file to upload. ekahau or ibwave file
+    json : dict
+        import_all_floorplans : bool
+        import_height : bool, default: True
+        import_orientation : bool, default: True
+        vendor_name : {'ekahau', 'ibwave'}
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/events/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    if type: query_params["type"]=type
-    if reason_code: query_params["reason_code"]=reason_code
-    if ssid: query_params["ssid"]=ssid
-    if ap: query_params["ap"]=ap
-    if proto: query_params["proto"]=proto
-    if band: query_params["band"]=band
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    multipart_form_data = {
+        "auto_deviceprofile_assignment":auto_deviceprofile_assignment,
+        "csv":csv,
+        "file":file,
+        "json":json,
+    }
+    uri = f"/api/v1/sites/{site_id}/maps/import"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    return resp
+
+def getSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteMap
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteWirelessClientEvents(mist_session:_APISession, site_id:str, type:str=None, reason_code:int=None, ssid:str=None, ap:str=None, proto:str=None, band:str=None, wlan_id:str=None, nacrule_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def deleteSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    map_id : str        
     
-    QUERY PARAMS
-    ------------
-    type : str
-      event type, e.g. MARVIS_EVENT_CLIENT_FBT_FAILURE
-    reason_code : int
-      for assoc/disassoc events
-    ssid : str
-      SSID Name
-    ap : str
-      AP MAC
-    proto : str{'b', 'g', 'n', 'ac', 'ax', 'a'}
-      802.11 standard
-    band : str{'24', '5'}
-      24 / 5
-    wlan_id : str
-      wlan_id
-    nacrule_id : str
-      nacrule_id
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteMap
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/events/search"
-    query_params={}
-    if type: query_params["type"]=type
-    if reason_code: query_params["reason_code"]=reason_code
-    if ssid: query_params["ssid"]=ssid
-    if ap: query_params["ap"]=ap
-    if proto: query_params["proto"]=proto
-    if band: query_params["band"]=band
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if nacrule_id: query_params["nacrule_id"]=nacrule_id
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def searchSiteWirelessClients(mist_session:_APISession, site_id:str, mac:str=None, ip_address:str=None, hostname:str=None, device:str=None, os:str=None, model:str=None, ap:str=None, ssid:str=None, text:str=None, nacrule_id:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def deleteSiteApAutoOrientation(mist_session:_APISession, map_id:str, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClients
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteApAutoOrientation
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
+    map_id : str
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    mac : str
-      partial / full MAC address
-    ip_address : str
-    hostname : str
-      partial / full hostname
-    device : str
-      device type, e.g. Mac, Nvidia, iPhone
-    os : str
-      os, e.g. Sierra, Yosemite, Windows 10
-    model : str
-      model, e.g. “MBP 15 late 2013”, 6, 6s, “8+ GSM”
-    ap : str
-      AP mac where the client has connected to
-    ssid : str
-    text : str
-      partial / full MAC address, hostname, username, psk_name or ip
-    nacrule_id : str
-      nacrule_id
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/search"
-    query_params={}
-    if mac: query_params["mac"]=mac
-    if ip_address: query_params["ip_address"]=ip_address
-    if hostname: query_params["hostname"]=hostname
-    if device: query_params["device"]=device
-    if os: query_params["os"]=os
-    if model: query_params["model"]=model
-    if ap: query_params["ap"]=ap
-    if ssid: query_params["ssid"]=ssid
-    if text: query_params["text"]=text
-    if nacrule_id: query_params["nacrule_id"]=nacrule_id
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_orient"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def countSiteWirelessClientSessions(mist_session:_APISession, site_id:str, distinct:str="mac", ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def startSiteApAutoOrientation(mist_session:_APISession, map_id:str, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteWirelessClientSessions
+    API doc: https://doc.mist-lab.fr/#operation/startSiteApAutoOrientation
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
+    map_id : str
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    distinct : str{'ssid', 'wlan_id', 'ap', 'mac', 'client_family', 'client_manufacture', 'client_model', 'client_os'}, default: mac
-    ap : str
-      AP MAC
-    band : str
-      24 /5
-    client_family : str
-      E.g. “Mac”, “iPhone”, “Apple watch”
-    client_manufacture : str
-      E.g. “Apple”
-    client_model : str
-      E.g. “8+”, “XS”
-    client_os : str
-      E.g. “Mojave”, “Windows 10”, “Linux”
-    ssid : str
-      SSID
-    wlan_id : str
-      wlan_id
-    page : int, default: 1
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/sessions/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    if ap: query_params["ap"]=ap
-    if band: query_params["band"]=band
-    if client_family: query_params["client_family"]=client_family
-    if client_manufacture: query_params["client_manufacture"]=client_manufacture
-    if client_model: query_params["client_model"]=client_model
-    if client_os: query_params["client_os"]=client_os
-    if ssid: query_params["ssid"]=ssid
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_orient"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def getSiteApAutoPlacement(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteApAutoPlacement
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteWirelessClientSessions(mist_session:_APISession, site_id:str, ap:str=None, band:str=None, client_family:str=None, client_manufacture:str=None, client_model:str=None, client_username:str=None, client_os:str=None, ssid:str=None, wlan_id:str=None, psk_id:str=None, psk_name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def deleteSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteWirelessClientSessions
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteApAutoplacement
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    map_id : str        
     
-    QUERY PARAMS
-    ------------
-    ap : str
-      AP MAC
-    band : str{'24', '5'}
-      5 / 24
-    client_family : str
-      E.g. “Mac”, “iPhone”, “Apple watch”
-    client_manufacture : str
-      E.g. “Apple”
-    client_model : str
-      E.g. “8+”, “XS”
-    client_username : str
-      Username
-    client_os : str
-      E.g. “Mojave”, “Windows 10”, “Linux”
-    ssid : str
-      SSID
-    wlan_id : str
-      wlan_id
-    psk_id : str
-    psk_name : str
-      PSK Name
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def runSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/runSiteApAutoplacement
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/sessions/search"
-    query_params={}
-    if ap: query_params["ap"]=ap
-    if band: query_params["band"]=band
-    if client_family: query_params["client_family"]=client_family
-    if client_manufacture: query_params["client_manufacture"]=client_manufacture
-    if client_model: query_params["client_model"]=client_model
-    if client_username: query_params["client_username"]=client_username
-    if client_os: query_params["client_os"]=client_os
-    if ssid: query_params["ssid"]=ssid
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if psk_id: query_params["psk_id"]=psk_id
-    if psk_name: query_params["psk_name"]=psk_name
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def unauthorizeSiteMultipleClients(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def clearSiteApAutoOrient(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteMultipleClients
+    API doc: https://doc.mist-lab.fr/#operation/clearSiteApAutoOrient
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    map_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/unauthorize"
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_auto_orient"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def reauthSiteDot1xWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+def clearSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/reauthSiteDot1xWirelessClient
+    API doc: https://doc.mist-lab.fr/#operation/clearSiteApAutoplacement
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    client_mac : str        
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/coa"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_autoplacement"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def disconnectSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+def deleteSiteMapImage(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/disconnectSiteWirelessClient
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMapImage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    client_mac : str        
+    map_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/disconnect"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def getSiteEventsForClient(mist_session:_APISession, site_id:str, client_mac:str, type:str=None, proto:str=None, band:str=None, channel:str=None, wlan_id:str=None, ssid:str=None, start:int=None, end:int=None, page:int=1, limit:int=100, duration:str="1d") -> _APIResponse:
+def addSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file:str=None, json:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteEventsForClient
+    API doc: https://doc.mist-lab.fr/#operation/addSiteMapImage
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    client_mac : str        
+    map_id : str        
     
-    QUERY PARAMS
-    ------------
-    type : str{'b', 'g', 'n'}
-      e.g. MARVIS_EVENT_CLIENT_DHCP_STUCK
-    proto : str{'a', 'b', 'g', 'n', 'ac', 'ax'}
-      a / b / g / n / ac / ax
-    band : str
-      24 / 5
-    channel : str
-    wlan_id : str
-    ssid : str
-    start : int
-    end : int
-    page : int, default: 1
-    limit : int, default: 100
-    duration : str, default: 1d        
+    BODY PARAMS
+    -----------
+    file : str
+        path to the file to upload. binary file
+    json : str
+        JSON string describing your upload
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/events"
-    query_params={}
-    if type: query_params["type"]=type
-    if proto: query_params["proto"]=proto
-    if band: query_params["band"]=band
-    if channel: query_params["channel"]=channel
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if ssid: query_params["ssid"]=ssid
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if duration: query_params["duration"]=duration
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    multipart_form_data = {
+        "file":file,
+        "json":json,
+    }
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
     return resp
+
+def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file:str=None, json:dict=None) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/replaceSiteMapImage
     
-def unauthorizeSiteWirelessClient(mist_session:_APISession, site_id:str, client_mac:str) -> _APIResponse:
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    file : str
+        path to the file to upload. 
+    json : dict
+        transform : dict
+        If `transform` is provided, all the locations of the objects on the map (AP, Zone, Vbeacon, Beacon) will be transformed as well (relative to the new Map)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
     """
-    API doc: https://doc.mist-lab.fr/#operation/unauthorizeSiteWirelessClient
+    multipart_form_data = {
+        "file":file,
+        "json":json,
+    }
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/replace"
+    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    return resp
+
+def bulkAssignSiteApsToMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/bulkAssignSiteApsToMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    client_mac : str        
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/clients/{client_mac}/unauthorize"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/set_map"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def confirmSiteApLocalizationData(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/confirmSiteApLocalizationData
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/use_auto_ap_values"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
+def importSiteWayfindings(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/importSiteWayfindings
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/wayfinding/import"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/count.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/count.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteZoneSessions(mist_session:_APISession, site_id:str, zone_type:str, distinct:str="scope_id", user_type:str="client", user:str=None, scope_id:str=None, scope:str="site", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteZoneSessions(mist_session:_APISession, site_id:str, zone_type:str, distinct:str="scope_id", user_type:str=None, user:str=None, scope_id:str=None, scope:str="site", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteZoneSessions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -27,22 +27,19 @@
     -----------
     site_id : str
     zone_type : str{'zones', 'rssizones'}        
     
     QUERY PARAMS
     ------------
     distinct : str{'user_type', 'user', 'scope_id', 'scope'}, default: scope_id
-    user_type : str{'client', 'sdkclient', 'asset'}, default: client
+    user_type : str{'sdkclient', 'client', 'asset'}
       user type
     user : str
-      client MAC / Asset MAC / SDK UUID
     scope_id : str
-      if `scope`==`map`/`zone`/`rssizone`, the scope id
     scope : str{'site', 'map', 'zone', 'rssizone'}, default: site
-      scope
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/deviceprofiles.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/vpns.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,66 +10,64 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteDeviceProfilesDerived")  
-def getSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteVpnsDerived")  
+def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteDeviceProfilesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteDeviceProfilesDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/deviceprofiles/derived"
+    uri = f"/api/v1/sites/{site_id}/vpns/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/devices.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/devices.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteDevices")  
 def getSiteDevices(mist_session:_APISession, site_id:str, type:str="ap", name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -27,15 +27,14 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway', 'all'}, default: ap
-      device type
     name : str
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
@@ -62,15 +61,14 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway', 'all'}, default: ap
-      device type
     name : str
     page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
@@ -96,16 +94,15 @@
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    country_code : str
-      country code for the site (for AP config generation), in [two-character](http://en.wikipedia.org/wiki/ISO_3166-1_alpha-2)        
+    country_code : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/ap_channels"
@@ -150,45 +147,44 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteDeviceConfigHistory(mist_session:_APISession, site_id:str, device_type:str="ap", mac:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteDeviceConfigHistory(mist_session:_APISession, site_id:str, type:str="ap", mac:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteDeviceConfigHistory
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    device_type : str{'ap', 'switch', 'gateway'}, default: ap
+    type : str{'ap', 'switch', 'gateway'}, default: ap
     mac : str
-      Device MAC Address
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/config_history/search"
     query_params={}
-    if device_type: query_params["device_type"]=device_type
+    if type: query_params["type"]=type
     if mac: query_params["mac"]=mac
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
@@ -249,15 +245,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteDeviceEvents(mist_session:_APISession, site_id:str, distinct:str="model", model:str=None, type:str=None, type_code:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteDeviceEvents(mist_session:_APISession, site_id:str, distinct:str="model", model:str=None, type:str=None, type_code:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -268,15 +264,14 @@
     
     QUERY PARAMS
     ------------
     distinct : str{'model', 'type', 'type_code', 'mac'}, default: model
     model : str
     type : str
     type_code : str
-    page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -285,63 +280,54 @@
     """
     uri = f"/api/v1/sites/{site_id}/devices/events/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
     if model: query_params["model"]=model
     if type: query_params["type"]=type
     if type_code: query_params["type_code"]=type_code
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteDeviceEvents(mist_session:_APISession, site_id:str, device_type:str=None, mac:str=None, model:str=None, text:str=None, timestamp:str=None, type:str=None, last_by:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteDeviceEvents(mist_session:_APISession, site_id:str, mac:str=None, model:str=None, text:str=None, timestamp:str=None, type:str=None, last_by:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    device_type : str{'ap', 'switch', 'gateway'}
     mac : str
-      device mac
     model : str
-      device model
     text : str
-      event message
     timestamp : str
-      event time
     type : str
-      see [Event Types Definition](/#operation/listDeviceEventsDefinitions)
     last_by : str
-      Return last/recent event for passed in field
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/events/search"
     query_params={}
-    if device_type: query_params["device_type"]=device_type
     if mac: query_params["mac"]=mac
     if model: query_params["model"]=model
     if text: query_params["text"]=text
     if timestamp: query_params["timestamp"]=timestamp
     if type: query_params["type"]=type
     if last_by: query_params["last_by"]=last_by
     if limit: query_params["limit"]=limit
@@ -435,30 +421,30 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteDeviceLastConfigs(mist_session:_APISession, site_id:str, device_type:str="ap", mac:str=None, version:str=None, name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteDeviceLastConfigs(mist_session:_APISession, site_id:str, type:str="ap", mac:str=None, version:str=None, name:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteDeviceLastConfigs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    device_type : str{'ap', 'switch', 'gateway'}, default: ap
+    type : str{'ap', 'switch', 'gateway'}, default: ap
     mac : str
     version : str
     name : str
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
@@ -466,15 +452,15 @@
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/last_config/search"
     query_params={}
-    if device_type: query_params["device_type"]=device_type
+    if type: query_params["type"]=type
     if mac: query_params["mac"]=mac
     if version: query_params["version"]=version
     if name: query_params["name"]=name
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
@@ -569,58 +555,36 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     hostname : str
-      partial / full hostname
     type : str{'ap', 'switch', 'gateway'}, default: ap
-      device type
     model : str
-      device model
     mac : str
-      device MAC
     version : str
-      version
     power_constrained : bool
-      power_constrained
     ip_address : str
     mxtunnel_status : str{'up', 'down'}
-      MxTunnel status, up / down
     mxedge_id : str
-      Mist Edge id, if AP is connecting to a Mist Edge
     lldp_system_name : str
-      LLDP system name
     lldp_system_desc : str
-      LLDP system description
     lldp_port_id : str
-      LLDP port id
     lldp_mgmt_addr : str
-      LLDP management ip address
     band_24_channel : int
-      Channel of band_24
     band_5_channel : int
-      Channel of band_5
     band_6_channel : int
-      Channel of band_6
     band_24_bandwith : int
-      Bandwidth of band_24
     band_5_bandwith : int
-      Bandwidth of band_5
     band_6_bandwith : int
-      Bandwidth of band_6
     eth0_port_speed : int
-      Port speed of eth0
     sort : str{'timestamp', 'mac', 'model', 'sku'}, default: timestamp
-      sort options
     desc_sort : str{'timestamp', 'mac', 'model', 'sku'}
-      sort options in reverse order
     stats : bool
-      whether to return device stats
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -682,15 +646,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/send_ble_beacon"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteDevicesUpgrade")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteDevicesUpgrade")  
 def getSiteDevicesUpgrade(mist_session:_APISession, site_id:str, status:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesUpgrade
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -813,17 +777,17 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade/{upgrade_id}/cancel"
     resp = mist_session.mist_post(uri=uri)
     return resp
     
-def upgraseSiteMultipleDevicesBios(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def upgradeSiteMultipleDevicesBios(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/upgraseSiteMultipleDevicesBios
+    API doc: https://doc.mist-lab.fr/#operation/upgradeSiteMultipleDevicesBios
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -840,15 +804,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/upgrade_bios"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteAvailableDeviceVersions")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteAvailableDeviceVersions")  
 def getSiteAvailableDeviceVersions(mist_session:_APISession, site_id:str, type:str="ap", model:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAvailableDeviceVersions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -857,17 +821,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway'}, default: ap
-      fetch version for device type (E.g. switch)
-    model : str
-      fetch version for device model, use/combine with `type` as needed (for switch and gateway devices)        
+    model : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/versions"
@@ -889,17 +851,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'ap', 'switch', 'gateway'}, default: ap
-      fetch version for device type (E.g. switch)
-    model : str
-      fetch version for device model, use/combine with `type` as needed (for switch and gateway devices)        
+    model : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/versions"
@@ -928,15 +888,15 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/devices/zerioze"
+    uri = f"/api/v1/sites/{site_id}/devices/zeroize"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
 def getSiteDevice(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDevice
     
@@ -1248,16 +1208,15 @@
     PATH PARAMS
     -----------
     site_id : str
     device_id : str        
     
     QUERY PARAMS
     ------------
-    sort : str{'true', 'false'}, default: false
-      Make output cmds sorted (for better readability) or not.        
+    sort : str{'true', 'false'}, default: false        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/config_cmd"
@@ -1603,14 +1562,37 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/release_dhcp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def reprovisionSiteOctermDevice(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/reprovisionSiteOctermDevice
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/reprovision"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
+    
 def getSiteDeviceZtpPassword(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceZtpPassword
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1733,14 +1715,42 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_arp"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def getSiteDeviceEvpnDatabase(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceEvpnDatabase
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/show_evpn_database"
+    resp = mist_session.mist_post(uri=uri, body=body)
+    return resp
+    
 def getSiteDeviceMacTable(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceMacTable
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1896,14 +1906,38 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/devices/{device_id}/support"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
+def getSiteDeviceSyntheticTest(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteDeviceSyntheticTest
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/devices/{device_id}/synthetic_test"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
 def triggerSiteDeviceSyntheticTest(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/triggerSiteDeviceSyntheticTest
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/events.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteRoamingEvents(mist_session:_APISession, site_id:str, type:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def getSiteRoamingEvents(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteRoamingEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -26,38 +26,35 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'success', 'fail', 'none'}
-      event type
-    page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/events/fast_roam"
     query_params={}
     if type: query_params["type"]=type
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteSystemEvents(mist_session:_APISession, site_id:str, distinct:str="type", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteSystemEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteSystemEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -65,29 +62,29 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type'}, default: type
-    page : int, default: 1
+    type : str
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/events/system/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
-    if page: query_params["page"]=page
+    if type: query_params["type"]=type
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/evpn_topologies.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/evpn_topologies.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,41 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteEvpnTopology(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteEvpnTopologies")  
+def getSiteEvpnTopologies(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteEvpnTopology
+    API doc: https://doc.mist-lab.fr/#operation/listSiteEvpnTopologies
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/evpn_topologies"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteEvpnTopologies(mist_session:_APISession, site_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteEvpnTopologies
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -60,17 +84,17 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/evpn_topologies"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteEvpnTolopogy(mist_session:_APISession, site_id:str, evpn_topology_id:str) -> _APIResponse:
+def getSiteEvpnTopology(mist_session:_APISession, site_id:str, evpn_topology_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteEvpnTolopogy
+    API doc: https://doc.mist-lab.fr/#operation/getSiteEvpnTopology
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/gatewaytemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/gatewaytemplates.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,16 +25,15 @@
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/gatewaytemplates/derived"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/guests.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/location.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,220 +10,225 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteAllGuestAuthorizations")  
-def getSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
+def getSiteBeamCoverageOverview(mist_session:_APISession, site_id:str, map_id:str=None, type:str=None, client_type:str=None, duration:str="1d", resolution:str="default", start:int=None, end:int=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
+    API doc: https://doc.mist-lab.fr/#operation/getSiteBeamCoverageOverview
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    wlan_id : str
-      UUID of single or multiple (Comma separated) WLAN under Site `site_id` (to filter by WLAN)        
+    map_id : str
+    type : str{'sdkclient', 'client', 'asset'}
+    client_type : str
+    duration : str, default: 1d
+    resolution : str{'default', 'fine'}, default: default
+    start : int
+    end : int        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests"
+    uri = f"/api/v1/sites/{site_id}/location/coverage"
     query_params={}
-    if wlan_id: query_params["wlan_id"]=wlan_id
+    if map_id: query_params["map_id"]=map_id
+    if type: query_params["type"]=type
+    if client_type: query_params["client_type"]=client_type
+    if duration: query_params["duration"]=duration
+    if resolution: query_params["resolution"]=resolution
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteAllGuestAuthorizations(mist_session:_APISession, site_id:str, wlan_id:str=None) -> _APIResponse:
+def getSiteMachineLearningCurrentStat(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteAllGuestAuthorizations
+    API doc: https://doc.mist-lab.fr/#operation/getSiteMachineLearningCurrentStat
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    wlan_id : str
-      UUID of single or multiple (Comma separated) WLAN under Site `site_id` (to filter by WLAN)        
+    map_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests"
+    uri = f"/api/v1/sites/{site_id}/location/ml/current"
     query_params={}
-    if wlan_id: query_params["wlan_id"]=wlan_id
+    if map_id: query_params["map_id"]=map_id
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteGuestAuthorizations(mist_session:_APISession, site_id:str, distinct:str="auth_method", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def getSiteDefaultPlfForModels(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteGuestAuthorizations
+    API doc: https://doc.mist-lab.fr/#operation/getSiteDefaultPlfForModels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    distinct : str{'auth_method', 'ssid', 'company'}, default: auth_method
-    page : int, default: 1
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
+    uri = f"/api/v1/sites/{site_id}/location/ml/defaults"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteGuestAuthorization(mist_session:_APISession, site_id:str, wlan_id:str=None, auth_method:str=None, ssid:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def clearSiteMlOverwriteForDevice(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteGuestAuthorization
+    API doc: https://doc.mist-lab.fr/#operation/clearSiteMlOverwriteForDevice
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
-    
-    QUERY PARAMS
-    ------------
-    wlan_id : str
-    auth_method : str
-    ssid : str
-    limit : int, default: 100
-    start : int
-    end : int
-    duration : str, default: 1d        
+    site_id : str
+    device_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests/search"
-    query_params={}
-    if wlan_id: query_params["wlan_id"]=wlan_id
-    if auth_method: query_params["auth_method"]=auth_method
-    if ssid: query_params["ssid"]=ssid
-    if limit: query_params["limit"]=limit
-    if start: query_params["start"]=start
-    if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/location/ml/device/{device_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def getSiteGuestAuthorization(mist_session:_APISession, site_id:str, guest_mac:str) -> _APIResponse:
+def overwriteSiteMlForDevice(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteGuestAuthorization
+    API doc: https://doc.mist-lab.fr/#operation/overwriteSiteMlForDevice
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    guest_mac : str        
+    device_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests/{guest_mac}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/location/ml/device/{device_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def deleteSiteGuestAuthorization(mist_session:_APISession, site_id:str, guest_mac:str) -> _APIResponse:
+def clearSiteMlOverwriteForMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteGuestAuthorization
+    API doc: https://doc.mist-lab.fr/#operation/clearSiteMlOverwriteForMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    guest_mac : str        
+    map_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests/{guest_mac}"
+    uri = f"/api/v1/sites/{site_id}/location/ml/map/{map_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteGuestAuthorization(mist_session:_APISession, site_id:str, guest_mac:str, body:object) -> _APIResponse:
+def overwriteSiteMlForMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteGuestAuthorization
+    API doc: https://doc.mist-lab.fr/#operation/overwriteSiteMlForMap
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    guest_mac : str        
+    map_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/guests/{guest_mac}"
+    uri = f"/api/v1/sites/{site_id}/location/ml/map/{map_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
+    
+def resetSiteMlStatsByMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/resetSiteMlStatsByMap
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    map_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/location/ml/reset/map/{map_id}"
+    resp = mist_session.mist_post(uri=uri)
+    return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/insights.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/insights.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteRogueAPs")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteRogueAPs")  
 def getSiteRogueAPs(mist_session:_APISession, site_id:str, type:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueAPs
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -167,15 +167,15 @@
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if interval: query_params["interval"]=interval
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteRogueClients")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteRogueClients")  
 def getSiteRogueClients(mist_session:_APISession, site_id:str, limit:int=100, start:int=None, end:int=None, duration:str="1d", interval:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRogueClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/licenses.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/licenses.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/location.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/pcaps.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,89 +10,94 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteBeamCoverageOverview(mist_session:_APISession, site_id:str, map_id:str=None, type:str="sdkclient", duration:str="1h", resolution:str="default", client_type:str=None, start:int=None, end:int=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSitePacketCaptures")  
+def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteBeamCoverageOverview
+    API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    map_id : str
-      map_id (filter by map_id)
-    type : str{'sdkclient', 'client', 'asset'}, default: sdkclient
-    duration : str{'1d', '5h', '1h', '30m'}, default: 1h
-      where the start time will be calculated (with end time is now)
-    resolution : str{'default', 'fine'}, default: default
-    client_type : str
-      client_type (as filter. optional)
+    page : int, default: 1
+    limit : int, default: 100
     start : int
-    end : int        
+    end : int
+    duration : str, default: 1d
+    client_mac : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/coverage"
+    uri = f"/api/v1/sites/{site_id}/pcaps"
     query_params={}
-    if map_id: query_params["map_id"]=map_id
-    if type: query_params["type"]=type
-    if duration: query_params["duration"]=duration
-    if resolution: query_params["resolution"]=resolution
-    if client_type: query_params["client_type"]=client_type
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
-    if end: query_params["end"]=end
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if client_mac: query_params["client_mac"]=client_mac
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteMachineLearningCurrentStat(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
+def listSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMachineLearningCurrentStat
+    API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    map_id : str
-      map_id (as filter, optional)        
+    page : int, default: 1
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d
+    client_mac : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/ml/current"
+    uri = f"/api/v1/sites/{site_id}/pcaps"
     query_params={}
-    if map_id: query_params["map_id"]=map_id
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if client_mac: query_params["client_mac"]=client_mac
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteDefaultPlfForModels(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteCapturingStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteDefaultPlfForModels
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCapturingStatus
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -100,139 +105,90 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/ml/defaults"
+    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def clearSiteMlOverwriteForDevice(mist_session:_APISession, site_id:str, device_id:str) -> _APIResponse:
+def stopSitePacketCapture(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/clearSiteMlOverwriteForDevice
+    API doc: https://doc.mist-lab.fr/#operation/stopSitePacketCapture
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    device_id : str        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/ml/device/{device_id}"
+    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def overwriteSiteMlForDevice(mist_session:_APISession, site_id:str, device_id:str, body:object) -> _APIResponse:
+def startSitePacketCapture(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/overwriteSiteMlForDevice
+    API doc: https://doc.mist-lab.fr/#operation/startSitePacketCapture
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    device_id : str        
+    site_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/ml/device/{device_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def clearSiteMlOverwriteForMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/clearSiteMlOverwriteForMap
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    map_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/location/ml/map/{map_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def overwriteSiteMlForMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def updateSitePacketCapture(mist_session:_APISession, site_id:str, pcap_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/overwriteSiteMlForMap
+    API doc: https://doc.mist-lab.fr/#operation/updateSitePacketCapture
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    pcap_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/location/ml/map/{map_id}"
+    uri = f"/api/v1/sites/{site_id}/pcaps/{pcap_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
-    
-def resetSiteMlStatsByMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/resetSiteMlStatsByMap
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    map_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/location/ml/reset/map/{map_id}"
-    resp = mist_session.mist_post(uri=uri)
-    return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/maps.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/sle.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,574 +10,585 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteMaps")  
-def getSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def getSiteSleClassifierDetails(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, classifier:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleClassifierDetails
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str
+    classifier : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    start : int
+    end : int
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps"
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/classifier/{classifier}/summary"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteMaps(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def getSiteSleMetricClassifiers(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteMaps
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleMetricClassifiers
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
-    
-    QUERY PARAMS
-    ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    site_id : str
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps"
-    query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/classifiers"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteMap(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def getSiteSleHistogram(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteMap
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleHistogram
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/histogram"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def importSiteMapsFile(mist_session:_APISession, site_id:str, auto_deviceprofile_assignment:bool=None, csv:str=None, file:str=None, json:dict=None) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/importSiteMaps
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    BODY PARAMS
-    -----------
-    auto_deviceprofile_assignment : bool
-        whether to auto assign device to deviceprofile by name
-    csv : str
-        path to the file to upload. csv file for ap name mapping, optional
-    file : str
-        path to the file to upload. ekahau or ibwave file
-    json : dict
-        import_all_floorplans : bool
-        import_height : bool, default: True
-        import_orientation : bool, default: True
-        vendor_name : {'ekahau', 'ibwave'}
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    multipart_form_data = {
-        "auto_deviceprofile_assignment":auto_deviceprofile_assignment,
-        "csv":csv,
-        "file":file,
-        "json":json,
-    }
-    uri = f"/api/v1/sites/{site_id}/maps/import"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
-    return resp
-
-def getSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def getSiteSleImpactSummary(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", fields:str=None, classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteMap
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactSummary
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
+    
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    fields : str{'wlan', 'device_type', 'device_os', 'band', 'ap', 'server', 'mxedge', 'switch', 'client', 'vlan', 'interface', 'chassis', 'gateway', 'peer_path', 'gateway_zones'}
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impact-summary"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if fields: query_params["fields"]=fields
+    if classifier: query_params["classifier"]=classifier
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteMap(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def getSiteSleImpactedApplications(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMap
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedApplications
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'switch', 'gateway'}
+    scope_id : str
+    metric : str        
+    
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-applications"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def updateSiteMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def getSiteSleImpactedAps(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteMap
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedAps
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def deleteSiteApAutoOrientation(mist_session:_APISession, map_id:str, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteApAutoOrientation
+    scope : str{'site'}
+    scope_id : str
+    metric : str        
     
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    map_id : str
-    site_id : str        
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_orient"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-aps"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def startSiteApAutoOrientation(mist_session:_APISession, map_id:str, site_id:str, body:object) -> _APIResponse:
+def getSiteSleImpactedChassis(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/startSiteApAutoOrientation
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedChassis
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    map_id : str
-    site_id : str        
+    site_id : str
+    scope : str{'site', 'switch', 'gateway'}
+    scope_id : str
+    metric : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_orient"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-chassis"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteApAutoPlacement(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def getSiteSleImpactedWiredClients(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteApAutoPlacement
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedWiredClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'switch', 'gateway'}
+    scope_id : str
+    metric : str        
+    
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-clients"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def getSiteSleImpactedGateways(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteApAutoplacement
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedGateways
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site'}
+    scope_id : str
+    metric : str        
+    
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-gateways"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def runSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def getSiteSleImpactedInterfaces(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/runSiteApAutoplacement
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedInterfaces
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'switch', 'gateway'}
+    scope_id : str
+    metric : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/auto_placement"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-interfaces"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def clearSiteApAutoOrient(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def getSiteSleImpactedSwitches(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/clearSiteApAutoOrient
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedSwitches
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site'}
+    scope_id : str
+    metric : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_auto_orient"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-switches"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def clearSiteApAutoplacement(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def getSiteSleImpactedWirelessClients(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d", classifier:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/clearSiteApAutoplacement
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleImpactedWirelessClients
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'ap'}
+    scope_id : str
+    metric : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d
+    classifier : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/clear_autoplacement"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/impacted-users"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if classifier: query_params["classifier"]=classifier
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteMapImage(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
+def getSiteSleSummary(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteMapImage
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleSummary
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
+    
+    QUERY PARAMS
+    ------------
+    start : int
+    end : int
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/summary"
+    query_params={}
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def addSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file:str=None, json:str=None) -> _APIResponse:
+def getSiteSleThreshold(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/addSiteMapImage
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSleThreshold
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
-    
-    BODY PARAMS
-    -----------
-    file : str
-        path to the file to upload. binary file
-    json : str
-        JSON string describing your upload
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    multipart_form_data = {
-        "file":file,
-        "json":json,
-    }
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/image"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/threshold"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
-
-def replaceSiteMapImageFile(mist_session:_APISession, site_id:str, map_id:str, file:str=None, json:dict=None) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/replaceSiteMapImage
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    map_id : str        
     
-    BODY PARAMS
-    -----------
-    file : str
-        path to the file to upload. 
-    json : dict
-        transform : dict
-        If `transform` is provided, all the locations of the objects on the map (AP, Zone, Vbeacon, Beacon) will be transformed as well (relative to the new Map)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    multipart_form_data = {
-        "file":file,
-        "json":json,
-    }
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/replace"
-    resp = mist_session.mist_post_file(uri=uri, multipart_form_data=multipart_form_data)
-    return resp
-
-def bulkAssignSiteApsToMap(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def replaceSiteSleThreshold(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/bulkAssignSiteApsToMap
+    API doc: https://doc.mist-lab.fr/#operation/replaceSiteSleThreshold
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/set_map"
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/threshold"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def confirmSiteApLocalizationData(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def updateSiteSleThreshold(mist_session:_APISession, site_id:str, scope:str, scope_id:str, metric:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/confirmSiteApLocalizationData
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteSleThreshold
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str
+    metric : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/use_auto_ap_values"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metric/{metric}/threshold"
+    resp = mist_session.mist_put(uri=uri, body=body)
     return resp
     
-def importSiteWayfindings(mist_session:_APISession, site_id:str, map_id:str, body:object) -> _APIResponse:
+def getSiteSlesMetrics(mist_session:_APISession, site_id:str, scope:str, scope_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/importSiteWayfindings
+    API doc: https://doc.mist-lab.fr/#operation/getSiteSlesMetrics
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    map_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    scope : str{'site', 'ap', 'switch', 'gateway', 'client'}
+    scope_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/maps/{map_id}/wayfinding/import"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/sle/{scope}/{scope_id}/metrics"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/mxedges.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/mxedges.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteMxEdges")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteMxEdges")  
 def getSiteMxEdges(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdges
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/mxedges"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def countSiteMxEdgeEvents(mist_session:_APISession, site_id:str, distinct:str="mxedge_id", mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", page:int=1, limit:int=100) -> _APIResponse:
+def countSiteMxEdgeEvents(mist_session:_APISession, site_id:str, distinct:str="mxedge_id", mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteMxEdgeEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -115,25 +115,20 @@
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'mxedge_id', 'type', 'mxcluster_id', 'package'}, default: mxedge_id
     mxedge_id : str
-      mist edge id
     mxcluster_id : str
-      mist edge cluster id
     type : str
-      mist edge event type [Supported Events](/#operation/listGatewayApplications)
     service : str
-      service running on mist edge(mxagent, tunterm etc)
     start : int
     end : int
     duration : str, default: 1d
-    page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
@@ -143,20 +138,19 @@
     if mxedge_id: query_params["mxedge_id"]=mxedge_id
     if mxcluster_id: query_params["mxcluster_id"]=mxcluster_id
     if type: query_params["type"]=type
     if service: query_params["service"]=service
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searcSitehMistEdgeEvents(mist_session:_APISession, site_id:str, mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", page:int=1, limit:int=100) -> _APIResponse:
+def searcSitehMistEdgeEvents(mist_session:_APISession, site_id:str, mxedge_id:str=None, mxcluster_id:str=None, type:str=None, service:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searcSitehMistEdgeEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -164,25 +158,20 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     mxedge_id : str
-      mist edge id
     mxcluster_id : str
-      mist edge cluster id
     type : str
-      mist edge event type [Supported Events](/#operation/listGatewayApplications)
     service : str
-      service running on mist edge(mxagent, tunterm etc)
     start : int
     end : int
     duration : str, default: 1d
-    page : int, default: 1
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
@@ -191,15 +180,14 @@
     if mxedge_id: query_params["mxedge_id"]=mxedge_id
     if mxcluster_id: query_params["mxcluster_id"]=mxcluster_id
     if type: query_params["type"]=type
     if service: query_params["service"]=service
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def getSiteMxEdge(mist_session:_APISession, site_id:str, mxedge_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteMxEdge
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/mxtunnels.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/mxtunnels.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/nac_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/nac_clients.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,45 +26,29 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type', 'last_nacrule_id', 'auth_type', 'last_vlan_id', 'last_nas_vendor', 'last_username', 'last_ap', 'mac', 'last_ssid', 'last_status', 'mdm_compliance_status', 'mdm_provider'}, default: type
-      NAC Policy Rule ID, if matched
     last_nacrule_id : str
-      NAC Policy Rule ID, if matched
     nacrule_matched : bool
-      NAC Policy Rule Matched
     auth_type : str
-      authentication type, e.g. “eap-tls”, “eap-ttls”, “eap-teap”, “mab”, “device-auth”
     last_vlan_id : str
-      Vlan ID
     last_nas_vendor : str
-      vendor of NAS device
     idp_id : str
-      SSO ID, if present and used
     last_ssid : str
-      SSID
     last_username : str
-      Username presented by the client
     timestamp : float
-      start time, in epoch
     last_ap : str
-      AP MAC connected to by client
     mac : str
-      MAC address
     last_status : str
-      Connection status of client i.e “permitted”, “denied, “session_ended”
     type : str
-      Client type i.e. “wireless”, “wired” etc.
     mdm_compliance_status : str
-      MDM compliancy of client i.e “compliant”, “not compliant”
     mdm_provider : str
-      MDM provider of client’s organisation eg “intune”, “jamf”
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
@@ -94,15 +78,15 @@
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteNacClientEvents(mist_session:_APISession, site_id:str, distinct:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def countSiteNacClientEvents(mist_session:_APISession, site_id:str, distinct:str=None, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteNacClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -110,92 +94,74 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type', 'nacrule_id', 'dryrun_nacrule_id', 'auth_type', 'vlan', 'nas_vendor', 'username', 'ap', 'mac', 'ssid'}
+    type : str
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/nac_clients/events/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searcSitegNacClientEvents(mist_session:_APISession, site_id:str, type:str=None, nacrule_id:str=None, nacrule_matched:bool=None, dryrun_nacrule_id:str=None, dryrun_nacrule_matched:bool=None, auth_type:str=None, vlan:int=None, nas_vendor:str=None, bssid:str=None, idp_id:str=None, idp_role:str=None, resp_attrs:list=None, ssid:str=None, username:str=None, ap:str=None, random_mac:bool=None, mac:str=None, timestamp:float=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searcsearcSiteNacClientEventsacClientEvents(mist_session:_APISession, site_id:str, type:str=None, nacrule_id:str=None, nacrule_matched:bool=None, dryrun_nacrule_id:str=None, dryrun_nacrule_matched:bool=None, auth_type:str=None, vlan:int=None, nas_vendor:str=None, bssid:str=None, idp_id:str=None, idp_role:str=None, resp_attrs:list=None, ssid:str=None, username:str=None, ap:str=None, random_mac:bool=None, mac:str=None, timestamp:float=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searcSitegNacClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/searcsearcSiteNacClientEventsacClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      event type, e.g. NAC_CLIENT_PERMIT
     nacrule_id : str
-      NAC Policy Rule ID, if matched
     nacrule_matched : bool
-      NAC Policy Rule Matched
     dryrun_nacrule_id : str
-      NAC Policy Dry Run Rule ID, if present and matched
     dryrun_nacrule_matched : bool
-      True - if dryrun rule present and matched with priority, False - if not matched or not present
     auth_type : str
-      authentication type, e.g.  “eap-tls”, “eap-ttls”, “eap-teap”, “mab”, “device-auth”
     vlan : int
-      Vlan ID
     nas_vendor : str
-      vendor of NAS device
     bssid : str
-      SSID
     idp_id : str
-      SSO ID, if present and used
     idp_role : str
-      IDP returned roles/groups for the user
     resp_attrs : list
       Radius attributes returned by NAC to NAS Devive
     ssid : str
-      SSID
     username : str
-      Username presented by the client
     ap : str
-      AP MAC
     random_mac : bool
-      AP random macMAC
     mac : str
-      MAC address
     timestamp : float
-      start time, in epoch
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/nac_clients/events/search"
@@ -217,16 +183,15 @@
     if ap: query_params["ap"]=ap
     if random_mac: query_params["random_mac"]=random_mac
     if mac: query_params["mac"]=mac
     if timestamp: query_params["timestamp"]=timestamp
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def searchSiteNacClients(mist_session:_APISession, site_id:str, last_nacrule_id:str=None, nacrule_matched:bool=None, auth_type:str=None, last_vlan_id:str=None, last_nas_vendor:str=None, idp_id:str=None, last_ssid:str=None, last_username:str=None, timestamp:float=None, last_ap:str=None, mac:str=None, last_status:str=None, type:str=None, mdm_compliance_status:str=None, mdm_provider:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteNacClients
     
@@ -238,43 +203,28 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     last_nacrule_id : str
-      NAC Policy Rule ID, if matched
     nacrule_matched : bool
-      NAC Policy Rule Matched
     auth_type : str
-      authentication type, e.g. “eap-tls”, “eap-ttls”, “eap-teap”, “mab”, “device-auth”
     last_vlan_id : str
-      Vlan ID
     last_nas_vendor : str
-      vendor of NAS device
     idp_id : str
-      SSO ID, if present and used
     last_ssid : str
-      SSID
     last_username : str
-      Username presented by the client
     timestamp : float
-      start time, in epoch
     last_ap : str
-      AP MAC connected to by client
     mac : str
-      MAC address
     last_status : str
-      Connection status of client i.e “permitted”, “denied, “session_ended”
     type : str
-      Client type i.e. “wireless”, “wired” etc.
     mdm_compliance_status : str
-      MDM compliancy of client i.e “compliant”, “not compliant”
     mdm_provider : str
-      MDM provider of client’s organisation eg “intune”, “jamf”
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/networks.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/visits.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,66 +10,53 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteNetworksDerived")  
-def getSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def searchSiteZoneSessions(mist_session:_APISession, site_id:str, zone_type:str, user_type:str=None, user:str=None, scope_id:str=None, scope:str="site", page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteZoneSessions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    zone_type : str{'zones', 'rssizones'}        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    user_type : str{'sdkclient', 'client', 'asset'}
+      user type, client (default) / sdkclient / asset
+    user : str
+    scope_id : str
+    scope : str{'site', 'map', 'zone', 'rssizone'}, default: site
+    page : int, default: 1
+    limit : int, default: 100
+    start : int
+    end : int
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
+    uri = f"/api/v1/sites/{site_id}/{zone_type}/visits/search"
     query_params={}
-    if resolve: query_params["resolve"]=resolve
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def listSiteNetworksDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteNetworksDerived
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    QUERY PARAMS
-    ------------
-    resolve : bool
-      whether resolve the site variables        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/networks/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
+    if user_type: query_params["user_type"]=user_type
+    if user: query_params["user"]=user
+    if scope_id: query_params["scope_id"]=scope_id
+    if scope: query_params["scope"]=scope
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/networktemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/rftemplates.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,35 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteNetworkTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def getSiteRfTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteNetworkTemplateDerived
+    API doc: https://doc.mist-lab.fr/#operation/getSiteRfTemplateDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/networktemplates/derived"
+    uri = f"/api/v1/sites/{site_id}/rftemplates/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/otherdevices.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/otherdevices.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteOtherDevices")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteOtherDevices")  
 def getSiteOtherDevices(mist_session:_APISession, site_id:str, vendor:str=None, mac:str=None, serial:str=None, model:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteOtherDevices
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -91,15 +91,15 @@
     if model: query_params["model"]=model
     if name: query_params["name"]=name
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteOtherDeviceEvents(mist_session:_APISession, site_id:str, distinct:str="mac", start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def countSiteOtherDeviceEvents(mist_session:_APISession, site_id:str, distinct:str="mac", type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteOtherDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -107,37 +107,37 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'mac', 'type', 'vendor', 'site_id'}, default: mac
+    type : str
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/otherdevices/events/count"
     query_params={}
     if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteOtherDeviceEvents(mist_session:_APISession, site_id:str, mac:str=None, device_mac:str=None, vendor:str=None, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchSiteOtherDeviceEvents(mist_session:_APISession, site_id:str, mac:str=None, device_mac:str=None, vendor:str=None, type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteOtherDeviceEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -145,26 +145,21 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      mac
     device_mac : str
-      mac of attached device
     vendor : str
-      vendor name
     type : str
-      event type
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/otherdevices/events/search"
@@ -172,12 +167,11 @@
     if mac: query_params["mac"]=mac
     if device_mac: query_params["device_mac"]=device_mac
     if vendor: query_params["vendor"]=vendor
     if type: query_params["type"]=type
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/pcaps.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/rogues.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,187 +10,148 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSitePacketCaptures")  
-def getSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
+def countSiteRogueEvents(mist_session:_APISession, site_id:str, distinct:str="bssid", type:str=None, ssid:str=None, bssid:str=None, ap_mac:str=None, channel:str=None, seen_on_lan:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
+    API doc: https://doc.mist-lab.fr/#operation/countSiteRogueEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
+    distinct : str{'bssid', 'ssid', 'ap', 'type'}, default: bssid
+    type : str{'honeypot', 'lan', 'others', 'spoof'}
+    ssid : str
+    bssid : str
+    ap_mac : str
+    channel : str
+    seen_on_lan : bool
     limit : int, default: 100
     start : int
     end : int
-    duration : str, default: 1d
-    client_mac : str
-      optional client mac filter        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/pcaps"
+    uri = f"/api/v1/sites/{site_id}/rogues/events/count"
     query_params={}
-    if page: query_params["page"]=page
+    if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
+    if ssid: query_params["ssid"]=ssid
+    if bssid: query_params["bssid"]=bssid
+    if ap_mac: query_params["ap_mac"]=ap_mac
+    if channel: query_params["channel"]=channel
+    if seen_on_lan: query_params["seen_on_lan"]=seen_on_lan
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if client_mac: query_params["client_mac"]=client_mac
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSitePacketCaptures(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d", client_mac:str=None) -> _APIResponse:
+def searchSiteRogueEvents(mist_session:_APISession, site_id:str, type:str=None, ssid:str=None, bssid:str=None, ap_mac:str=None, channel:int=None, seen_on_lan:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSitePacketCaptures
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteRogueEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
+    type : str{'honeypot', 'lan', 'others', 'spoof'}
+    ssid : str
+    bssid : str
+    ap_mac : str
+    channel : int
+    seen_on_lan : bool
     limit : int, default: 100
     start : int
     end : int
-    duration : str, default: 1d
-    client_mac : str
-      optional client mac filter        
+    duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/pcaps"
+    uri = f"/api/v1/sites/{site_id}/rogues/events/search"
     query_params={}
-    if page: query_params["page"]=page
+    if type: query_params["type"]=type
+    if ssid: query_params["ssid"]=ssid
+    if bssid: query_params["bssid"]=bssid
+    if ap_mac: query_params["ap_mac"]=ap_mac
+    if channel: query_params["channel"]=channel
+    if seen_on_lan: query_params["seen_on_lan"]=seen_on_lan
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
-    if duration: query_params["duration"]=duration
-    if client_mac: query_params["client_mac"]=client_mac
+    if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteCapturingStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteRogueAP(mist_session:_APISession, site_id:str, rogue_bssid:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCapturingStatus
+    API doc: https://doc.mist-lab.fr/#operation/getSiteRogueAP
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    site_id : str
+    rogue_bssid : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
+    uri = f"/api/v1/sites/{site_id}/rogues/{rogue_bssid}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def stopSitePacketCapture(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/stopSitePacketCapture
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def startSitePacketCapture(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def deauthSiteWirelessClientsConnectedToARogue(mist_session:_APISession, site_id:str, rogue_bssid:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/startSitePacketCapture
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/pcaps/capture"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
-def updateSitePacketCapture(mist_session:_APISession, site_id:str, pcap_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/updateSitePacketCapture
+    API doc: https://doc.mist-lab.fr/#operation/deauthSiteWirelessClientsConnectedToARogue
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    pcap_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    rogue_bssid : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/pcaps/{pcap_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/rogues/{rogue_bssid}/deauth_clients"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/psks.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/psks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSitePsks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSitePsks")  
 def getSitePsks(mist_session:_APISession, site_id:str, ssid:str=None, role:str=None, name:str=None, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSitePsks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/rfdiags.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/rfdiags.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/rftemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/networktemplates.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,36 +10,35 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteRfTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def getSiteNetworkTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteRfTemplateDerived
+    API doc: https://doc.mist-lab.fr/#operation/getSiteNetworkTemplateDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/rftemplates/derived"
+    uri = f"/api/v1/sites/{site_id}/networktemplates/derived"
     query_params={}
     if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/rrm.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/rrm.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,41 +33,73 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rrm/current"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteCurrentRrmConsiderationsForAnApOnASpecificBand(mist_session:_APISession, site_id:str, device_id:str, band:str) -> _APIResponse:
+def getSiteCurrentRrmConsiderations(mist_session:_APISession, site_id:str, device_id:str, band:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentRrmConsiderationsForAnApOnASpecificBand
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentRrmConsiderations
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
     device_id : str
-    band : str
-      radio band        
+    band : str{'24', '5', '6'}
+      802.11 Band        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/rrm/current/devices/{device_id}/band/{band}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def getSiteRrmEvents(mist_session:_APISession, site_id:str, band:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def getSiteCurrentRrmNeighbors(mist_session:_APISession, site_id:str, device_id:str, band:str, band:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentRrmNeighbors
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    device_id : str
+    band : str{'24', '5', '6'}
+      802.11 Band        
+    
+    QUERY PARAMS
+    ------------
+    band : str{'24', '5', '6'}
+      802.11 Band        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/rrm/current/devices/{device_id}/neighbors"
+    query_params={}
+    if band: query_params["band"]=band
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def getSiteRrmEvents(mist_session:_APISession, site_id:str, band:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/getSiteRrmEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -75,14 +107,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     band : str{'24', '5', '6'}
+      802.11 Band
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/rssizones.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/rssizones.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteRssiZones")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteRssiZones")  
 def getSiteRssiZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteRssiZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/servicepolicies.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/servicepolicies.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteServicePoliciesDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteServicePoliciesDerived")  
 def getSiteServicePoliciesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteServicePoliciesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -26,16 +26,15 @@
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/servicepolicies/derived"
@@ -55,16 +54,15 @@
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/servicepolicies/derived"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/services.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wxrules.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,180 +10,194 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteServicesDerived")  
-def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWxRules")  
+def getSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    page : int, default: 1
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/services/derived"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
-    if resolve: query_params["resolve"]=resolve
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    page : int, default: 1
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/services/derived"
+    uri = f"/api/v1/sites/{site_id}/wxrules"
     query_params={}
-    if resolve: query_params["resolve"]=resolve
+    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def countSiteServicePathEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, text:str=None, vpn_name:str=None, vpn_path:str=None, policy:str=None, port_id:str=None, model:str=None, version:str=None, timestamp:float=None, mac:str=None) -> _APIResponse:
+def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteServicePathEvents
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    distinct : str{'type', 'mac', 'vpn_name', 'vpn_path', 'policy', 'port_id', 'model', 'site_id'}, default: type
-    type : str
-      Event type, e.g. GW_SERVICE_PATH_DOWN
-    text : str
-      Description of the event including the reason it is triggered
-    vpn_name : str
-      Peer name
-    vpn_path : str
-      Peer path name
-    policy : str
-      Service policy associated with that specific path
-    port_id : str
-      Network interface
-    model : str
-      Device model
-    version : str
-      Device firmware version
-    timestamp : float
-      Start time, in epoch
-    mac : str
-      MAC address        
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/services/events/count"
-    query_params={}
-    if distinct: query_params["distinct"]=distinct
-    if type: query_params["type"]=type
-    if text: query_params["text"]=text
-    if vpn_name: query_params["vpn_name"]=vpn_name
-    if vpn_path: query_params["vpn_path"]=vpn_path
-    if policy: query_params["policy"]=policy
-    if port_id: query_params["port_id"]=port_id
-    if model: query_params["model"]=model
-    if version: query_params["version"]=version
-    if timestamp: query_params["timestamp"]=timestamp
-    if mac: query_params["mac"]=mac
-    resp = mist_session.mist_get(uri=uri, query=query_params)
+    uri = f"/api/v1/sites/{site_id}/wxrules"
+    resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def searchSiteServicePathEvents(mist_session:_APISession, site_id:str, type:str=None, text:str=None, vpn_name:str=None, vpn_path:str=None, policy:str=None, port_id:str=None, model:str=None, version:str=None, timestamp:float=None, mac:str=None) -> _APIResponse:
+def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/searchSiteServicePathEvents
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    QUERY PARAMS
-    ------------
-    type : str
-      Event type, e.g. GW_SERVICE_PATH_DOWN
-    text : str
-      Description of the event including the reason it is triggered
-    vpn_name : str
-      Peer name
-    vpn_path : str
-      Peer path name
-    policy : str
-      Service policy associated with that specific path
-    port_id : str
-      Network interface
-    model : str
-      Device model
-    version : str
-      Device firmware version
-    timestamp : float
-      Start time, in epoch
-    mac : str
-      MAC address        
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
+    query_params={}
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    wxrules_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/services/events/search"
-    query_params={}
-    if type: query_params["type"]=type
-    if text: query_params["text"]=text
-    if vpn_name: query_params["vpn_name"]=vpn_name
-    if vpn_path: query_params["vpn_path"]=vpn_path
-    if policy: query_params["policy"]=policy
-    if port_id: query_params["port_id"]=port_id
-    if model: query_params["model"]=model
-    if version: query_params["version"]=version
-    if timestamp: query_params["timestamp"]=timestamp
-    if mac: query_params["mac"]=mac
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
+    
+def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    wxrules_id : str        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    query_params={}
+    resp = mist_session.mist_delete(uri=uri, query=query_params)
+    return resp
+    
+def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    wxrules_id : str        
+    
+    BODY PARAMS
+    -----------
+    body : dict
+        JSON object to send to Mist Cloud (see API doc above for more details)
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    resp = mist_session.mist_put(uri=uri, body=body)
+    return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/setting.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/setting.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/sites.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/subscriptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteInfo(mist_session:_APISession, site_id:str) -> _APIResponse:
+def UnsubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -28,62 +28,34 @@
     site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def deleteSite(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSite
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}"
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteInfo(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def SubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteInfo
+    API doc: https://doc.mist-lab.fr/#operation/SubscribeSiteAlarms
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
+    uri = f"/api/v1/sites/{site_id}/subscriptions"
+    resp = mist_session.mist_post(uri=uri)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/sitetemplates.py` & `mistapi-0.48.0/src/mistapi/api/v1/orgs/ocdevices.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,36 +10,35 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSiteTemplateDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def getOrgJuniperDevicesCommand(mist_session:_APISession, org_id:str, site_id:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSiteTemplateDerived
+    API doc: https://doc.mist-lab.fr/#operation/getOrgJuniperDevicesCommand
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
     QUERY PARAMS
     ------------
-    resolve : bool
-      whether resolve the site variables        
+    site_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/sitetemplates/derived"
+    uri = f"/api/v1/orgs/{org_id}/ocdevices/outbound_ssh_cmd"
     query_params={}
-    if resolve: query_params["resolve"]=resolve
+    if site_id: query_params["site_id"]=site_id
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/skyatp.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/skyatp.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteSkyatpEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, mac:str=None, device_mac:str=None, threat_level:int=None, ip_address:str=None, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def countSiteSkyatpEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, mac:str=None, device_mac:str=None, threat_level:int=None, ip_address:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/countSiteSkyatpEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -27,23 +27,18 @@
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'type', 'mac', 'device_mac', 'threat_level'}, default: type
     type : str
-      event type, e.g. cc, fs, mw
     mac : str
-      client MAC
     device_mac : str
-      device MAC
     threat_level : int
-      threat level
     ip_address : str
-    page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -54,15 +49,14 @@
     query_params={}
     if distinct: query_params["distinct"]=distinct
     if type: query_params["type"]=type
     if mac: query_params["mac"]=mac
     if device_mac: query_params["device_mac"]=device_mac
     if threat_level: query_params["threat_level"]=threat_level
     if ip_address: query_params["ip_address"]=ip_address
-    if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
@@ -78,21 +72,17 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      event type, e.g. cc, fs, mw
     mac : str
-      client MAC
     device_mac : str
-      device MAC
     threat_level : int
-      threat level
     ip_address : str
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/ssr.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/ssr.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/stats.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/stats.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,21 +49,17 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'ap', 'wcid', 'ssid', 'wlan_id app', 'device_mac', 'src_ip', 'port_id', 'app', 'category', 'service'}
-      Default for wireless devices is `ap`. Default for wired devices is `device_mac`
     device_mac : str
-      MAC of the device
     app : str
-      Application name
-    wired : str
-      If a device is wired or wireless. Default is False.        
+    wired : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/apps/count"
@@ -71,15 +67,15 @@
     if distinct: query_params["distinct"]=distinct
     if device_mac: query_params["device_mac"]=device_mac
     if app: query_params["app"]=app
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteAssetsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteAssetsStats")  
 def getSiteAssetsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteAssetsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -266,15 +262,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteBeaconsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteBeaconsStats")  
 def getSiteBeaconsStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteBeaconsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -409,19 +405,16 @@
     -----------
     site_id : str
     client_mac : str        
     
     QUERY PARAMS
     ------------
     meeting_id : str
-      meeting_id
     mac : str
-      device identifier
     app : str
-      Third party app name
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
@@ -455,15 +448,14 @@
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distrinct : str{'mac'}, default: mac
     rating : int
-      feedback rating (e.g. "rating=1" or "rating=1,2")
     app : str
     start : str
     end : str        
     
     RETURN
     -----------
     mistapi.APIResponse
@@ -491,17 +483,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      device identifier
     app : str
-      Third party app name
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -515,15 +505,102 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWirelessClientsStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteTroubleshootCalls")  
+def getSiteTroubleshootCalls(mist_session:_APISession, site_id:str, client_mac:str, meeting_id:str, mac:str=None, app:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteTroubleshootCalls
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    client_mac : str        
+    
+    QUERY PARAMS
+    ------------
+    meeting_id : str
+    mac : str
+    app : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100
+    page : int, default: 1        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/stats/calls/troubleshoot"
+    query_params={}
+    if meeting_id: query_params["meeting_id"]=meeting_id
+    if mac: query_params["mac"]=mac
+    if app: query_params["app"]=app
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+def listSiteTroubleshootCalls(mist_session:_APISession, site_id:str, client_mac:str, meeting_id:str, mac:str=None, app:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+    """
+    API doc: https://doc.mist-lab.fr/#operation/listSiteTroubleshootCalls
+    
+    PARAMS
+    -----------
+    mistapi.APISession : mist_session
+        mistapi session including authentication and Mist host information
+    
+    PATH PARAMS
+    -----------
+    site_id : str
+    client_mac : str        
+    
+    QUERY PARAMS
+    ------------
+    meeting_id : str
+    mac : str
+    app : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100
+    page : int, default: 1        
+    
+    RETURN
+    -----------
+    mistapi.APIResponse
+        response from the API call
+    """
+    uri = f"/api/v1/sites/{site_id}/stats/calls/troubleshoot"
+    query_params={}
+    if meeting_id: query_params["meeting_id"]=meeting_id
+    if mac: query_params["mac"]=mac
+    if app: query_params["app"]=app
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    if page: query_params["page"]=page
+    resp = mist_session.mist_get(uri=uri, query=query_params)
+    return resp
+    
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWirelessClientsStats")  
 def getSiteWirelessClientsStats(mist_session:_APISession, site_id:str, wired:bool=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWirelessClientsStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -617,15 +694,15 @@
     """
     uri = f"/api/v1/sites/{site_id}/stats/clients/{client_mac}"
     query_params={}
     if wired: query_params["wired"]=wired
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteDevicesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteDevicesStats")  
 def getSiteDevicesStats(mist_session:_APISession, site_id:str, type:str="ap", status:str="all", page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDevicesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -734,15 +811,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/devices/{device_id}/clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteDiscoveredAssets")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteDiscoveredAssets")  
 def getSiteDiscoveredAssets(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteDiscoveredAssets
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -823,17 +900,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     scope : str{'site', 'switch'}, default: site
-      metric scope, optional
     type : str{'inactive_wired_vlans', 'switch_ap_affinity', 'poe_compliance', 'version_compliance'}
-      metric type, inactive_wired_vlans/switch_ap_affinity/poe_compliance/version_compliance, optional
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -901,17 +976,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     threshold : str
-      configurable # ap per switch threshold, default 12
-    system_name : str
-      system name for switch level metrics, optional        
+    system_name : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/discovered_switches/metrics"
@@ -1107,15 +1180,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/sdkclients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteUnconnectedClientStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteUnconnectedClientStats")  
 def getSiteUnconnectedClientStats(mist_session:_APISession, site_id:str, map_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUnconnectedClientStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1156,15 +1229,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/maps/{map_id}/unconnected_clients"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteMxEdgesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteMxEdgesStats")  
 def getSiteMxEdgesStats(mist_session:_APISession, site_id:str, page:int=1, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteMxEdgesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -1278,65 +1351,39 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'port_id', 'port_mac', 'full_duplex', 'mac', 'neighbor_mac', 'neighbor_port_desc', 'neighbor_system_name', 'poe_disabled', 'poe_mode', 'poe_on', 'speed', 'up'}, default: mac
-      port_id, port_mac, full_duplex, mac, neighbor_macneighbor_port_desc, neighbor_system_name, poe_disabled, poe_mode, poe_on, speed, up
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true` && has Authenticator role
     up : bool
-      indicates if interface is up
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -1376,15 +1423,15 @@
     if limit: query_params["limit"]=limit
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteSwOrGwPorts(mist_session:_APISession, site_id:str, full_duplex:bool=None, mac:str=None, type:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_errors:int=None, rx_errors:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, mac_limit:int=None, mac_count:int=None, up:bool=None, active:bool=None, jitter:float=None, loss:float=None, latency:float=None, stp_state:str=None, stp_role:str=None, xcvr_part_number:str=None, auth_state:str=None, lte_imsi:str=None, lte_iccid:str=None, lte_imei:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
+def searchSiteSwOrGwPorts(mist_session:_APISession, site_id:str, full_duplex:bool=None, mac:str=None, device_type:str=None, neighbor_mac:str=None, neighbor_port_desc:str=None, neighbor_system_name:str=None, poe_disabled:bool=None, poe_mode:str=None, poe_on:bool=None, port_id:str=None, port_mac:str=None, power_draw:float=None, tx_pkts:int=None, rx_pkts:int=None, rx_bytes:int=None, tx_bps:int=None, rx_bps:int=None, tx_errors:int=None, rx_errors:int=None, tx_mcast_pkts:int=None, tx_bcast_pkts:int=None, rx_mcast_pkts:int=None, rx_bcast_pkts:int=None, speed:int=None, mac_limit:int=None, mac_count:int=None, up:bool=None, active:bool=None, jitter:float=None, loss:float=None, latency:float=None, stp_state:str=None, stp_role:str=None, xcvr_part_number:str=None, auth_state:str=None, lte_imsi:str=None, lte_iccid:str=None, lte_imei:str=None, limit:int=100, start:int=None, end:int=None, duration:str="1d") -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteSwOrGwPorts
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -1392,104 +1439,66 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
-    type : str{'ap', 'ble', 'switch', 'gateway', 'mxedge', 'nac'}
-      device type
+    device_type : str{'ap', 'ble', 'switch', 'gateway', 'mxedge', 'nac'}
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_errors : int
-      Output errors
     rx_errors : int
-      Input errors
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     mac_limit : int
-      Limit on number of dynamically learned macs
     mac_count : int
-      Number of mac addresses in the forwarding table
     up : bool
-      indicates if interface is up
     active : bool
-      indicates if interface is active/inactive
     jitter : float
-      Last sampled jitter of the interface
     loss : float
-      Last sampled loss of the interface
     latency : float
-      Last sampled latency of the interface
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     xcvr_part_number : str
-      Optic Slot Partnumber, Check for null/empty
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true` && has Authenticator role
     lte_imsi : str
-      LTE IMSI value, Check for null/empty
     lte_iccid : str
-      LTE ICCID value, Check for null/empty
     lte_imei : str
-      LTE IMEI value, Check for null/empty
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/ports/search"
     query_params={}
     if full_duplex: query_params["full_duplex"]=full_duplex
     if mac: query_params["mac"]=mac
-    if type: query_params["type"]=type
+    if device_type: query_params["device_type"]=device_type
     if neighbor_mac: query_params["neighbor_mac"]=neighbor_mac
     if neighbor_port_desc: query_params["neighbor_port_desc"]=neighbor_port_desc
     if neighbor_system_name: query_params["neighbor_system_name"]=neighbor_system_name
     if poe_disabled: query_params["poe_disabled"]=poe_disabled
     if poe_mode: query_params["poe_mode"]=poe_mode
     if poe_on: query_params["poe_on"]=poe_on
     if port_id: query_params["port_id"]=port_id
@@ -1564,65 +1573,39 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'port_id', 'port_mac', 'full_duplex', 'mac', 'neighbor_mac', 'neighbor_port_desc', 'neighbor_system_name', 'poe_disabled', 'poe_mode', 'poe_on', 'speed', 'up'}, default: mac
-      port_id, port_mac, full_duplex, mac, neighbor_macneighbor_port_desc, neighbor_system_name, poe_disabled, poe_mode, poe_on, speed, up
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true`
     up : bool
-      indicates if interface is up
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -1678,63 +1661,38 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     full_duplex : bool
-      indicates full or half duplex
     mac : str
-      device identifier
     neighbor_mac : str
-      Chassis identifier of the chassis type listed
     neighbor_port_desc : str
-      Description supplied by the system on the interface E.g. “GigabitEthernet2/0/39”
     neighbor_system_name : str
-      Name supplied by the system on the interface E.g. neighbor system name E.g. “Kumar-Acc-SW.mist.local”
     poe_disabled : bool
-      is the POE configured not be disabled.
     poe_mode : str
-      poe mode depending on class E.g. “802.3at”
     poe_on : bool
-      is the device attached to POE
     port_id : str
-      interface name
     port_mac : str
-      interface mac address
     power_draw : float
-      Amount of power being used by the interface at the time the command is executed. Unit in watts.
     tx_pkts : int
-      Output packets
     rx_pkts : int
-      Input packets
     rx_bytes : int
-      Input bytes
     tx_bps : int
-      Output rate
     rx_bps : int
-      Input rate
     tx_mcast_pkts : int
-      Multicast output packets
     tx_bcast_pkts : int
-      Broadcast output packets
     rx_mcast_pkts : int
-      Multicast input packets
     rx_bcast_pkts : int
-      Broadcast input packets
     speed : int
-      port speed
     stp_state : str{'forwarding', 'blocking', 'learning', 'listening', 'disabled'}
-      if `up`==`true`
     stp_role : str{'designated', 'backup', 'alternate', 'root', 'root-prevented'}
-      if `up`==`true`
     auth_state : str{'init', 'authenticated', 'authenticating', 'held'}
-      if `up`==`true` && has Authenticator role
     up : bool
-      indicates if interface is up
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
@@ -1788,16 +1746,15 @@
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str{'active_ports_summary'}
     scope : str{'site', 'switch'}
-    switch_mac : str
-      switch mac, used only with metric `type`==`active_ports_summary`        
+    switch_mac : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/switches/metrics"
@@ -1827,15 +1784,15 @@
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/stats/wxrules"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteZonesStats")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteZonesStats")  
 def getSiteZonesStats(mist_session:_APISession, site_id:str, map_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteZonesStats
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/subscriptions.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wan_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,52 +10,45 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def UnsubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countSiteWanClientEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/UnsubscribeSiteAlarms
+    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def SubscribeSiteAlarms(mist_session:_APISession, site_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/SubscribeSiteAlarms
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
+    QUERY PARAMS
+    ------------
+    distinct : str{'type', 'hostname', 'ip', 'mfg', 'mac'}, default: type
+    type : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/subscriptions"
-    resp = mist_session.mist_post(uri=uri)
+    uri = f"/api/v1/sites/{site_id}/wan_client/events/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/synthetic_test.py` & `mistapi-0.48.0/src/mistapi/api/v1/installer/orgs/deviceprofiles.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,57 +10,64 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def getSiteSyntheticTestStatus(mist_session:_APISession, site_id:str) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listInstallerDeviceProfiles")  
+def getInstallerDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteSyntheticTestStatus
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
+    
+    QUERY PARAMS
+    ------------
+    type : str{'ap', 'switch', 'gateway'}, default: ap        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    query_params={}
+    uri = f"/api/v1/installer/orgs/{org_id}/deviceprofiles"
+    query_params={}
+    if type: query_params["type"]=type
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def triggerSiteSyntheticTest(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def listInstallerDeviceProfiles(mist_session:_APISession, org_id:str, type:str="ap") -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/triggerSiteSyntheticTest
+    API doc: https://doc.mist-lab.fr/#operation/listInstallerDeviceProfiles
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str        
+    org_id : str        
     
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
+    QUERY PARAMS
+    ------------
+    type : str{'ap', 'switch', 'gateway'}, default: ap        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/synthetic_test"
-    resp = mist_session.mist_post(uri=uri, body=body)
+    uri = f"/api/v1/installer/orgs/{org_id}/deviceprofiles"
+    query_params={}
+    if type: query_params["type"]=type
+    resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/uisettings.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/uisettings.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteUiSettings")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteUiSettings")  
 def getSiteUiSettings(mist_session:_APISession, site_id:str) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteUiSettings
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/vbeacons.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/vbeacons.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteVBeacons")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteVBeacons")  
 def getSiteVBeacons(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteVBeacons
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/vpns.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/system_events.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,66 +10,46 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteVpnsDerived")  
-def getSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSystemEventsDefinitions")  
+def getSystemEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSystemEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    QUERY PARAMS
-    ------------
-    resolve : bool
-      whether resolve the site variables        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vpns/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
+    uri = f"/api/v1/const/system_events"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteVpnsDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
+def listSystemEventsDefinitions(mist_session:_APISession) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteVpnsDerived
+    API doc: https://doc.mist-lab.fr/#operation/listSystemEventsDefinitions
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    QUERY PARAMS
-    ------------
-    resolve : bool
-      whether resolve the site variables        
-    
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/vpns/derived"
-    query_params={}
-    if resolve: query_params["resolve"]=resolve
+    uri = f"/api/v1/const/system_events"
+    query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wan_client.py` & `mistapi-0.48.0/src/mistapi/api/v1/const/default_gateway_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,35 +10,33 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def countSiteWanClientEvents(mist_session:_APISession, site_id:str, distinct:str="type") -> _APIResponse:
+def getGatewayDefaultConfig(mist_session:_APISession, model:str, ha:str=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/countSiteWanClientEvents
+    API doc: https://doc.mist-lab.fr/#operation/getGatewayDefaultConfig
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
     QUERY PARAMS
     ------------
-    distinct : str{'type', 'hostname', 'ip', 'mfg', 'mac'}, default: type        
+    model : str
+    ha : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wan_client/events/count"
+    uri = f"/api/v1/const/default_gateway_config"
     query_params={}
-    if distinct: query_params["distinct"]=distinct
+    if model: query_params["model"]=model
+    if ha: query_params["ha"]=ha
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wan_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wan_clients.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
     if limit: query_params["limit"]=limit
     if page: query_params["page"]=page
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def searchSiteWanClientEvents(mist_session:_APISession, site_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, nacrule_id:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
+def searchSiteWanClientEvents(mist_session:_APISession, site_id:str, type:str=None, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, nacrule_id:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteWanClientEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
@@ -64,30 +64,23 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     type : str
-      Event type, e.g. CLIENT_IP_ASSIGNED, CLIENT_IP_RENEWED, CLIENT_IP_EXPIRED
     mac : str
-      partial / full MAC address
     hostname : str
-      partial / full hostname
     ip : str
-      client IP
     mfg : str
-      Manufacture
     nacrule_id : str
-      nacrule_id
     start : int
     end : int
     duration : str, default: 1d
-    limit : int, default: 100
-    page : int, default: 1        
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wan_clients/events/search"
@@ -97,16 +90,15 @@
     if hostname: query_params["hostname"]=hostname
     if ip: query_params["ip"]=ip
     if mfg: query_params["mfg"]=mfg
     if nacrule_id: query_params["nacrule_id"]=nacrule_id
     if start: query_params["start"]=start
     if end: query_params["end"]=end
     if duration: query_params["duration"]=duration
-    if limit: query_params["limit"]=limit
-    if page: query_params["page"]=page
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
 def searchSiteWanClients(mist_session:_APISession, site_id:str, mac:str=None, hostname:str=None, ip:str=None, mfg:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100, page:int=1) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/searchSiteWanClients
     
@@ -118,21 +110,17 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     mac : str
-      partial / full MAC address
     hostname : str
-      partial / full hostname
     ip : str
-      client IP
     mfg : str
-      Manufacture
     start : int
     end : int
     duration : str, default: 1d
     limit : int, default: 100
     page : int, default: 1        
     
     RETURN
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/webhooks.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/webhooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWebhooks")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWebhooks")  
 def getSiteWebhooks(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWebhooks
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wired_clients.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wired_clients.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,21 +27,17 @@
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     distinct : str{'port_id', 'vlan', 'mac'}, default: mac
     mac : str
-      client mac
     device_mac : str
-      device mac
     port_id : str
-      port id
     vlan : str
-      vlan
     page : int, default: 1
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
@@ -76,29 +72,21 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     device_mac : str
-      device mac
     mac : str
-      client mac
     ip : str
-      client ip
     port_id : str
-      port id
     vlan : str
-      vlan
     manufacture : str
-      manufacture
     text : str
-      single entry of hostname/mac
     nacrule_id : str
-      nacrule_id
     limit : int, default: 100
     start : int
     end : int
     duration : str, default: 1d        
     
     RETURN
     -----------
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wlans.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wlans.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWlans")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWlans")  
 def getSiteWlans(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlans
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -98,15 +98,15 @@
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWlanDerived")  
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWlanDerived")  
 def getSiteWlanDerived(mist_session:_APISession, site_id:str, resolve:bool=None, wlan_id:str=None) -> _APIResponse:
     """
     API doc: https://doc.mist-lab.fr/#operation/listSiteWlanDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
@@ -115,17 +115,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     resolve : bool
-      whether to resolve SITE_VARS
-    wlan_id : str
-      filter by WLAN ID        
+    wlan_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/derived"
@@ -147,17 +145,15 @@
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
     resolve : bool
-      whether to resolve SITE_VARS
-    wlan_id : str
-      filter by WLAN ID        
+    wlan_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
     uri = f"/api/v1/sites/{site_id}/wlans/derived"
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wxrules.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/wxtunnels.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWxRules")  
-def getSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteWxTunnels")  
+def getSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxRules(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxRules
+    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxRule(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,110 +94,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxRulesDerived(mist_session:_APISession, site_id:str) -> _APIResponse:
+def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRulesDerived
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxrules/derived"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxrules_id : str        
+    wxtunnel_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str) -> _APIResponse:
+def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxrules_id : str        
+    wxtunnel_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxRule(mist_session:_APISession, site_id:str, wxrules_id:str, body:object) -> _APIResponse:
+def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxRule
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxrules_id : str        
+    wxtunnel_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxrules/{wxrules_id}"
+    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wxtags.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/services.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,218 +10,174 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWxTags")  
-def getSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteServicesDerived")  
+def getSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
+    uri = f"/api/v1/sites/{site_id}/services/derived"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxTags(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteServicesDerived(mist_session:_APISession, site_id:str, resolve:bool=None) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTags
+    API doc: https://doc.mist-lab.fr/#operation/listSiteServicesDerived
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
     QUERY PARAMS
     ------------
-    page : int, default: 1
-    limit : int, default: 100        
+    resolve : bool        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
+    uri = f"/api/v1/sites/{site_id}/services/derived"
     query_params={}
-    if page: query_params["page"]=page
-    if limit: query_params["limit"]=limit
+    if resolve: query_params["resolve"]=resolve
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxTag(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTag
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags"
-    resp = mist_session.mist_post(uri=uri, body=body)
-    return resp
-    
-def getSiteApplicationList(mist_session:_APISession, site_id:str) -> _APIResponse:
+def countSiteServicePathEvents(mist_session:_APISession, site_id:str, distinct:str="type", type:str=None, text:str=None, vpn_name:str=None, vpn_path:str=None, policy:str=None, port_id:str=None, model:str=None, version:str=None, timestamp:float=None, mac:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteApplicationList
+    API doc: https://doc.mist-lab.fr/#operation/countSiteServicePathEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str        
     
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags/apps"
-    query_params={}
-    resp = mist_session.mist_get(uri=uri, query=query_params)
-    return resp
-    
-def getSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTag
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    wxtag_id : str        
+    QUERY PARAMS
+    ------------
+    distinct : str{'type', 'mac', 'vpn_name', 'vpn_path', 'policy', 'port_id', 'model', 'site_id'}, default: type
+    type : str
+    text : str
+    vpn_name : str
+    vpn_path : str
+    policy : str
+    port_id : str
+    model : str
+    version : str
+    timestamp : float
+    mac : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/services/events/count"
+    query_params={}
+    if distinct: query_params["distinct"]=distinct
+    if type: query_params["type"]=type
+    if text: query_params["text"]=text
+    if vpn_name: query_params["vpn_name"]=vpn_name
+    if vpn_path: query_params["vpn_path"]=vpn_path
+    if policy: query_params["policy"]=policy
+    if port_id: query_params["port_id"]=port_id
+    if model: query_params["model"]=model
+    if version: query_params["version"]=version
+    if timestamp: query_params["timestamp"]=timestamp
+    if mac: query_params["mac"]=mac
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTag
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
-    
-    PATH PARAMS
-    -----------
-    site_id : str
-    wxtag_id : str        
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
-    query_params={}
-    resp = mist_session.mist_delete(uri=uri, query=query_params)
-    return resp
-    
-def updateSiteWxTag(mist_session:_APISession, site_id:str, wxtag_id:str, body:object) -> _APIResponse:
+def searchSiteServicePathEvents(mist_session:_APISession, site_id:str, type:str=None, text:str=None, vpn_name:str=None, vpn_path:str=None, policy:str=None, port_id:str=None, model:str=None, version:str=None, timestamp:float=None, mac:str=None, start:int=None, end:int=None, duration:str="1d", limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTag
+    API doc: https://doc.mist-lab.fr/#operation/searchSiteServicePathEvents
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
-    site_id : str
-    wxtag_id : str        
-    
-    BODY PARAMS
-    -----------
-    body : dict
-        JSON object to send to Mist Cloud (see API doc above for more details)
-    
-    RETURN
-    -----------
-    mistapi.APIResponse
-        response from the API call
-    """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}"
-    resp = mist_session.mist_put(uri=uri, body=body)
-    return resp
-    
-def getSiteCurrentMatchingClientsOfAWxTag(mist_session:_APISession, site_id:str, wxtag_id:str) -> _APIResponse:
-    """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteCurrentMatchingClientsOfAWxTag
-    
-    PARAMS
-    -----------
-    mistapi.APISession : mist_session
-        mistapi session including authentication and Mist host information
+    site_id : str        
     
-    PATH PARAMS
-    -----------
-    site_id : str
-    wxtag_id : str        
+    QUERY PARAMS
+    ------------
+    type : str
+    text : str
+    vpn_name : str
+    vpn_path : str
+    policy : str
+    port_id : str
+    model : str
+    version : str
+    timestamp : float
+    mac : str
+    start : int
+    end : int
+    duration : str, default: 1d
+    limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtags/{wxtag_id}/clients"
-    query_params={}
+    uri = f"/api/v1/sites/{site_id}/services/events/search"
+    query_params={}
+    if type: query_params["type"]=type
+    if text: query_params["text"]=text
+    if vpn_name: query_params["vpn_name"]=vpn_name
+    if vpn_path: query_params["vpn_path"]=vpn_path
+    if policy: query_params["policy"]=policy
+    if port_id: query_params["port_id"]=port_id
+    if model: query_params["model"]=model
+    if version: query_params["version"]=version
+    if timestamp: query_params["timestamp"]=timestamp
+    if mac: query_params["mac"]=mac
+    if start: query_params["start"]=start
+    if end: query_params["end"]=end
+    if duration: query_params["duration"]=duration
+    if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/sites/wxtunnels.py` & `mistapi-0.48.0/src/mistapi/api/v1/sites/zones.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.47.5", details="function replaced with listSiteWxTunnels")  
-def getSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+@deprecation.deprecated(deprecated_in="0.37.7", removed_in="0.52.0", current_version="0.48.0", details="function replaced with listSiteZones")  
+def getSiteZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -34,24 +34,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def listSiteWxTunnels(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
+def listSiteZones(mist_session:_APISession, site_id:str, page:int=1, limit:int=100) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/listSiteWxTunnels
+    API doc: https://doc.mist-lab.fr/#operation/listSiteZones
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -64,24 +64,24 @@
     limit : int, default: 100        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     query_params={}
     if page: query_params["page"]=page
     if limit: query_params["limit"]=limit
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def createSiteWxTunnel(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
+def createSiteZone(mist_session:_APISession, site_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/createSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/createSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
@@ -94,87 +94,87 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels"
+    uri = f"/api/v1/sites/{site_id}/zones"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
     
-def getSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
+def getSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/getSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/getSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtunnel_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_get(uri=uri, query=query_params)
     return resp
     
-def deleteSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str) -> _APIResponse:
+def deleteSiteZone(mist_session:_APISession, site_id:str, zone_id:str) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/deleteSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/deleteSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtunnel_id : str        
+    zone_id : str        
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     query_params={}
     resp = mist_session.mist_delete(uri=uri, query=query_params)
     return resp
     
-def updateSiteWxTunnel(mist_session:_APISession, site_id:str, wxtunnel_id:str, body:object) -> _APIResponse:
+def updateSiteZone(mist_session:_APISession, site_id:str, zone_id:str, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/updateSiteWxTunnel
+    API doc: https://doc.mist-lab.fr/#operation/updateSiteZone
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     PATH PARAMS
     -----------
     site_id : str
-    wxtunnel_id : str        
+    zone_id : str        
     
     BODY PARAMS
     -----------
     body : dict
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/sites/{site_id}/wxtunnels/{wxtunnel_id}"
+    uri = f"/api/v1/sites/{site_id}/zones/{zone_id}"
     resp = mist_session.mist_put(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/api/v1/utils/test_telstra.py` & `mistapi-0.48.0/src/mistapi/api/v1/utils/test_twilio.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 --------------------------------------------------------------------------------
 '''
 
 from mistapi import APISession as _APISession
 from mistapi.__api_response import APIResponse as _APIResponse
 import deprecation
 
-def testSiteWlanTelstraSetup(mist_session:_APISession, body:object) -> _APIResponse:
+def testSiteWlanTwilioSetup(mist_session:_APISession, body:object) -> _APIResponse:
     """
-    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTelstraSetup
+    API doc: https://doc.mist-lab.fr/#operation/testSiteWlanTwilioSetup
     
     PARAMS
     -----------
     mistapi.APISession : mist_session
         mistapi session including authentication and Mist host information
     
     BODY PARAMS
@@ -29,11 +29,11 @@
         JSON object to send to Mist Cloud (see API doc above for more details)
     
     RETURN
     -----------
     mistapi.APIResponse
         response from the API call
     """
-    uri = f"/api/v1/utils/test_telstra"
+    uri = f"/api/v1/utils/test_twilio"
     resp = mist_session.mist_post(uri=uri, body=body)
     return resp
```

### Comparing `mistapi-0.47.5/src/mistapi/cli.py` & `mistapi-0.48.0/src/mistapi/cli.py`

 * *Files identical despite different names*

### Comparing `mistapi-0.47.5/src/mistapi.egg-info/PKG-INFO` & `mistapi-0.48.0/src/mistapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistapi
-Version: 0.47.5
+Version: 0.48.0
 Summary: Python package to simplify the Mist System APIs usage
 Author-email: Thomas Munzer <tmunzer@juniper.net>
 License: MIT
 Project-URL: Source, https://github.com/tmunzer/mistapi_python
 Project-URL: Bug Tracker, https://github.com/tmunzer/mistapi_python/issues
 Keywords: Mist,Juniper,API
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mistapi-0.47.5/src/mistapi.egg-info/SOURCES.txt` & `mistapi-0.48.0/src/mistapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 src/mistapi/__models/privilege.py
 src/mistapi/api/__init__.py
 src/mistapi/api/v1/__init__.py
 src/mistapi/api/v1/const/__init__.py
 src/mistapi/api/v1/const/alarm_defs.py
 src/mistapi/api/v1/const/ap_channels.py
 src/mistapi/api/v1/const/ap_led_status.py
+src/mistapi/api/v1/const/app_categories.py
+src/mistapi/api/v1/const/app_subcategories.py
 src/mistapi/api/v1/const/applications.py
 src/mistapi/api/v1/const/client_events.py
 src/mistapi/api/v1/const/countries.py
 src/mistapi/api/v1/const/default_gateway_config.py
 src/mistapi/api/v1/const/device_events.py
 src/mistapi/api/v1/const/device_models.py
 src/mistapi/api/v1/const/gateway_applications.py
@@ -34,14 +36,15 @@
 src/mistapi/api/v1/const/languages.py
 src/mistapi/api/v1/const/license_types.py
 src/mistapi/api/v1/const/mxedge_events.py
 src/mistapi/api/v1/const/mxedge_models.py
 src/mistapi/api/v1/const/nac_events.py
 src/mistapi/api/v1/const/otherdevice_events.py
 src/mistapi/api/v1/const/otherdevice_models.py
+src/mistapi/api/v1/const/system_events.py
 src/mistapi/api/v1/const/traffic_types.py
 src/mistapi/api/v1/installer/__init__.py
 src/mistapi/api/v1/installer/orgs/__init__.py
 src/mistapi/api/v1/installer/orgs/alarmtemplates.py
 src/mistapi/api/v1/installer/orgs/deviceprofiles.py
 src/mistapi/api/v1/installer/orgs/devices.py
 src/mistapi/api/v1/installer/orgs/rftemplates.py
@@ -83,15 +86,14 @@
 src/mistapi/api/v1/orgs/admins.py
 src/mistapi/api/v1/orgs/alarms.py
 src/mistapi/api/v1/orgs/alarmtemplates.py
 src/mistapi/api/v1/orgs/apitokens.py
 src/mistapi/api/v1/orgs/aptemplates.py
 src/mistapi/api/v1/orgs/assetfilters.py
 src/mistapi/api/v1/orgs/assets.py
-src/mistapi/api/v1/orgs/call.py
 src/mistapi/api/v1/orgs/cert.py
 src/mistapi/api/v1/orgs/claim.py
 src/mistapi/api/v1/orgs/clients.py
 src/mistapi/api/v1/orgs/clone.py
 src/mistapi/api/v1/orgs/crl.py
 src/mistapi/api/v1/orgs/deviceprofiles.py
 src/mistapi/api/v1/orgs/devices.py
@@ -107,21 +109,23 @@
 src/mistapi/api/v1/orgs/logs.py
 src/mistapi/api/v1/orgs/maps.py
 src/mistapi/api/v1/orgs/mist_nac.py
 src/mistapi/api/v1/orgs/mxclusters.py
 src/mistapi/api/v1/orgs/mxedges.py
 src/mistapi/api/v1/orgs/mxtunnels.py
 src/mistapi/api/v1/orgs/nac_clients.py
+src/mistapi/api/v1/orgs/nacportals.py
 src/mistapi/api/v1/orgs/nacrules.py
 src/mistapi/api/v1/orgs/nactags.py
 src/mistapi/api/v1/orgs/networks.py
 src/mistapi/api/v1/orgs/networktemplates.py
 src/mistapi/api/v1/orgs/ocdevices.py
 src/mistapi/api/v1/orgs/orgs.py
 src/mistapi/api/v1/orgs/otherdevices.py
+src/mistapi/api/v1/orgs/pcaps.py
 src/mistapi/api/v1/orgs/pma.py
 src/mistapi/api/v1/orgs/pskportals.py
 src/mistapi/api/v1/orgs/psks.py
 src/mistapi/api/v1/orgs/rftemplates.py
 src/mistapi/api/v1/orgs/sdkclients.py
 src/mistapi/api/v1/orgs/sdkinvites.py
 src/mistapi/api/v1/orgs/sdktemplates.py
@@ -136,14 +140,15 @@
 src/mistapi/api/v1/orgs/ssos.py
 src/mistapi/api/v1/orgs/ssr.py
 src/mistapi/api/v1/orgs/stats.py
 src/mistapi/api/v1/orgs/subscriptions.py
 src/mistapi/api/v1/orgs/templates.py
 src/mistapi/api/v1/orgs/tickets.py
 src/mistapi/api/v1/orgs/troubleshoot.py
+src/mistapi/api/v1/orgs/usermacs.py
 src/mistapi/api/v1/orgs/vars.py
 src/mistapi/api/v1/orgs/vpns.py
 src/mistapi/api/v1/orgs/wan_client.py
 src/mistapi/api/v1/orgs/wan_clients.py
 src/mistapi/api/v1/orgs/webhooks.py
 src/mistapi/api/v1/orgs/wired_clients.py
 src/mistapi/api/v1/orgs/wlans.py
@@ -169,15 +174,14 @@
 src/mistapi/api/v1/sites/alarms.py
 src/mistapi/api/v1/sites/anomaly.py
 src/mistapi/api/v1/sites/apps.py
 src/mistapi/api/v1/sites/aptemplates.py
 src/mistapi/api/v1/sites/assetfilters.py
 src/mistapi/api/v1/sites/assets.py
 src/mistapi/api/v1/sites/beacons.py
-src/mistapi/api/v1/sites/call.py
 src/mistapi/api/v1/sites/clients.py
 src/mistapi/api/v1/sites/count.py
 src/mistapi/api/v1/sites/deviceprofiles.py
 src/mistapi/api/v1/sites/devices.py
 src/mistapi/api/v1/sites/events.py
 src/mistapi/api/v1/sites/evpn_topologies.py
 src/mistapi/api/v1/sites/gatewaytemplates.py
```

