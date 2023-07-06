# Comparing `tmp/idem_gcp-1.2.0.tar.gz` & `tmp/idem_gcp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem_gcp-1.2.0.tar", last modified: Tue Jun 20 07:50:38 2023, max compression
+gzip compressed data, was "idem_gcp-2.0.0.tar", last modified: Thu Jul  6 15:19:51 2023, max compression
```

## Comparing `idem_gcp-1.2.0.tar` & `idem_gcp-2.0.0.tar`

### file list

```diff
@@ -1,201 +1,194 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/
--rw-r--r--   0 root         (0) root         (0)    11342 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7881 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6761 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/init.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/acct/gcp/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/autogen/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/autogen/gcp/
--rw-r--r--   0 root         (0) root         (0)     9958 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/autogen/gcp/schema_parser.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/autogen/init.py
--rw-r--r--   0 root         (0) root         (0)     1749 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     4101 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    10239 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)     4092 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     3759 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2737 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     6946 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)    16748 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)     7479 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)     6938 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)    10946 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)     5200 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)     5925 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    49424 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    17133 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)     4958 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)     6819 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)    15742 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     7311 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     5977 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)     7766 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     5810 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/target_pool.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/zone.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/contracts/
--rw-r--r--   0 root         (0) root         (0)      501 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)     9330 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)     7914 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     4382 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/bucket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/exec/gcp_api/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/exec/gcp_api/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/helpers/
--rw-r--r--   0 root         (0) root         (0)      834 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/exc.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/log.py
--rw-r--r--   0 root         (0) root         (0)     1314 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/helpers/returns.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
--rw-r--r--   0 root         (0) root         (0)      187 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.139737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
--rw-r--r--   0 root         (0) root         (0)      236 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)      238 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)      270 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/disk_type.py
--rw-r--r--   0 root         (0) root         (0)      147 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/global_operation.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)      153 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/machine_type.py
--rw-r--r--   0 root         (0) root         (0)      143 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)      204 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/region_backend_service.py
--rw-r--r--   0 root         (0) root         (0)      175 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/region_operation.py
--rw-r--r--   0 root         (0) root         (0)      165 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)      116 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/target_pool.py
--rw-r--r--   0 root         (0) root         (0)      124 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/zone.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/compute/zone_operation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)      170 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)      183 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)      219 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/resources/
--rw-r--r--   0 root         (0) root         (0)    22702 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/resources/properties.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)    30514 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
--rw-r--r--   0 root         (0) root         (0)    29172 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
--rw-r--r--   0 root         (0) root         (0)    16925 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/import_job.py
--rw-r--r--   0 root         (0) root         (0)     7655 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/key_ring.py
--rw-r--r--   0 root         (0) root         (0)     2549 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/location.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)    81756 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/backend_service.py
--rw-r--r--   0 root         (0) root         (0)    29638 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    18544 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/firewall.py
--rw-r--r--   0 root         (0) root         (0)    27526 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/forwarding_rule.py
--rw-r--r--   0 root         (0) root         (0)    35507 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/health_check.py
--rw-r--r--   0 root         (0) root         (0)    24598 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/image.py
--rw-r--r--   0 root         (0) root         (0)    89505 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)    13426 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)    14791 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/machine_image.py
--rw-r--r--   0 root         (0) root         (0)    22275 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)     6821 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/node_template.py
--rw-r--r--   0 root         (0) root         (0)     8342 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/reservation.py
--rw-r--r--   0 root         (0) root         (0)    14697 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/resource_policy.py
--rw-r--r--   0 root         (0) root         (0)    17272 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/snapshot.py
--rw-r--r--   0 root         (0) root         (0)    20407 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     8557 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/compute/target_pool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/
--rw-r--r--   0 root         (0) root         (0)    12073 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_account.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/
--rw-r--r--   0 root         (0) root         (0)     9632 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)    15877 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.143737 idem_gcp-1.2.0/idem_gcp/states/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)    41239 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/states/gcp/storage/bucket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/
--rw-r--r--   0 root         (0) root         (0)     1800 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/case.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/
--rw-r--r--   0 root         (0) root         (0)     5296 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/patch.py
--rw-r--r--   0 root         (0) root         (0)     3953 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/
--rw-r--r--   0 root         (0) root         (0)     9834 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/disk.py
--rw-r--r--   0 root         (0) root         (0)    11892 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance.py
--rw-r--r--   0 root         (0) root         (0)      722 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance_group.py
--rw-r--r--   0 root         (0) root         (0)     5276 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/network.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)     4000 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/conversion_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/
--rw-r--r--   0 root         (0) root         (0)     1116 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_context.py
--rw-r--r--   0 root         (0) root         (0)      533 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_param.py
--rw-r--r--   0 root         (0) root         (0)     1544 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/generic_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/
--rw-r--r--   0 root         (0) root         (0)      704 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
--rw-r--r--   0 root         (0) root         (0)     2771 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
--rw-r--r--   0 root         (0) root         (0)     1547 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
--rw-r--r--   0 root         (0) root         (0)      522 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
--rw-r--r--   0 root         (0) root         (0)     1284 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/scope.py
--rw-r--r--   0 root         (0) root         (0)     1519 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/hub_resolver.py
--rw-r--r--   0 root         (0) root         (0)    21776 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/init.py
--rw-r--r--   0 root         (0) root         (0)     5614 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/operation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1923 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/policy.py
--rw-r--r--   0 root         (0) root         (0)    18555 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/resolver.py
--rw-r--r--   0 root         (0) root         (0)    18698 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/resource_prop_utils.py
--rw-r--r--   0 root         (0) root         (0)     1530 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/sanitizers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/
--rw-r--r--   0 root         (0) root         (0)      874 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/finding.py
--rw-r--r--   0 root         (0) root         (0)     1845 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/results_collector.py
--rw-r--r--   0 root         (0) root         (0)     2725 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
--rw-r--r--   0 root         (0) root         (0)     1283 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py
--rw-r--r--   0 root         (0) root         (0)     2310 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/scm_utils.py
--rw-r--r--   0 root         (0) root         (0)      597 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/session.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/state_operation_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/
--rw-r--r--   0 root         (0) root         (0)     2334 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/bucket.py
--rw-r--r--   0 root         (0) root         (0)    19738 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/idem_gcp/tool/gcp/utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2023-06-20 07:50:37.000000 idem_gcp-1.2.0/idem_gcp/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 07:50:38.135737 idem_gcp-1.2.0/idem_gcp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7881 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6140 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-20 07:50:38.000000 idem_gcp-1.2.0/idem_gcp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-06-20 07:50:38.147737 idem_gcp-1.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3303 2023-06-20 07:50:23.000000 idem_gcp-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)    11342 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6761 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/acct/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/acct/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      603 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/acct/gcp/contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/acct/gcp/service_account.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/autogen/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/autogen/gcp/
+-rw-r--r--   0 root         (0) root         (0)     9958 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/autogen/gcp/schema_parser.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/autogen/init.py
+-rw-r--r--   0 root         (0) root         (0)     1749 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/exec/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     4101 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    10239 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)     4092 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2737 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     6946 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    16748 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)     7479 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)     6938 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    10946 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)     5200 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)     5925 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    49424 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    17133 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     4958 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)     6819 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    15742 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     7311 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     5977 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)     6275 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     5810 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/zone.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp/contracts/
+-rw-r--r--   0 root         (0) root         (0)      501 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp/iam/
+-rw-r--r--   0 root         (0) root         (0)     9188 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/iam/service_account.py
+-rw-r--r--   0 root         (0) root         (0)     7814 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/iam/service_account_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     4382 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/exec/gcp_api/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/exec/gcp_api/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/helpers/
+-rw-r--r--   0 root         (0) root         (0)      834 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/helpers/exc.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/helpers/log.py
+-rw-r--r--   0 root         (0) root         (0)     1314 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/helpers/returns.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/metadata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/
+-rw-r--r--   0 root         (0) root         (0)      187 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/crypto_key_versions.py
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/crypto_keys/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/import_jobs/init.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/accelerator_type.py
+-rw-r--r--   0 root         (0) root         (0)      236 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      238 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)      270 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/disk_type.py
+-rw-r--r--   0 root         (0) root         (0)      147 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/global_operation.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)      153 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)      143 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)      204 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/region_backend_service.py
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/region_operation.py
+-rw-r--r--   0 root         (0) root         (0)      165 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)      100 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      116 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/target_pool.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/zone.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/compute/zone_operation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/iam/
+-rw-r--r--   0 root         (0) root         (0)      230 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/iam/service_account.py
+-rw-r--r--   0 root         (0) root         (0)      183 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/iam/service_account_key.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/metadata/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)      224 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/metadata/gcp/storage/objectAccessControls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/resources/
+-rw-r--r--   0 root         (0) root         (0)    22683 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/resources/properties.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/states/gcp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)    30514 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/crypto_key.py
+-rw-r--r--   0 root         (0) root         (0)    29172 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py
+-rw-r--r--   0 root         (0) root         (0)    16925 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/import_job.py
+-rw-r--r--   0 root         (0) root         (0)     7655 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)     2549 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/location.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)    82024 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/backend_service.py
+-rw-r--r--   0 root         (0) root         (0)    29638 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    18544 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/firewall.py
+-rw-r--r--   0 root         (0) root         (0)    27526 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/forwarding_rule.py
+-rw-r--r--   0 root         (0) root         (0)    35507 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/health_check.py
+-rw-r--r--   0 root         (0) root         (0)    24598 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/image.py
+-rw-r--r--   0 root         (0) root         (0)    89505 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)    13426 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)    14791 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/machine_image.py
+-rw-r--r--   0 root         (0) root         (0)    22275 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)     6821 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/node_template.py
+-rw-r--r--   0 root         (0) root         (0)     8342 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/reservation.py
+-rw-r--r--   0 root         (0) root         (0)    14697 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/resource_policy.py
+-rw-r--r--   0 root         (0) root         (0)    17272 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    20407 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     8557 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/compute/target_pool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/states/gcp/iam/
+-rw-r--r--   0 root         (0) root         (0)    12586 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/iam/service_account.py
+-rw-r--r--   0 root         (0) root         (0)     9516 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/iam/service_account_key.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.409524 idem_gcp-2.0.0/idem_gcp/states/gcp/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)    16100 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/recursive_contracts/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/states/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)    41239 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/states/gcp/storage/bucket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/
+-rw-r--r--   0 root         (0) root         (0)     1800 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/case.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/cloudkms/
+-rw-r--r--   0 root         (0) root         (0)     5296 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/cloudkms/patch.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/
+-rw-r--r--   0 root         (0) root         (0)     9834 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/disk.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/instance.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/instance_group.py
+-rw-r--r--   0 root         (0) root         (0)     5276 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/network.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)     4000 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/conversion_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/exec_context.py
+-rw-r--r--   0 root         (0) root         (0)      533 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/exec_param.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/generic_exec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.401524 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/post_exec/
+-rw-r--r--   0 root         (0) root         (0)      704 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py
+-rw-r--r--   0 root         (0) root         (0)      522 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/recursive_contracts/init.py
+-rw-r--r--   0 root         (0) root         (0)      309 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/scope.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/hub_resolver.py
+-rw-r--r--   0 root         (0) root         (0)    21776 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/init.py
+-rw-r--r--   0 root         (0) root         (0)     5614 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/operation_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1923 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/policy.py
+-rw-r--r--   0 root         (0) root         (0)    18555 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/resolver.py
+-rw-r--r--   0 root         (0) root         (0)    18365 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/resource_prop_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/sanitizers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/finding.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/results_collector.py
+-rw-r--r--   0 root         (0) root         (0)     2725 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py
+-rw-r--r--   0 root         (0) root         (0)     1283 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/scm_utils.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/state_operation_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/idem_gcp/tool/gcp/storage/
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/storage/bucket.py
+-rw-r--r--   0 root         (0) root         (0)    20220 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/idem_gcp/tool/gcp/utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-06 15:19:50.000000 idem_gcp-2.0.0/idem_gcp/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 15:19:51.405524 idem_gcp-2.0.0/idem_gcp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7881 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6054 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-06 15:19:51.000000 idem_gcp-2.0.0/idem_gcp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-06 15:19:51.413524 idem_gcp-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3303 2023-07-06 15:19:36.000000 idem_gcp-2.0.0/setup.py
```

### Comparing `idem_gcp-1.2.0/LICENSE` & `idem_gcp-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/PKG-INFO` & `idem_gcp-2.0.0/idem_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idem_gcp
-Version: 1.2.0
+Name: idem-gcp
+Version: 2.0.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/-/issues
```

### Comparing `idem_gcp-1.2.0/README.rst` & `idem_gcp-2.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/acct/gcp/contracts/init.py` & `idem_gcp-2.0.0/idem_gcp/acct/gcp/contracts/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/acct/gcp/service_account.py` & `idem_gcp-2.0.0/idem_gcp/acct/gcp/service_account.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/autogen/gcp/schema_parser.py` & `idem_gcp-2.0.0/idem_gcp/autogen/gcp/schema_parser.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/conf.py` & `idem_gcp-2.0.0/idem_gcp/conf.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/import_job.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/import_job.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/key_ring.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/key_ring.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/cloudkms/location.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/cloudkms/location.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/accelerator_type.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/backend_service.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/backend_service.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/disk_type.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/disk_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/firewall.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/firewall.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/forwarding_rule.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/health_check.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/health_check.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/image.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/instance_group.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_image.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/machine_image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/machine_type.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/machine_type.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/network.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/node_template.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/node_template.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/reservation.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/reservation.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/resource_policy.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/snapshot.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/subnetwork.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/target_pool.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/target_pool.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/compute/zone.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/compute/zone.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_account.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/iam/service_account.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,96 @@
 """Exec module for managing ServiceAccounts."""
+import re
 from typing import Callable
 
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 __func_alias__ = {"list_": "list"}
+RESOURCE_TYPE = "iam.service_account"
+RESOURCE_TYPE_FULL = f"gcp.{RESOURCE_TYPE}"
 
 
 async def list_(hub, ctx, project: str = None):
     r"""Lists every ServiceAccount that belongs to a specific project.
 
     Args:
         project(str, Required):
             The resource name of the project associated with the service accounts.
     """
     project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
 
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_account",
+        resource_type=RESOURCE_TYPE,
         method_name="list",
         method_params={"ctx": ctx, "name": f"projects/{project}"},
     )
 
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def get(
     hub,
     ctx,
-    project: str = None,
+    project_id: str = None,
     unique_id: str = None,
     email: str = None,
     name: str = None,
     resource_id: str = None,
 ):
     r"""Returns the specified ServiceAccount resource.
 
     Args:
-        project(str, Optional):
+        project_id(str, Optional):
             Project ID for this request.
         unique_id(str, Optional):
             The unique, stable numeric ID for the service account.
         email(str, Optional):
             The email address of the service account.
         name(str, Optional):
             Name of the service account in the provider API.
         resource_id(str, Optional):
             An identifier of the resource in the provider. Defaults to None.
 
     Examples:
-        .. code-block: sls
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.iam.projects.service_account.get
+              - path: gcp.iam.service_account.get
               - kwargs:
                   name: service-account-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
     }
-    if unique_id or email:
-        project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
-        identifier = unique_id or email
-        name = f"projects/{project}/serviceAccounts/{identifier}"
+    if not resource_id:
+        project_id = hub.tool.gcp.utils.get_project_from_account(ctx, project_id)
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE, locals()
+        )
 
-    name = name or resource_id
-    if not name:
-        result["result"] = False
+    if not resource_id and re.match(r"^projects/.+/serviceAccounts/.+$", name or ""):
+        resource_id = name
+
+    if not resource_id:
         result["comment"] = [
-            f"gcp.iam.projects.service_account#get(): either resource_id or name or unique_id or email"
+            f"{RESOURCE_TYPE_FULL}#get(): either resource_id or name or unique_id or email"
             f" must be specified."
         ]
         return result
 
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_account",
+        resource_type=RESOURCE_TYPE,
         method_name="get",
-        method_params={"ctx": ctx, "name": name},
+        method_params={"ctx": ctx, "name": resource_id},
     )
 
-    ret = await hub.tool.gcp.generate.generic_exec.execute(execution_context)
-
-    result["comment"] += ret["comment"]
-    if not ret["result"]:
-        result["result"] = False
-        return result
-
-    result["ret"] = ret["ret"]
-    return result
+    return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
 async def undelete(
     hub,
     ctx,
     unique_id: str,
     project: str = None,
@@ -121,24 +118,22 @@
         "comment": [],
         "ret": None,
         "result": True,
     }
 
     if not unique_id:
         result["result"] = False
-        result["comment"] = [
-            f"gcp.iam.projects.service_account#undelete(): unique_id is required"
-        ]
+        result["comment"] = [f"{RESOURCE_TYPE_FULL}#undelete(): unique_id is required"]
         return result
 
     project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
     resource_id = f"projects/{project}/serviceAccounts/{unique_id}"
 
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_account",
+        resource_type=RESOURCE_TYPE,
         method_name="undelete",
         method_params={"ctx": ctx, "name": resource_id},
     )
 
     ret = await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
     result["comment"] += ret["comment"]
@@ -196,17 +191,16 @@
     project: str = None,
     unique_id: str = None,
     email: str = None,
     resource_id: str = None,
 ):
     r"""Enables a service account that have previously been disabled.
 
-     If the service account is already enabled, then this method has no effect.
-
-     If the service account was disabled by other means — for example, if Google disabled the service account because it was compromised—you cannot use this method to enable the service account.
+    If the service account is already enabled, then this method has no effect.
+    If the service account was disabled by other means — for example, if Google disabled the service account because it was compromised—you cannot use this method to enable the service account.
 
     Args:
         project(str, Optional):
             Project ID for this request.
         unique_id(str, Optional):
             The unique, stable numeric ID for the service account.
         email(str, Optional):
@@ -248,24 +242,24 @@
     if unique_id or email:
         project = hub.tool.gcp.utils.get_project_from_account(ctx, project)
         identifier = unique_id or email
         resource_id = f"projects/{project}/serviceAccounts/{identifier}"
     elif not resource_id:
         result["result"] = False
         result["comment"] = [
-            f"gcp.iam.projects.service_account#{api_method}(): "
+            f"{RESOURCE_TYPE_FULL}#{api_method}(): "
             f"either resource_id or unique_id or email should be specified."
         ]
         return result
 
     async def validate_resource():
         """Validate subsequent get requests return expected output."""
         get_ret = await hub.tool.gcp.generate.generic_exec.execute(
             ExecutionContext(
-                resource_type="iam.projects.service_account",
+                resource_type=RESOURCE_TYPE,
                 method_name="get",
                 method_params={"ctx": ctx, "name": resource_id},
             )
         )
         try:
             assert get_ret["result"]
             validate(get_ret["ret"])
@@ -279,15 +273,15 @@
         result["ret"] = get_ret["ret"]
         return result
 
     if ctx.get("rerun_data"):
         return await validate_resource()
 
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_account",
+        resource_type=RESOURCE_TYPE,
         method_name=api_method,
         method_params={"ctx": ctx, "name": resource_id},
     )
 
     ret = await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
     result["comment"] += ret["comment"]
```

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/iam/projects/service_accounts/key.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/iam/service_account_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Exec module for managing ServiceAccountKeys."""
 from typing import Callable
 
 from idem_gcp.tool.gcp.generate.exec_context import ExecutionContext
 
 __func_alias__ = {"list_": "list"}
-RESOURCE_TYPE = "iam.projects.service_accounts.key"
-RESOURCE_TYPE_FULL = "gcp.iam.projects.service_accounts.key"
+RESOURCE_TYPE = "iam.service_account_key"
+RESOURCE_TYPE_FULL = f"gcp.{RESOURCE_TYPE}"
 
 
 async def list_(hub, ctx, sa_resource_id: str, project: str = None):
     r"""Lists every ServiceAccountKey that belongs to a specific project.
 
     Args:
         sa_resource_id(str):
             Resource id of the service account following the pattern projects/{project}/serviceAccounts/{id}.
         project(str, Optional):
             The resource name of the project associated with the service accounts.
     """
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_accounts.key",
+        resource_type="iam.service_account_key",
         method_name="list",
         method_params={"ctx": ctx, "name": sa_resource_id},
     )
 
     return await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
 
@@ -45,20 +45,20 @@
         key_id(str, Optional):
             Id of the service account key in GCP.
         name(str, Optional):
             Name of the service account in the provider API.
         resource_id(str, Optional):
             An identifier of the service account key in idem. Defaults to None.
 
-        Examples:
-        .. code-block: sls
+    Examples:
+        .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.iam.projects.service_accounts.key.get
+              - path: gcp.iam.service_account_key.get
               - kwargs:
                   name: service-account-key-name
     """
     result = {
         "comment": [],
         "ret": None,
         "result": True,
@@ -69,21 +69,21 @@
             f"projects/{project}/serviceAccounts/{service_account_id}/keys/{key_id}"
         )
 
     name = name or resource_id
     if not name:
         result["result"] = False
         result["comment"] = [
-            f"gcp.iam.projects.service_accounts.key#get(): either name, service_account_id and key_id or resource_id"
+            f"gcp.iam.service_account_key#get(): either name, service_account_id and key_id or resource_id"
             f" must be specified."
         ]
         return result
 
     execution_context = ExecutionContext(
-        resource_type="iam.projects.service_accounts.key",
+        resource_type="iam.service_account_key",
         method_name="get",
         method_params={"ctx": ctx, "name": name},
     )
 
     ret = await hub.tool.gcp.generate.generic_exec.execute(execution_context)
 
     result["comment"] += ret["comment"]
@@ -108,15 +108,15 @@
             The public key to associate with the service account. Must be an RSA public key that is wrapped in an X.509 v3 certificate. Include the first line, -----BEGIN CERTIFICATE-----, and the last line, -----END CERTIFICATE-----. A base64-encoded string.
 
     Examples:
         .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.iam.projects.service_accounts.key.upload
+              - path: gcp.iam.service_account_key.upload
               - kwargs:
                   service_account_id: projects/{...}/serviceAccounts/{...}
                   public_key_data: <base64-encoded X.509 v3 certificate>
     """
     result = {
         "comment": [],
         "ret": None,
@@ -166,15 +166,15 @@
             Resource id of the service account key
 
     Examples:
         .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.iam.projects.service_accounts.key.disable
+              - path: gcp.iam.service_account_key.disable
               - kwargs:
                   resource_id: projects/{...}/serviceAccounts/{...}/keys/{...}
     """
 
     def validate(get_ret):
         assert get_ret.get("disabled")
 
@@ -189,15 +189,15 @@
             Resource id of the service account key
 
     Examples:
         .. code-block:: sls
 
             random-name:
               exec.run:
-              - path: gcp.iam.projects.service_accounts.key.enable
+              - path: gcp.iam.service_account_key.enable
               - kwargs:
                   resource_id: projects/{...}/serviceAccounts/{...}/keys/{...}
     """
 
     def validate(get_ret):
         assert "disabled" not in get_ret
```

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp/storage/bucket.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/exec/gcp_api/init.py` & `idem_gcp-2.0.0/idem_gcp/exec/gcp_api/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/helpers/exc.py` & `idem_gcp-2.0.0/idem_gcp/helpers/exc.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/helpers/log.py` & `idem_gcp-2.0.0/idem_gcp/helpers/log.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/helpers/returns.py` & `idem_gcp-2.0.0/idem_gcp/helpers/returns.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/resources/properties.yaml` & `idem_gcp-2.0.0/idem_gcp/resources/properties.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1140,15 +1140,15 @@
     - id
     - protocol
     - sessionAffinity
     - loadBalancingScheme
     - localityLbPolicy
     - compressionMode
 
-iam.projects.service_account:
+iam.service_account:
   request_parameters:
     list:
       - name
     get:
       - name
     create:
       - name
@@ -1204,15 +1204,15 @@
     - region
   fields_enum_type:
     - id
     - sessionAffinity
   resource_id:
     - name
 
-iam.projects.service_accounts.key:
+iam.service_account_key:
   request_parameters:
     list:
       - name
     get:
       - name
     create:
       -name
```

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/crypto_key.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/crypto_key_version.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/import_job.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/import_job.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/key_ring.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/key_ring.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/cloudkms/location.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/cloudkms/location.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/backend_service.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/backend_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -913,23 +913,32 @@
 
     if not ctx.get("rerun_data"):
         delete_ret = (
             await hub.exec.gcp_api.client.compute.region_backend_service.delete(
                 ctx, resource_id=resource_id, request_id=request_id
             )
         )
-        if hub.tool.gcp.operation_utils.is_operation(delete_ret["ret"]):
+        if not delete_ret.get(
+            "result"
+        ) or not hub.tool.gcp.operation_utils.is_operation(delete_ret.get("ret")):
             result["result"] = False
-            result["comment"] += delete_ret["comment"]
-            result["rerun_data"] = {
-                "operation_id": hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
-                    delete_ret["ret"].get("selfLink"), "compute.region_operation"
-                )
-            }
+            result["comment"].append(
+                f"Unexpected return value from gcp.compute.region_backend_service.delete - {delete_ret}"
+            )
             return result
+
+        result["result"] = True
+        result["comment"] += delete_ret["comment"]
+        result["rerun_data"] = {
+            "operation_id": hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
+                delete_ret["ret"].get("selfLink"),
+                "compute.region_operation",
+            ),
+        }
+        return result
     else:
         # delete() has been called on some previous iteration
         handle_operation_ret = await hub.tool.gcp.operation_utils.handle_operation(
             ctx, ctx.get("rerun_data"), "compute.backend_service"
         )
         if not handle_operation_ret["result"]:
             result["comment"] += handle_operation_ret["comment"]
```

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/disk.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/firewall.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/firewall.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/forwarding_rule.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/forwarding_rule.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/health_check.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/health_check.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/image.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/instance_group.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/machine_image.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/machine_image.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/network.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/node_template.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/node_template.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/reservation.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/reservation.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/resource_policy.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/resource_policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/snapshot.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/snapshot.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/subnetwork.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/compute/target_pool.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/compute/target_pool.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_account.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/iam/service_account.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """State module for managing Service Accounts."""
 import copy
 from typing import Any
 from typing import Dict
 
 
 __contracts__ = ["resource"]
-RESOURCE_TYPE = "iam.projects.service_account"
-RESOURCE_TYPE_FULL = "gcp.iam.projects.service_account"
+RESOURCE_TYPE = "iam.service_account"
+RESOURCE_TYPE_FULL = f"gcp.{RESOURCE_TYPE}"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     resource_id: str = None,
@@ -65,68 +65,79 @@
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             resource_is_present:
-              gcp.iam.projects.service_account.present:
+              gcp.iam.service_account.present:
                 - name: value
                 - project_id: value
     """
     project_id = hub.tool.gcp.utils.get_project_from_account(ctx, project_id)
 
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
-    resource_type_camel = hub.tool.gcp.case.camel(RESOURCE_TYPE_FULL.split(".")[-1])
-
-    if hub.tool.gcp.resource_prop_utils.properties_mismatch_resource_id(
-        RESOURCE_TYPE, resource_id, {**locals(), resource_type_camel: name}
-    ):
-        result["comment"].append(
-            hub.tool.gcp.comment_utils.properties_mismatch_resource_id_comment(
-                RESOURCE_TYPE_FULL, name
-            )
-        )
-
     # Wait until resource is available in GCP
     if ctx.get("rerun_data"):
         service_account = ctx.get("rerun_data").get("old_state")
 
-        old_get_ret = await hub.exec.gcp.iam.projects.service_account.get(
+        old_get_ret = await hub.exec.gcp.iam.service_account.get(
             ctx, resource_id=service_account["resource_id"]
         )
 
         if not old_get_ret["result"]:
             result["comment"] += old_get_ret["comment"]
             result["rerun_data"] = ctx.get("rerun_data")
             return result
 
-        result["old_state"] = old_get_ret["ret"]
+        result["old_state"] = service_account
         result["new_state"] = old_get_ret["ret"]
 
         return result
 
+    get_resource_only_with_resource_id = hub.OPT.idem.get(
+        "get_resource_only_with_resource_id", False
+    )
+
     if resource_id:
-        old_get_ret = await hub.exec.gcp.iam.projects.service_account.get(
+        old_get_ret = await hub.exec.gcp.iam.service_account.get(
             ctx, resource_id=resource_id
         )
 
-        if not old_get_ret["result"]:
+        if not old_get_ret["result"] or (
+            not old_get_ret["ret"] and get_resource_only_with_resource_id
+        ):
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
 
         result["old_state"] = copy.deepcopy(copy.copy(old_get_ret["ret"]))
+    elif not get_resource_only_with_resource_id:
+        resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
+            RESOURCE_TYPE, locals()
+        )
+
+        get_ret = await hub.exec.gcp.iam.service_account.get(
+            ctx, resource_id=resource_id, name=name
+        )
+
+        if not get_ret["result"]:
+            result["result"] = False
+            result["comment"] += get_ret["comment"]
+            return result
+
+        if get_ret["ret"]:
+            result["old_state"] = get_ret["ret"]
 
     if result["old_state"]:
         new_state = {
             "name": name,
             "resource_id": resource_id,
             "project_id": project_id,
             "unique_id": unique_id,
@@ -139,14 +150,15 @@
         }
         new_state = {k: v for (k, v) in new_state.items() if v is not None}
 
         changes = hub.tool.gcp.utils.compare_states(
             result["old_state"],
             new_state,
             RESOURCE_TYPE,
+            additional_exclude_paths=["name"],
         )
         if not changes:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.up_to_date_comment(RESOURCE_TYPE_FULL, name)
             )
             result["new_state"] = result["old_state"]
             return result
@@ -166,46 +178,54 @@
                 )
             )
             result["new_state"] = result["old_state"]
             return result
 
         update_mask = []
         service_account = {}
-        if display_name:
+        if display_name is not None and display_name != result["old_state"].get(
+            "display_name"
+        ):
             service_account["display_name"] = display_name
             update_mask.append("displayName")
-        if description:
+        if description is not None and description != result["old_state"].get(
+            "description"
+        ):
             service_account["description"] = description
             update_mask.append("description")
 
         if ctx["test"]:
             result["comment"].append(
                 hub.tool.gcp.comment_utils.would_update_comment(
                     RESOURCE_TYPE_FULL, result["old_state"]["resource_id"]
                 )
             )
             result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
                 {**result["old_state"], **service_account}
             )
             return result
 
-        patch_ret = await hub.exec.gcp_api.client.iam.projects.service_account.patch(
+        patch_ret = await hub.exec.gcp_api.client.iam.service_account.patch(
             ctx,
             name=resource_id,
             body={
                 "service_account": service_account,
                 "update_mask": ",".join(update_mask),
             },
         )
         if not patch_ret["result"]:
             result["result"] = False
             result["comment"] += patch_ret["comment"]
             return result
 
-        result["new_state"] = {**result["old_state"], **patch_ret["ret"]}
+        result["new_state"] = {
+            **result["old_state"],
+            **patch_ret["ret"],
+            **service_account,
+        }
         result["comment"].append(
             hub.tool.gcp.comment_utils.update_comment(
                 RESOURCE_TYPE_FULL, result["new_state"]["resource_id"]
             )
         )
         return result
     else:
@@ -237,15 +257,15 @@
 
         resource_body = {"account_id": account_id}
         service_account = {"display_name": display_name, "description": description}
         service_account = {k: v for (k, v) in service_account.items() if v is not None}
         if service_account:
             resource_body["service_account"] = service_account
 
-        create_ret = await hub.exec.gcp_api.client.iam.projects.service_account.create(
+        create_ret = await hub.exec.gcp_api.client.iam.service_account.create(
             ctx, name=f"projects/{project_id}", body=resource_body
         )
 
         if not create_ret["result"]:
             result["result"] = False
             result["comment"] += create_ret["comment"]
             return result
@@ -278,16 +298,17 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        resource_is_absent:
-          gcp.iam.projects.service_account.absent
+            resource_is_absent:
+              gcp.iam.service_account.absent:
+              - resource_id: resource-id
     """
     result = {
         "result": True,
         "old_state": ctx.get("old_state"),
         "new_state": None,
         "name": name,
         "comment": [],
@@ -296,17 +317,15 @@
     if not resource_id:
         # we don't have enough information to know what to delete
         result["comment"].append(
             hub.tool.gcp.comment_utils.already_absent_comment(RESOURCE_TYPE_FULL, name)
         )
         return result
 
-    get_ret = await hub.exec.gcp.iam.projects.service_account.get(
-        ctx, resource_id=resource_id
-    )
+    get_ret = await hub.exec.gcp.iam.service_account.get(ctx, resource_id=resource_id)
 
     if not get_ret["result"]:
         result["result"] = False
         result["comment"].append(
             hub.tool.gcp.comment_utils.resource_not_found_comment(
                 RESOURCE_TYPE_FULL, resource_id
             )
@@ -324,15 +343,15 @@
 
     if ctx["test"]:
         result["comment"].append(
             hub.tool.gcp.comment_utils.would_delete_comment(RESOURCE_TYPE_FULL, name)
         )
         return result
 
-    del_ret = await hub.exec.gcp_api.client.iam.projects.service_account.delete(
+    del_ret = await hub.exec.gcp_api.client.iam.service_account.delete(
         ctx, name=resource_id
     )
 
     if not del_ret["result"]:
         result["result"] = False
         result["comment"].extend(del_ret["comment"])
         return result
@@ -351,33 +370,33 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.iam.projects.service_accounts
+            $ idem describe gcp.iam.service_accounts
     """
     result = {}
 
-    describe_ret = await hub.exec.gcp.iam.projects.service_account.list(
+    describe_ret = await hub.exec.gcp.iam.service_account.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not describe_ret["result"]:
         hub.log.debug(
-            f"Could not describe gcp.iam.projects.service_account {describe_ret['comment']}"
+            f"Could not describe gcp.iam.service_account {describe_ret['comment']}"
         )
         return {}
 
     for resource in describe_ret["ret"]:
         resource_id = resource.get("resource_id")
 
         result[resource_id] = {
-            "gcp.iam.projects.service_account.present": [
+            "gcp.iam.service_account.present": [
                 {parameter_key: parameter_value}
                 for parameter_key, parameter_value in resource.items()
             ]
         }
 
     return result
```

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/iam/projects/service_accounts/key.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/iam/service_account_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """State module for managing ServiceAccountKeys."""
 from typing import Any
 from typing import Dict
 
 __contracts__ = ["resource"]
-RESOURCE_TYPE = "iam.projects.service_accounts.key"
-RESOURCE_TYPE_FULL = "gcp.iam.projects.service_accounts.key"
+RESOURCE_TYPE = "iam.service_account_key"
+RESOURCE_TYPE_FULL = f"gcp.{RESOURCE_TYPE}"
 
 
 async def present(
     hub,
     ctx,
     name: str,
     resource_id: str = None,
@@ -36,29 +36,29 @@
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
             resource_is_present:
-              gcp.iam.projects.service_accounts.key.present:
+              gcp.iam.service_account_key.present:
               - private_key_type: TYPE_PKCS12_FILE
               - key_algorithm: KEY_ALG_RSA_2048
               - service_account_id: projects/project/serviceAccounts/test@test.iam.gserviceaccount.com
     """
     result = {
         "result": True,
         "old_state": None,
         "new_state": None,
         "name": name,
         "comment": [],
     }
 
     if resource_id:
-        old_get_ret = await hub.exec.gcp.iam.projects.service_accounts.key.get(
+        old_get_ret = await hub.exec.gcp.iam.service_account_key.get(
             ctx, resource_id=resource_id
         )
 
         if not old_get_ret["result"] or (not old_get_ret["ret"] and ctx["rerun_data"]):
             result["result"] = False
             result["comment"] += old_get_ret["comment"]
             return result
@@ -114,20 +114,18 @@
             result["new_state"] = hub.tool.gcp.sanitizers.sanitize_resource_urls(
                 resource_body
             )
             result["new_state"]["resource_id"] = resource_id
             return result
 
         # Create
-        create_ret = (
-            await hub.exec.gcp_api.client.iam.projects.service_accounts.key.create(
-                ctx,
-                name=service_account_id,
-                body=resource_body,
-            )
+        create_ret = await hub.exec.gcp_api.client.iam.service_account_key.create(
+            ctx,
+            name=service_account_id,
+            body=resource_body,
         )
         if not create_ret["result"] or not create_ret["ret"]:
             result["result"] = False
             if create_ret["comment"] and next(
                 (
                     comment
                     for comment in create_ret["comment"]
@@ -172,16 +170,17 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: sls
 
-        resource_is_absent:
-          gcp.iam.projects.service_accounts.key.absent
+            resource_is_absent:
+              gcp.iam.service_account_key.absent:
+              - resource_id: resource-id
     """
     result = {
         "result": True,
         "old_state": ctx.get("old_state"),
         "new_state": None,
         "name": name,
         "comment": [],
@@ -190,15 +189,15 @@
     if not resource_id:
         # we don't have enough information to know what to delete
         result["comment"].append(
             hub.tool.gcp.comment_utils.already_absent_comment(RESOURCE_TYPE_FULL, name)
         )
         return result
 
-    get_ret = await hub.exec.gcp.iam.projects.service_accounts.key.get(
+    get_ret = await hub.exec.gcp.iam.service_account_key.get(
         ctx, resource_id=resource_id
     )
 
     if not get_ret["result"]:
         result["result"] = False
         result["comment"].append(
             hub.tool.gcp.comment_utils.resource_not_found_comment(
@@ -218,15 +217,15 @@
 
     if ctx["test"]:
         result["comment"].append(
             hub.tool.gcp.comment_utils.would_delete_comment(RESOURCE_TYPE_FULL, name)
         )
         return result
 
-    del_ret = await hub.exec.gcp_api.client.iam.projects.service_accounts.key.delete(
+    del_ret = await hub.exec.gcp_api.client.iam.service_account_key.delete(
         ctx, name=resource_id
     )
 
     if not del_ret["result"]:
         result["result"] = False
         result["comment"].extend(del_ret["comment"])
         return result
@@ -245,44 +244,44 @@
 
     Returns:
         Dict[str, Any]
 
     Examples:
         .. code-block:: bash
 
-            $ idem describe gcp.iam.projects.service_accounts.key
+            $ idem describe gcp.iam.service_account_key
     """
     result = {}
 
-    list_accounts_ret = await hub.exec.gcp.iam.projects.service_account.list(
+    list_accounts_ret = await hub.exec.gcp.iam.service_account.list(
         ctx, project=ctx.acct.project_id
     )
 
     if not list_accounts_ret["result"]:
         hub.log.debug(
             f"Could not describe {RESOURCE_TYPE_FULL} {list_accounts_ret['comment']}"
         )
         return result
 
     for resource in list_accounts_ret["ret"]:
         sa_resource_id = resource.get("resource_id")
 
-        key_ret = await hub.exec.gcp.iam.projects.service_accounts.key.list(
+        key_ret = await hub.exec.gcp.iam.service_account_key.list(
             ctx, project=ctx.acct.project_id, sa_resource_id=sa_resource_id
         )
 
         if not key_ret["result"]:
             hub.log.debug(
                 f"Could not describe {RESOURCE_TYPE_FULL} in {sa_resource_id}: {key_ret['comment']}"
             )
         else:
             for service_account_key in key_ret["ret"]:
                 resource_id = service_account_key.get("resource_id")
                 result[resource_id] = {
-                    "gcp.iam.projects.service_accounts.key.present": [
+                    "gcp.iam.service_account_key.present": [
                         {parameter_key: parameter_value}
                         for parameter_key, parameter_value in service_account_key.items()
                     ]
                 }
 
     return result
```

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/recursive_contracts/init.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/recursive_contracts/init.py`

 * *Files 8% similar despite different names*

```diff
@@ -171,25 +171,14 @@
             else:
                 result["comment"].append(
                     hub.tool.gcp.comment_utils.create_comment(
                         gcp_service_resource_type, name
                     )
                 )
 
-            ctx_kwargs = {k: v for (k, v) in ctx.kwargs.items() if v is not None}
-            diff = hub.tool.gcp.utils.compare_states(
-                result["new_state"], ctx_kwargs, service_resource_type
-            )
-            values_mismatch: set = diff.get("relevant_changes")
-            if values_mismatch:
-                values_mismatch.discard("root['ctx']")
-                if values_mismatch:
-                    result["comment"].append(
-                        f"Values mismatch between actual and desired states: {values_mismatch}"
-                    )
             return result
 
         result["old_state"] = old_get_ret["ret"]
     elif not get_resource_only_with_resource_id:
         resource_id = hub.tool.gcp.resource_prop_utils.construct_resource_id(
             service_resource_type, local_params
         )
@@ -226,31 +215,51 @@
         hub: The redistributed pop central hub. The root of the namespace that pop operates on.
         ctx: Invocation context for this command.
 
     Returns:
         The changes with removed exclude paths from them.
 
     """
+    state_ctx = ctx.kwargs.get("ctx")
     if ctx.ret and "old_state" in ctx.ret and "new_state" in ctx.ret:
         old_state = ctx.ret.get("old_state")
         new_state = ctx.ret.get("new_state")
 
-        state_ctx = ctx.kwargs.get("ctx")
         resource_state_path = state_ctx.get("tag").split("_|")[0]
         service_resource_type = (
             hub.tool.gcp.resource_prop_utils.get_service_resource_type(
                 resource_state_path
             )
         )
 
         changes = hub.tool.gcp.utils.compare_changes(
             old_state, new_state, service_resource_type
         )
         ctx.ret["changes"] = changes
 
+    if (
+        ctx.ret
+        and not state_ctx.get("test")
+        and ctx.ret.get("new_state")
+        and ctx.ret.get("result")
+    ):
+        # Handle properties mismatch between desired and achieved state
+        ctx_kwargs = {k: v for (k, v) in ctx.kwargs.items() if v is not None}
+        diff = hub.tool.gcp.utils.compare_states(
+            ctx.ret["new_state"], ctx_kwargs, service_resource_type
+        )
+        values_mismatch: set = diff.get("relevant_changes")
+        if values_mismatch:
+            values_mismatch.discard("root['ctx']")
+            values_mismatch.discard("root['project']")
+            if values_mismatch:
+                ctx.ret["comment"].append(
+                    f"Values mismatch between actual and desired states: {values_mismatch}"
+                )
+
 
 async def call_absent(hub, ctx):
     r"""Wrapper for absent function.
 
     This method handles the parameters given in the ctx and deletes a resource only if
     the parameters are valid and the resource can be found using them.
```

### Comparing `idem_gcp-1.2.0/idem_gcp/states/gcp/storage/bucket.py` & `idem_gcp-2.0.0/idem_gcp/states/gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/case.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/case.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/cloudkms/patch.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/cloudkms/patch.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/comment_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/disk.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/disk.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/instance.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/instance_group.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/instance_group.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/network.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/network.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/compute/subnetwork.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/compute/subnetwork.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/conversion_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_context.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/exec_context.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/exec_param.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/exec_param.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/generic_exec.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/generic_exec.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/post_exec/item_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/post_exec/operation_processor.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/function_getter.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/parameter_sanitizer.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/generate/operators/pre_exec/resource_id_extractor.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/hub_resolver.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/hub_resolver.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/init.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/init.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/operation_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/operation_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/policy.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/policy.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/resolver.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/resolver.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/resource_prop_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/resource_prop_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -339,46 +339,36 @@
                 hub.tool.gcp.resource_prop_utils.parse_link_to_resource_id(
                     name, resource_type, log_warnings=False
                 )
                 is not None
             ):
                 return name
         except ValueError:
-            ...
+            pass
 
     filtered_without_none_properties = (
         {k: v for k, v in input_props.items() if v is not None}
         if input_props is not None
         else {}
     )
     resource_paths: List[str] = hub.tool.gcp.resource_prop_utils.get_resource_paths(
         resource_type
     )
-    result = None
     for path in resource_paths:
         try:
             r = path.format(**filtered_without_none_properties)
-            if r.find("{") != -1 or r.find("}") != -1:
-                # not fully matched
-                r = None
+            if r.find("{") == -1 and r.find("}") == -1:
+                # fully matched
+                return r
         except KeyError:
-            r = None
-        if r:
-            if result:
-                msg = f"Could not construct resource ID because multiple resource paths of {resource_type} match the input arguments."
-                hub.log.error(msg)
-                return None
-            result = r
-
-    if not result:
-        msg = f"Could not construct resource ID because no resource paths of {resource_type} match the input arguments."
-        hub.log.warning(msg)
-        return None
+            ...
 
-    return result
+    msg = f"Could not construct resource ID because no resource paths of {resource_type} match the input arguments."
+    hub.log.warning(msg)
+    return None
 
 
 def parse_link_to_zone(hub, link: str) -> str:
     return link.split("/")[-1]
 
 
 def get_path_parameters_for_path(hub, resource_path: str) -> Set[str]:
```

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/sanitizers.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/sanitizers.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/finding.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/finding.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/results_collector.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/results_collector.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/schema_compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/schema_naming_checker.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/schema/scm_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/schema/scm_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/state_comparison_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/state_operation_utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/state_operation_utils.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/storage/bucket.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/storage/bucket.py`

 * *Files identical despite different names*

### Comparing `idem_gcp-1.2.0/idem_gcp/tool/gcp/utils.py` & `idem_gcp-2.0.0/idem_gcp/tool/gcp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,21 @@
     if not dictionary_items_removed:
         return relevant_items_removed
 
     defined_relevant_dict_items_removed = (
         hub.tool.gcp.resource_prop_utils.get_relevant_dict_items_removed(resource_type)
     )
 
+    # Example:
+    # Relevant items removed are the dictionary items of compute.instance property labels
+    # Property -> [compute.instance] -> labels.dictKeysPlaceholder
+    # As dict label keys are user defined, we mark them with the dictKeysPlaceholder in properties.yaml
+    # Every property from properties.yaml is converted from camel to snake case -> dict_keys_placeholder
+    # Regex -> "^root\\['labels'\\]\\['\\w+'\\]$"
+    # Match -> "root['labels']['label_key_example']"
     defined_relevant_dict_items_removed_regexes = [
         _build_deep_diff_property_regex_pattern(x)
         for x in defined_relevant_dict_items_removed
     ]
 
     for item in dictionary_items_removed:
         # check if the removed item matches with one of the properties which removal is relevant
@@ -304,15 +311,15 @@
 
     properties = source.split(".")
     for prop in properties:
         if "[]" in prop:
             prop_name = prop.replace("[]", "")
             result += f"\\['{prop_name}'\\]\\[\\d+\\]"
         if "dict_keys_placeholder" == prop:
-            prop_name = prop.replace("dict_keys_placeholder", "\\['\\w+'\\]")
+            prop_name = prop.replace("dict_keys_placeholder", "\\['.+'\\]")
             result += prop_name
         else:
             result += f"\\['{prop}'\\]"
 
     # mark the regex ending
     result += "$"
     return re.compile(result)
```

### Comparing `idem_gcp-1.2.0/idem_gcp.egg-info/PKG-INFO` & `idem_gcp-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: idem-gcp
-Version: 1.2.0
+Name: idem_gcp
+Version: 2.0.0
 Summary: GCP Cloud Provider for Idem
 Home-page: https://gitlab.com/vmware/idem/idem-gcp
 Author: VMware, Inc.
 Author-email: idemproject@vmware.com
 License: Apache Software License 2.0
 Project-URL: Code, https://gitlab.com/vmware/idem/idem-gcp
 Project-URL: Issue tracker, https://gitlab.com/vmware/idem/idem-gcp/-/issues
```

### Comparing `idem_gcp-1.2.0/idem_gcp.egg-info/SOURCES.txt` & `idem_gcp-2.0.0/idem_gcp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 idem_gcp/exec/gcp/compute/reservation.py
 idem_gcp/exec/gcp/compute/resource_policy.py
 idem_gcp/exec/gcp/compute/snapshot.py
 idem_gcp/exec/gcp/compute/subnetwork.py
 idem_gcp/exec/gcp/compute/target_pool.py
 idem_gcp/exec/gcp/compute/zone.py
 idem_gcp/exec/gcp/contracts/init.py
-idem_gcp/exec/gcp/iam/projects/service_account.py
-idem_gcp/exec/gcp/iam/projects/service_accounts/key.py
+idem_gcp/exec/gcp/iam/service_account.py
+idem_gcp/exec/gcp/iam/service_account_key.py
 idem_gcp/exec/gcp/storage/bucket.py
 idem_gcp/exec/gcp_api/init.py
 idem_gcp/helpers/exc.py
 idem_gcp/helpers/log.py
 idem_gcp/helpers/returns.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/init.py
 idem_gcp/metadata/gcp/cloudkms/projects/locations/key_rings/init.py
@@ -73,16 +73,16 @@
 idem_gcp/metadata/gcp/compute/reservation.py
 idem_gcp/metadata/gcp/compute/resource_policy.py
 idem_gcp/metadata/gcp/compute/snapshot.py
 idem_gcp/metadata/gcp/compute/subnetwork.py
 idem_gcp/metadata/gcp/compute/target_pool.py
 idem_gcp/metadata/gcp/compute/zone.py
 idem_gcp/metadata/gcp/compute/zone_operation.py
-idem_gcp/metadata/gcp/iam/projects/service_account.py
-idem_gcp/metadata/gcp/iam/projects/service_accounts/key.py
+idem_gcp/metadata/gcp/iam/service_account.py
+idem_gcp/metadata/gcp/iam/service_account_key.py
 idem_gcp/metadata/gcp/storage/bucket.py
 idem_gcp/metadata/gcp/storage/objectAccessControls.py
 idem_gcp/resources/properties.yaml
 idem_gcp/states/gcp/init.py
 idem_gcp/states/gcp/cloudkms/crypto_key.py
 idem_gcp/states/gcp/cloudkms/crypto_key_version.py
 idem_gcp/states/gcp/cloudkms/import_job.py
@@ -100,29 +100,28 @@
 idem_gcp/states/gcp/compute/network.py
 idem_gcp/states/gcp/compute/node_template.py
 idem_gcp/states/gcp/compute/reservation.py
 idem_gcp/states/gcp/compute/resource_policy.py
 idem_gcp/states/gcp/compute/snapshot.py
 idem_gcp/states/gcp/compute/subnetwork.py
 idem_gcp/states/gcp/compute/target_pool.py
-idem_gcp/states/gcp/iam/projects/service_account.py
-idem_gcp/states/gcp/iam/projects/service_accounts/key.py
+idem_gcp/states/gcp/iam/service_account.py
+idem_gcp/states/gcp/iam/service_account_key.py
 idem_gcp/states/gcp/recursive_contracts/init.py
 idem_gcp/states/gcp/storage/bucket.py
 idem_gcp/tool/gcp/case.py
 idem_gcp/tool/gcp/comment_utils.py
 idem_gcp/tool/gcp/conversion_utils.py
 idem_gcp/tool/gcp/hub_resolver.py
 idem_gcp/tool/gcp/init.py
 idem_gcp/tool/gcp/operation_utils.py
 idem_gcp/tool/gcp/policy.py
 idem_gcp/tool/gcp/resolver.py
 idem_gcp/tool/gcp/resource_prop_utils.py
 idem_gcp/tool/gcp/sanitizers.py
-idem_gcp/tool/gcp/session.py
 idem_gcp/tool/gcp/state_comparison_utils.py
 idem_gcp/tool/gcp/state_operation_utils.py
 idem_gcp/tool/gcp/utils.py
 idem_gcp/tool/gcp/cloudkms/crypto_key_version_utils.py
 idem_gcp/tool/gcp/cloudkms/patch.py
 idem_gcp/tool/gcp/compute/disk.py
 idem_gcp/tool/gcp/compute/instance.py
```

### Comparing `idem_gcp-1.2.0/setup.py` & `idem_gcp-2.0.0/setup.py`

 * *Files identical despite different names*

