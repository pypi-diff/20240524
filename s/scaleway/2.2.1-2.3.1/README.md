# Comparing `tmp/scaleway-2.2.1.tar.gz` & `tmp/scaleway-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaleway-2.2.1.tar", max compression
+gzip compressed data, was "scaleway-2.3.1.tar", max compression
```

## Comparing `scaleway-2.2.1.tar` & `scaleway-2.3.1.tar`

### file list

```diff
@@ -1,226 +1,231 @@
--rw-r--r--   0        0        0       76 2024-05-14 12:14:18.420369 scaleway-2.2.1/README.md
--rw-r--r--   0        0        0     1112 2024-05-14 12:14:34.792216 scaleway-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      905 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/__init__.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/__init__.py
--rw-r--r--   0        0        0      714 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/__init__.py
--rw-r--r--   0        0        0     8456 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/api.py
--rw-r--r--   0        0        0     2850 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/marshalling.py
--rw-r--r--   0        0        0     2638 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v2/types.py
--rw-r--r--   0        0        0      828 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/__init__.py
--rw-r--r--   0        0        0     8180 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/api.py
--rw-r--r--   0        0        0     2910 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/marshalling.py
--rw-r--r--   0        0        0     2678 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/account/v3/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/__init__.py
--rw-r--r--   0        0        0     1674 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18924 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/api.py
--rw-r--r--   0        0        0      496 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/content.py
--rw-r--r--   0        0        0     8890 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8104 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/applesilicon/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/__init__.py
--rw-r--r--   0        0        0     5338 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/__init__.py
--rw-r--r--   0        0        0    52768 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/api.py
--rw-r--r--   0        0        0     1063 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/content.py
--rw-r--r--   0        0        0    31590 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/marshalling.py
--rw-r--r--   0        0        0    27983 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/baremetal/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/__init__.py
--rw-r--r--   0        0        0     1414 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/__init__.py
--rw-r--r--   0        0        0     9098 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/api.py
--rw-r--r--   0        0        0     7732 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/marshalling.py
--rw-r--r--   0        0        0     7103 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2alpha1/types.py
--rw-r--r--   0        0        0     2078 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/__init__.py
--rw-r--r--   0        0        0    18927 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/api.py
--rw-r--r--   0        0        0    11343 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/marshalling.py
--rw-r--r--   0        0        0    12804 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/billing/v2beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/__init__.py
--rw-r--r--   0        0        0     2398 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/__init__.py
--rw-r--r--   0        0        0    27041 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/api.py
--rw-r--r--   0        0        0      922 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/content.py
--rw-r--r--   0        0        0    13085 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    13168 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/block/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/__init__.py
--rw-r--r--   0        0        0     4656 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/__init__.py
--rw-r--r--   0        0        0    46974 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/api.py
--rw-r--r--   0        0        0    20821 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/marshalling.py
--rw-r--r--   0        0        0    20051 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1/types.py
--rw-r--r--   0        0        0     3758 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/__init__.py
--rw-r--r--   0        0        0    33332 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/api.py
--rw-r--r--   0        0        0      418 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/content.py
--rw-r--r--   0        0        0    21727 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/marshalling.py
--rw-r--r--   0        0        0    15330 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/cockpit/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.420369 scaleway-2.2.1/scaleway/container/__init__.py
--rw-r--r--   0        0        0     5100 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/__init__.py
--rw-r--r--   0        0        0    63615 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/api.py
--rw-r--r--   0        0        0     1581 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/content.py
--rw-r--r--   0        0        0    27167 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/marshalling.py
--rw-r--r--   0        0        0    27207 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/container/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/__init__.py
--rw-r--r--   0        0        0    19280 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/__init__.py
--rw-r--r--   0        0        0   138198 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/api.py
--rw-r--r--   0        0        0     2688 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/content.py
--rw-r--r--   0        0        0    99051 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/marshalling.py
--rw-r--r--   0        0        0    74459 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/dedibox/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/__init__.py
--rw-r--r--   0        0        0     9342 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/__init__.py
--rw-r--r--   0        0        0   103285 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/api.py
--rw-r--r--   0        0        0     1614 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/content.py
--rw-r--r--   0        0        0    52204 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/marshalling.py
--rw-r--r--   0        0        0    42675 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/document_db/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/__init__.py
--rw-r--r--   0        0        0    13096 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/__init__.py
--rw-r--r--   0        0        0    91007 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/api.py
--rw-r--r--   0        0        0     1948 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/content.py
--rw-r--r--   0        0        0    90138 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/marshalling.py
--rw-r--r--   0        0        0    36143 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/domain/v2beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/__init__.py
--rw-r--r--   0        0        0     1766 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/__init__.py
--rw-r--r--   0        0        0    20507 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/api.py
--rw-r--r--   0        0        0      649 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/content.py
--rw-r--r--   0        0        0     8075 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8804 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/flexibleip/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/__init__.py
--rw-r--r--   0        0        0     5594 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/__init__.py
--rw-r--r--   0        0        0    65530 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/api.py
--rw-r--r--   0        0        0     1573 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/content.py
--rw-r--r--   0        0        0    29502 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/marshalling.py
--rw-r--r--   0        0        0    28712 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/function/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/__init__.py
--rw-r--r--   0        0        0     5586 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/__init__.py
--rw-r--r--   0        0        0    84589 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/api.py
--rw-r--r--   0        0        0    33530 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    30388 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/iam/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.424369 scaleway-2.2.1/scaleway/instance/__init__.py
--rw-r--r--   0        0        0    13930 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/__init__.py
--rw-r--r--   0        0        0   151681 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/api.py
--rw-r--r--   0        0        0     2388 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/content.py
--rw-r--r--   0        0        0   116222 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/marshalling.py
--rw-r--r--   0        0        0    65154 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/types.py
--rw-r--r--   0        0        0     6858 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/instance/v1/types_private.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/__init__.py
--rw-r--r--   0        0        0     5818 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/__init__.py
--rw-r--r--   0        0        0    61877 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/api.py
--rw-r--r--   0        0        0      363 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/content.py
--rw-r--r--   0        0        0    33920 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/marshalling.py
--rw-r--r--   0        0        0    29997 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/iot/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/__init__.py
--rw-r--r--   0        0        0      804 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/__init__.py
--rw-r--r--   0        0        0    13650 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/api.py
--rw-r--r--   0        0        0     6467 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/marshalling.py
--rw-r--r--   0        0        0     6550 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipam/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/__init__.py
--rw-r--r--   0        0        0     2572 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    33644 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/api.py
--rw-r--r--   0        0        0      552 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/content.py
--rw-r--r--   0        0        0    12468 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    11507 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/ipfs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/__init__.py
--rw-r--r--   0        0        0     1760 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/__init__.py
--rw-r--r--   0        0        0    18492 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/api.py
--rw-r--r--   0        0        0      402 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/content.py
--rw-r--r--   0        0        0    11319 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     7454 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/jobs/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/__init__.py
--rw-r--r--   0        0        0     5436 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/__init__.py
--rw-r--r--   0        0        0    59478 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/api.py
--rw-r--r--   0        0        0      934 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/content.py
--rw-r--r--   0        0        0    40014 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/marshalling.py
--rw-r--r--   0        0        0    44925 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/k8s/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/__init__.py
--rw-r--r--   0        0        0    13124 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/__init__.py
--rw-r--r--   0        0        0   228542 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/api.py
--rw-r--r--   0        0        0     1107 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/content.py
--rw-r--r--   0        0        0    82875 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/marshalling.py
--rw-r--r--   0        0        0    91077 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/lb/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/__init__.py
--rw-r--r--   0        0        0     3026 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/__init__.py
--rw-r--r--   0        0        0    31541 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/api.py
--rw-r--r--   0        0        0      443 2024-05-14 12:14:18.428369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/content.py
--rw-r--r--   0        0        0    17687 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/marshalling.py
--rw-r--r--   0        0        0    14475 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/llm_inference/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/__init__.py
--rw-r--r--   0        0        0     1470 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/__init__.py
--rw-r--r--   0        0        0    14905 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/api.py
--rw-r--r--   0        0        0     6721 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/marshalling.py
--rw-r--r--   0        0        0     5135 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/marketplace/v2/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/__init__.py
--rw-r--r--   0        0        0     3766 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/__init__.py
--rw-r--r--   0        0        0    42072 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/api.py
--rw-r--r--   0        0        0    18036 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/marshalling.py
--rw-r--r--   0        0        0    16867 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/mnq/v1beta1/types.py
--rw-r--r--   0        0        0        0 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/py.typed
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/__init__.py
--rw-r--r--   0        0        0     4200 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/__init__.py
--rw-r--r--   0        0        0    42961 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/api.py
--rw-r--r--   0        0        0      843 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/content.py
--rw-r--r--   0        0        0    18882 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    19382 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/qaas/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/__init__.py
--rw-r--r--   0        0        0    10564 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/__init__.py
--rw-r--r--   0        0        0   119808 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/api.py
--rw-r--r--   0        0        0     1950 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/content.py
--rw-r--r--   0        0        0    57699 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/marshalling.py
--rw-r--r--   0        0        0    48945 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/rdb/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/__init__.py
--rw-r--r--   0        0        0     3760 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/__init__.py
--rw-r--r--   0        0        0    44423 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/api.py
--rw-r--r--   0        0        0      488 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/content.py
--rw-r--r--   0        0        0    21902 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/marshalling.py
--rw-r--r--   0        0        0    17769 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/redis/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/__init__.py
--rw-r--r--   0        0        0     1962 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/__init__.py
--rw-r--r--   0        0        0    29203 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/api.py
--rw-r--r--   0        0        0      710 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/content.py
--rw-r--r--   0        0        0     8195 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/marshalling.py
--rw-r--r--   0        0        0    11276 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/registry/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/__init__.py
--rw-r--r--   0        0        0     3160 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/__init__.py
--rw-r--r--   0        0        0    51007 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/api.py
--rw-r--r--   0        0        0    15815 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    21526 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1alpha1/types.py
--rw-r--r--   0        0        0     3050 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/__init__.py
--rw-r--r--   0        0        0    36548 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/api.py
--rw-r--r--   0        0        0    15383 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/marshalling.py
--rw-r--r--   0        0        0    18709 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/secret/v1beta1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/__init__.py
--rw-r--r--   0        0        0     1528 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/__init__.py
--rw-r--r--   0        0        0    19895 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/api.py
--rw-r--r--   0        0        0      427 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/content.py
--rw-r--r--   0        0        0     6440 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py
--rw-r--r--   0        0        0     8013 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/types.py
--rw-r--r--   0        0        0      194 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/__init__.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/api.py
--rw-r--r--   0        0        0      129 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/marshalling.py
--rw-r--r--   0        0        0      469 2024-05-14 12:14:18.432369 scaleway-2.2.1/scaleway/std/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/__init__.py
--rw-r--r--   0        0        0     2646 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/__init__.py
--rw-r--r--   0        0        0    26537 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/api.py
--rw-r--r--   0        0        0      549 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/content.py
--rw-r--r--   0        0        0    18141 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    16807 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/tem/v1alpha1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/__init__.py
--rw-r--r--   0        0        0     1088 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/__init__.py
--rw-r--r--   0        0        0    11588 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/api.py
--rw-r--r--   0        0        0      349 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/content.py
--rw-r--r--   0        0        0     6231 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/marshalling.py
--rw-r--r--   0        0        0     3231 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/test/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/__init__.py
--rw-r--r--   0        0        0      818 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/__init__.py
--rw-r--r--   0        0        0    11732 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/api.py
--rw-r--r--   0        0        0     3338 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/marshalling.py
--rw-r--r--   0        0        0     4368 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v1/types.py
--rw-r--r--   0        0        0     1932 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/__init__.py
--rw-r--r--   0        0        0    31050 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/api.py
--rw-r--r--   0        0        0    10469 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/marshalling.py
--rw-r--r--   0        0        0    10678 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpc/v2/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/__init__.py
--rw-r--r--   0        0        0     4846 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/__init__.py
--rw-r--r--   0        0        0    81299 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/api.py
--rw-r--r--   0        0        0      755 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/content.py
--rw-r--r--   0        0        0    30617 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/marshalling.py
--rw-r--r--   0        0        0    35539 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/vpcgw/v1/types.py
--rw-r--r--   0        0        0      127 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/__init__.py
--rw-r--r--   0        0        0     2510 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/__init__.py
--rw-r--r--   0        0        0    22954 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/api.py
--rw-r--r--   0        0        0      421 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/content.py
--rw-r--r--   0        0        0    14989 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/marshalling.py
--rw-r--r--   0        0        0    14450 2024-05-14 12:14:18.436369 scaleway-2.2.1/scaleway/webhosting/v1alpha1/types.py
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 scaleway-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0       76 2024-05-24 15:04:33.747407 scaleway-2.3.1/README.md
+-rw-r--r--   0        0        0     1112 2024-05-24 15:04:54.031408 scaleway-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0      905 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/__init__.py
+-rw-r--r--   0        0        0      714 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v2/__init__.py
+-rw-r--r--   0        0        0     8470 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v2/api.py
+-rw-r--r--   0        0        0     2850 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v2/marshalling.py
+-rw-r--r--   0        0        0     2638 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v2/types.py
+-rw-r--r--   0        0        0      828 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v3/__init__.py
+-rw-r--r--   0        0        0     8194 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v3/api.py
+-rw-r--r--   0        0        0     2910 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v3/marshalling.py
+-rw-r--r--   0        0        0     2678 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/account/v3/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/__init__.py
+-rw-r--r--   0        0        0     1790 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18991 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/v1alpha1/api.py
+-rw-r--r--   0        0        0      496 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/v1alpha1/content.py
+-rw-r--r--   0        0        0    10147 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8395 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/applesilicon/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/__init__.py
+-rw-r--r--   0        0        0     5338 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/v1/__init__.py
+-rw-r--r--   0        0        0    52773 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/v1/api.py
+-rw-r--r--   0        0        0     1063 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/v1/content.py
+-rw-r--r--   0        0        0    31699 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/v1/marshalling.py
+-rw-r--r--   0        0        0    28106 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/baremetal/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/__init__.py
+-rw-r--r--   0        0        0     1414 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2alpha1/__init__.py
+-rw-r--r--   0        0        0     9130 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2alpha1/api.py
+-rw-r--r--   0        0        0     7732 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2alpha1/marshalling.py
+-rw-r--r--   0        0        0     7103 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2alpha1/types.py
+-rw-r--r--   0        0        0     2078 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2beta1/__init__.py
+-rw-r--r--   0        0        0    18959 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2beta1/api.py
+-rw-r--r--   0        0        0    11343 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    12804 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/billing/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/__init__.py
+-rw-r--r--   0        0        0     2398 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    27033 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/v1alpha1/api.py
+-rw-r--r--   0        0        0      949 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/v1alpha1/content.py
+-rw-r--r--   0        0        0    13085 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    13194 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/block/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/cockpit/__init__.py
+-rw-r--r--   0        0        0     4656 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/cockpit/v1/__init__.py
+-rw-r--r--   0        0        0    46974 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/cockpit/v1/api.py
+-rw-r--r--   0        0        0    20821 2024-05-24 15:04:33.747407 scaleway-2.3.1/scaleway/cockpit/v1/marshalling.py
+-rw-r--r--   0        0        0    20051 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1/types.py
+-rw-r--r--   0        0        0     3758 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1beta1/__init__.py
+-rw-r--r--   0        0        0    33253 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1beta1/api.py
+-rw-r--r--   0        0        0      418 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1beta1/content.py
+-rw-r--r--   0        0        0    21727 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    15330 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/cockpit/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/__init__.py
+-rw-r--r--   0        0        0     5100 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/v1beta1/__init__.py
+-rw-r--r--   0        0        0    63646 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/v1beta1/api.py
+-rw-r--r--   0        0        0     1581 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/v1beta1/content.py
+-rw-r--r--   0        0        0    27167 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    27207 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/container/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/__init__.py
+-rw-r--r--   0        0        0    19280 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/v1/__init__.py
+-rw-r--r--   0        0        0   138198 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/v1/api.py
+-rw-r--r--   0        0        0     2688 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/v1/content.py
+-rw-r--r--   0        0        0    99051 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/v1/marshalling.py
+-rw-r--r--   0        0        0    74459 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/dedibox/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/__init__.py
+-rw-r--r--   0        0        0     9342 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/v1beta1/__init__.py
+-rw-r--r--   0        0        0   103348 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/v1beta1/api.py
+-rw-r--r--   0        0        0     1614 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/v1beta1/content.py
+-rw-r--r--   0        0        0    52204 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    42675 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/document_db/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/__init__.py
+-rw-r--r--   0        0        0    13096 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/v2beta1/__init__.py
+-rw-r--r--   0        0        0    91001 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/v2beta1/api.py
+-rw-r--r--   0        0        0     1948 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/v2beta1/content.py
+-rw-r--r--   0        0        0    90138 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/v2beta1/marshalling.py
+-rw-r--r--   0        0        0    36143 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/domain/v2beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/__init__.py
+-rw-r--r--   0        0        0     1766 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    20562 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/v1alpha1/api.py
+-rw-r--r--   0        0        0      649 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/v1alpha1/content.py
+-rw-r--r--   0        0        0     8075 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8804 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/flexibleip/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/__init__.py
+-rw-r--r--   0        0        0     5594 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/v1beta1/__init__.py
+-rw-r--r--   0        0        0    65595 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/v1beta1/api.py
+-rw-r--r--   0        0        0     1573 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/v1beta1/content.py
+-rw-r--r--   0        0        0    29502 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    28712 2024-05-24 15:04:33.751407 scaleway-2.3.1/scaleway/function/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iam/__init__.py
+-rw-r--r--   0        0        0     5586 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iam/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    84707 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iam/v1alpha1/api.py
+-rw-r--r--   0        0        0    33530 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iam/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    30388 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iam/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/__init__.py
+-rw-r--r--   0        0        0     3020 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/v1beta1/__init__.py
+-rw-r--r--   0        0        0    31589 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/v1beta1/api.py
+-rw-r--r--   0        0        0      443 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/v1beta1/content.py
+-rw-r--r--   0        0        0    17687 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    14467 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/inference/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/__init__.py
+-rw-r--r--   0        0        0    14202 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/__init__.py
+-rw-r--r--   0        0        0   154206 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/api.py
+-rw-r--r--   0        0        0     2388 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/content.py
+-rw-r--r--   0        0        0   117421 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/marshalling.py
+-rw-r--r--   0        0        0    66206 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/types.py
+-rw-r--r--   0        0        0     6858 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/instance/v1/types_private.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/__init__.py
+-rw-r--r--   0        0        0     5818 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/v1/__init__.py
+-rw-r--r--   0        0        0    61882 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/v1/api.py
+-rw-r--r--   0        0        0      363 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/v1/content.py
+-rw-r--r--   0        0        0    33920 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/v1/marshalling.py
+-rw-r--r--   0        0        0    29997 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/iot/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipam/__init__.py
+-rw-r--r--   0        0        0      870 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipam/v1/__init__.py
+-rw-r--r--   0        0        0    15471 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipam/v1/api.py
+-rw-r--r--   0        0        0     6739 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipam/v1/marshalling.py
+-rw-r--r--   0        0        0     6884 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipam/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipfs/__init__.py
+-rw-r--r--   0        0        0     2572 2024-05-24 15:04:33.755407 scaleway-2.3.1/scaleway/ipfs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    33644 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/ipfs/v1alpha1/api.py
+-rw-r--r--   0        0        0      552 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/ipfs/v1alpha1/content.py
+-rw-r--r--   0        0        0    12468 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/ipfs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    11507 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/ipfs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/__init__.py
+-rw-r--r--   0        0        0     1760 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    18523 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/v1alpha1/api.py
+-rw-r--r--   0        0        0      402 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/v1alpha1/content.py
+-rw-r--r--   0        0        0    11319 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     7454 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/jobs/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/__init__.py
+-rw-r--r--   0        0        0     5436 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/v1/__init__.py
+-rw-r--r--   0        0        0    59532 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/v1/api.py
+-rw-r--r--   0        0        0      934 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/v1/content.py
+-rw-r--r--   0        0        0    40014 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/v1/marshalling.py
+-rw-r--r--   0        0        0    44925 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/k8s/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/key_manager/__init__.py
+-rw-r--r--   0        0        0     1658 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/key_manager/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    21783 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/key_manager/v1alpha1/api.py
+-rw-r--r--   0        0        0     9741 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/key_manager/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     9936 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/key_manager/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/__init__.py
+-rw-r--r--   0        0        0    13124 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/v1/__init__.py
+-rw-r--r--   0        0        0   228535 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/v1/api.py
+-rw-r--r--   0        0        0     1107 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/v1/content.py
+-rw-r--r--   0        0        0    82875 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/v1/marshalling.py
+-rw-r--r--   0        0        0    91077 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/lb/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/marketplace/__init__.py
+-rw-r--r--   0        0        0     1470 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/marketplace/v2/__init__.py
+-rw-r--r--   0        0        0    15002 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/marketplace/v2/api.py
+-rw-r--r--   0        0        0     6721 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/marketplace/v2/marshalling.py
+-rw-r--r--   0        0        0     5135 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/marketplace/v2/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/mnq/__init__.py
+-rw-r--r--   0        0        0     3766 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/mnq/v1beta1/__init__.py
+-rw-r--r--   0        0        0    42079 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/mnq/v1beta1/api.py
+-rw-r--r--   0        0        0    18036 2024-05-24 15:04:33.759407 scaleway-2.3.1/scaleway/mnq/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    16867 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/mnq/v1beta1/types.py
+-rw-r--r--   0        0        0        0 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/py.typed
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/__init__.py
+-rw-r--r--   0        0        0     4200 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    42961 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/v1alpha1/api.py
+-rw-r--r--   0        0        0      843 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/v1alpha1/content.py
+-rw-r--r--   0        0        0    18882 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    19382 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/qaas/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/__init__.py
+-rw-r--r--   0        0        0    10624 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/v1/__init__.py
+-rw-r--r--   0        0        0   120098 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/v1/api.py
+-rw-r--r--   0        0        0     1950 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/v1/content.py
+-rw-r--r--   0        0        0    58660 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/v1/marshalling.py
+-rw-r--r--   0        0        0    49240 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/rdb/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/__init__.py
+-rw-r--r--   0        0        0     3760 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/v1/__init__.py
+-rw-r--r--   0        0        0    44498 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/v1/api.py
+-rw-r--r--   0        0        0      488 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/v1/content.py
+-rw-r--r--   0        0        0    21902 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/v1/marshalling.py
+-rw-r--r--   0        0        0    17769 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/redis/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/__init__.py
+-rw-r--r--   0        0        0     1962 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/v1/__init__.py
+-rw-r--r--   0        0        0    29244 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/v1/api.py
+-rw-r--r--   0        0        0      710 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/v1/content.py
+-rw-r--r--   0        0        0     8195 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/v1/marshalling.py
+-rw-r--r--   0        0        0    11276 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/registry/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/__init__.py
+-rw-r--r--   0        0        0     3160 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    51087 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1alpha1/api.py
+-rw-r--r--   0        0        0    15815 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    21526 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1alpha1/types.py
+-rw-r--r--   0        0        0     3050 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1beta1/__init__.py
+-rw-r--r--   0        0        0    36583 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1beta1/api.py
+-rw-r--r--   0        0        0    15383 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1beta1/marshalling.py
+-rw-r--r--   0        0        0    18709 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/secret/v1beta1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/__init__.py
+-rw-r--r--   0        0        0     1528 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    19892 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/api.py
+-rw-r--r--   0        0        0      427 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/content.py
+-rw-r--r--   0        0        0     6440 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0     8013 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/types.py
+-rw-r--r--   0        0        0      194 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/std/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/std/api.py
+-rw-r--r--   0        0        0      129 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/std/marshalling.py
+-rw-r--r--   0        0        0      469 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/std/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/tem/__init__.py
+-rw-r--r--   0        0        0     2646 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/tem/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    26610 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/tem/v1alpha1/api.py
+-rw-r--r--   0        0        0      549 2024-05-24 15:04:33.763407 scaleway-2.3.1/scaleway/tem/v1alpha1/content.py
+-rw-r--r--   0        0        0    18141 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/tem/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    16807 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/tem/v1alpha1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/__init__.py
+-rw-r--r--   0        0        0     1088 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/v1/__init__.py
+-rw-r--r--   0        0        0    11588 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/v1/api.py
+-rw-r--r--   0        0        0      349 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/v1/content.py
+-rw-r--r--   0        0        0     6231 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/v1/marshalling.py
+-rw-r--r--   0        0        0     3231 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/test/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/__init__.py
+-rw-r--r--   0        0        0      818 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v1/__init__.py
+-rw-r--r--   0        0        0    11810 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v1/api.py
+-rw-r--r--   0        0        0     3338 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v1/marshalling.py
+-rw-r--r--   0        0        0     4368 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v1/types.py
+-rw-r--r--   0        0        0     2140 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v2/__init__.py
+-rw-r--r--   0        0        0    35436 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v2/api.py
+-rw-r--r--   0        0        0    11405 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v2/marshalling.py
+-rw-r--r--   0        0        0    12227 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpc/v2/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/__init__.py
+-rw-r--r--   0        0        0     4846 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/v1/__init__.py
+-rw-r--r--   0        0        0    81330 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/v1/api.py
+-rw-r--r--   0        0        0      755 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/v1/content.py
+-rw-r--r--   0        0        0    30617 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/v1/marshalling.py
+-rw-r--r--   0        0        0    35539 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/vpcgw/v1/types.py
+-rw-r--r--   0        0        0      127 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/__init__.py
+-rw-r--r--   0        0        0     2510 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/v1alpha1/__init__.py
+-rw-r--r--   0        0        0    22994 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/v1alpha1/api.py
+-rw-r--r--   0        0        0      421 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/v1alpha1/content.py
+-rw-r--r--   0        0        0    14989 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/v1alpha1/marshalling.py
+-rw-r--r--   0        0        0    14450 2024-05-24 15:04:33.767407 scaleway-2.3.1/scaleway/webhosting/v1alpha1/types.py
+-rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 scaleway-2.3.1/PKG-INFO
```

### Comparing `scaleway-2.2.1/pyproject.toml` & `scaleway-2.3.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scaleway"
-version = "2.2.1"
+version = "2.3.1"
 description = "Scaleway SDK for Python"
 authors = ["Scaleway <opensource@scaleway.com>"]
 license = "BSD"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
@@ -20,15 +20,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-scaleway-core = "2.2.1"
+scaleway-core = "2.3.1"
 
 [tool.poetry.group.dev.dependencies]
 scaleway-core = { path = "../scaleway-core", develop = true }
 ruff = ">=0.0.286,<0.4.3"
 mypy = "^1.5.1"
 
 [build-system]
```

### Comparing `scaleway-2.2.1/scaleway/__init__.py` & `scaleway-2.3.1/scaleway/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v2/__init__.py` & `scaleway-2.3.1/scaleway/account/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v2/api.py` & `scaleway-2.3.1/scaleway/account/v2/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     marshal_CreateProjectRequest,
     marshal_UpdateProjectRequest,
 )
 
 
 class AccountV2API(API):
     """
-    This API allows you to manage projects.
+    This API allows you to manage your Scaleway Projects.
     """
 
     def create_project(
         self,
         *,
         name: Optional[str] = None,
         organization_id: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/account/v2/marshalling.py` & `scaleway-2.3.1/scaleway/account/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v2/types.py` & `scaleway-2.3.1/scaleway/account/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v3/__init__.py` & `scaleway-2.3.1/scaleway/account/v3/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v3/api.py` & `scaleway-2.3.1/scaleway/account/v3/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     marshal_ProjectApiCreateProjectRequest,
     marshal_ProjectApiUpdateProjectRequest,
 )
 
 
 class AccountV3ProjectAPI(API):
     """
-    This API allows you to manage projects.
+    This API allows you to manage your Scaleway Projects.
     """
 
     def create_project(
         self,
         *,
         description: str,
         name: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/account/v3/marshalling.py` & `scaleway-2.3.1/scaleway/account/v3/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/account/v3/types.py` & `scaleway-2.3.1/scaleway/account/v3/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/applesilicon/v1alpha1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 from .types import ListServersRequestOrderBy
 from .types import ServerStatus
 from .content import SERVER_TRANSIENT_STATUSES
 from .types import ServerTypeStock
 from .types import OS
 from .types import ServerTypeCPU
 from .types import ServerTypeDisk
+from .types import ServerTypeGPU
 from .types import ServerTypeMemory
+from .types import ServerTypeNetwork
 from .types import ServerType
 from .types import Server
 from .types import CreateServerRequest
 from .types import DeleteServerRequest
 from .types import GetOSRequest
 from .types import GetServerRequest
 from .types import GetServerTypeRequest
@@ -30,15 +32,17 @@
     "ListServersRequestOrderBy",
     "ServerStatus",
     "SERVER_TRANSIENT_STATUSES",
     "ServerTypeStock",
     "OS",
     "ServerTypeCPU",
     "ServerTypeDisk",
+    "ServerTypeGPU",
     "ServerTypeMemory",
+    "ServerTypeNetwork",
     "ServerType",
     "Server",
     "CreateServerRequest",
     "DeleteServerRequest",
     "GetOSRequest",
     "GetServerRequest",
     "GetServerTypeRequest",
```

### Comparing `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/applesilicon/v1alpha1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,17 @@
     marshal_CreateServerRequest,
     marshal_ReinstallServerRequest,
     marshal_UpdateServerRequest,
 )
 
 
 class ApplesiliconV1Alpha1API(API):
-    """ """
+    """
+    This API allows you to manage your Apple silicon machines.
+    """
 
     def list_server_types(
         self,
         *,
         zone: Optional[Zone] = None,
     ) -> ListServerTypesResponse:
         """
```

### Comparing `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/applesilicon/v1alpha1/marshalling.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from dateutil import parser
 
 from scaleway_core.profile import ProfileDefaults
 from .types import (
     OS,
     ServerTypeCPU,
     ServerTypeDisk,
+    ServerTypeGPU,
     ServerTypeMemory,
+    ServerTypeNetwork,
     ServerType,
     Server,
     ListOSResponse,
     ListServerTypesResponse,
     ListServersResponse,
     CreateServerRequest,
     ReinstallServerRequest,
@@ -80,14 +82,18 @@
     if field is not None:
         args["name"] = field
 
     field = data.get("core_count", None)
     if field is not None:
         args["core_count"] = field
 
+    field = data.get("frequency", None)
+    if field is not None:
+        args["frequency"] = field
+
     return ServerTypeCPU(**args)
 
 
 def unmarshal_ServerTypeDisk(data: Any) -> ServerTypeDisk:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerTypeDisk' failed as data isn't a dictionary."
@@ -102,14 +108,29 @@
     field = data.get("type", None)
     if field is not None:
         args["type_"] = field
 
     return ServerTypeDisk(**args)
 
 
+def unmarshal_ServerTypeGPU(data: Any) -> ServerTypeGPU:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ServerTypeGPU' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("count", None)
+    if field is not None:
+        args["count"] = field
+
+    return ServerTypeGPU(**args)
+
+
 def unmarshal_ServerTypeMemory(data: Any) -> ServerTypeMemory:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerTypeMemory' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -121,14 +142,29 @@
     field = data.get("type", None)
     if field is not None:
         args["type_"] = field
 
     return ServerTypeMemory(**args)
 
 
+def unmarshal_ServerTypeNetwork(data: Any) -> ServerTypeNetwork:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ServerTypeNetwork' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("public_bandwidth_bps", None)
+    if field is not None:
+        args["public_bandwidth_bps"] = field
+
+    return ServerTypeNetwork(**args)
+
+
 def unmarshal_ServerType(data: Any) -> ServerType:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ServerType' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -161,14 +197,26 @@
 
     field = data.get("minimum_lease_duration", None)
     if field is not None:
         args["minimum_lease_duration"] = field
     else:
         args["minimum_lease_duration"] = None
 
+    field = data.get("gpu", None)
+    if field is not None:
+        args["gpu"] = unmarshal_ServerTypeGPU(field)
+    else:
+        args["gpu"] = None
+
+    field = data.get("network", None)
+    if field is not None:
+        args["network"] = unmarshal_ServerTypeNetwork(field)
+    else:
+        args["network"] = None
+
     field = data.get("default_os", None)
     if field is not None:
         args["default_os"] = unmarshal_OS(field)
     else:
         args["default_os"] = None
 
     return ServerType(**args)
```

### Comparing `scaleway-2.2.1/scaleway/applesilicon/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/applesilicon/v1alpha1/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,30 +99,42 @@
 
 @dataclass
 class ServerTypeCPU:
     name: str
 
     core_count: int
 
+    frequency: int
+
 
 @dataclass
 class ServerTypeDisk:
     capacity: int
 
     type_: str
 
 
 @dataclass
+class ServerTypeGPU:
+    count: int
+
+
+@dataclass
 class ServerTypeMemory:
     capacity: int
 
     type_: str
 
 
 @dataclass
+class ServerTypeNetwork:
+    public_bandwidth_bps: int
+
+
+@dataclass
 class ServerType:
     name: str
     """
     Name of the type.
     """
 
     stock: ServerTypeStock
@@ -146,14 +158,24 @@
     """
 
     minimum_lease_duration: Optional[str]
     """
     Minimum duration of the lease in seconds (example. 3.4s).
     """
 
+    gpu: Optional[ServerTypeGPU]
+    """
+    GPU description.
+    """
+
+    network: Optional[ServerTypeNetwork]
+    """
+    Network description.
+    """
+
     default_os: Optional[OS]
     """
     The default OS for this server type.
     """
 
 
 @dataclass
```

### Comparing `scaleway-2.2.1/scaleway/baremetal/v1/__init__.py` & `scaleway-2.3.1/scaleway/baremetal/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/baremetal/v1/api.py` & `scaleway-2.3.1/scaleway/baremetal/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     marshal_UpdateServerRequest,
     marshal_UpdateSettingRequest,
 )
 
 
 class BaremetalV1API(API):
     """
-    This API allows to manage your Elastic Metal server.
+    This API allows you to manage your Elastic Metal servers.
     """
 
     def list_servers(
         self,
         *,
         zone: Optional[Zone] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/baremetal/v1/content.py` & `scaleway-2.3.1/scaleway/baremetal/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/baremetal/v1/marshalling.py` & `scaleway-2.3.1/scaleway/baremetal/v1/marshalling.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,14 +368,18 @@
     if field is not None:
         args["stock"] = field
 
     field = data.get("bandwidth", None)
     if field is not None:
         args["bandwidth"] = field
 
+    field = data.get("max_bandwidth", None)
+    if field is not None:
+        args["max_bandwidth"] = field
+
     field = data.get("commercial_range", None)
     if field is not None:
         args["commercial_range"] = field
 
     field = data.get("disks", None)
     if field is not None:
         args["disks"] = (
```

### Comparing `scaleway-2.2.1/scaleway/baremetal/v1/types.py` & `scaleway-2.3.1/scaleway/baremetal/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -533,14 +533,19 @@
     """
 
     bandwidth: int
     """
     Public bandwidth available (in bits/s) with the offer.
     """
 
+    max_bandwidth: int
+    """
+    Maximum public bandwidth available (in bits/s) depending on available options.
+    """
+
     commercial_range: str
     """
     Commercial range of the offer.
     """
 
     disks: List[Disk]
     """
```

### Comparing `scaleway-2.2.1/scaleway/billing/v2alpha1/__init__.py` & `scaleway-2.3.1/scaleway/billing/v2alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/billing/v2alpha1/api.py` & `scaleway-2.3.1/scaleway/billing/v2alpha1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     unmarshal_ListDiscountsResponse,
     unmarshal_ListInvoicesResponse,
 )
 
 
 class BillingV2Alpha1API(API):
     """
-    This API allows you to query your consumption.
+    This API allows you to manage and query your Scaleway billing and consumption.
     """
 
     def get_consumption(
         self,
         *,
         organization_id: Optional[str] = None,
     ) -> GetConsumptionResponse:
```

### Comparing `scaleway-2.2.1/scaleway/billing/v2alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/billing/v2alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/billing/v2alpha1/types.py` & `scaleway-2.3.1/scaleway/billing/v2alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/billing/v2beta1/__init__.py` & `scaleway-2.3.1/scaleway/billing/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/billing/v2beta1/api.py` & `scaleway-2.3.1/scaleway/billing/v2beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     unmarshal_ListInvoicesResponse,
     unmarshal_ListTaxesResponse,
 )
 
 
 class BillingV2Beta1API(API):
     """
-    This API allows you to query your consumption.
+    This API allows you to manage and query your Scaleway billing and consumption.
     """
 
     def list_consumptions(
         self,
         *,
         order_by: Optional[ListConsumptionsRequestOrderBy] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/billing/v2beta1/marshalling.py` & `scaleway-2.3.1/scaleway/billing/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/billing/v2beta1/types.py` & `scaleway-2.3.1/scaleway/billing/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/block/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/block/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/block/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/block/v1alpha1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     marshal_UpdateSnapshotRequest,
     marshal_UpdateVolumeRequest,
 )
 
 
 class BlockV1Alpha1API(API):
     """
-    This API allows you to use and manage your Block Storage volumes.
+    This API allows you to manage your Block Storage volumes.
     """
 
     def list_volume_types(
         self,
         *,
         zone: Optional[Zone] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/block/v1alpha1/content.py` & `scaleway-2.3.1/scaleway/block/v1alpha1/content.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,11 +24,12 @@
 Lists transient statutes of the enum :class:`SnapshotStatus <SnapshotStatus>`.
 """
 VOLUME_TRANSIENT_STATUSES: List[VolumeStatus] = [
     VolumeStatus.CREATING,
     VolumeStatus.DELETING,
     VolumeStatus.RESIZING,
     VolumeStatus.SNAPSHOTTING,
+    VolumeStatus.UPDATING,
 ]
 """
 Lists transient statutes of the enum :class:`VolumeStatus <VolumeStatus>`.
 """
```

### Comparing `scaleway-2.2.1/scaleway/block/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/block/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/block/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/block/v1alpha1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     IN_USE = "in_use"
     DELETING = "deleting"
     DELETED = "deleted"
     RESIZING = "resizing"
     ERROR = "error"
     SNAPSHOTTING = "snapshotting"
     LOCKED = "locked"
+    UPDATING = "updating"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
 @dataclass
 class Reference:
```

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1/__init__.py` & `scaleway-2.3.1/scaleway/cockpit/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1/api.py` & `scaleway-2.3.1/scaleway/cockpit/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1/marshalling.py` & `scaleway-2.3.1/scaleway/cockpit/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1/types.py` & `scaleway-2.3.1/scaleway/cockpit/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/cockpit/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1beta1/api.py` & `scaleway-2.3.1/scaleway/cockpit/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     marshal_SelectPlanRequest,
     marshal_TriggerTestAlertRequest,
 )
 
 
 class CockpitV1Beta1API(API):
     """
-    The Cockpit API allows you to activate your Cockpit to store metrics and logs. It also provides you with a dedicated Grafana for dashboarding to visualize your metrics and logs.
+    This API allows you to manage your Scaleway Cockpit, for storing and visualizing metrics and logs.
     """
 
     def activate_cockpit(
         self,
         *,
         project_id: Optional[str] = None,
     ) -> Cockpit:
```

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/cockpit/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/cockpit/v1beta1/types.py` & `scaleway-2.3.1/scaleway/cockpit/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/container/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/container/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/container/v1beta1/api.py` & `scaleway-2.3.1/scaleway/container/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     marshal_UpdateNamespaceRequest,
     marshal_UpdateTriggerRequest,
 )
 
 
 class ContainerV1Beta1API(API):
     """
-    Serverless Containers API.
+    This API allows you to manage your Serverless Containers.
     """
 
     def list_namespaces(
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/container/v1beta1/content.py` & `scaleway-2.3.1/scaleway/container/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/container/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/container/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/container/v1beta1/types.py` & `scaleway-2.3.1/scaleway/container/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/dedibox/v1/__init__.py` & `scaleway-2.3.1/scaleway/dedibox/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/dedibox/v1/api.py` & `scaleway-2.3.1/scaleway/dedibox/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/dedibox/v1/content.py` & `scaleway-2.3.1/scaleway/dedibox/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/dedibox/v1/marshalling.py` & `scaleway-2.3.1/scaleway/dedibox/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/dedibox/v1/types.py` & `scaleway-2.3.1/scaleway/dedibox/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/document_db/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/document_db/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/document_db/v1beta1/api.py` & `scaleway-2.3.1/scaleway/document_db/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,17 @@
     marshal_UpdateSnapshotRequest,
     marshal_UpdateUserRequest,
     marshal_UpgradeInstanceRequest,
 )
 
 
 class DocumentDbV1Beta1API(API):
-    """ """
+    """
+    This API allows you to manage your Document Databases.
+    """
 
     def list_database_engines(
         self,
         *,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         version: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/document_db/v1beta1/content.py` & `scaleway-2.3.1/scaleway/document_db/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/document_db/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/document_db/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/document_db/v1beta1/types.py` & `scaleway-2.3.1/scaleway/document_db/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/domain/v2beta1/__init__.py` & `scaleway-2.3.1/scaleway/domain/v2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/domain/v2beta1/api.py` & `scaleway-2.3.1/scaleway/domain/v2beta1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
 from ...std.types import (
     LanguageCode as StdLanguageCode,
 )
 
 
 class DomainV2Beta1API(API):
     """
-    Manage your domains, DNS zones and records with the Domains and DNS API.
+    This API allows you to manage your domains, DNS zones and records.
     """
 
     def list_dns_zones(
         self,
         *,
         domain: str,
         organization_id: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/domain/v2beta1/content.py` & `scaleway-2.3.1/scaleway/domain/v2beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/domain/v2beta1/marshalling.py` & `scaleway-2.3.1/scaleway/domain/v2beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/domain/v2beta1/types.py` & `scaleway-2.3.1/scaleway/domain/v2beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/flexibleip/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/flexibleip/v1alpha1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     marshal_MoveMACAddrRequest,
     marshal_UpdateFlexibleIPRequest,
 )
 
 
 class FlexibleipV1Alpha1API(API):
     """
-    Elastic Metal - Flexible IP API.
+    This API allows you to manage your Elastic Metal servers' flexible public IP addresses.
     """
 
     def create_flexible_ip(
         self,
         *,
         description: str,
         is_ipv6: bool,
```

### Comparing `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/content.py` & `scaleway-2.3.1/scaleway/flexibleip/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/flexibleip/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/flexibleip/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/flexibleip/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/function/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/function/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/function/v1beta1/api.py` & `scaleway-2.3.1/scaleway/function/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,17 @@
     marshal_UpdateFunctionRequest,
     marshal_UpdateNamespaceRequest,
     marshal_UpdateTriggerRequest,
 )
 
 
 class FunctionV1Beta1API(API):
-    """ """
+    """
+    This API allows you to manage your Serverless Functions.
+    """
 
     def list_namespaces(
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/function/v1beta1/content.py` & `scaleway-2.3.1/scaleway/function/v1beta1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/function/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/function/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/function/v1beta1/types.py` & `scaleway-2.3.1/scaleway/function/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iam/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/iam/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iam/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/iam/v1alpha1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     marshal_UpdateSSHKeyRequest,
     marshal_UpdateUserRequest,
 )
 
 
 class IamV1Alpha1API(API):
     """
-    IAM API.
+    This API allows you to manage Identity and Access Management (IAM) across your Scaleway Organizations, Projects and resources.
     """
 
     def list_ssh_keys(
         self,
         *,
         order_by: Optional[ListSSHKeysRequestOrderBy] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/iam/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/iam/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iam/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/iam/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/instance/v1/__init__.py` & `scaleway-2.3.1/scaleway/instance/v1/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,15 @@
 from .types import CreateSecurityGroupRuleResponse
 from .types import CreateServerRequest
 from .types import CreateServerResponse
 from .types import CreateSnapshotRequest
 from .types import CreateSnapshotResponse
 from .types import CreateVolumeRequest
 from .types import CreateVolumeResponse
+from .types import DeleteEncryptedRdpPasswordRequest
 from .types import DeleteImageRequest
 from .types import DeleteIpRequest
 from .types import DeletePlacementGroupRequest
 from .types import DeletePrivateNICRequest
 from .types import DeleteSecurityGroupRequest
 from .types import DeleteSecurityGroupRuleRequest
 from .types import DeleteServerRequest
@@ -111,14 +112,16 @@
 from .types import DetachServerVolumeResponse
 from .types import ExportSnapshotRequest
 from .types import ExportSnapshotResponse
 from .types import GetBootscriptRequest
 from .types import GetBootscriptResponse
 from .types import GetDashboardRequest
 from .types import GetDashboardResponse
+from .types import GetEncryptedRdpPasswordRequest
+from .types import GetEncryptedRdpPasswordResponse
 from .types import GetImageRequest
 from .types import GetImageResponse
 from .types import GetIpRequest
 from .types import GetIpResponse
 from .types import GetPlacementGroupRequest
 from .types import GetPlacementGroupResponse
 from .types import GetPlacementGroupServersRequest
@@ -292,14 +295,15 @@
     "CreateSecurityGroupRuleResponse",
     "CreateServerRequest",
     "CreateServerResponse",
     "CreateSnapshotRequest",
     "CreateSnapshotResponse",
     "CreateVolumeRequest",
     "CreateVolumeResponse",
+    "DeleteEncryptedRdpPasswordRequest",
     "DeleteImageRequest",
     "DeleteIpRequest",
     "DeletePlacementGroupRequest",
     "DeletePrivateNICRequest",
     "DeleteSecurityGroupRequest",
     "DeleteSecurityGroupRuleRequest",
     "DeleteServerRequest",
@@ -310,14 +314,16 @@
     "DetachServerVolumeResponse",
     "ExportSnapshotRequest",
     "ExportSnapshotResponse",
     "GetBootscriptRequest",
     "GetBootscriptResponse",
     "GetDashboardRequest",
     "GetDashboardResponse",
+    "GetEncryptedRdpPasswordRequest",
+    "GetEncryptedRdpPasswordResponse",
     "GetImageRequest",
     "GetImageResponse",
     "GetIpRequest",
     "GetIpResponse",
     "GetPlacementGroupRequest",
     "GetPlacementGroupResponse",
     "GetPlacementGroupServersRequest",
```

### Comparing `scaleway-2.2.1/scaleway/instance/v1/api.py` & `scaleway-2.3.1/scaleway/instance/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     CreateVolumeResponse,
     DetachServerVolumeRequest,
     DetachServerVolumeResponse,
     ExportSnapshotRequest,
     ExportSnapshotResponse,
     GetBootscriptResponse,
     GetDashboardResponse,
+    GetEncryptedRdpPasswordResponse,
     GetImageResponse,
     GetIpResponse,
     GetPlacementGroupResponse,
     GetPlacementGroupServersResponse,
     GetPrivateNICResponse,
     GetSecurityGroupResponse,
     GetSecurityGroupRuleResponse,
@@ -161,14 +162,15 @@
     unmarshal_CreateServerResponse,
     unmarshal_CreateSnapshotResponse,
     unmarshal_CreateVolumeResponse,
     unmarshal_DetachServerVolumeResponse,
     unmarshal_ExportSnapshotResponse,
     unmarshal_GetBootscriptResponse,
     unmarshal_GetDashboardResponse,
+    unmarshal_GetEncryptedRdpPasswordResponse,
     unmarshal_GetImageResponse,
     unmarshal_GetIpResponse,
     unmarshal_GetPlacementGroupResponse,
     unmarshal_GetPlacementGroupServersResponse,
     unmarshal_GetPrivateNICResponse,
     unmarshal_GetSecurityGroupResponse,
     unmarshal_GetSecurityGroupRuleResponse,
@@ -243,15 +245,15 @@
     marshal__SetServerRequest,
     marshal__SetSnapshotRequest,
 )
 
 
 class InstanceV1API(API):
     """
-    Instance API.
+    This API allows you to manage your Instances.
     """
 
     def get_server_types_availability(
         self,
         *,
         zone: Optional[Zone] = None,
         per_page: Optional[int] = None,
@@ -524,14 +526,15 @@
         boot_type: Optional[BootType] = None,
         bootscript: Optional[str] = None,
         organization: Optional[str] = None,
         project: Optional[str] = None,
         tags: Optional[List[str]] = None,
         security_group: Optional[str] = None,
         placement_group: Optional[str] = None,
+        admin_password_encryption_ssh_key_id: Optional[str] = None,
     ) -> CreateServerResponse:
         """
         Create an Instance.
         Create a new Instance of the specified commercial type in the specified zone. Pay attention to the volumes parameter, which takes an object which can be used in different ways to achieve different behaviors.
         Get more information in the [Technical Information](#technical-information) section of the introduction.
         :param commercial_type: Define the Instance commercial type (i.e. GP1-S).
         :param image: Instance image ID or label.
@@ -548,14 +551,15 @@
         :param organization: Instance Organization ID.
         One-Of ('project_identifier'): at most one of 'project', 'organization' could be set.
         :param project: Instance Project ID.
         One-Of ('project_identifier'): at most one of 'project', 'organization' could be set.
         :param tags: Instance tags.
         :param security_group: Security group ID.
         :param placement_group: Placement group ID if Instance must be part of a placement group.
+        :param admin_password_encryption_ssh_key_id: UUID of the SSH RSA key that will be used to encrypt the initial admin password for OS requiring it. Mandatory for Windows OS.
         :return: :class:`CreateServerResponse <CreateServerResponse>`
 
         Usage:
         ::
 
             result = api._create_server(
                 commercial_type="example",
@@ -581,14 +585,15 @@
                     public_ip=public_ip,
                     public_ips=public_ips,
                     boot_type=boot_type,
                     bootscript=bootscript,
                     tags=tags,
                     security_group=security_group,
                     placement_group=placement_group,
+                    admin_password_encryption_ssh_key_id=admin_password_encryption_ssh_key_id,
                     project=project,
                     organization=organization,
                 ),
                 self.client,
             ),
         )
 
@@ -4165,7 +4170,69 @@
                     snapshot_id=snapshot_id,
                 ),
                 self.client,
             ),
         )
 
         self._throw_on_error(res)
+
+    def get_encrypted_rdp_password(
+        self,
+        *,
+        server_id: str,
+        zone: Optional[Zone] = None,
+    ) -> GetEncryptedRdpPasswordResponse:
+        """
+        Get the encrypted RDP password.
+        Get the initial administrator password for Windows RDP. This password is encrypted using the SSH RSA key specified at the time of Instance creation.
+        :param server_id: UUID of the Instance.
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+        :return: :class:`GetEncryptedRdpPasswordResponse <GetEncryptedRdpPasswordResponse>`
+
+        Usage:
+        ::
+
+            result = api.get_encrypted_rdp_password(
+                server_id="example",
+            )
+        """
+
+        param_zone = validate_path_param("zone", zone or self.client.default_zone)
+        param_server_id = validate_path_param("server_id", server_id)
+
+        res = self._request(
+            "GET",
+            f"/instance/v1/zones/{param_zone}/servers/{param_server_id}/encrypted_rdp_password",
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_GetEncryptedRdpPasswordResponse(res.json())
+
+    def delete_encrypted_rdp_password(
+        self,
+        *,
+        server_id: str,
+        zone: Optional[Zone] = None,
+    ) -> None:
+        """
+        Delete the encrypted RDP password.
+        Delete the initial administrator password for Windows RDP.
+        :param server_id: UUID of the Instance.
+        :param zone: Zone to target. If none is passed will use default zone from the config.
+
+        Usage:
+        ::
+
+            result = api.delete_encrypted_rdp_password(
+                server_id="example",
+            )
+        """
+
+        param_zone = validate_path_param("zone", zone or self.client.default_zone)
+        param_server_id = validate_path_param("server_id", server_id)
+
+        res = self._request(
+            "DELETE",
+            f"/instance/v1/zones/{param_zone}/servers/{param_server_id}/encrypted_rdp_password",
+        )
+
+        self._throw_on_error(res)
```

### Comparing `scaleway-2.2.1/scaleway/instance/v1/content.py` & `scaleway-2.3.1/scaleway/instance/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/instance/v1/marshalling.py` & `scaleway-2.3.1/scaleway/instance/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     CreateSnapshotResponse,
     CreateVolumeResponse,
     DetachServerVolumeResponse,
     ExportSnapshotResponse,
     GetBootscriptResponse,
     Dashboard,
     GetDashboardResponse,
+    GetEncryptedRdpPasswordResponse,
     GetImageResponse,
     GetIpResponse,
     GetPlacementGroupResponse,
     PlacementGroupServer,
     GetPlacementGroupServersResponse,
     GetPrivateNICResponse,
     GetSecurityGroupResponse,
@@ -1561,14 +1562,45 @@
         args["dashboard"] = unmarshal_Dashboard(field)
     else:
         args["dashboard"] = None
 
     return GetDashboardResponse(**args)
 
 
+def unmarshal_GetEncryptedRdpPasswordResponse(
+    data: Any,
+) -> GetEncryptedRdpPasswordResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'GetEncryptedRdpPasswordResponse' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("value", None)
+    if field is not None:
+        args["value"] = field
+    else:
+        args["value"] = None
+
+    field = data.get("admin_password_encryption_ssh_key_description", None)
+    if field is not None:
+        args["admin_password_encryption_ssh_key_description"] = field
+    else:
+        args["admin_password_encryption_ssh_key_description"] = None
+
+    field = data.get("admin_password_encryption_ssh_key_id", None)
+    if field is not None:
+        args["admin_password_encryption_ssh_key_id"] = field
+    else:
+        args["admin_password_encryption_ssh_key_id"] = None
+
+    return GetEncryptedRdpPasswordResponse(**args)
+
+
 def unmarshal_GetImageResponse(data: Any) -> GetImageResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'GetImageResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -3085,14 +3117,19 @@
 
     if request.security_group is not None:
         output["security_group"] = request.security_group
 
     if request.placement_group is not None:
         output["placement_group"] = request.placement_group
 
+    if request.admin_password_encryption_ssh_key_id is not None:
+        output["admin_password_encryption_ssh_key_id"] = (
+            request.admin_password_encryption_ssh_key_id
+        )
+
     return output
 
 
 def marshal_CreateSnapshotRequest(
     request: CreateSnapshotRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
```

### Comparing `scaleway-2.2.1/scaleway/instance/v1/types.py` & `scaleway-2.3.1/scaleway/instance/v1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1854,14 +1854,19 @@
     """
 
     placement_group: Optional[str]
     """
     Placement group ID if Instance must be part of a placement group.
     """
 
+    admin_password_encryption_ssh_key_id: Optional[str]
+    """
+    UUID of the SSH RSA key that will be used to encrypt the initial admin password for OS requiring it. Mandatory for Windows OS.
+    """
+
     project: Optional[str]
 
     organization: Optional[str]
 
 
 @dataclass
 class CreateServerResponse:
@@ -1956,14 +1961,27 @@
 
 @dataclass
 class CreateVolumeResponse:
     volume: Optional[Volume]
 
 
 @dataclass
+class DeleteEncryptedRdpPasswordRequest:
+    server_id: str
+    """
+    UUID of the Instance.
+    """
+
+    zone: Optional[Zone]
+    """
+    Zone to target. If none is passed will use default zone from the config.
+    """
+
+
+@dataclass
 class DeleteImageRequest:
     image_id: str
     """
     UUID of the image you want to delete.
     """
 
     zone: Optional[Zone]
@@ -2169,14 +2187,45 @@
 
 @dataclass
 class GetDashboardResponse:
     dashboard: Optional[Dashboard]
 
 
 @dataclass
+class GetEncryptedRdpPasswordRequest:
+    server_id: str
+    """
+    UUID of the Instance.
+    """
+
+    zone: Optional[Zone]
+    """
+    Zone to target. If none is passed will use default zone from the config.
+    """
+
+
+@dataclass
+class GetEncryptedRdpPasswordResponse:
+    value: Optional[str]
+    """
+    The encrypted RDP password.
+    """
+
+    admin_password_encryption_ssh_key_description: Optional[str]
+    """
+    The description of the SSH key used for ciphering.
+    """
+
+    admin_password_encryption_ssh_key_id: Optional[str]
+    """
+    The UUID of the SSH key used for ciphering.
+    """
+
+
+@dataclass
 class GetImageRequest:
     image_id: str
     """
     UUID of the image you want to get.
     """
 
     zone: Optional[Zone]
```

### Comparing `scaleway-2.2.1/scaleway/instance/v1/types_private.py` & `scaleway-2.3.1/scaleway/instance/v1/types_private.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iot/v1/__init__.py` & `scaleway-2.3.1/scaleway/iot/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iot/v1/api.py` & `scaleway-2.3.1/scaleway/iot/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     marshal_UpdateHubRequest,
     marshal_UpdateRouteRequest,
 )
 
 
 class IotV1API(API):
     """
-    This API allows you to manage IoT hubs and devices.
+    This API allows you to manage your IoT hubs and devices.
     """
 
     def list_hubs(
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/iot/v1/marshalling.py` & `scaleway-2.3.1/scaleway/iot/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/iot/v1/types.py` & `scaleway-2.3.1/scaleway/iot/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/ipam/v1/__init__.py` & `scaleway-2.3.1/scaleway/ipam/v1/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .types import Source
 from .types import IP
 from .types import BookIPRequest
 from .types import GetIPRequest
 from .types import ListIPsRequest
 from .types import ListIPsResponse
 from .types import ReleaseIPRequest
+from .types import ReleaseIPSetRequest
 from .types import UpdateIPRequest
 from .api import IpamV1API
 
 __all__ = [
     "ListIPsRequestOrderBy",
     "ResourceType",
     "Resource",
@@ -22,10 +23,11 @@
     "Source",
     "IP",
     "BookIPRequest",
     "GetIPRequest",
     "ListIPsRequest",
     "ListIPsResponse",
     "ReleaseIPRequest",
+    "ReleaseIPSetRequest",
     "UpdateIPRequest",
     "IpamV1API",
 ]
```

### Comparing `scaleway-2.2.1/scaleway/ipam/v1/api.py` & `scaleway-2.3.1/scaleway/ipam/v1/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,29 +15,31 @@
 )
 from .types import (
     ListIPsRequestOrderBy,
     ResourceType,
     BookIPRequest,
     IP,
     ListIPsResponse,
+    ReleaseIPSetRequest,
     Reverse,
     Source,
     UpdateIPRequest,
 )
 from .marshalling import (
     unmarshal_IP,
     unmarshal_ListIPsResponse,
     marshal_BookIPRequest,
+    marshal_ReleaseIPSetRequest,
     marshal_UpdateIPRequest,
 )
 
 
 class IpamV1API(API):
     """
-    This API allows you to manage IP addresses with Scaleway's IP Address Management tool.
+    This API allows you to manage your Scaleway IP addresses with our IP Address Management tool.
     """
 
     def book_ip(
         self,
         *,
         source: Source,
         is_ipv6: bool,
@@ -118,14 +120,48 @@
             "DELETE",
             f"/ipam/v1/regions/{param_region}/ips/{param_ip_id}",
             body={},
         )
 
         self._throw_on_error(res)
 
+    def release_ip_set(
+        self,
+        *,
+        region: Optional[Region] = None,
+        ip_ids: Optional[List[str]] = None,
+    ) -> None:
+        """
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param ip_ids:
+
+        Usage:
+        ::
+
+            result = api.release_ip_set()
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+
+        res = self._request(
+            "POST",
+            f"/ipam/v1/regions/{param_region}/ip-sets/release",
+            body=marshal_ReleaseIPSetRequest(
+                ReleaseIPSetRequest(
+                    region=region,
+                    ip_ids=ip_ids,
+                ),
+                self.client,
+            ),
+        )
+
+        self._throw_on_error(res)
+
     def get_ip(
         self,
         *,
         ip_id: str,
         region: Optional[Region] = None,
     ) -> IP:
         """
@@ -209,14 +245,16 @@
         region: Optional[Region] = None,
         order_by: Optional[ListIPsRequestOrderBy] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
         zonal: Optional[str] = None,
         private_network_id: Optional[str] = None,
+        subnet_id: Optional[str] = None,
+        vpc_id: Optional[str] = None,
         attached: Optional[bool] = None,
         resource_id: Optional[str] = None,
         resource_type: Optional[ResourceType] = None,
         mac_address: Optional[str] = None,
         tags: Optional[List[str]] = None,
         organization_id: Optional[str] = None,
         is_ipv6: Optional[bool] = None,
@@ -227,17 +265,20 @@
         List existing IPs in the specified region using various filters. For example, you can filter for IPs within a specified Private Network, or for public IPs within a specified Project. By default, the IPs returned in the list are ordered by creation date in ascending order, though this can be modified via the order_by field.
         :param region: Region to target. If none is passed will use default region from the config.
         :param order_by: Sort order of the returned IPs.
         :param page: Page number to return, from the paginated results.
         :param page_size: Maximum number of IPs to return per page.
         :param project_id: Project ID to filter for. Only IPs belonging to this Project will be returned.
         :param zonal: Zone to filter for. Only IPs that are zonal, and in this zone, will be returned.
-        One-Of ('source'): at most one of 'zonal', 'private_network_id' could be set.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
         :param private_network_id: Only IPs that are private, and in this Private Network, will be returned.
-        One-Of ('source'): at most one of 'zonal', 'private_network_id' could be set.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
+        :param subnet_id: Only IPs inside this exact subnet will be returned.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
+        :param vpc_id: Only IPs owned by resources in this VPC will be returned.
         :param attached: Defines whether to filter only for IPs which are attached to a resource.
         :param resource_id: Resource ID to filter for. Only IPs attached to this resource will be returned.
         :param resource_type: Resource type to filter for. Only IPs attached to this type of resource will be returned.
         :param mac_address: MAC address to filter for. Only IPs attached to a resource with this MAC address will be returned.
         :param tags: Tags to filter for, only IPs with one or more matching tags will be returned.
         :param organization_id: Organization ID to filter for. Only IPs belonging to this Organization will be returned.
         :param is_ipv6: Defines whether to filter only for IPv4s or IPv6s.
@@ -267,17 +308,19 @@
                 "page": page,
                 "page_size": page_size or self.client.default_page_size,
                 "project_id": project_id or self.client.default_project_id,
                 "resource_id": resource_id,
                 "resource_name": resource_name,
                 "resource_type": resource_type,
                 "tags": tags,
+                "vpc_id": vpc_id,
                 **resolve_one_of(
                     [
                         OneOfPossibility("private_network_id", private_network_id),
+                        OneOfPossibility("subnet_id", subnet_id),
                         OneOfPossibility("zonal", zonal),
                     ]
                 ),
             },
         )
 
         self._throw_on_error(res)
@@ -289,14 +332,16 @@
         region: Optional[Region] = None,
         order_by: Optional[ListIPsRequestOrderBy] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
         zonal: Optional[str] = None,
         private_network_id: Optional[str] = None,
+        subnet_id: Optional[str] = None,
+        vpc_id: Optional[str] = None,
         attached: Optional[bool] = None,
         resource_id: Optional[str] = None,
         resource_type: Optional[ResourceType] = None,
         mac_address: Optional[str] = None,
         tags: Optional[List[str]] = None,
         organization_id: Optional[str] = None,
         is_ipv6: Optional[bool] = None,
@@ -307,17 +352,20 @@
         List existing IPs in the specified region using various filters. For example, you can filter for IPs within a specified Private Network, or for public IPs within a specified Project. By default, the IPs returned in the list are ordered by creation date in ascending order, though this can be modified via the order_by field.
         :param region: Region to target. If none is passed will use default region from the config.
         :param order_by: Sort order of the returned IPs.
         :param page: Page number to return, from the paginated results.
         :param page_size: Maximum number of IPs to return per page.
         :param project_id: Project ID to filter for. Only IPs belonging to this Project will be returned.
         :param zonal: Zone to filter for. Only IPs that are zonal, and in this zone, will be returned.
-        One-Of ('source'): at most one of 'zonal', 'private_network_id' could be set.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
         :param private_network_id: Only IPs that are private, and in this Private Network, will be returned.
-        One-Of ('source'): at most one of 'zonal', 'private_network_id' could be set.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
+        :param subnet_id: Only IPs inside this exact subnet will be returned.
+        One-Of ('source'): at most one of 'zonal', 'private_network_id', 'subnet_id' could be set.
+        :param vpc_id: Only IPs owned by resources in this VPC will be returned.
         :param attached: Defines whether to filter only for IPs which are attached to a resource.
         :param resource_id: Resource ID to filter for. Only IPs attached to this resource will be returned.
         :param resource_type: Resource type to filter for. Only IPs attached to this type of resource will be returned.
         :param mac_address: MAC address to filter for. Only IPs attached to a resource with this MAC address will be returned.
         :param tags: Tags to filter for, only IPs with one or more matching tags will be returned.
         :param organization_id: Organization ID to filter for. Only IPs belonging to this Organization will be returned.
         :param is_ipv6: Defines whether to filter only for IPv4s or IPv6s.
@@ -336,19 +384,21 @@
             fetcher=self.list_i_ps,
             args={
                 "region": region,
                 "order_by": order_by,
                 "page": page,
                 "page_size": page_size,
                 "project_id": project_id,
+                "vpc_id": vpc_id,
                 "attached": attached,
                 "resource_id": resource_id,
                 "resource_type": resource_type,
                 "mac_address": mac_address,
                 "tags": tags,
                 "organization_id": organization_id,
                 "is_ipv6": is_ipv6,
                 "resource_name": resource_name,
                 "zonal": zonal,
                 "private_network_id": private_network_id,
+                "subnet_id": subnet_id,
             },
         )
```

### Comparing `scaleway-2.2.1/scaleway/ipam/v1/marshalling.py` & `scaleway-2.3.1/scaleway/ipam/v1/marshalling.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .types import (
     Resource,
     Reverse,
     Source,
     IP,
     ListIPsResponse,
     BookIPRequest,
+    ReleaseIPSetRequest,
     UpdateIPRequest,
 )
 
 
 def unmarshal_Resource(data: Any) -> Resource:
     if not isinstance(data, dict):
         raise TypeError(
@@ -210,15 +211,15 @@
 def marshal_BookIPRequest(
     request: BookIPRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.source is not None:
-        output["source"] = (marshal_Source(request.source, defaults),)
+        output["source"] = marshal_Source(request.source, defaults)
 
     if request.is_ipv6 is not None:
         output["is_ipv6"] = request.is_ipv6
 
     if request.project_id is not None:
         output["project_id"] = request.project_id or defaults.default_project_id
 
@@ -227,14 +228,26 @@
 
     if request.tags is not None:
         output["tags"] = request.tags
 
     return output
 
 
+def marshal_ReleaseIPSetRequest(
+    request: ReleaseIPSetRequest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+
+    if request.ip_ids is not None:
+        output["ip_ids"] = request.ip_ids
+
+    return output
+
+
 def marshal_Reverse(
     request: Reverse,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
 
     if request.hostname is not None:
```

### Comparing `scaleway-2.2.1/scaleway/ipam/v1/types.py` & `scaleway-2.3.1/scaleway/ipam/v1/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,14 +226,19 @@
     """
 
     project_id: Optional[str]
     """
     Project ID to filter for. Only IPs belonging to this Project will be returned.
     """
 
+    vpc_id: Optional[str]
+    """
+    Only IPs owned by resources in this VPC will be returned.
+    """
+
     attached: Optional[bool]
     """
     Defines whether to filter only for IPs which are attached to a resource.
     """
 
     resource_id: Optional[str]
     """
@@ -270,14 +275,16 @@
     Attached resource name to filter for, only IPs attached to a resource with this string within their name will be returned.
     """
 
     zonal: Optional[str]
 
     private_network_id: Optional[str]
 
+    subnet_id: Optional[str]
+
 
 @dataclass
 class ListIPsResponse:
     total_count: int
 
     ips: List[IP]
 
@@ -292,14 +299,24 @@
     region: Optional[Region]
     """
     Region to target. If none is passed will use default region from the config.
     """
 
 
 @dataclass
+class ReleaseIPSetRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    ip_ids: Optional[List[str]]
+
+
+@dataclass
 class UpdateIPRequest:
     ip_id: str
     """
     IP ID.
     """
 
     region: Optional[Region]
```

### Comparing `scaleway-2.2.1/scaleway/ipfs/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/ipfs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/ipfs/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/ipfs/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/ipfs/v1alpha1/content.py` & `scaleway-2.3.1/scaleway/ipfs/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/ipfs/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/ipfs/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/ipfs/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/ipfs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/jobs/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/jobs/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/jobs/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/jobs/v1alpha1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     marshal_StartJobDefinitionRequest,
     marshal_UpdateJobDefinitionRequest,
 )
 
 
 class JobsV1Alpha1API(API):
     """
-    Serverless Jobs API.
+    This API allows you to manage your Serverless Jobs.
     """
 
     def create_job_definition(
         self,
         *,
         cpu_limit: int,
         memory_limit: int,
```

### Comparing `scaleway-2.2.1/scaleway/jobs/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/jobs/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/jobs/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/jobs/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/k8s/v1/__init__.py` & `scaleway-2.3.1/scaleway/k8s/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/k8s/v1/api.py` & `scaleway-2.3.1/scaleway/k8s/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     marshal_UpgradeClusterRequest,
     marshal_UpgradePoolRequest,
 )
 
 
 class K8SV1API(API):
     """
-    Kubernetes API.
+    This API allows you to manage Kubernetes Kapsule and Kosmos clusters.
     """
 
     def list_clusters(
         self,
         *,
         region: Optional[Region] = None,
         organization_id: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/k8s/v1/content.py` & `scaleway-2.3.1/scaleway/k8s/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/k8s/v1/marshalling.py` & `scaleway-2.3.1/scaleway/k8s/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/k8s/v1/types.py` & `scaleway-2.3.1/scaleway/k8s/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/lb/v1/__init__.py` & `scaleway-2.3.1/scaleway/lb/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/lb/v1/api.py` & `scaleway-2.3.1/scaleway/lb/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -3211,15 +3211,15 @@
         )
 
         self._throw_on_error(res)
 
 
 class LbV1API(API):
     """
-    This API allows you to manage your load balancer service.
+    This API allows you to manage your Load Balancers.
     """
 
     def list_lbs(
         self,
         *,
         region: Optional[Region] = None,
         name: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/lb/v1/content.py` & `scaleway-2.3.1/scaleway/lb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/lb/v1/marshalling.py` & `scaleway-2.3.1/scaleway/lb/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/lb/v1/types.py` & `scaleway-2.3.1/scaleway/lb/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/llm_inference/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/inference/v1beta1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 from .types import ListModelsResponse
 from .types import ListNodeTypesRequest
 from .types import ListNodeTypesResponse
 from .types import SetDeploymentACLRulesRequest
 from .types import SetDeploymentACLRulesResponse
 from .types import UpdateDeploymentRequest
 from .types import UpdateEndpointRequest
-from .api import LlmInferenceV1Beta1API
+from .api import InferenceV1Beta1API
 
 __all__ = [
     "DeploymentStatus",
     "DEPLOYMENT_TRANSIENT_STATUSES",
     "ListDeploymentsRequestOrderBy",
     "ListModelsRequestOrderBy",
     "NodeTypeStock",
@@ -81,9 +81,9 @@
     "ListModelsResponse",
     "ListNodeTypesRequest",
     "ListNodeTypesResponse",
     "SetDeploymentACLRulesRequest",
     "SetDeploymentACLRulesResponse",
     "UpdateDeploymentRequest",
     "UpdateEndpointRequest",
-    "LlmInferenceV1Beta1API",
+    "InferenceV1Beta1API",
 ]
```

### Comparing `scaleway-2.2.1/scaleway/llm_inference/v1beta1/api.py` & `scaleway-2.3.1/scaleway/inference/v1beta1/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,16 +59,18 @@
     marshal_CreateEndpointRequest,
     marshal_SetDeploymentACLRulesRequest,
     marshal_UpdateDeploymentRequest,
     marshal_UpdateEndpointRequest,
 )
 
 
-class LlmInferenceV1Beta1API(API):
-    """ """
+class InferenceV1Beta1API(API):
+    """
+    This API allows you to manage your Inference services.
+    """
 
     def list_deployments(
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
         page_size: Optional[int] = None,
@@ -478,15 +480,15 @@
         disable_auth: Optional[bool] = None,
     ) -> Endpoint:
         """
         Update an endpoint.
         Update an existing Endpoint.
         :param endpoint_id: ID of the endpoint to update.
         :param region: Region to target. If none is passed will use default region from the config.
-        :param disable_auth: By default, LLM deployments are protected by IAM authentication.
+        :param disable_auth: By default, deployments are protected by IAM authentication.
         When setting this field to true, the authentication will be disabled.
         :return: :class:`Endpoint <Endpoint>`
 
         Usage:
         ::
 
             result = api.update_endpoint(
@@ -754,15 +756,15 @@
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
     ) -> ListModelsResponse:
         """
         List models.
-        List all available LLM models.
+        List all available models.
         :param region: Region to target. If none is passed will use default region from the config.
         :param order_by: Order in which to return results.
         :param page: Page number to return.
         :param page_size: Maximum number of models to return per page.
         :param project_id: Filter by Project ID.
         :param name: Filter by model name.
         :param tags: Filter by tags.
@@ -803,15 +805,15 @@
         page_size: Optional[int] = None,
         project_id: Optional[str] = None,
         name: Optional[str] = None,
         tags: Optional[List[str]] = None,
     ) -> List[Model]:
         """
         List models.
-        List all available LLM models.
+        List all available models.
         :param region: Region to target. If none is passed will use default region from the config.
         :param order_by: Order in which to return results.
         :param page: Page number to return.
         :param page_size: Maximum number of models to return per page.
         :param project_id: Filter by Project ID.
         :param name: Filter by model name.
         :param tags: Filter by tags.
```

### Comparing `scaleway-2.2.1/scaleway/llm_inference/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/inference/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/llm_inference/v1beta1/types.py` & `scaleway-2.3.1/scaleway/inference/v1beta1/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
     """
 
 
 @dataclass
 class EndpointSpec:
     disable_auth: bool
     """
-    By default, LLM deployments are protected by IAM authentication.
+    By default, deployments are protected by IAM authentication.
 When setting this field to true, the authentication will be disabled.
     """
 
     public: Optional[EndpointSpecPublic]
 
     private_network: Optional[EndpointSpecPrivateNetwork]
 
@@ -813,10 +813,10 @@
     region: Optional[Region]
     """
     Region to target. If none is passed will use default region from the config.
     """
 
     disable_auth: Optional[bool]
     """
-    By default, LLM deployments are protected by IAM authentication.
+    By default, deployments are protected by IAM authentication.
 When setting this field to true, the authentication will be disabled.
     """
```

### Comparing `scaleway-2.2.1/scaleway/marketplace/v2/__init__.py` & `scaleway-2.3.1/scaleway/marketplace/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/marketplace/v2/api.py` & `scaleway-2.3.1/scaleway/marketplace/v2/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,17 @@
     unmarshal_ListImagesResponse,
     unmarshal_ListLocalImagesResponse,
     unmarshal_ListVersionsResponse,
 )
 
 
 class MarketplaceV2API(API):
-    """ """
+    """
+    This API allows you to find available images for use when launching a Scaleway Instance.
+    """
 
     def list_images(
         self,
         *,
         include_eol: bool,
         page_size: Optional[int] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/marketplace/v2/marshalling.py` & `scaleway-2.3.1/scaleway/marketplace/v2/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/marketplace/v2/types.py` & `scaleway-2.3.1/scaleway/marketplace/v2/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/mnq/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/mnq/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/mnq/v1beta1/api.py` & `scaleway-2.3.1/scaleway/mnq/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     marshal_SqsApiDeactivateSqsRequest,
     marshal_SqsApiUpdateSqsCredentialsRequest,
 )
 
 
 class MnqV1Beta1NatsAPI(API):
     """
-    This API allows you to manage Scaleway Messaging and Queueing NATS accounts.
+    This API allows you to manage Scaleway Messaging and Queuing NATS accounts.
     """
 
     def create_nats_account(
         self,
         *,
         region: Optional[Region] = None,
         name: Optional[str] = None,
@@ -496,15 +496,15 @@
                 "order_by": order_by,
             },
         )
 
 
 class MnqV1Beta1SnsAPI(API):
     """
-    This API allows you to manage Scaleway Messaging and Queueing SNS brokers.
+    This API allows you to manage your Scaleway Messaging and Queuing SNS brokers.
     """
 
     def activate_sns(
         self,
         *,
         region: Optional[Region] = None,
         project_id: Optional[str] = None,
@@ -856,15 +856,15 @@
                 "order_by": order_by,
             },
         )
 
 
 class MnqV1Beta1SqsAPI(API):
     """
-    This API allows you to manage Scaleway Messaging and Queueing SQS brokers.
+    This API allows you to manage your Scaleway Messaging and Queuing SQS brokers.
     """
 
     def activate_sqs(
         self,
         *,
         region: Optional[Region] = None,
         project_id: Optional[str] = None,
```

### Comparing `scaleway-2.2.1/scaleway/mnq/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/mnq/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/mnq/v1beta1/types.py` & `scaleway-2.3.1/scaleway/mnq/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/qaas/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/qaas/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/qaas/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/qaas/v1alpha1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/qaas/v1alpha1/content.py` & `scaleway-2.3.1/scaleway/qaas/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/qaas/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/qaas/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/qaas/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/qaas/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/rdb/v1/__init__.py` & `scaleway-2.3.1/scaleway/rdb/v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 from .types import Endpoint
 from .types import EndpointSpecLoadBalancer
 from .types import EndpointSpecPrivateNetwork
 from .types import ReadReplicaEndpointSpecDirectAccess
 from .types import ReadReplicaEndpointSpecPrivateNetwork
 from .types import EngineVersion
 from .types import BackupSchedule
+from .types import EncryptionAtRest
 from .types import InstanceSetting
 from .types import LogsPolicy
 from .types import Maintenance
 from .types import ReadReplica
 from .types import UpgradableVersion
 from .types import Volume
 from .types import NodeTypeVolumeConstraintSizes
@@ -184,14 +185,15 @@
     "Endpoint",
     "EndpointSpecLoadBalancer",
     "EndpointSpecPrivateNetwork",
     "ReadReplicaEndpointSpecDirectAccess",
     "ReadReplicaEndpointSpecPrivateNetwork",
     "EngineVersion",
     "BackupSchedule",
+    "EncryptionAtRest",
     "InstanceSetting",
     "LogsPolicy",
     "Maintenance",
     "ReadReplica",
     "UpgradableVersion",
     "Volume",
     "NodeTypeVolumeConstraintSizes",
```

### Comparing `scaleway-2.2.1/scaleway/rdb/v1/api.py` & `scaleway-2.3.1/scaleway/rdb/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     Database,
     DatabaseBackup,
     DatabaseEngine,
     DeleteInstanceACLRulesRequest,
     DeleteInstanceACLRulesResponse,
     DeleteInstanceSettingsRequest,
     DeleteInstanceSettingsResponse,
+    EncryptionAtRest,
     Endpoint,
     EndpointSpec,
     Instance,
     InstanceLog,
     InstanceMetrics,
     InstanceSetting,
     ListDatabaseBackupsResponse,
@@ -155,15 +156,17 @@
     marshal_UpdateSnapshotRequest,
     marshal_UpdateUserRequest,
     marshal_UpgradeInstanceRequest,
 )
 
 
 class RdbV1API(API):
-    """ """
+    """
+    This API allows you to manage your Managed Databases for PostgreSQL and MySQL.
+    """
 
     def list_database_engines(
         self,
         *,
         region: Optional[Region] = None,
         name: Optional[str] = None,
         version: Optional[str] = None,
@@ -971,14 +974,15 @@
         disable_backup: bool,
         volume_size: int,
         backup_same_region: bool,
         tags: Optional[List[str]] = None,
         init_settings: Optional[List[InstanceSetting]] = None,
         volume_type: Optional[VolumeType] = None,
         init_endpoints: Optional[List[EndpointSpec]] = None,
+        encryption: Optional[EncryptionAtRest] = None,
     ) -> Instance:
         """
         Create a Database Instance.
         Create a new Database Instance. You must set the `engine`, `user_name`, `password` and `node_type` parameters. Optionally, you can specify the volume type and size.
         :param engine: Database engine of the Database Instance (PostgreSQL, MySQL, ...).
         :param user_name: Username created when the Database Instance is created.
         :param password: Password of the user.
@@ -993,14 +997,15 @@
         :param disable_backup: Defines whether or not backups are disabled.
         :param volume_size: Volume size when volume_type is not lssd.
         :param backup_same_region: Defines whether to or not to store logical backups in the same region as the Database Instance.
         :param tags: Tags to apply to the Database Instance.
         :param init_settings: List of engine settings to be set upon Database Instance initialization.
         :param volume_type: Type of volume where data is stored (lssd, bssd, ...).
         :param init_endpoints: One or multiple EndpointSpec used to expose your Database Instance. A load_balancer public endpoint is systematically created.
+        :param encryption: Encryption at rest settings for your Database Instance.
         :return: :class:`Instance <Instance>`
 
         Usage:
         ::
 
             result = api.create_instance(
                 engine="example",
@@ -1033,14 +1038,15 @@
                     disable_backup=disable_backup,
                     volume_size=volume_size,
                     backup_same_region=backup_same_region,
                     tags=tags,
                     init_settings=init_settings,
                     volume_type=volume_type,
                     init_endpoints=init_endpoints,
+                    encryption=encryption,
                     project_id=project_id,
                     organization_id=organization_id,
                 ),
                 self.client,
             ),
         )
```

### Comparing `scaleway-2.2.1/scaleway/rdb/v1/content.py` & `scaleway-2.3.1/scaleway/rdb/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/rdb/v1/marshalling.py` & `scaleway-2.3.1/scaleway/rdb/v1/marshalling.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     Endpoint,
     Maintenance,
     ReadReplica,
     DatabaseBackup,
     Database,
     InstanceLog,
     BackupSchedule,
+    EncryptionAtRest,
     InstanceSetting,
     LogsPolicy,
     UpgradableVersion,
     Volume,
     Instance,
     Privilege,
     SnapshotVolumeType,
@@ -462,14 +463,29 @@
         )
     else:
         args["next_run_at"] = None
 
     return BackupSchedule(**args)
 
 
+def unmarshal_EncryptionAtRest(data: Any) -> EncryptionAtRest:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'EncryptionAtRest' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("enabled", None)
+    if field is not None:
+        args["enabled"] = field
+
+    return EncryptionAtRest(**args)
+
+
 def unmarshal_InstanceSetting(data: Any) -> InstanceSetting:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'InstanceSetting' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
@@ -674,14 +690,20 @@
 
     field = data.get("logs_policy", None)
     if field is not None:
         args["logs_policy"] = unmarshal_LogsPolicy(field)
     else:
         args["logs_policy"] = None
 
+    field = data.get("encryption", None)
+    if field is not None:
+        args["encryption"] = unmarshal_EncryptionAtRest(field)
+    else:
+        args["encryption"] = None
+
     return Instance(**args)
 
 
 def unmarshal_Privilege(data: Any) -> Privilege:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'Privilege' failed as data isn't a dictionary."
@@ -1698,14 +1720,26 @@
 
     if request.node_type is not None:
         output["node_type"] = request.node_type
 
     return output
 
 
+def marshal_EncryptionAtRest(
+    request: EncryptionAtRest,
+    defaults: ProfileDefaults,
+) -> Dict[str, Any]:
+    output: Dict[str, Any] = {}
+
+    if request.enabled is not None:
+        output["enabled"] = request.enabled
+
+    return output
+
+
 def marshal_CreateInstanceRequest(
     request: CreateInstanceRequest,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
     output: Dict[str, Any] = {}
     output.update(
         resolve_one_of(
@@ -1761,14 +1795,17 @@
         output["volume_type"] = str(request.volume_type)
 
     if request.init_endpoints is not None:
         output["init_endpoints"] = [
             marshal_EndpointSpec(item, defaults) for item in request.init_endpoints
         ]
 
+    if request.encryption is not None:
+        output["encryption"] = marshal_EncryptionAtRest(request.encryption, defaults)
+
     return output
 
 
 def marshal_ReadReplicaEndpointSpecPrivateNetworkIpamConfig(
     request: ReadReplicaEndpointSpecPrivateNetworkIpamConfig,
     defaults: ProfileDefaults,
 ) -> Dict[str, Any]:
```

### Comparing `scaleway-2.2.1/scaleway/rdb/v1/types.py` & `scaleway-2.3.1/scaleway/rdb/v1/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -488,14 +488,19 @@
     next_run_at: Optional[datetime]
     """
     Next run of the backup schedule (accurate to 10 minutes).
     """
 
 
 @dataclass
+class EncryptionAtRest:
+    enabled: bool
+
+
+@dataclass
 class InstanceSetting:
     name: str
 
     value: str
 
 
 @dataclass
@@ -958,14 +963,19 @@
     """
 
     logs_policy: Optional[LogsPolicy]
     """
     Logs policy of the Database Instance.
     """
 
+    encryption: Optional[EncryptionAtRest]
+    """
+    Encryption at rest settings for your Database Instance.
+    """
+
 
 @dataclass
 class NodeType:
     name: str
     """
     Node Type name identifier.
     """
@@ -1391,14 +1401,19 @@
     """
 
     init_endpoints: Optional[List[EndpointSpec]]
     """
     One or multiple EndpointSpec used to expose your Database Instance. A load_balancer public endpoint is systematically created.
     """
 
+    encryption: Optional[EncryptionAtRest]
+    """
+    Encryption at rest settings for your Database Instance.
+    """
+
     project_id: Optional[str]
 
     organization_id: Optional[str]
 
 
 @dataclass
 class CreateReadReplicaEndpointRequest:
```

### Comparing `scaleway-2.2.1/scaleway/redis/v1/__init__.py` & `scaleway-2.3.1/scaleway/redis/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/redis/v1/api.py` & `scaleway-2.3.1/scaleway/redis/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,17 @@
     marshal_SetEndpointsRequest,
     marshal_UpdateClusterRequest,
     marshal_UpdateEndpointRequest,
 )
 
 
 class RedisV1API(API):
-    """ """
+    """
+    This API allows you to manage your Managed Databases for Redis™.
+    """
 
     def create_cluster(
         self,
         *,
         version: str,
         node_type: str,
         zone: Optional[Zone] = None,
```

### Comparing `scaleway-2.2.1/scaleway/redis/v1/marshalling.py` & `scaleway-2.3.1/scaleway/redis/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/redis/v1/types.py` & `scaleway-2.3.1/scaleway/redis/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/registry/v1/__init__.py` & `scaleway-2.3.1/scaleway/registry/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/registry/v1/api.py` & `scaleway-2.3.1/scaleway/registry/v1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     marshal_UpdateImageRequest,
     marshal_UpdateNamespaceRequest,
 )
 
 
 class RegistryV1API(API):
     """
-    Container Registry API.
+    This API allows you to manage your Container Registry resources.
     """
 
     def list_namespaces(
         self,
         *,
         region: Optional[Region] = None,
         page: Optional[int] = None,
```

### Comparing `scaleway-2.2.1/scaleway/registry/v1/content.py` & `scaleway-2.3.1/scaleway/registry/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/registry/v1/marshalling.py` & `scaleway-2.3.1/scaleway/registry/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/registry/v1/types.py` & `scaleway-2.3.1/scaleway/registry/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/secret/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/secret/v1alpha1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     marshal_UpdateSecretRequest,
     marshal_UpdateSecretVersionRequest,
 )
 
 
 class SecretV1Alpha1API(API):
     """
-    This API allows you to conveniently store, access and share sensitive data.
+    This API allows you to manage your Secret Manager services, for storing, accessing and sharing sensitive data such as passwords, API keys and certificates.
     """
 
     def create_secret(
         self,
         *,
         name: str,
         is_protected: bool,
```

### Comparing `scaleway-2.2.1/scaleway/secret/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/secret/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/secret/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1beta1/__init__.py` & `scaleway-2.3.1/scaleway/secret/v1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1beta1/api.py` & `scaleway-2.3.1/scaleway/secret/v1beta1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     marshal_UpdateSecretRequest,
     marshal_UpdateSecretVersionRequest,
 )
 
 
 class SecretV1Beta1API(API):
     """
-    This API allows you to conveniently store, access and share sensitive data such as passwords, API keys and certificates.
+    This API allows you to manage your Secret Manager services, for storing, accessing and sharing sensitive data such as passwords, API keys and certificates.
     """
 
     def create_secret(
         self,
         *,
         name: str,
         protected: bool,
```

### Comparing `scaleway-2.2.1/scaleway/secret/v1beta1/marshalling.py` & `scaleway-2.3.1/scaleway/secret/v1beta1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/secret/v1beta1/types.py` & `scaleway-2.3.1/scaleway/secret/v1beta1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     marshal_RestoreDatabaseFromBackupRequest,
     marshal_UpdateDatabaseRequest,
 )
 
 
 class ServerlessSqldbV1Alpha1API(API):
     """
-    This API allows you to manage your Serverless SQL DB databases.
+    This API allows you to manage your Serverless SQL Databases.
     """
 
     def create_database(
         self,
         *,
         name: str,
         cpu_min: int,
```

### Comparing `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/serverless_sqldb/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/serverless_sqldb/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/tem/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/tem/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/tem/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/tem/v1alpha1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
     unmarshal_Statistics,
     marshal_CreateDomainRequest,
     marshal_CreateEmailRequest,
 )
 
 
 class TemV1Alpha1API(API):
-    """ """
+    """
+    This API allows you to manage your Transactional Email services.
+    """
 
     def create_email(
         self,
         *,
         subject: str,
         text: str,
         html: str,
```

### Comparing `scaleway-2.2.1/scaleway/tem/v1alpha1/content.py` & `scaleway-2.3.1/scaleway/tem/v1alpha1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/tem/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/tem/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/tem/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/tem/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/test/v1/__init__.py` & `scaleway-2.3.1/scaleway/test/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/test/v1/api.py` & `scaleway-2.3.1/scaleway/test/v1/api.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/test/v1/marshalling.py` & `scaleway-2.3.1/scaleway/test/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/test/v1/types.py` & `scaleway-2.3.1/scaleway/test/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpc/v1/__init__.py` & `scaleway-2.3.1/scaleway/vpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpc/v1/api.py` & `scaleway-2.3.1/scaleway/vpc/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     marshal_CreatePrivateNetworkRequest,
     marshal_UpdatePrivateNetworkRequest,
 )
 
 
 class VpcV1API(API):
     """
-    VPC API.
+    This API allows you to manage your Virtual Private Clouds (VPCs) and Private Networks.
     """
 
     def list_private_networks(
         self,
         *,
         zone: Optional[Zone] = None,
         order_by: Optional[ListPrivateNetworksRequestOrderBy] = None,
```

### Comparing `scaleway-2.2.1/scaleway/vpc/v1/marshalling.py` & `scaleway-2.3.1/scaleway/vpc/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpc/v1/types.py` & `scaleway-2.3.1/scaleway/vpc/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpc/v2/__init__.py` & `scaleway-2.3.1/scaleway/vpc/v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # This file was automatically generated. DO NOT EDIT.
 # If you have any remark or suggestion do not hesitate to open an issue.
 from .types import ListPrivateNetworksRequestOrderBy
+from .types import ListSubnetsRequestOrderBy
 from .types import ListVPCsRequestOrderBy
 from .types import Subnet
 from .types import PrivateNetwork
 from .types import VPC
 from .types import AddSubnetsRequest
 from .types import AddSubnetsResponse
 from .types import CreatePrivateNetworkRequest
@@ -15,25 +16,28 @@
 from .types import DeleteVPCRequest
 from .types import EnableDHCPRequest
 from .types import EnableRoutingRequest
 from .types import GetPrivateNetworkRequest
 from .types import GetVPCRequest
 from .types import ListPrivateNetworksRequest
 from .types import ListPrivateNetworksResponse
+from .types import ListSubnetsRequest
+from .types import ListSubnetsResponse
 from .types import ListVPCsRequest
 from .types import ListVPCsResponse
 from .types import MigrateZonalPrivateNetworksRequest
 from .types import SetSubnetsRequest
 from .types import SetSubnetsResponse
 from .types import UpdatePrivateNetworkRequest
 from .types import UpdateVPCRequest
 from .api import VpcV2API
 
 __all__ = [
     "ListPrivateNetworksRequestOrderBy",
+    "ListSubnetsRequestOrderBy",
     "ListVPCsRequestOrderBy",
     "Subnet",
     "PrivateNetwork",
     "VPC",
     "AddSubnetsRequest",
     "AddSubnetsResponse",
     "CreatePrivateNetworkRequest",
@@ -44,14 +48,16 @@
     "DeleteVPCRequest",
     "EnableDHCPRequest",
     "EnableRoutingRequest",
     "GetPrivateNetworkRequest",
     "GetVPCRequest",
     "ListPrivateNetworksRequest",
     "ListPrivateNetworksResponse",
+    "ListSubnetsRequest",
+    "ListSubnetsResponse",
     "ListVPCsRequest",
     "ListVPCsResponse",
     "MigrateZonalPrivateNetworksRequest",
     "SetSubnetsRequest",
     "SetSubnetsResponse",
     "UpdatePrivateNetworkRequest",
     "UpdateVPCRequest",
```

### Comparing `scaleway-2.2.1/scaleway/vpc/v2/api.py` & `scaleway-2.3.1/scaleway/vpc/v2/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,37 +10,41 @@
 from scaleway_core.utils import (
     random_name,
     validate_path_param,
     fetch_all_pages,
 )
 from .types import (
     ListPrivateNetworksRequestOrderBy,
+    ListSubnetsRequestOrderBy,
     ListVPCsRequestOrderBy,
     AddSubnetsRequest,
     AddSubnetsResponse,
     CreatePrivateNetworkRequest,
     CreateVPCRequest,
     DeleteSubnetsRequest,
     DeleteSubnetsResponse,
     ListPrivateNetworksResponse,
+    ListSubnetsResponse,
     ListVPCsResponse,
     MigrateZonalPrivateNetworksRequest,
     PrivateNetwork,
     SetSubnetsRequest,
     SetSubnetsResponse,
+    Subnet,
     UpdatePrivateNetworkRequest,
     UpdateVPCRequest,
     VPC,
 )
 from .marshalling import (
     unmarshal_PrivateNetwork,
     unmarshal_VPC,
     unmarshal_AddSubnetsResponse,
     unmarshal_DeleteSubnetsResponse,
     unmarshal_ListPrivateNetworksResponse,
+    unmarshal_ListSubnetsResponse,
     unmarshal_ListVPCsResponse,
     unmarshal_SetSubnetsResponse,
     marshal_AddSubnetsRequest,
     marshal_CreatePrivateNetworkRequest,
     marshal_CreateVPCRequest,
     marshal_DeleteSubnetsRequest,
     marshal_MigrateZonalPrivateNetworksRequest,
@@ -48,15 +52,15 @@
     marshal_UpdatePrivateNetworkRequest,
     marshal_UpdateVPCRequest,
 )
 
 
 class VpcV2API(API):
     """
-    VPC API.
+    This API allows you to manage your Virtual Private Clouds (VPCs) and Private Networks.
     """
 
     def list_vp_cs(
         self,
         *,
         region: Optional[Region] = None,
         order_by: Optional[ListVPCsRequestOrderBy] = None,
@@ -728,23 +732,123 @@
             f"/vpc/v2/regions/{param_region}/vpcs/{param_vpc_id}/enable-routing",
             body={},
         )
 
         self._throw_on_error(res)
         return unmarshal_VPC(res.json())
 
+    def list_subnets(
+        self,
+        *,
+        region: Optional[Region] = None,
+        order_by: Optional[ListSubnetsRequestOrderBy] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        organization_id: Optional[str] = None,
+        project_id: Optional[str] = None,
+        subnet_ids: Optional[List[str]] = None,
+        vpc_id: Optional[str] = None,
+    ) -> ListSubnetsResponse:
+        """
+        List subnets.
+        List any Private Network's subnets. See ListPrivateNetworks to list a specific Private Network's subnets.
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param order_by: Sort order of the returned subnets.
+        :param page: Page number to return, from the paginated results.
+        :param page_size: Maximum number of Private Networks to return per page.
+        :param organization_id: Organization ID to filter for. Only subnets belonging to this Organization will be returned.
+        :param project_id: Project ID to filter for. Only subnets belonging to this Project will be returned.
+        :param subnet_ids: Subnet IDs to filter for. Only subnets matching the specified IDs will be returned.
+        :param vpc_id: VPC ID to filter for. Only subnets belonging to this VPC will be returned.
+        :return: :class:`ListSubnetsResponse <ListSubnetsResponse>`
+
+        Usage:
+        ::
+
+            result = api.list_subnets()
+        """
+
+        param_region = validate_path_param(
+            "region", region or self.client.default_region
+        )
+
+        res = self._request(
+            "GET",
+            f"/vpc/v2/regions/{param_region}/subnets",
+            params={
+                "order_by": order_by,
+                "organization_id": organization_id
+                or self.client.default_organization_id,
+                "page": page,
+                "page_size": page_size or self.client.default_page_size,
+                "project_id": project_id or self.client.default_project_id,
+                "subnet_ids": subnet_ids,
+                "vpc_id": vpc_id,
+            },
+        )
+
+        self._throw_on_error(res)
+        return unmarshal_ListSubnetsResponse(res.json())
+
+    def list_subnets_all(
+        self,
+        *,
+        region: Optional[Region] = None,
+        order_by: Optional[ListSubnetsRequestOrderBy] = None,
+        page: Optional[int] = None,
+        page_size: Optional[int] = None,
+        organization_id: Optional[str] = None,
+        project_id: Optional[str] = None,
+        subnet_ids: Optional[List[str]] = None,
+        vpc_id: Optional[str] = None,
+    ) -> List[Subnet]:
+        """
+        List subnets.
+        List any Private Network's subnets. See ListPrivateNetworks to list a specific Private Network's subnets.
+        :param region: Region to target. If none is passed will use default region from the config.
+        :param order_by: Sort order of the returned subnets.
+        :param page: Page number to return, from the paginated results.
+        :param page_size: Maximum number of Private Networks to return per page.
+        :param organization_id: Organization ID to filter for. Only subnets belonging to this Organization will be returned.
+        :param project_id: Project ID to filter for. Only subnets belonging to this Project will be returned.
+        :param subnet_ids: Subnet IDs to filter for. Only subnets matching the specified IDs will be returned.
+        :param vpc_id: VPC ID to filter for. Only subnets belonging to this VPC will be returned.
+        :return: :class:`List[Subnet] <List[Subnet]>`
+
+        Usage:
+        ::
+
+            result = api.list_subnets_all()
+        """
+
+        return fetch_all_pages(
+            type=ListSubnetsResponse,
+            key="subnets",
+            fetcher=self.list_subnets,
+            args={
+                "region": region,
+                "order_by": order_by,
+                "page": page,
+                "page_size": page_size,
+                "organization_id": organization_id,
+                "project_id": project_id,
+                "subnet_ids": subnet_ids,
+                "vpc_id": vpc_id,
+            },
+        )
+
     def set_subnets(
         self,
         *,
         private_network_id: str,
         region: Optional[Region] = None,
         subnets: Optional[List[str]] = None,
     ) -> SetSubnetsResponse:
         """
-        Set the subnets of a Private Network.
+        Set a Private Network's subnets.
         Set subnets for an existing Private Network. Note that the method is PUT and not PATCH. Any existing subnets will be removed in favor of the new specified set of subnets.
         :param private_network_id: Private Network ID.
         :param region: Region to target. If none is passed will use default region from the config.
         :param subnets: Private Network subnets CIDR.
         :return: :class:`SetSubnetsResponse <SetSubnetsResponse>`
 
         Usage:
```

### Comparing `scaleway-2.2.1/scaleway/vpc/v2/marshalling.py` & `scaleway-2.3.1/scaleway/vpc/v2/marshalling.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .types import (
     Subnet,
     PrivateNetwork,
     VPC,
     AddSubnetsResponse,
     DeleteSubnetsResponse,
     ListPrivateNetworksResponse,
+    ListSubnetsResponse,
     ListVPCsResponse,
     SetSubnetsResponse,
     AddSubnetsRequest,
     CreatePrivateNetworkRequest,
     CreateVPCRequest,
     DeleteSubnetsRequest,
     MigrateZonalPrivateNetworksRequest,
@@ -41,14 +42,26 @@
     if field is not None:
         args["id"] = field
 
     field = data.get("subnet", None)
     if field is not None:
         args["subnet"] = field
 
+    field = data.get("project_id", None)
+    if field is not None:
+        args["project_id"] = field
+
+    field = data.get("private_network_id", None)
+    if field is not None:
+        args["private_network_id"] = field
+
+    field = data.get("vpc_id", None)
+    if field is not None:
+        args["vpc_id"] = field
+
     field = data.get("created_at", None)
     if field is not None:
         args["created_at"] = parser.isoparse(field) if isinstance(field, str) else field
     else:
         args["created_at"] = None
 
     field = data.get("updated_at", None)
@@ -227,14 +240,35 @@
     field = data.get("total_count", None)
     if field is not None:
         args["total_count"] = field
 
     return ListPrivateNetworksResponse(**args)
 
 
+def unmarshal_ListSubnetsResponse(data: Any) -> ListSubnetsResponse:
+    if not isinstance(data, dict):
+        raise TypeError(
+            "Unmarshalling the type 'ListSubnetsResponse' failed as data isn't a dictionary."
+        )
+
+    args: Dict[str, Any] = {}
+
+    field = data.get("subnets", None)
+    if field is not None:
+        args["subnets"] = (
+            [unmarshal_Subnet(v) for v in field] if field is not None else None
+        )
+
+    field = data.get("total_count", None)
+    if field is not None:
+        args["total_count"] = field
+
+    return ListSubnetsResponse(**args)
+
+
 def unmarshal_ListVPCsResponse(data: Any) -> ListVPCsResponse:
     if not isinstance(data, dict):
         raise TypeError(
             "Unmarshalling the type 'ListVPCsResponse' failed as data isn't a dictionary."
         )
 
     args: Dict[str, Any] = {}
```

### Comparing `scaleway-2.2.1/scaleway/vpc/v2/types.py` & `scaleway-2.3.1/scaleway/vpc/v2/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,22 @@
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
         return str(self.value)
 
 
+class ListSubnetsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
+    CREATED_AT_ASC = "created_at_asc"
+    CREATED_AT_DESC = "created_at_desc"
+
+    def __str__(self) -> str:
+        return str(self.value)
+
+
 class ListVPCsRequestOrderBy(str, Enum, metaclass=StrEnumMeta):
     CREATED_AT_ASC = "created_at_asc"
     CREATED_AT_DESC = "created_at_desc"
     NAME_ASC = "name_asc"
     NAME_DESC = "name_desc"
 
     def __str__(self) -> str:
@@ -43,14 +51,29 @@
     """
 
     subnet: str
     """
     Subnet CIDR.
     """
 
+    project_id: str
+    """
+    Scaleway Project the subnet belongs to.
+    """
+
+    private_network_id: str
+    """
+    Private Network the subnet belongs to.
+    """
+
+    vpc_id: str
+    """
+    VPC the subnet belongs to.
+    """
+
     created_at: Optional[datetime]
     """
     Subnet creation date.
     """
 
     updated_at: Optional[datetime]
     """
@@ -418,14 +441,64 @@
 class ListPrivateNetworksResponse:
     private_networks: List[PrivateNetwork]
 
     total_count: int
 
 
 @dataclass
+class ListSubnetsRequest:
+    region: Optional[Region]
+    """
+    Region to target. If none is passed will use default region from the config.
+    """
+
+    order_by: Optional[ListSubnetsRequestOrderBy]
+    """
+    Sort order of the returned subnets.
+    """
+
+    page: Optional[int]
+    """
+    Page number to return, from the paginated results.
+    """
+
+    page_size: Optional[int]
+    """
+    Maximum number of Private Networks to return per page.
+    """
+
+    organization_id: Optional[str]
+    """
+    Organization ID to filter for. Only subnets belonging to this Organization will be returned.
+    """
+
+    project_id: Optional[str]
+    """
+    Project ID to filter for. Only subnets belonging to this Project will be returned.
+    """
+
+    subnet_ids: Optional[List[str]]
+    """
+    Subnet IDs to filter for. Only subnets matching the specified IDs will be returned.
+    """
+
+    vpc_id: Optional[str]
+    """
+    VPC ID to filter for. Only subnets belonging to this VPC will be returned.
+    """
+
+
+@dataclass
+class ListSubnetsResponse:
+    subnets: List[Subnet]
+
+    total_count: int
+
+
+@dataclass
 class ListVPCsRequest:
     region: Optional[Region]
     """
     Region to target. If none is passed will use default region from the config.
     """
 
     order_by: Optional[ListVPCsRequestOrderBy]
```

### Comparing `scaleway-2.2.1/scaleway/vpcgw/v1/__init__.py` & `scaleway-2.3.1/scaleway/vpcgw/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpcgw/v1/api.py` & `scaleway-2.3.1/scaleway/vpcgw/v1/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     marshal_UpdateIPRequest,
     marshal_UpdatePATRuleRequest,
 )
 
 
 class VpcgwV1API(API):
     """
-    Public Gateways API.
+    This API allows you to manage your Public Gateways.
     """
 
     def list_gateways(
         self,
         *,
         zone: Optional[Zone] = None,
         order_by: Optional[ListGatewaysRequestOrderBy] = None,
```

### Comparing `scaleway-2.2.1/scaleway/vpcgw/v1/content.py` & `scaleway-2.3.1/scaleway/vpcgw/v1/content.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpcgw/v1/marshalling.py` & `scaleway-2.3.1/scaleway/vpcgw/v1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/vpcgw/v1/types.py` & `scaleway-2.3.1/scaleway/vpcgw/v1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/webhosting/v1alpha1/__init__.py` & `scaleway-2.3.1/scaleway/webhosting/v1alpha1/__init__.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/webhosting/v1alpha1/api.py` & `scaleway-2.3.1/scaleway/webhosting/v1alpha1/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 from ...std.types import (
     LanguageCode as StdLanguageCode,
 )
 
 
 class WebhostingV1Alpha1API(API):
     """
-    Web Hosting API.
+    This API allows you to manage your Web Hosting services.
     """
 
     def create_hosting(
         self,
         *,
         offer_id: str,
         domain: str,
```

### Comparing `scaleway-2.2.1/scaleway/webhosting/v1alpha1/marshalling.py` & `scaleway-2.3.1/scaleway/webhosting/v1alpha1/marshalling.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/scaleway/webhosting/v1alpha1/types.py` & `scaleway-2.3.1/scaleway/webhosting/v1alpha1/types.py`

 * *Files identical despite different names*

### Comparing `scaleway-2.2.1/PKG-INFO` & `scaleway-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaleway
-Version: 2.2.1
+Version: 2.3.1
 Summary: Scaleway SDK for Python
 License: BSD
 Author: Scaleway
 Author-email: opensource@scaleway.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -19,14 +19,14 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Software Development
-Requires-Dist: scaleway-core (==2.2.1)
+Requires-Dist: scaleway-core (==2.3.1)
 Description-Content-Type: text/markdown
 
 # Scaleway Python SDK
 
 This SDK enables you to interact with Scaleway APIs.
```

