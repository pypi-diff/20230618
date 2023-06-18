# Comparing `tmp/pulumi_vsphere-4.6.0a1686638681.tar.gz` & `tmp/pulumi_vsphere-4.6.0a1687057203.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_vsphere-4.6.0a1686638681.tar", last modified: Tue Jun 13 06:52:36 2023, max compression
+gzip compressed data, was "pulumi_vsphere-4.6.0a1687057203.tar", last modified: Sun Jun 18 03:05:53 2023, max compression
```

## Comparing `pulumi_vsphere-4.6.0a1686638681.tar` & `pulumi_vsphere-4.6.0a1687057203.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:52:36.934190 pulumi_vsphere-4.6.0a1686638681/
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-13 06:52:36.934190 pulumi_vsphere-4.6.0a1686638681/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:52:36.930190 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/
--rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    87225 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)   237133 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24459 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_host_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:52:36.934190 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/content_library.py
--rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    91913 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)   134499 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/distributed_port_group.py
--rw-r--r--   0 runner    (1001) docker     (123)   263381 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/dpm_host_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/entity_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_compute_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_compute_cluster_host_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_content_library.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_content_library_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datastore_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_distributed_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host_pci_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host_thumbprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_license.py
--rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_ovf_vm_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_role.py
--rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_tag_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_vmfs_disks.py
--rw-r--r--   0 runner    (1001) docker     (123)    58963 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/ha_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host.py
--rw-r--r--   0 runner    (1001) docker     (123)    56784 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host_port_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    61643 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host_virtual_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/license.py
--rw-r--r--   0 runner    (1001) docker     (123)    48202 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/nas_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    87056 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54091 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/resource_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/storage_drs_vm_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/tag_category.py
--rw-r--r--   0 runner    (1001) docker     (123)    48255 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vapp_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vapp_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    28150 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)   270022 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_machine_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vm_storage_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    34596 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vmfs_datastore.py
--rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vnic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:52:36.934190 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:52:36.934190 pulumi_vsphere-4.6.0a1686638681/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-13 06:52:36.000000 pulumi_vsphere-4.6.0a1686638681/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:05:53.822279 pulumi_vsphere-4.6.0a1687057203/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-18 03:05:53.818279 pulumi_vsphere-4.6.0a1687057203/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:05:53.818279 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/
+-rw-r--r--   0 runner    (1001) docker     (123)     9765 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87225 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)   237133 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24459 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17554 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21613 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_dependency_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24422 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_host_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:05:53.818279 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/content_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15640 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18866 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91913 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16842 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134499 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/distributed_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)   263381 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15371 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/dpm_host_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16657 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12429 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/entity_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25630 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_compute_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_compute_cluster_host_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_content_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_content_library_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datastore_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6814 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_distributed_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host_pci_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host_thumbprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_license.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7058 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32193 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_ovf_vm_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7358 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55448 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_vmfs_disks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58963 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/ha_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45915 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56784 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host_port_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61643 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host_virtual_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/license.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48202 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/nas_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87056 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54091 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/resource_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8528 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20828 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/storage_drs_vm_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9943 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/tag_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48255 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vapp_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29555 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vapp_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28150 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)   270022 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23926 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_machine_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vm_storage_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34596 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vmfs_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28500 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vnic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 03:05:53.818279 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 03:05:53.822279 pulumi_vsphere-4.6.0a1687057203/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-06-18 03:05:53.000000 pulumi_vsphere-4.6.0a1687057203/setup.py
```

### Comparing `pulumi_vsphere-4.6.0a1686638681/PKG-INFO` & `pulumi_vsphere-4.6.0a1687057203/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_vsphere
-Version: 4.6.0a1686638681
+Version: 4.6.0a1687057203
 Summary: A Pulumi package for creating vsphere resources
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi vsphere
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_vsphere-4.6.0a1686638681/README.md` & `pulumi_vsphere-4.6.0a1687057203/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/__init__.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/_inputs.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/_utilities.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_host_group.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_host_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_affinity_rule.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_anti_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_dependency_rule.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_dependency_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_group.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/compute_cluster_vm_host_rule.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/compute_cluster_vm_host_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/config/vars.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/content_library.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/content_library_item.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/custom_attribute.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datacenter.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datastore_cluster.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datastore_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/datastore_cluster_vm_anti_affinity_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/distributed_port_group.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/distributed_port_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/distributed_virtual_switch.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/distributed_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/dpm_host_override.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/dpm_host_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/drs_vm_override.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/drs_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/entity_permissions.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/entity_permissions.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/file.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/folder.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_compute_cluster.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_compute_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_compute_cluster_host_group.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_compute_cluster_host_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_content_library.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_content_library.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_content_library_item.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_content_library_item.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_custom_attribute.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datacenter.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datacenter.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datastore.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_datastore_cluster.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_datastore_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_distributed_virtual_switch.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_distributed_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_dynamic.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_dynamic.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_folder.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_folder.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host_pci_device.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host_pci_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_host_thumbprint.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_host_thumbprint.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_license.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_network.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_ovf_vm_template.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_ovf_vm_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_policy.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_resource_pool.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_resource_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_role.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_tag.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_tag_category.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_tag_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_vapp_container.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_virtual_machine.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/get_vmfs_disks.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/get_vmfs_disks.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/ha_vm_override.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/ha_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host_port_group.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host_port_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/host_virtual_switch.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/host_virtual_switch.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/license.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/license.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/nas_datastore.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/nas_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/outputs.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/provider.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/resource_pool.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/resource_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/role.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/storage_drs_vm_override.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/storage_drs_vm_override.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/tag.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/tag_category.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/tag_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vapp_container.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vapp_container.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vapp_entity.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vapp_entity.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_disk.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_machine.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/virtual_machine_snapshot.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/virtual_machine_snapshot.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vm_storage_policy.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vm_storage_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vmfs_datastore.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vmfs_datastore.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere/vnic.py` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere/vnic.py`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/PKG-INFO` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-vsphere
-Version: 4.6.0a1686638681
+Version: 4.6.0a1687057203
 Summary: A Pulumi package for creating vsphere resources
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-vsphere
 Keywords: pulumi vsphere
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_vsphere-4.6.0a1686638681/pulumi_vsphere.egg-info/SOURCES.txt` & `pulumi_vsphere-4.6.0a1687057203/pulumi_vsphere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_vsphere-4.6.0a1686638681/setup.py` & `pulumi_vsphere-4.6.0a1687057203/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.6.0a1686638681"
-PLUGIN_VERSION = "4.6.0-alpha.1686638681+95a227d6"
+VERSION = "4.6.0a1687057203"
+PLUGIN_VERSION = "4.6.0-alpha.1687057203+f6b48469"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vsphere', PLUGIN_VERSION])
         except OSError as error:
```

