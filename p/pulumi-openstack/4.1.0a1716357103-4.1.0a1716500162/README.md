# Comparing `tmp/pulumi_openstack-4.1.0a1716357103.tar.gz` & `tmp/pulumi_openstack-4.1.0a1716500162.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_openstack-4.1.0a1716357103.tar", last modified: Wed May 22 05:54:01 2024, max compression
+gzip compressed data, was "pulumi_openstack-4.1.0a1716500162.tar", last modified: Thu May 23 21:38:22 2024, max compression
```

## Comparing `pulumi_openstack-4.1.0a1716357103.tar` & `pulumi_openstack-4.1.0a1716500162.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.627889 pulumi_openstack-4.1.0a1716357103/
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-22 05:54:01.627889 pulumi_openstack-4.1.0a1716357103/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.587888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/
--rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.591888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_availability_zones_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_quotaset_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_snapshot_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_snapshot_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_volume_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_volume_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/qos_association_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/qos_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    28669 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/quote_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    28669 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/quote_set_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    44956 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    38859 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_attach_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_type_access_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17714 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_type_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    37568 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.595888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35443 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18179 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/aggregate_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32397 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/flavor_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    18614 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/floating_ip_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_aggregate_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_availability_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_flavor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_hypervisor_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_instance_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_limits_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_quota_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    88272 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/interface_attach.py
--rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/keypair.py
--rw-r--r--   0 runner    (1001) docker     (127)    33291 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    42864 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/quota_set_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19310 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/sec_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    23028 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/server_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    24340 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/volume_attach.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.595888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.599888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59231 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    97457 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    16346 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    21057 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_node_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    40483 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/node_group.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.599888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    29350 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.599888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/get_dns_zone.py
--rw-r--r--   0 runner    (1001) docker     (127)    29088 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    18738 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/transfer_accept.py
--rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/transfer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    30905 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/zone.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.603888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30298 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    38798 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/group_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    31065 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    46944 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/rule_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_group_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_rule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.603888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    36231 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/application_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/ec2_credential_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/endpoint_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_auth_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/group_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/inherit_role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    16691 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/role_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/service_v3.py
--rw-r--r--   0 runner    (1001) docker     (127)    38943 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/user_membership_v3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.607888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/get_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/get_image_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    68742 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image_access_accept.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.607888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31316 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/container_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/get_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    18940 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/get_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    22757 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/order_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    46831 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/secret_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.611888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/get_flavor_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    31088 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/l7_policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    30636 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/l7_rule_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    56161 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)    44643 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    35077 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/member_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/members.py
--rw-r--r--   0 runner    (1001) docker     (127)    39158 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    34035 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/monitor_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    30742 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/pool_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    27771 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/quota.py
--rw-r--r--   0 runner    (1001) docker     (127)    39016 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/vip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.619888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16090 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/address_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    42850 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/floating_ip_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_address_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_floating_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_network.py
--rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_port.py
--rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_port_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_dscp_marking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_quota_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_sec_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet_ids_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_trunk.py
--rw-r--r--   0 runner    (1001) docker     (127)    55597 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    25544 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    74334 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port.py
--rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port_forwarding_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port_sec_group_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19679 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_bandwidth_limit_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_dscp_marking_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/quota_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    21098 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/rbac_policy_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    49877 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router.py
--rw-r--r--   0 runner    (1001) docker     (127)    19055 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    17431 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    19914 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/sec_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    40095 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/sec_group_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    58657 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    53352 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet_route.py
--rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/trunk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.619888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    56422 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/container_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20156 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/temp_url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.619888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    49598 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/stack_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    42404 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.623888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_availbility_zones.py
--rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_share.py
--rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_share_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29901 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/security_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    42581 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share.py
--rw-r--r--   0 runner    (1001) docker     (127)    25161 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share_access.py
--rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.623888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22372 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/endpoint_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/ike_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    33689 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/ip_sec_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    27860 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    56548 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/site_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 05:54:01.623888 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-22 05:54:01.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-05-22 05:54:01.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 05:54:01.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 05:54:01.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 05:54:01.000000 pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 05:53:55.000000 pulumi_openstack-4.1.0a1716357103/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 05:54:01.627889 pulumi_openstack-4.1.0a1716357103/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.849160 pulumi_openstack-4.1.0a1716500162/
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-23 21:38:22.849160 pulumi_openstack-4.1.0a1716500162/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8755 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.809160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/
+-rw-r--r--   0 runner    (1001) docker     (127)    22384 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.813160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_availability_zones_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_quotaset_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_snapshot_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_snapshot_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7868 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_volume_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_volume_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15235 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12942 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/qos_association_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13607 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/qos_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28669 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/quote_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28669 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/quote_set_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44956 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38859 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_attach_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12970 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_type_access_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17714 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_type_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29620 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37568 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.817160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35443 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18179 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/aggregate_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32397 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12752 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/flavor_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18614 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/floating_ip_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_aggregate_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_availability_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11231 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_flavor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6173 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_hypervisor_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12252 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_instance_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5781 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16375 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_limits_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12042 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_quota_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    88272 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20990 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/interface_attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/keypair.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33291 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42864 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/quota_set_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19310 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23028 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/server_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24340 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/volume_attach.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.817160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7088 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.817160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59231 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97457 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16346 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21057 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_node_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40483 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/node_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.821160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12788 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15948 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29350 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11089 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.821160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15682 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/get_dns_zone.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29088 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18738 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/transfer_accept.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/transfer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30905 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/zone.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.821160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30298 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7350 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38798 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/group_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27450 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31065 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40012 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46944 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/rule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12479 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_group_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16215 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_rule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.825160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36231 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/application_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18169 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/ec2_credential_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19326 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/endpoint_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12233 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_auth_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8708 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5109 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12564 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/group_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17610 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/inherit_role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22026 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10560 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16691 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/role_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13628 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/service_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38943 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13405 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/user_membership_v3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.825160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21045 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13536 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/get_image_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68742 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20355 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image_access_accept.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.829160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31316 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/container_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/get_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18940 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/get_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22757 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/order_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18182 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46831 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/secret_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.833160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/get_flavor_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31088 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/l7_policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30636 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/l7_rule_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56161 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44643 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35077 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20873 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/member_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14093 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39158 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34035 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/monitor_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30742 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/pool_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27771 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/quota.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39016 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/vip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.841160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16090 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19004 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/address_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42850 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15063 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/floating_ip_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6509 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_address_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10568 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_floating_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14634 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15158 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_port_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_dscp_marking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8328 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_quota_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15189 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet_ids_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9733 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_trunk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55597 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25544 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74334 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27314 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port_forwarding_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19846 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port_sec_group_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19679 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_bandwidth_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13519 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_dscp_marking_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29320 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29003 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/quota_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21098 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/rbac_policy_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49877 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19055 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17431 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19914 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/sec_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40095 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/sec_group_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58657 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53352 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/trunk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.841160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45389 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56422 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/container_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20156 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/temp_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.845160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49598 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/stack_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42404 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.845160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_availbility_zones.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12999 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12110 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_share_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8266 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29901 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/security_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42581 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25161 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.845160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22372 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/endpoint_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33283 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/ike_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33689 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/ip_sec_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27860 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56548 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/site_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:38:22.849160 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9219 2024-05-23 21:38:22.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-05-23 21:38:22.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:38:22.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 21:38:22.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 21:38:22.000000 pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-23 21:38:16.000000 pulumi_openstack-4.1.0a1716500162/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:38:22.849160 pulumi_openstack-4.1.0a1716500162/setup.cfg
```

### Comparing `pulumi_openstack-4.1.0a1716357103/PKG-INFO` & `pulumi_openstack-4.1.0a1716500162/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_openstack
-Version: 4.1.0a1716357103
+Version: 4.1.0a1716500162
 Summary: A Pulumi package for creating and managing OpenStack cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-openstack
 Keywords: pulumi,openstack
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_openstack-4.1.0a1716357103/README.md` & `pulumi_openstack-4.1.0a1716500162/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/_utilities.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_availability_zones_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_availability_zones_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_quotaset_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_quotaset_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_snapshot_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_snapshot_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_snapshot_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_snapshot_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_volume_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_volume_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/get_volume_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/get_volume_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/qos_association_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/qos_association_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/qos_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/qos_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/quote_set_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/quote_set_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/quote_set_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/quote_set_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_attach.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_attach_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_attach_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_type_access_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_type_access_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_type_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_type_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/blockstorage/volume_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/blockstorage/volume_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/aggregate_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/aggregate_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/flavor.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/flavor.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/flavor_access.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/flavor_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/floating_ip.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/floating_ip_associate.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/floating_ip_associate.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_aggregate_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_aggregate_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_availability_zones.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_availability_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_flavor.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_flavor.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_hypervisor_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_hypervisor_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_instance_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_instance_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_keypair.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_limits_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_limits_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/get_quota_set_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/get_quota_set_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/instance.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/interface_attach.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/interface_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/keypair.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/keypair.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/quota_set_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/quota_set_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/sec_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/sec_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/server_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/server_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/compute/volume_attach.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/compute/volume_attach.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/__init__.pyi` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/config/vars.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/cluster.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/cluster_template.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_cluster.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_cluster_template.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_cluster_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/get_node_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/get_node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/containerinfra/node_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/containerinfra/node_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/configuration.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/database.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/database.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/instance.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/database/user.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/database/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/get_dns_zone.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/get_dns_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/record_set.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/record_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/transfer_accept.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/transfer_accept.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/transfer_request.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/transfer_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/dns/zone.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/dns/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/firewall.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/get_policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/group_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/policy_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/policy_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/firewall/rule_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/firewall/rule_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_group_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_group_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_policy_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_policy_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/get_fw_rule_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/get_fw_rule_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/application_credential.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/application_credential.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/ec2_credential_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/ec2_credential_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/endpoint_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/endpoint_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_auth_scope.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_auth_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_endpoint.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_endpoint.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_project.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_project.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_role.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_service.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/get_user.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/group_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/group_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/inherit_role_assignment.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/inherit_role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/project.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/project.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/role.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/role_assignment.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/role_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/service_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/service_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/user.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/identity/user_membership_v3.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/identity/user_membership_v3.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/get_image.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/get_image_ids.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/get_image_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image_access.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/images/image_access_accept.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/images/image_access_accept.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/container_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/container_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/get_container.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/get_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/get_secret.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/get_secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/order_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/order_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/keymanager/secret_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/keymanager/secret_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/get_flavor_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/get_flavor_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/l7_policy_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/l7_policy_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/l7_rule_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/l7_rule_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/listener.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/listener.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/load_balancer.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/member.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/member.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/member_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/member_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/members.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/members.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/monitor.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/monitor_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/monitor_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/pool.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/pool_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/pool_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/quota.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/loadbalancer/vip.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/loadbalancer/vip.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/address_scope.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/address_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/floating_ip.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/floating_ip_associate.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/floating_ip_associate.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_address_scope.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_address_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_floating_ip.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_floating_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_network.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_port.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_port.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_port_ids.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_port_ids.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_bandwidth_limit_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_dscp_marking_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_dscp_marking_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_minimum_bandwidth_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_qos_policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_qos_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_quota_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_quota_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_router.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_router.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_sec_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_sec_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet_ids_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet_ids_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_subnet_pool.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_subnet_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/get_trunk.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/get_trunk.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/network.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port_forwarding_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port_forwarding_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/port_sec_group_associate.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/port_sec_group_associate.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_bandwidth_limit_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_bandwidth_limit_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_dscp_marking_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_dscp_marking_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_minimum_bandwidth_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/qos_policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/qos_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/quota_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/quota_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/rbac_policy_v2.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/rbac_policy_v2.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router_interface.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router_interface.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/router_route.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/router_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/sec_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/sec_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/sec_group_rule.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/sec_group_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet_pool.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/subnet_route.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/subnet_route.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/networking/trunk.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/networking/trunk.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/container.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/container_object.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/container_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/objectstorage/temp_url.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/objectstorage/temp_url.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/orchestration/stack_v1.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/orchestration/stack_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/provider.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/__init__.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_availbility_zones.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_availbility_zones.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_share.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_share.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_share_network.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_share_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/get_snapshot.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/get_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/security_service.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/security_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share_access.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/sharedfilesystem/share_network.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/sharedfilesystem/share_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/_inputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/endpoint_group.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/endpoint_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/ike_policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/ike_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/ip_sec_policy.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/ip_sec_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/outputs.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/service.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack/vpnaas/site_connection.py` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack/vpnaas/site_connection.py`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/PKG-INFO` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_openstack
-Version: 4.1.0a1716357103
+Version: 4.1.0a1716500162
 Summary: A Pulumi package for creating and managing OpenStack cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-openstack
 Keywords: pulumi,openstack
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_openstack-4.1.0a1716357103/pulumi_openstack.egg-info/SOURCES.txt` & `pulumi_openstack-4.1.0a1716500162/pulumi_openstack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_openstack-4.1.0a1716357103/pyproject.toml` & `pulumi_openstack-4.1.0a1716500162/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_openstack"
   description = "A Pulumi package for creating and managing OpenStack cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "openstack"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "4.1.0a1716357103"
+  version = "4.1.0a1716500162"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-openstack"
 
 [build-system]
```

