# Comparing `tmp/pulumi_meraki-0.2.0a1716250106.tar.gz` & `tmp/pulumi_meraki-0.2.0a1716483448.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_meraki-0.2.0a1716250106.tar", last modified: Tue May 21 00:11:12 2024, max compression
+gzip compressed data, was "pulumi_meraki-0.2.0a1716483448.tar", last modified: Thu May 23 17:08:22 2024, max compression
```

## Comparing `pulumi_meraki-0.2.0a1716250106.tar` & `pulumi_meraki-0.2.0a1716483448.tar`

### file list

```diff
@@ -1,521 +1,521 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.397379 pulumi_meraki-0.2.0a1716250106/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 00:11:12.397379 pulumi_meraki-0.2.0a1716250106/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.305379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/
--rw-r--r--   0 runner    (1001) docker     (127)    46345 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.305379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37054 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_identities_me.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_entitlements.py
--rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_subscriptions_compliance_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_claim_key_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    54773 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.305379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.317380 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   179477 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_radio_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_uplinks_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_vmx_authentication_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/blink_leds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_custom_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_generate_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_quality_and_retention.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_sense.py
--rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_video_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_wireless_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_gateway_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_gateway_port_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_sims.py
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_radio_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_uplinks_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_analytics_live.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_custom_analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_quality_and_retention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_sense.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_video_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_video_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_wireless_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_gateway_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_gateway_port_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_sims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_arp_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_cable_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_ping_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_throughput_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_wake_on_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_lldp_cdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_sensor_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_ports_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_interfaces_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_warm_spare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_bluetooth_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_connection_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_latency_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_radio_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_arp_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_cable.py
--rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_ping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_ping_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_throughput_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_wake_on_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)   340260 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/sensor_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)    74768 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_ports_cycle.py
--rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    42819 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_interfaces_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_warm_spare.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_alternate_management_interface_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_bluetooth_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_radio_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_organizations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.369379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/
--rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1110295 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/alerts_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_connectivity_monitoring_destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_content_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_cellular_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_firewalled_services.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_inbound_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_l3_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_l7_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_one_to_many_nat_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_one_to_one_nat_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_port_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    21768 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_prefixes_delegated_statics.py
--rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_rf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_security_intrusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_security_malware.py
--rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_single_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_ssids.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_custom_performance_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_uplink_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_uplink_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_vpn_exclusions.py
--rw-r--r--   0 runner    (1001) docker     (127)    54577 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vlans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vlans_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    19240 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vpn_bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vpn_site_to_site_vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_warm_spare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_warm_spare_swap.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/bind.py
--rw-r--r--   0 runner    (1001) docker     (127)    35277 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/camera_quality_retention_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/camera_wireless_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_connectivity_monitoring_destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_uplink.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_provision.py
--rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_splash_authorization_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_claim_vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_rollbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events_defer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events_rollbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)    41592 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/floor_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_alerts_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_alerts_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_connectivity_monitoring_destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_content_filtering.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_content_filtering_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_cellular_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_firewalled_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_inbound_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l3_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules_application_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_one_to_many_nat_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_one_to_one_nat_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_port_forwarding_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_prefixes_delegated_statics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_rf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_security_intrusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_security_malware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_single_lan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_ssids.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vlans.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vlans_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vpn_bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vpn_site_to_site_vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_warm_spare.py
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_bluetooth_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_camera_quality_retention_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_camera_wireless_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_connectivity_monitoring_destinations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_uplink.py
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_splash_authorization_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_events_event_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_floor_plans.py
--rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_health_alerts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_insight_applications_health_by_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_meraki_auth_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_netflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_pii_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_sm_devices_for_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_sm_owners_for_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_policies_by_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_current_overview_by_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_overview_by_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_mqtt_brokers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_bypass_activation_lock_attempts.py
--rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_cellular_usage_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_certs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_connectivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_desktop_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_device_command_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_device_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_network_adapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_performance_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_security_centers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_wlan_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_target_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_trusted_access_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_user_access_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users_device_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users_softwares.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_access_control_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_access_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_alternate_management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_trusted_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_warnings_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_v4_servers_seen.py
--rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dscp_to_cos_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_link_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_mtu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_port_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_qos_rules_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_multicast.py
--rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_multicast_rendezvous_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_interfaces_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_storm_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_syslog_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_topology_link_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_shaping_application_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_shaping_dscp_tagging_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_vlan_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_vlan_profiles_assignments_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_http_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_payload_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_webhook_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_alternate_management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_bluetooth_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_channel_utilization_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_client_count_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_clients_connection_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_clients_latency_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_connection_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_data_rate_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_devices_connection_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ethernet_ports_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_failed_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_latency_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_latency_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_mesh_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_rf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_signal_quality_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids.py
--rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_bonjour_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_device_type_group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_eap_override.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_firewall_l3_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_firewall_l7_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_hotspot20.py
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_identity_psks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_splash_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_traffic_shaping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_usage_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    30295 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    23867 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/meraki_auth_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/mqtt_brokers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/netflow.py
--rw-r--r--   0 runner    (1001) docker     (127)  1940280 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/pii_requests_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sensor_alerts_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sensor_mqtt_brokers.py
--rw-r--r--   0 runner    (1001) docker     (127)    23054 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_bypass_activation_lock_attempts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_checkin.py
--rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_install_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_modify_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_reboot.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_refresh_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_shutdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_unenroll.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_uninstall_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_wipe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_target_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_user_access_devices_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/split.py
--rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_access_control_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)    56184 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_access_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_alternate_management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dhcp_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    15590 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dhcp_server_policy_arp_inspection_trusted_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dscp_to_cos_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_link_aggregations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_mtu.py
--rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_port_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)    24153 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_qos_rules_order.py
--rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_multicast.py
--rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_multicast_rendezvous_points.py
--rw-r--r--   0 runner    (1001) docker     (127)    24291 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks.py
--rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_add.py
--rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)    26416 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    45852 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_interfaces_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_static_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_storm_control.py
--rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/syslog_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/traffic_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/unbind.py
--rw-r--r--   0 runner    (1001) docker     (127)    15846 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/vlan_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/vlan_profiles_assignments_reassign.py
--rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/webhooks_http_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/webhooks_payload_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_alternate_management_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_billing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_bluetooth_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles_assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles_set_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    36424 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_rf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    22838 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)   174106 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_bonjour_forwarding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_device_type_group_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_eap_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_firewall_l3_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_firewall_l7_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    27512 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_hotspot20.py
--rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_identity_psks.py
--rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_schedules.py
--rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_splash_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_traffic_shaping_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.397379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   269412 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/action_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20771 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)    25510 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/admins.py
--rw-r--r--   0 runner    (1001) docker     (127)    20807 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/alerts_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_security_intrusion.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_vpn_third_party_vpnpeers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_vpn_vpn_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/branding_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/branding_policies_priorities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/camera_custom_analytics_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    18966 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/camera_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)    15201 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/config_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    75016 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/config_templates_switch_profiles_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/early_access_features_opt_ins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_action_batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_acls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_admins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_alerts_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests_overview_response_codes_by_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_security_intrusion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_traffic_shaping_vpn_exclusions_by_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_uplinks_statuses_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_uplinks_usage_by_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_vpn_third_party_vpnpeers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_vpn_vpn_firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_branding_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_branding_policies_priorities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_boundaries_areas_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_boundaries_lines_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_custom_analytics_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_detections_history_by_boundary_by_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_cellular_gateway_uplink_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_bandwidth_usage_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates_switch_profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates_switch_profiles_ports.py
--rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_availabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_availabilities_change_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_boots_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_power_modules_statuses_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_provisioning_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_statuses_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_uplinks_addresses_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_uplinks_loss_and_latency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_early_access_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_early_access_features_opt_ins.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_firmware_upgrades.py
--rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_firmware_upgrades_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_insight_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_insight_monitored_media_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licenses_overview.py
--rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licensing_coterm_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_login_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_openapi_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_policy_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_policy_objects_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml_idps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sensor_readings_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sensor_readings_latest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_admins_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_apns_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_sentry_policies_assignments_by_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_vpp_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_appliances_by_utilization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_clients_by_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_clients_manufacturers_by_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_devices_by_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_devices_models_by_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_networks_by_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_ssids_by_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_switches_by_energy_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_switch_ports_by_switch.py
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_uplinks_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_webhooks_callbacks_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_webhooks_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_device_by_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)    16927 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_network_by_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_ethernet_statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    16524 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_device.py
--rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/insight_monitored_media_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_claim.py
--rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_export_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_prepare.py
--rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_release.py
--rw-r--r--   0 runner    (1001) docker     (127)    27098 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_assign_seats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_move.py
--rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_move_seats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_renew_seats.py
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licensing_coterm_licenses_move.py
--rw-r--r--   0 runner    (1001) docker     (127)    44808 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/login_security.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/networks_combine.py
--rw-r--r--   0 runner    (1001) docker     (127)   754190 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/policy_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/policy_objects_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml.py
--rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml_idps.py
--rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/sm_admins_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/sm_sentry_policies_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)    26679 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/snmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/switch_devices_clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:11:12.397379 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 00:11:12.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-21 00:11:12.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:11:12.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 00:11:12.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 00:11:12.000000 pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-21 00:11:05.000000 pulumi_meraki-0.2.0a1716250106/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:11:12.397379 pulumi_meraki-0.2.0a1716250106/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.808960 pulumi_meraki-0.2.0a1716483448/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-23 17:08:22.808960 pulumi_meraki-0.2.0a1716483448/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.700959 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/
+-rw-r--r--   0 runner    (1001) docker     (127)    46345 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.704959 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37054 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_identities_me.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_entitlements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_subscriptions_compliance_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12580 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8221 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_claim_key_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54773 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.704959 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.716959 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   179477 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14059 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_radio_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16878 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_uplinks_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7958 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_vmx_authentication_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33371 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9278 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/blink_leds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13135 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_custom_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9014 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_generate_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27514 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_quality_and_retention.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_sense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9894 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_video_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8981 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_wireless_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16651 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_gateway_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8784 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_gateway_port_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11199 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_sims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_radio_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_uplinks_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_analytics_live.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_custom_analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_quality_and_retention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_sense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_video_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_video_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_wireless_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_gateway_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_gateway_port_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_sims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_arp_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_cable_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_ping_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_throughput_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_wake_on_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_lldp_cdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_sensor_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6014 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_ports_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_interfaces_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_warm_spare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_bluetooth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_connection_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11639 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_latency_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_radio_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15873 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_arp_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16920 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_cable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10836 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11066 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_ping_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16045 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_throughput_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17673 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_wake_on_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11179 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)   340260 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13710 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/sensor_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74768 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9785 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_ports_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24573 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42819 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_interfaces_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20057 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11149 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_warm_spare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_alternate_management_interface_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_bluetooth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_radio_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24499 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14264 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_organizations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.776960 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/
+-rw-r--r--   0 runner    (1001) docker     (127)    12381 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1110295 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/alerts_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_connectivity_monitoring_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_content_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_cellular_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_firewalled_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_inbound_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13775 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_l3_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_l7_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9033 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_one_to_many_nat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8974 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_one_to_one_nat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9151 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_port_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21768 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17791 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_prefixes_delegated_statics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17963 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_rf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12718 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_security_intrusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15333 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_security_malware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13694 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15784 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_single_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36668 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_ssids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_custom_performance_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13599 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11740 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_uplink_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24464 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_uplink_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9652 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_vpn_exclusions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54577 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9056 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vlans_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19240 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vpn_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vpn_site_to_site_vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18392 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_warm_spare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_warm_spare_swap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22129 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35277 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/camera_quality_retention_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16168 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/camera_wireless_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_connectivity_monitoring_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14079 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12547 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_uplink.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_provision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12197 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_splash_authorization_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9715 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_claim_vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8901 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9267 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_rollbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events_defer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events_rollbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11010 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41592 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/floor_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_alerts_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_alerts_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_connectivity_monitoring_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_content_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_content_filtering_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_cellular_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_firewalled_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_inbound_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l3_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules_application_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4114 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_one_to_many_nat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_one_to_one_nat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_port_forwarding_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_prefixes_delegated_statics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_rf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_security_intrusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_security_malware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_single_lan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_ssids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4196 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vlans_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vpn_bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vpn_site_to_site_vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_warm_spare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_bluetooth_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_camera_quality_retention_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_camera_wireless_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_connectivity_monitoring_destinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3862 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_uplink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8052 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_splash_authorization_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21331 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_events_event_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_floor_plans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_health_alerts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_insight_applications_health_by_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4703 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_meraki_auth_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3385 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_netflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_pii_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9152 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_sm_devices_for_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9115 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_sm_owners_for_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10680 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_policies_by_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_current_overview_by_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_overview_by_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_mqtt_brokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_bypass_activation_lock_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17260 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4955 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_cellular_usage_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_certs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_connectivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9337 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_desktop_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_device_command_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_device_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_network_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9575 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_performance_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_security_centers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_wlan_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5783 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_trusted_access_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8453 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_user_access_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7157 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users_device_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users_softwares.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_access_control_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_alternate_management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_trusted_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9559 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_warnings_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10974 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_v4_servers_seen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3821 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dscp_to_cos_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_link_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_mtu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_port_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_qos_rules_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_multicast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5299 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_multicast_rendezvous_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_interfaces_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6006 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3678 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_storm_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_syslog_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_topology_link_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4112 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_shaping_application_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_shaping_dscp_tagging_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_vlan_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12366 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_vlan_profiles_assignments_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_http_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_payload_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_webhook_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_alternate_management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_bluetooth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15225 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_channel_utilization_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_client_count_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_clients_connection_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12959 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_clients_latency_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_connection_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14472 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_data_rate_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10929 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_devices_connection_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4857 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ethernet_ports_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12428 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_failed_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15467 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_latency_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_latency_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8470 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_mesh_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_rf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14885 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_signal_quality_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4298 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4745 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_bonjour_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_device_type_group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_eap_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_firewall_l3_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4929 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_firewall_l7_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_hotspot20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_identity_psks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4518 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_splash_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4810 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_traffic_shaping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14824 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_usage_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30295 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23867 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/meraki_auth_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10707 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/mqtt_brokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17756 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/netflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1940280 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/pii_requests_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18702 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sensor_alerts_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10954 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sensor_mqtt_brokers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23054 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12592 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_bypass_activation_lock_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_checkin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9484 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10179 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_install_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_modify_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8917 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_reboot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_refresh_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8987 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_shutdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9809 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_unenroll.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_uninstall_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8847 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_wipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12990 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_target_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_user_access_devices_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/split.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11912 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_access_control_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56184 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17602 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_alternate_management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dhcp_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15590 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dhcp_server_policy_arp_inspection_trusted_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dscp_to_cos_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_link_aggregations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11067 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_mtu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17741 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_port_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24153 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_qos_rules_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13030 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_multicast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15321 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_multicast_rendezvous_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24291 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18184 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12437 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11973 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12096 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26416 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45852 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_interfaces_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22796 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_static_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_storm_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9436 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/syslog_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/traffic_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8602 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/unbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15846 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/vlan_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9477 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/vlan_profiles_assignments_reassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16903 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/webhooks_http_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22819 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/webhooks_payload_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17735 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_alternate_management_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10490 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21287 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_bluetooth_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15733 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9617 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles_set_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36424 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_rf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22838 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)   174106 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14775 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_bonjour_forwarding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13378 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_device_type_group_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16110 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_eap_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14006 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_firewall_l3_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12421 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_firewall_l7_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27512 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_hotspot20.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20883 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_identity_psks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_schedules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52405 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_splash_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17948 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_traffic_shaping_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.804960 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   269412 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18679 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/action_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18038 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20771 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21544 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9761 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25510 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/admins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20807 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/alerts_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_security_intrusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_vpn_third_party_vpnpeers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12058 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_vpn_vpn_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15393 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23017 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/branding_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/branding_policies_priorities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11775 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/camera_custom_analytics_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18966 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/camera_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10047 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15201 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/config_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75016 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/config_templates_switch_profiles_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14660 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/early_access_features_opt_ins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5604 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_action_batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_acls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3938 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_admins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_alerts_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19677 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15208 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests_overview_response_codes_by_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_security_intrusion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10527 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_traffic_shaping_vpn_exclusions_by_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_uplinks_statuses_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_uplinks_usage_by_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4156 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_vpn_third_party_vpnpeers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_vpn_vpn_firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_branding_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4038 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_branding_policies_priorities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_boundaries_areas_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_boundaries_lines_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_custom_analytics_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_detections_history_by_boundary_by_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12434 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_cellular_gateway_uplink_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_bandwidth_usage_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9054 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates_switch_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6970 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates_switch_profiles_ports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_availabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_availabilities_change_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15313 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_boots_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16135 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_power_modules_statuses_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16734 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_provisioning_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6582 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_statuses_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15900 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_uplinks_addresses_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9899 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_uplinks_loss_and_latency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3984 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_early_access_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_early_access_features_opt_ins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_firmware_upgrades.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14989 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_firmware_upgrades_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_insight_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_insight_monitored_media_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19756 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5602 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11374 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licenses_overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10645 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licensing_coterm_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_login_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4564 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_openapi_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9284 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_policy_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9644 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_policy_objects_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml_idps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15945 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sensor_readings_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12583 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sensor_readings_latest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_admins_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_apns_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_sentry_policies_assignments_by_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_vpp_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7711 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_appliances_by_utilization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_clients_by_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_clients_manufacturers_by_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_devices_by_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7621 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_devices_models_by_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8820 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_networks_by_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_ssids_by_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_switches_by_energy_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19060 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_switch_ports_by_switch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_uplinks_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4925 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_webhooks_callbacks_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_webhooks_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16054 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16098 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_device_by_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16927 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_network_by_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10376 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_ethernet_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16503 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16524 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16608 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/insight_monitored_media_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_claim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9333 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_export_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19918 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27098 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_assign_seats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9062 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9237 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_move_seats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_renew_seats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licensing_coterm_licenses_move.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44808 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/login_security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/networks_combine.py
+-rw-r--r--   0 runner    (1001) docker     (127)   754190 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27082 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/policy_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/policy_objects_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8325 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15100 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml_idps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/sm_admins_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/sm_sentry_policies_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26679 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/snmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/switch_devices_clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8880 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15765 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9831 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:08:22.804960 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-23 17:08:22.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-23 17:08:22.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:08:22.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 17:08:22.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 17:08:22.000000 pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-23 17:08:16.000000 pulumi_meraki-0.2.0a1716483448/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:08:22.808960 pulumi_meraki-0.2.0a1716483448/setup.cfg
```

### Comparing `pulumi_meraki-0.2.0a1716250106/PKG-INFO` & `pulumi_meraki-0.2.0a1716483448/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pulumi_meraki
-Version: 0.2.0a1716250106
-Summary: A Pulumi package for creating and managing Meraki resources
+Version: 0.2.0a1716483448
+Summary: A Pulumi package for creating and managing Cisco Meraki resources
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-meraki
 Project-URL: Repository, https://github.com/pulumi/pulumi-meraki
 Keywords: pulumi,meraki,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
 
-# Meraki Resource Provider
+# Cisco Meraki Resource Provider
 
-The Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
+The Cisco Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `pulumi_meraki-0.2.0a1716250106/README.md` & `pulumi_meraki-0.2.0a1716483448/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Meraki Resource Provider
+# Cisco Meraki Resource Provider
 
-The Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
+The Cisco Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/__init__.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/_utilities.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/__init__.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/_inputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_identities_me.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_identities_me.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_entitlements.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_entitlements.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_subscriptions.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_subscriptions.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/get_licensing_subscription_subscriptions_compliance_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/get_licensing_subscription_subscriptions_compliance_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_bind.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_bind.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_claim.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/licensing_subscription_subscriptions_claim_key_validate.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/licensing_subscription_subscriptions_claim_key_validate.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/administered/outputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/administered/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/__init__.pyi` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/config/vars.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/__init__.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/_inputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_radio_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_radio_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_uplinks_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_uplinks_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/appliance_vmx_authentication_token.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/appliance_vmx_authentication_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/base.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/base.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/blink_leds.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/blink_leds.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_custom_analytics.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_custom_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_generate_snapshot.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_generate_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_quality_and_retention.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_quality_and_retention.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_sense.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_sense.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_video_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_video_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/camera_wireless_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/camera_wireless_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_gateway_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_gateway_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_gateway_port_forwarding_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_gateway_port_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/cellular_sims.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/cellular_sims.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_performance.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_performance.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_radio_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_radio_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_appliance_uplinks_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_appliance_uplinks_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_analytics_live.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_analytics_live.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_custom_analytics.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_custom_analytics.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_quality_and_retention.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_quality_and_retention.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_sense.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_sense.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_video_link.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_video_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_video_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_video_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_camera_wireless_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_camera_wireless_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_gateway_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_gateway_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_gateway_port_forwarding_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_gateway_port_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_cellular_sims.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_cellular_sims.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_arp_table.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_arp_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_cable_test.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_cable_test.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_ping.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_ping_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_ping_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_throughput_test.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_throughput_test.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_live_tools_wake_on_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_live_tools_wake_on_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_lldp_cdp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_lldp_cdp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_sensor_relationships.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_sensor_relationships.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_ports_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_ports_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_interfaces.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_interfaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_interfaces_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_interfaces_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_routing_static_routes.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_routing_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_switch_warm_spare.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_switch_warm_spare.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_bluetooth_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_bluetooth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_connection_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_connection_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_latency_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_latency_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_radio_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_radio_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/get_wireless_status.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/get_wireless_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_arp_table.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_arp_table.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_cable.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_cable.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_ping.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_ping.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_ping_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_ping_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_throughput_test.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_throughput_test.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/live_tools_wake_on_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/live_tools_wake_on_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/outputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/sensor_relationships.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/sensor_relationships.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_ports_cycle.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_ports_cycle.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_interfaces.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_interfaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_interfaces_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_interfaces_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_routing_static_routes.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_routing_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/switch_warm_spare.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/switch_warm_spare.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_alternate_management_interface_ipv6.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_alternate_management_interface_ipv6.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_bluetooth_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_bluetooth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/devices/wireless_radio_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/devices/wireless_radio_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_devices.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_networks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/get_organizations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/get_organizations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/__init__.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/_inputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/alerts_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/alerts_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_connectivity_monitoring_destinations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_connectivity_monitoring_destinations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_content_filtering.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_content_filtering.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_cellular_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_cellular_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_firewalled_services.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_firewalled_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_inbound_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_inbound_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_l3_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_l3_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_l7_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_l7_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_one_to_many_nat_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_one_to_many_nat_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_one_to_one_nat_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_one_to_one_nat_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_port_forwarding_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_port_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_firewall_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_firewall_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_prefixes_delegated_statics.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_prefixes_delegated_statics.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_rf_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_rf_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_security_intrusion.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_security_intrusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_security_malware.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_security_malware.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_single_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_single_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_ssids.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_ssids.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_custom_performance_classes.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_custom_performance_classes.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_uplink_bandwidth.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_uplink_bandwidth.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_uplink_selection.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_uplink_selection.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_traffic_shaping_vpn_exclusions.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_traffic_shaping_vpn_exclusions.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vlans.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vlans.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vlans_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vlans_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vpn_bgp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vpn_bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_vpn_site_to_site_vpn.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_vpn_site_to_site_vpn.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_warm_spare.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_warm_spare.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/appliance_warm_spare_swap.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/appliance_warm_spare_swap.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/base.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/base.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/bind.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/bind.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/camera_quality_retention_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/camera_quality_retention_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/camera_wireless_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/camera_wireless_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_connectivity_monitoring_destinations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_connectivity_monitoring_destinations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_subnet_pool.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_subnet_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/cellular_gateway_uplink.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/cellular_gateway_uplink.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_policy.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_provision.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_provision.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/clients_splash_authorization_status.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/clients_splash_authorization_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_claim.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_claim_vmx.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_claim_vmx.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/devices_remove.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/devices_remove.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_rollbacks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_rollbacks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events_defer.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events_defer.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_events_rollbacks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_events_rollbacks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/firmware_upgrades_staged_stages.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/firmware_upgrades_staged_stages.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/floor_plans.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/floor_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_alerts_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_alerts_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_alerts_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_alerts_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_connectivity_monitoring_destinations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_connectivity_monitoring_destinations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_content_filtering.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_content_filtering.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_content_filtering_categories.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_content_filtering_categories.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_cellular_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_cellular_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_firewalled_services.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_firewalled_services.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_inbound_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_inbound_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l3_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l3_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules_application_categories.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_l7_firewall_rules_application_categories.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_one_to_many_nat_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_one_to_many_nat_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_one_to_one_nat_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_one_to_one_nat_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_port_forwarding_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_port_forwarding_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_firewall_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_firewall_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_prefixes_delegated_statics.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_prefixes_delegated_statics.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_rf_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_rf_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_security_intrusion.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_security_intrusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_security_malware.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_security_malware.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_single_lan.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_single_lan.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_ssids.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_ssids.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_bandwidth.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_bandwidth.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_selection.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_traffic_shaping_uplink_selection.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vlans.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vlans.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vlans_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vlans_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vpn_bgp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vpn_bgp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_vpn_site_to_site_vpn.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_vpn_site_to_site_vpn.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_appliance_warm_spare.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_appliance_warm_spare.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_bluetooth_clients.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_bluetooth_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_camera_quality_retention_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_camera_quality_retention_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_camera_wireless_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_camera_wireless_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_connectivity_monitoring_destinations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_connectivity_monitoring_destinations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_subnet_pool.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_subnet_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_cellular_gateway_uplink.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_cellular_gateway_uplink.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_policy.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_clients_splash_authorization_status.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_clients_splash_authorization_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_events.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_events_event_types.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_events_event_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_events.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_firmware_upgrades_staged_stages.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_firmware_upgrades_staged_stages.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_floor_plans.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_floor_plans.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_group_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_health_alerts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_health_alerts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_insight_applications_health_by_time.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_insight_applications_health_by_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_meraki_auth_users.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_meraki_auth_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_netflow.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_netflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_pii_keys.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_pii_keys.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_requests.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_requests.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_sm_devices_for_key.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_sm_devices_for_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_pii_sm_owners_for_key.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_pii_sm_owners_for_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_policies_by_client.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_policies_by_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_current_overview_by_metric.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_current_overview_by_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_overview_by_metric.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_overview_by_metric.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_alerts_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_alerts_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_mqtt_brokers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_mqtt_brokers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sensor_relationships.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sensor_relationships.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_bypass_activation_lock_attempts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_bypass_activation_lock_attempts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_cellular_usage_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_cellular_usage_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_certs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_certs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_connectivity.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_connectivity.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_desktop_logs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_desktop_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_device_command_logs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_device_command_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_device_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_device_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_network_adapters.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_network_adapters.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_performance_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_performance_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_security_centers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_security_centers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_devices_wlan_lists.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_devices_wlan_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_target_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_target_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_trusted_access_configs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_trusted_access_configs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_user_access_devices.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_user_access_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users_device_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users_device_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_sm_users_softwares.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_sm_users_softwares.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_snmp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_snmp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_access_control_lists.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_access_control_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_access_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_access_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_alternate_management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_alternate_management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_trusted_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_trusted_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_warnings_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_server_policy_arp_inspection_warnings_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dhcp_v4_servers_seen.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dhcp_v4_servers_seen.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_dscp_to_cos_mappings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_dscp_to_cos_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_link_aggregations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_link_aggregations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_mtu.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_mtu.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_port_schedules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_port_schedules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_qos_rules_order.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_qos_rules_order.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_multicast.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_multicast.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_multicast_rendezvous_points.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_multicast_rendezvous_points.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_routing_ospf.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_routing_ospf.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_interfaces.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_interfaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_interfaces_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_interfaces_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stacks_routing_static_routes.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stacks_routing_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_storm_control.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_storm_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_switch_stp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_switch_stp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_syslog_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_syslog_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_topology_link_layer.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_topology_link_layer.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_analysis.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_shaping_application_categories.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_shaping_application_categories.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_traffic_shaping_dscp_tagging_options.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_traffic_shaping_dscp_tagging_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_vlan_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_vlan_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_vlan_profiles_assignments_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_vlan_profiles_assignments_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_http_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_http_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_payload_templates.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_payload_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_webhooks_webhook_tests.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_webhooks_webhook_tests.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_alternate_management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_alternate_management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_billing.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_bluetooth_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_bluetooth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_channel_utilization_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_channel_utilization_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_client_count_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_client_count_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_clients_connection_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_clients_connection_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_clients_latency_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_clients_latency_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_connection_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_connection_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_data_rate_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_data_rate_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_devices_connection_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_devices_connection_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ethernet_ports_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ethernet_ports_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_failed_connections.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_failed_connections.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_latency_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_latency_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_latency_stats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_latency_stats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_mesh_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_mesh_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_rf_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_rf_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_signal_quality_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_signal_quality_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_bonjour_forwarding.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_bonjour_forwarding.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_device_type_group_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_device_type_group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_eap_override.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_eap_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_firewall_l3_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_firewall_l3_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_firewall_l7_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_firewall_l7_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_hotspot20.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_hotspot20.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_identity_psks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_identity_psks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_schedules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_schedules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_splash_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_splash_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_traffic_shaping_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_traffic_shaping_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_ssids_vpn.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_ssids_vpn.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/get_wireless_usage_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/get_wireless_usage_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/group_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/meraki_auth_users.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/meraki_auth_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/mqtt_brokers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/mqtt_brokers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/netflow.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/netflow.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/outputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/pii_requests_delete.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/pii_requests_delete.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sensor_alerts_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sensor_alerts_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sensor_mqtt_brokers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sensor_mqtt_brokers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_bypass_activation_lock_attempts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_bypass_activation_lock_attempts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_checkin.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_checkin.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_fields.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_fields.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_install_apps.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_install_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_lock.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_lock.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_modify_tags.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_modify_tags.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_move.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_move.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_reboot.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_reboot.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_refresh_details.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_refresh_details.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_shutdown.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_shutdown.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_unenroll.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_unenroll.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_uninstall_apps.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_uninstall_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_devices_wipe.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_devices_wipe.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_target_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_target_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/sm_user_access_devices_delete.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/sm_user_access_devices_delete.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/snmp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/snmp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/split.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/split.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_access_control_lists.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_access_control_lists.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_access_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_access_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_alternate_management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_alternate_management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dhcp_server_policy.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dhcp_server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dhcp_server_policy_arp_inspection_trusted_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dhcp_server_policy_arp_inspection_trusted_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_dscp_to_cos_mappings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_dscp_to_cos_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_link_aggregations.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_link_aggregations.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_mtu.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_mtu.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_port_schedules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_port_schedules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_qos_rules_order.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_qos_rules_order.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_multicast.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_multicast.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_multicast_rendezvous_points.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_multicast_rendezvous_points.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_routing_ospf.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_routing_ospf.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_add.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_add.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_remove.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_remove.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_interfaces.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_interfaces.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_interfaces_dhcp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_interfaces_dhcp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stacks_routing_static_routes.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stacks_routing_static_routes.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_storm_control.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_storm_control.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/switch_stp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/switch_stp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/syslog_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/syslog_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/traffic_analysis.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/traffic_analysis.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/unbind.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/unbind.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/vlan_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/vlan_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/vlan_profiles_assignments_reassign.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/vlan_profiles_assignments_reassign.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/webhooks_http_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/webhooks_http_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/webhooks_payload_templates.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/webhooks_payload_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_alternate_management_interface.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_alternate_management_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_billing.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_billing.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_bluetooth_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_bluetooth_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles_assign.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles_assign.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ethernet_ports_profiles_set_default.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ethernet_ports_profiles_set_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_rf_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_rf_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_bonjour_forwarding.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_bonjour_forwarding.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_device_type_group_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_device_type_group_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_eap_override.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_eap_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_firewall_l3_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_firewall_l3_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_firewall_l7_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_firewall_l7_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_hotspot20.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_hotspot20.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_identity_psks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_identity_psks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_schedules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_schedules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_splash_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_splash_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_traffic_shaping_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_traffic_shaping_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/networks/wireless_ssids_vpn.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/networks/wireless_ssids_vpn.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/__init__.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/_inputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/action_batches.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/action_batches.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_acls.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/adaptive_policy_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/adaptive_policy_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/admins.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/admins.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/alerts_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/alerts_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_security_intrusion.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_security_intrusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_vpn_third_party_vpnpeers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_vpn_third_party_vpnpeers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/appliance_vpn_vpn_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/appliance_vpn_vpn_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/base.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/base.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/branding_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/branding_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/branding_policies_priorities.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/branding_policies_priorities.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/camera_custom_analytics_artifacts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/camera_custom_analytics_artifacts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/camera_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/camera_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/claim.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/clone.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/clone.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/config_templates.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/config_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/config_templates_switch_profiles_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/config_templates_switch_profiles_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/early_access_features_opt_ins.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/early_access_features_opt_ins.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_action_batches.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_action_batches.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_acls.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_acls.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_adaptive_policy_settings.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_adaptive_policy_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_admins.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_admins.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_alerts_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_alerts_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_api_requests_overview_response_codes_by_interval.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_api_requests_overview_response_codes_by_interval.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_security_intrusion.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_security_intrusion.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_traffic_shaping_vpn_exclusions_by_network.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_traffic_shaping_vpn_exclusions_by_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_uplinks_statuses_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_uplinks_statuses_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_uplinks_usage_by_network.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_uplinks_usage_by_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_vpn_third_party_vpnpeers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_vpn_third_party_vpnpeers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_appliance_vpn_vpn_firewall_rules.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_appliance_vpn_vpn_firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_branding_policies.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_branding_policies.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_branding_policies_priorities.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_branding_policies_priorities.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_boundaries_areas_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_boundaries_areas_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_boundaries_lines_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_boundaries_lines_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_custom_analytics_artifacts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_custom_analytics_artifacts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_detections_history_by_boundary_by_interval.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_detections_history_by_boundary_by_interval.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_permissions.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_camera_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_camera_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_cellular_gateway_uplink_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_cellular_gateway_uplink_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_bandwidth_usage_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_bandwidth_usage_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_clients_search.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_clients_search.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates_switch_profiles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates_switch_profiles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_config_templates_switch_profiles_ports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_config_templates_switch_profiles_ports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_availabilities.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_availabilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_availabilities_change_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_availabilities_change_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_boots_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_boots_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_power_modules_statuses_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_power_modules_statuses_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_provisioning_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_provisioning_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_statuses_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_statuses_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_uplinks_addresses_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_uplinks_addresses_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_devices_uplinks_loss_and_latency.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_devices_uplinks_loss_and_latency.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_early_access_features.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_early_access_features.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_early_access_features_opt_ins.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_early_access_features_opt_ins.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_firmware_upgrades.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_firmware_upgrades.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_firmware_upgrades_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_firmware_upgrades_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_insight_applications.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_insight_applications.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_insight_monitored_media_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_insight_monitored_media_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_devices.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_imports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_imports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_networks.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_inventory_onboarding_cloud_monitoring_networks.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licenses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licenses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licenses_overview.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licenses_overview.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_licensing_coterm_licenses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_licensing_coterm_licenses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_login_security.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_login_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_openapi_spec.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_openapi_spec.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_policy_objects.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_policy_objects.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_policy_objects_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_policy_objects_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml_idps.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml_idps.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_saml_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_saml_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sensor_readings_history.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sensor_readings_history.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sensor_readings_latest.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sensor_readings_latest.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_admins_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_admins_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_apns_cert.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_apns_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_sentry_policies_assignments_by_network.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_sentry_policies_assignments_by_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_sm_vpp_accounts.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_sm_vpp_accounts.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_snmp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_snmp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_appliances_by_utilization.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_appliances_by_utilization.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_clients_by_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_clients_by_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_clients_manufacturers_by_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_clients_manufacturers_by_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_devices_by_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_devices_by_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_devices_models_by_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_devices_models_by_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_networks_by_status.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_networks_by_status.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_ssids_by_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_ssids_by_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_summary_top_switches_by_energy_usage.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_summary_top_switches_by_energy_usage.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_switch_ports_by_switch.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_switch_ports_by_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_uplinks_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_uplinks_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_webhooks_callbacks_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_webhooks_callbacks_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_webhooks_logs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_webhooks_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_network.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_by_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_device_by_interval.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_device_by_interval.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_network_by_interval.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_channel_utilization_history_by_network_by_interval.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_ethernet_statuses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_ethernet_statuses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_client.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_client.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_device.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_network.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/get_wireless_devices_packet_loss_by_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/insight_monitored_media_servers.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/insight_monitored_media_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_claim.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_export_events.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_export_events.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_imports.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_imports.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_prepare.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_onboarding_cloud_monitoring_prepare.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/inventory_release.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/inventory_release.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_assign_seats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_assign_seats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_move.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_move.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_move_seats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_move_seats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licenses_renew_seats.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licenses_renew_seats.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/licensing_coterm_licenses_move.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/licensing_coterm_licenses_move.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/login_security.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/login_security.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/networks_combine.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/networks_combine.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/outputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/policy_objects.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/policy_objects.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/policy_objects_groups.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/policy_objects_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml_idps.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml_idps.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/saml_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/saml_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/sm_admins_roles.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/sm_admins_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/sm_sentry_policies_assignments.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/sm_sentry_policies_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/snmp.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/snmp.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/switch_devices_clone.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/switch_devices_clone.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/organizations/users.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/organizations/users.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/outputs.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki/provider.py` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/PKG-INFO` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pulumi_meraki
-Version: 0.2.0a1716250106
-Summary: A Pulumi package for creating and managing Meraki resources
+Version: 0.2.0a1716483448
+Summary: A Pulumi package for creating and managing Cisco Meraki resources
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/pulumi/pulumi-meraki
 Project-URL: Repository, https://github.com/pulumi/pulumi-meraki
 Keywords: pulumi,meraki,category/network
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0
 Requires-Dist: semver>=2.8.1
 
-# Meraki Resource Provider
+# Cisco Meraki Resource Provider
 
-The Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
+The Cisco Meraki Resource Provider lets you manage [meraki](https://www.pulumi.com/registry/packages/meraki/) resources.
 
 ## Installing
 
 This package is available for several languages/platforms:
 
 ### Node.js (JavaScript/TypeScript)
```

### Comparing `pulumi_meraki-0.2.0a1716250106/pulumi_meraki.egg-info/SOURCES.txt` & `pulumi_meraki-0.2.0a1716483448/pulumi_meraki.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_meraki-0.2.0a1716250106/pyproject.toml` & `pulumi_meraki-0.2.0a1716483448/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_meraki"
-  description = "A Pulumi package for creating and managing Meraki resources"
+  description = "A Pulumi package for creating and managing Cisco Meraki resources"
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "meraki", "category/network"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.2.0a1716250106"
+  version = "0.2.0a1716483448"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://github.com/pulumi/pulumi-meraki"
     Repository = "https://github.com/pulumi/pulumi-meraki"
 
 [build-system]
```

