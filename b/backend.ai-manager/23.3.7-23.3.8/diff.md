# Comparing `tmp/backend.ai-manager-23.3.7.tar.gz` & `tmp/backend.ai-manager-23.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.7.tar", last modified: Mon Jul  3 16:26:16 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.8.tar", last modified: Thu Jul  6 04:38:16 2023, max compression
```

## Comparing `backend.ai-manager-23.3.7.tar` & `backend.ai-manager-23.3.8.tar`

### file list

```diff
@@ -1,250 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.702409 backend.ai-manager-23.3.7/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.702409 backend.ai-manager-23.3.7/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.706410 backend.ai-manager-23.3.7/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   121225 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.710409 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.714409 backend.ai-manager-23.3.7/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.714409 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    34759 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54934 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    56694 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    43458 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61786 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    30006 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/ai/backend/manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-03 16:26:16.000000 backend.ai-manager-23.3.7/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:26:16.730410 backend.ai-manager-23.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-03 16:26:15.000000 backend.ai-manager-23.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.800408 backend.ai-manager-23.3.8/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.800408 backend.ai-manager-23.3.8/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.804407 backend.ai-manager-23.3.8/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.804407 backend.ai-manager-23.3.8/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121225 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.820408 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34759 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54934 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57492 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62224 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30221 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/setup.py
```

### Comparing `backend.ai-manager-23.3.7/PKG-INFO` & `backend.ai-manager-23.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/service.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.8/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.8/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/config.py` & `backend.ai-manager-23.3.8/ai/backend/manager/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/harbor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/defs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.8/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.8/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/ordering.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/routing.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     batch_result_in_session,
 )
 from .group import GroupRow
 from .kernel import ComputeContainer, KernelRow, KernelStatus
 from .minilang.ordering import OrderSpecItem, QueryOrderParser
 from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
 from .user import UserRow
-from .utils import ExtendedAsyncSAEngine, execute_with_retry, sql_json_merge
+from .utils import ExtendedAsyncSAEngine, agg_to_array, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Row
 
     from .gql import GraphQueryContext
 
 
@@ -551,14 +551,15 @@
         "cluster_mode",
         sa.String(length=16),
         nullable=False,
         default=ClusterMode.SINGLE_NODE,
         server_default=ClusterMode.SINGLE_NODE.name,
     )
     cluster_size = sa.Column("cluster_size", sa.Integer, nullable=False, default=1)
+    agent_ids = sa.Column("agent_ids", sa.ARRAY(sa.String), nullable=True)
     kernels = relationship("KernelRow", back_populates="session")
 
     # Resource ownership
     scaling_group_name = sa.Column(
         "scaling_group_name", sa.ForeignKey("scaling_groups.name"), index=True, nullable=True
     )
     scaling_group = relationship("ScalingGroupRow", back_populates="sessions")
@@ -1242,14 +1243,15 @@
     startup_command = graphene.String()
     result = graphene.String()
     commit_status = graphene.String()
     abusing_reports = graphene.List(lambda: graphene.JSONString)
     idle_checks = graphene.JSONString()
 
     # resources
+    agent_ids = graphene.List(lambda: graphene.String)
     resource_opts = graphene.JSONString()
     scaling_group = graphene.String()
     service_ports = graphene.JSONString()
     mounts = graphene.List(lambda: graphene.String)
     vfolder_mounts = graphene.List(lambda: graphene.String)
     occupying_slots = graphene.JSONString()
     occupied_slots = graphene.JSONString()  # legacy
@@ -1307,14 +1309,15 @@
             "status_history": row.status_history or {},
             "created_at": row.created_at,
             "terminated_at": row.terminated_at,
             "starts_at": row.starts_at,
             "startup_command": row.startup_command,
             "result": row.result.name,
             # resources
+            "agent_ids": row.agent_ids,
             "scaling_group": row.scaling_group_name,
             "service_ports": row.main_kernel.service_ports,
             "mounts": [mount.name for mount in row.vfolder_mounts],
             "vfolder_mounts": row.vfolder_mounts,
             # statistics
             "num_queries": row.num_queries,
         }
@@ -1415,16 +1418,17 @@
         graph_ctx: GraphQueryContext = info.context
         return await graph_ctx.idle_checker_host.get_idle_check_report(self.session_id)
 
     _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", lambda s: SessionTypes[s]),
         "name": ("sessions_name", None),
+        "agent_ids": ("sessions_agent_ids", None),
         "domain_name": ("sessions_domain_name", None),
-        "group_name": ("groups_name", None),
+        "group_name": ("group_name", None),
         "user_email": ("users_email", None),
         "full_name": ("users_full_name", None),
         "access_key": ("sessions_access_key", None),
         "scaling_group": ("sessions_scaling_group_name", None),
         "cluster_mode": ("sessions_cluster_mode", lambda s: ClusterMode[s]),
         "cluster_size": ("sessions_cluster_size", None),
         "status": ("sessions_status", lambda s: SessionStatus[s]),
@@ -1438,16 +1442,17 @@
 
     _queryorder_colmap: Mapping[str, OrderSpecItem] = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", None),
         "name": ("sessions_name", None),
         # "image": "image",
         # "architecture": "architecture",
+        "agent_ids": ("sessions_agent_ids", None),
         "domain_name": ("sessions_domain_name", None),
-        "group_name": ("groups_name", None),
+        "group_name": ("group_name", None),
         "user_email": ("users_email", None),
         "full_name": ("users_full_name", None),
         "access_key": ("sessions_access_key", None),
         "scaling_group": ("sessions_scaling_group_name", None),
         "cluster_mode": ("sessions_cluster_mode", None),
         # "cluster_template": "cluster_template",
         "cluster_size": ("sessions_cluster_size", None),
@@ -1470,18 +1475,21 @@
         status: Optional[str] = None,
         filter: Optional[str] = None,
     ) -> int:
         if isinstance(status, str):
             status_list = [SessionStatus[s] for s in status.split(",")]
         elif isinstance(status, SessionStatus):
             status_list = [status]
-        j = sa.join(SessionRow, GroupRow, SessionRow.group_id == GroupRow.id).join(
-            UserRow, SessionRow.user_uuid == UserRow.uuid
+        j = (
+            # joins with GroupRow and UserRow do not need to be LEFT OUTER JOIN since those foreign keys are not nullable.
+            sa.join(SessionRow, GroupRow, SessionRow.group_id == GroupRow.id)
+            .join(UserRow, SessionRow.user_uuid == UserRow.uuid)
+            .join(KernelRow, SessionRow.id == KernelRow.session_id)
         )
-        query = sa.select([sa.func.count()]).select_from(j)
+        query = sa.select([sa.func.count(sa.distinct(SessionRow.id))]).select_from(j)
         if domain_name is not None:
             query = query.where(SessionRow.domain_name == domain_name)
         if group_id is not None:
             query = query.where(SessionRow.group_id == group_id)
         if access_key is not None:
             query = query.where(SessionRow.access_key == access_key)
         if status is not None:
@@ -1509,26 +1517,30 @@
     ) -> Sequence[ComputeSession | None]:
         if status is None:
             status_list = None
         elif isinstance(status, str):
             status_list = [SessionStatus[s] for s in status.split(",")]
         elif isinstance(status, SessionStatus):
             status_list = [status]
-        j = sa.join(SessionRow, GroupRow, SessionRow.group_id == GroupRow.id).join(
-            UserRow, SessionRow.user_uuid == UserRow.uuid
+        j = (
+            # joins with GroupRow and UserRow do not need to be LEFT OUTER JOIN since those foreign keys are not nullable.
+            sa.join(SessionRow, GroupRow, SessionRow.group_id == GroupRow.id).join(
+                UserRow, SessionRow.user_uuid == UserRow.uuid
+            )
         )
         query = (
             sa.select(
                 SessionRow,
-                GroupRow.name.label("group_name"),
+                agg_to_array(GroupRow.name).label("group_name"),
                 UserRow.email,
                 UserRow.full_name,
             )
             .select_from(j)
-            .options(selectinload(SessionRow.kernels))
+            .options(selectinload(SessionRow.kernels.and_(KernelRow.cluster_role == DEFAULT_ROLE)))
+            .group_by(SessionRow, UserRow.email, UserRow.full_name)
             .limit(limit)
             .offset(offset)
         )
         if domain_name is not None:
             query = query.where(SessionRow.domain_name == domain_name)
         if group_id is not None:
             query = query.where(SessionRow.group_id == group_id)
```

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.8/ai/backend/manager/models/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/openapi.py` & `backend.ai-manager-23.3.8/ai/backend/manager/openapi.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.8/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.8/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.8/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.8/ai/backend/manager/registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -715,14 +715,15 @@
                     )
                     await kernel_db_sess.execute(query)
 
             await execute_with_retry(_update_generic_failure)
             raise
 
         async def _finalize_scheduled() -> None:
+            agent_ids: list[AgentId] = []
             async with self.db.begin_session() as db_sess:
                 now = datetime.now(tzutc())
                 kernel_query = (
                     sa.update(KernelRow)
                     .values(
                         agent=agent_alloc_ctx.agent_id,
                         agent_addr=agent_alloc_ctx.agent_addr,
@@ -738,19 +739,22 @@
                                 KernelStatus.SCHEDULED.name: now.isoformat(),
                             },
                         ),
                     )
                     .where(KernelRow.session_id == sess_ctx.id)
                 )
                 await db_sess.execute(kernel_query)
+                if agent_alloc_ctx.agent_id is not None:
+                    agent_ids.append(agent_alloc_ctx.agent_id)
 
                 session_query = (
                     sa.update(SessionRow)
                     .values(
                         scaling_group_name=sgroup_name,
+                        agent_ids=agent_ids,
                         status=SessionStatus.SCHEDULED,
                         status_info="scheduled",
                         status_data={},
                         # status_changed=now,
                         status_history=sql_json_merge(
                             SessionRow.status_history,
                             (),
@@ -918,14 +922,15 @@
                     assert agent_alloc_ctx is not None
                     kernel_agent_bindings.append(KernelAgentBinding(kernel, agent_alloc_ctx, set()))
 
         assert len(kernel_agent_bindings) == len(sess_ctx.kernels)
         # Proceed to PREPARING only when all kernels are successfully scheduled.
 
         async def _finalize_scheduled() -> None:
+            agent_ids: list[AgentId] = []
             async with self.db.begin_session() as db_sess:
                 for binding in kernel_agent_bindings:
                     now = datetime.now(tzutc())
                     kernel_query = (
                         sa.update(KernelRow)
                         .values(
                             agent=binding.agent_alloc_ctx.agent_id,
@@ -942,19 +947,22 @@
                                     KernelStatus.SCHEDULED.name: now.isoformat(),
                                 },
                             ),
                         )
                         .where(KernelRow.session_id == sess_ctx.id)
                     )
                     await db_sess.execute(kernel_query)
+                    if binding.agent_alloc_ctx.agent_id is not None:
+                        agent_ids.append(binding.agent_alloc_ctx.agent_id)
 
                 session_query = (
                     sa.update(SessionRow)
                     .values(
                         scaling_group_name=sgroup_name,
+                        agent_ids=agent_ids,
                         status=SessionStatus.SCHEDULED,
                         status_info="scheduled",
                         status_data={},
                         # status_changed=now,
                         status_history=sql_json_merge(
                             SessionRow.status_history,
                             (),
```

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/server.py` & `backend.ai-manager-23.3.8/ai/backend/manager/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,30 @@
         # added session event webhook option to session creation API
         # added architecture option when making image aliases
         "v6.20220315",
         # added payload encryption / decryption on selected transfer
         "v6.20220615",
         # added config/resource-slots/details, model mgmt & serving APIs
         "v6.20230315",
+        # added quota scopes (per-user/per-project quota configs)
+        # added user & project resource policies
+        # deprecated per-vfolder quota configs (BREAKING)
+        "v7.20230615",
     ]
 )
 LATEST_REV_DATES: Final = {
     1: "20160915",
     2: "20170915",
     3: "20181215",
     4: "20190615",
     5: "20191215",
     6: "20230315",
+    7: "20230615",
 }
-LATEST_API_VERSION: Final = "v6.20230315"
+LATEST_API_VERSION: Final = "v7.20230615"
 
 log = BraceStyleAdapter(logging.getLogger(__spec__.name))  # type: ignore[name-defined]
 
 PUBLIC_INTERFACES: Final = [
     "pidx",
     "background_task_manager",
     "local_config",
```

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/types.py` & `backend.ai-manager-23.3.8/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/ai/backend/manager/utils.py` & `backend.ai-manager-23.3.8/ai/backend/manager/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.7
+Version: 23.3.8
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.7/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,15 @@
 ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
 ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
 ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
 ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
 ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
 ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
 ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
 ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
 ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
 ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
 ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
 ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
 ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
 ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
```

### Comparing `backend.ai-manager-23.3.7/backend.ai_manager.egg-info/requires.txt` & `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 aiohttp_sse>=2.0
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 alembic~=1.8.1
 async_timeout~=4.0
 attrs>=20.3
-backend.ai-cli==23.03.7
-backend.ai-common==23.03.7
-backend.ai-plugin==23.03.7
+backend.ai-cli==23.03.8
+backend.ai-common==23.03.8
+backend.ai-plugin==23.03.8
 callosum~=0.9.10
 click>=7.1.2
 cryptography>=2.8
 graphene~=2.1.9
 lark-parser~=0.11.3
 more-itertools~=8.13.0
 msgpack>=1.0.5rc1
```

### Comparing `backend.ai-manager-23.3.7/backend_shim.py` & `backend.ai-manager-23.3.8/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.7/setup.py` & `backend.ai-manager-23.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.7
+        """backend.ai-cli==23.03.8
 """,
-        """backend.ai-common==23.03.7
+        """backend.ai-common==23.03.8
 """,
-        """backend.ai-plugin==23.03.7
+        """backend.ai-plugin==23.03.8
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
@@ -378,11 +378,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.7
+    'version': """23.03.8
 """,
     'zip_safe': False,
 })
```

