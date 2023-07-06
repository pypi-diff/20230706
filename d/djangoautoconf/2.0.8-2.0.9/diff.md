# Comparing `tmp/djangoautoconf-2.0.8.tar.gz` & `tmp/djangoautoconf-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\djangoautoconf-2.0.8.tar", last modified: Tue Aug 30 08:22:05 2022, max compression
+gzip compressed data, was "dist\djangoautoconf-2.0.9.tar", last modified: Thu Jul  6 06:53:44 2023, max compression
```

## Comparing `djangoautoconf-2.0.8.tar` & `djangoautoconf-2.0.9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:05.215048 djangoautoconf-2.0.8/
--rw-rw-rw-   0        0        0      174 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/AUTHORS.rst
--rw-rw-rw-   0        0        0     3344 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0      160 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/HISTORY.rst
--rw-rw-rw-   0        0        0     1485 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/LICENSE
--rw-rw-rw-   0        0        0      188 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4059 2022-08-30 08:22:05.211052 djangoautoconf-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2328 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/README.rst
-drwxrwxrwx   0        0        0        0 2022-08-30 08:21:58.807870 djangoautoconf-2.0.8/djangoautoconf/
--rw-rw-rw-   0        0        0      145 2022-08-30 08:21:19.000000 djangoautoconf-2.0.8/djangoautoconf/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:21:58.977864 djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/__init__.py
--rw-rw-rw-   0        0        0     1950 2022-06-20 03:13:38.000000 djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/ajax_select_channel_generator.py
--rw-rw-rw-   0        0        0     2711 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/channel_creator_for_model.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:00.434411 djangoautoconf-2.0.8/djangoautoconf/auth/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/__init__.py
--rw-rw-rw-   0        0        0      748 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/ldap_backend_wrapper.py
--rw-rw-rw-   0        0        0     1281 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/login.py
--rw-rw-rw-   0        0        0      292 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/login_exceptions.py
--rw-rw-rw-   0        0        0      564 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/req_auth.py
--rw-rw-rw-   0        0        0       86 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/req_auth_base_backend.py
--rw-rw-rw-   0        0        0      827 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/req_auth_super_password_backend.py
--rw-rw-rw-   0        0        0      258 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/session_backend.py
--rw-rw-rw-   0        0        0      545 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auth/username_password_backend.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:01.636000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/__init__.py
--rw-rw-rw-   0        0        0      770 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/action_feature.py
--rw-rw-rw-   0        0        0      603 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/additional_attr.py
--rw-rw-rw-   0        0        0      567 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_attr_feature.py
--rw-rw-rw-   0        0        0      591 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_feature_base.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:01.970002 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/__init__.py
--rw-rw-rw-   0        0        0     3077 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/admin_tagging_feature.py
--rw-rw-rw-   0        0        0     1155 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/foreign_key_sort.py
--rw-rw-rw-   0        0        0     6260 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_register.py
--rw-rw-rw-   0        0        0      761 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/filter_horizontal_feature.py
--rw-rw-rw-   0        0        0      678 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/filter_item_feature.py
--rw-rw-rw-   0        0        0     1991 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/foreign_key_auto_complete.py
--rw-rw-rw-   0        0        0      937 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/guardian_feature.py
--rw-rw-rw-   0        0        0     1391 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/import_export_feature.py
--rw-rw-rw-   0        0        0     2831 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/list_and_search.py
--rw-rw-rw-   0        0        0      728 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/model_with_full_permission_feature.py
--rw-rw-rw-   0        0        0      660 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/reversion_feature.py
--rw-rw-rw-   0        0        0      541 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_signals.py
--rw-rw-rw-   0        0        0     6013 2022-08-30 06:14:11.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_urls.py
--rw-rw-rw-   0        0        0     3258 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_conf_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:02.173003 djangoautoconf-2.0.8/djangoautoconf/auto_detection/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_detection/__init__.py
--rw-rw-rw-   0        0        0      169 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_detection/default_routing.py
--rw-rw-rw-   0        0        0     1272 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/auto_detection/routing_auto_detection.py
--rw-rw-rw-   0        0        0     9224 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/base_setting_storage.py
--rw-rw-rw-   0        0        0     1512 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/base_settings.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:02.402011 djangoautoconf-2.0.8/djangoautoconf/class_based_views/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/__init__.py
--rw-rw-rw-   0        0        0     1987 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/ajax_views.py
--rw-rw-rw-   0        0        0     4015 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/create_view_factory.py
--rw-rw-rw-   0        0        0     2981 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/detail_with_inline_view.py
--rw-rw-rw-   0        0        0     1096 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/form_factory.py
--rw-rw-rw-   0        0        0     3045 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/class_based_views/template_view_factory.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:02.690013 djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/__init__.py
--rw-rw-rw-   0        0        0     1678 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/database_connection_maintainer.py
--rw-rw-rw-   0        0        0     3688 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/msg_process_cmd_base.py
--rw-rw-rw-   0        0        0     2822 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_adv_zip_template_loader.py
--rw-rw-rw-   0        0        0    10468 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_autoconf.py
--rw-rw-rw-   0        0        0     1410 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_dev_server_auto_conf.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:02.782021 djangoautoconf-2.0.8/djangoautoconf/django_rest_framework_utils/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_rest_framework_utils/__init__.py
--rw-rw-rw-   0        0        0     6242 2022-06-20 03:23:46.000000 djangoautoconf-2.0.8/djangoautoconf/django_rest_framework_utils/serializer_generator.py
--rw-rw-rw-   0        0        0     4233 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_setting_manager.py
--rw-rw-rw-   0        0        0     1541 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_utils.py
--rw-rw-rw-   0        0        0      932 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/django_zip_template_loader.py
--rw-rw-rw-   0        0        0     2668 2022-06-20 03:24:24.000000 djangoautoconf-2.0.8/djangoautoconf/djangoautoconf_settings.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:02.987016 djangoautoconf-2.0.8/djangoautoconf/keys_default/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/keys_default/__init__.py
--rw-rw-rw-   0        0        0       57 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/keys_default/admin_account_template.py
--rw-rw-rw-   0        0        0       44 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/keys_default/ldap_settings_template.py
--rw-rw-rw-   0        0        0     2465 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/local_key_manager.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:03.184023 djangoautoconf-2.0.8/djangoautoconf/log_utils/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/log_utils/__init__.py
--rw-rw-rw-   0        0        0      492 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/log_utils/log_path_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:03.274026 djangoautoconf-2.0.8/djangoautoconf/management/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:03.484025 djangoautoconf-2.0.8/djangoautoconf/management/commands/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/__init__.py
--rw-rw-rw-   0        0        0      363 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/collectcmd.py
--rw-rw-rw-   0        0        0      866 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/create_default_super_user.py
--rw-rw-rw-   0        0        0     1492 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/dump_settings.py
--rw-rw-rw-   0        0        0      920 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/remove_app_tables.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:03.564032 djangoautoconf-2.0.8/djangoautoconf/management/commands/web_manage_tools/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/web_manage_tools/__init__.py
--rw-rw-rw-   0        0        0      184 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/management/commands/web_manage_tools/user_creator.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:04.213034 djangoautoconf-2.0.8/djangoautoconf/model_utils/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/__init__.py
--rw-rw-rw-   0        0        0     5019 2022-06-20 03:15:07.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/adv_tastypie_resource.py
--rw-rw-rw-   0        0        0     2544 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/import_export_utils.py
--rw-rw-rw-   0        0        0      313 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/len_definitions.py
--rw-rw-rw-   0        0        0     2440 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/model_attr_utils.py
--rw-rw-rw-   0        0        0     3026 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/model_duplicator.py
--rw-rw-rw-   0        0        0     1969 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/model_reversion.py
--rw-rw-rw-   0        0        0     3736 2022-06-20 03:15:35.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/tastypie_utils.py
--rw-rw-rw-   0        0        0     1455 2022-06-20 03:23:46.000000 djangoautoconf-2.0.8/djangoautoconf/model_utils/url_for_models.py
--rw-rw-rw-   0        0        0      988 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/object_copier.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:04.376041 djangoautoconf-2.0.8/djangoautoconf/obs/
--rw-rw-rw-   0        0        0     3458 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/obs/auto_conf_admin_utils.py
--rw-rw-rw-   0        0        0      237 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/obs/dict_setting_storage.py
--rw-rw-rw-   0        0        0     3018 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/obs/version_mismatch_work_around.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:04.546039 djangoautoconf-2.0.8/djangoautoconf/project_template/
--rw-rw-rw-   0        0        0      166 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/project_template/admin.py
--rw-rw-rw-   0        0        0      217 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/project_template/urls.py
--rw-rw-rw-   0        0        0     3908 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/req_with_auth.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:04.757051 djangoautoconf-2.0.8/djangoautoconf/setting_utils/
--rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/setting_utils/__init__.py
--rw-rw-rw-   0        0        0     1309 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/setting_utils/app_folders.py
--rw-rw-rw-   0        0        0      473 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/setting_utils/app_module_utils.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:04.970050 djangoautoconf-2.0.8/djangoautoconf/settings_templates/
--rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/settings_templates/__init__.py
--rw-rw-rw-   0        0        0       43 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/settings_templates/github_api_keys_template.py
--rw-rw-rw-   0        0        0       69 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/settings_templates/smtp_account_template.py
--rw-rw-rw-   0        0        0       81 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/settings_templates/smtp_settings_template.py
--rw-rw-rw-   0        0        0      583 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/sqlite_database.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:22:05.203051 djangoautoconf-2.0.8/djangoautoconf/templates/
--rw-rw-rw-   0        0        0       74 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/templates/base.html
--rw-rw-rw-   0        0        0      760 2022-08-30 06:27:17.000000 djangoautoconf-2.0.8/djangoautoconf/templates/base_with_nav.html
--rw-rw-rw-   0        0        0     1608 2022-06-20 01:51:52.000000 djangoautoconf-2.0.8/djangoautoconf/templates/detail_with_inline_view.html
--rw-rw-rw-   0        0        0     1933 2022-06-20 03:12:14.000000 djangoautoconf-2.0.8/djangoautoconf/urls.py
-drwxrwxrwx   0        0        0        0 2022-08-30 08:21:58.877875 djangoautoconf-2.0.8/djangoautoconf.egg-info/
--rw-rw-rw-   0        0        0     4059 2022-08-30 08:21:55.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5082 2022-08-30 08:21:56.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-30 08:21:55.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-20 03:18:26.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      235 2022-08-30 08:21:55.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2022-08-30 08:21:55.000000 djangoautoconf-2.0.8/djangoautoconf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-30 08:22:05.215048 djangoautoconf-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3203 2022-06-20 03:23:46.000000 djangoautoconf-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.895767 djangoautoconf-2.0.9/
+-rw-rw-rw-   0        0        0      174 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/AUTHORS.rst
+-rw-rw-rw-   0        0        0     3344 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0      160 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/HISTORY.rst
+-rw-rw-rw-   0        0        0     1485 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0      188 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4059 2023-07-06 06:53:44.891764 djangoautoconf-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2328 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.168757 djangoautoconf-2.0.9/djangoautoconf/
+-rw-rw-rw-   0        0        0      145 2023-07-06 06:44:41.000000 djangoautoconf-2.0.9/djangoautoconf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.259758 djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/__init__.py
+-rw-rw-rw-   0        0        0     1950 2022-06-20 03:13:38.000000 djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/ajax_select_channel_generator.py
+-rw-rw-rw-   0        0        0     2711 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/channel_creator_for_model.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.340757 djangoautoconf-2.0.9/djangoautoconf/auth/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/__init__.py
+-rw-rw-rw-   0        0        0      748 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/ldap_backend_wrapper.py
+-rw-rw-rw-   0        0        0     1281 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/login.py
+-rw-rw-rw-   0        0        0      292 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/login_exceptions.py
+-rw-rw-rw-   0        0        0      564 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/req_auth.py
+-rw-rw-rw-   0        0        0       86 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/req_auth_base_backend.py
+-rw-rw-rw-   0        0        0      827 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/req_auth_super_password_backend.py
+-rw-rw-rw-   0        0        0      258 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/session_backend.py
+-rw-rw-rw-   0        0        0      545 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auth/username_password_backend.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.453757 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/__init__.py
+-rw-rw-rw-   0        0        0      770 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/action_feature.py
+-rw-rw-rw-   0        0        0      603 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/additional_attr.py
+-rw-rw-rw-   0        0        0      567 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_attr_feature.py
+-rw-rw-rw-   0        0        0      591 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_feature_base.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.481760 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/__init__.py
+-rw-rw-rw-   0        0        0     3077 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/admin_tagging_feature.py
+-rw-rw-rw-   0        0        0     1155 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/foreign_key_sort.py
+-rw-rw-rw-   0        0        0     6260 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_register.py
+-rw-rw-rw-   0        0        0      761 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/filter_horizontal_feature.py
+-rw-rw-rw-   0        0        0      678 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/filter_item_feature.py
+-rw-rw-rw-   0        0        0     1991 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/foreign_key_auto_complete.py
+-rw-rw-rw-   0        0        0      937 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/guardian_feature.py
+-rw-rw-rw-   0        0        0     1391 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/import_export_feature.py
+-rw-rw-rw-   0        0        0     2831 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/list_and_search.py
+-rw-rw-rw-   0        0        0      728 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/model_with_full_permission_feature.py
+-rw-rw-rw-   0        0        0      660 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/reversion_feature.py
+-rw-rw-rw-   0        0        0      541 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_signals.py
+-rw-rw-rw-   0        0        0     6013 2022-08-30 06:14:11.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_urls.py
+-rw-rw-rw-   0        0        0     3258 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_conf_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.502759 djangoautoconf-2.0.9/djangoautoconf/auto_detection/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_detection/__init__.py
+-rw-rw-rw-   0        0        0      169 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_detection/default_routing.py
+-rw-rw-rw-   0        0        0     1272 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/auto_detection/routing_auto_detection.py
+-rw-rw-rw-   0        0        0     9224 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/base_setting_storage.py
+-rw-rw-rw-   0        0        0     1512 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/base_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.552759 djangoautoconf-2.0.9/djangoautoconf/class_based_views/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/__init__.py
+-rw-rw-rw-   0        0        0     1987 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/ajax_views.py
+-rw-rw-rw-   0        0        0     4015 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/create_view_factory.py
+-rw-rw-rw-   0        0        0     2981 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/detail_with_inline_view.py
+-rw-rw-rw-   0        0        0     1096 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/form_factory.py
+-rw-rw-rw-   0        0        0     3045 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/class_based_views/template_view_factory.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.574768 djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/__init__.py
+-rw-rw-rw-   0        0        0     1678 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/database_connection_maintainer.py
+-rw-rw-rw-   0        0        0     3688 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/msg_process_cmd_base.py
+-rw-rw-rw-   0        0        0     2822 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_adv_zip_template_loader.py
+-rw-rw-rw-   0        0        0    10468 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_autoconf.py
+-rw-rw-rw-   0        0        0     1410 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_dev_server_auto_conf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.592763 djangoautoconf-2.0.9/djangoautoconf/django_rest_framework_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_rest_framework_utils/__init__.py
+-rw-rw-rw-   0        0        0     6242 2022-06-20 03:23:46.000000 djangoautoconf-2.0.9/djangoautoconf/django_rest_framework_utils/serializer_generator.py
+-rw-rw-rw-   0        0        0     4233 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_setting_manager.py
+-rw-rw-rw-   0        0        0     1571 2023-07-06 06:50:29.000000 djangoautoconf-2.0.9/djangoautoconf/django_utils.py
+-rw-rw-rw-   0        0        0      932 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/django_zip_template_loader.py
+-rw-rw-rw-   0        0        0     2668 2022-06-20 03:24:24.000000 djangoautoconf-2.0.9/djangoautoconf/djangoautoconf_settings.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.616759 djangoautoconf-2.0.9/djangoautoconf/keys_default/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/keys_default/__init__.py
+-rw-rw-rw-   0        0        0       57 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/keys_default/admin_account_template.py
+-rw-rw-rw-   0        0        0       44 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/keys_default/ldap_settings_template.py
+-rw-rw-rw-   0        0        0     2465 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/local_key_manager.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.633762 djangoautoconf-2.0.9/djangoautoconf/log_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/log_utils/__init__.py
+-rw-rw-rw-   0        0        0      492 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/log_utils/log_path_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.638760 djangoautoconf-2.0.9/djangoautoconf/management/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.674762 djangoautoconf-2.0.9/djangoautoconf/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/__init__.py
+-rw-rw-rw-   0        0        0      363 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/collectcmd.py
+-rw-rw-rw-   0        0        0      866 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/create_default_super_user.py
+-rw-rw-rw-   0        0        0     1492 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/dump_settings.py
+-rw-rw-rw-   0        0        0      920 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/remove_app_tables.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.691763 djangoautoconf-2.0.9/djangoautoconf/management/commands/web_manage_tools/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/web_manage_tools/__init__.py
+-rw-rw-rw-   0        0        0      184 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/management/commands/web_manage_tools/user_creator.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.768762 djangoautoconf-2.0.9/djangoautoconf/model_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/__init__.py
+-rw-rw-rw-   0        0        0     5019 2022-06-20 03:15:07.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/adv_tastypie_resource.py
+-rw-rw-rw-   0        0        0     2544 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/import_export_utils.py
+-rw-rw-rw-   0        0        0      313 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/len_definitions.py
+-rw-rw-rw-   0        0        0     2440 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/model_attr_utils.py
+-rw-rw-rw-   0        0        0     3026 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/model_duplicator.py
+-rw-rw-rw-   0        0        0     1969 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/model_reversion.py
+-rw-rw-rw-   0        0        0     3736 2022-06-20 03:15:35.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/tastypie_utils.py
+-rw-rw-rw-   0        0        0     1455 2022-06-20 03:23:46.000000 djangoautoconf-2.0.9/djangoautoconf/model_utils/url_for_models.py
+-rw-rw-rw-   0        0        0      988 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/object_copier.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.791763 djangoautoconf-2.0.9/djangoautoconf/obs/
+-rw-rw-rw-   0        0        0     3458 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/obs/auto_conf_admin_utils.py
+-rw-rw-rw-   0        0        0      237 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/obs/dict_setting_storage.py
+-rw-rw-rw-   0        0        0     3018 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/obs/version_mismatch_work_around.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.807766 djangoautoconf-2.0.9/djangoautoconf/project_template/
+-rw-rw-rw-   0        0        0      166 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/project_template/admin.py
+-rw-rw-rw-   0        0        0      217 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/project_template/urls.py
+-rw-rw-rw-   0        0        0     3908 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/req_with_auth.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.831776 djangoautoconf-2.0.9/djangoautoconf/setting_utils/
+-rw-rw-rw-   0        0        0        0 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/setting_utils/__init__.py
+-rw-rw-rw-   0        0        0     1309 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/setting_utils/app_folders.py
+-rw-rw-rw-   0        0        0      473 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/setting_utils/app_module_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.862772 djangoautoconf-2.0.9/djangoautoconf/settings_templates/
+-rw-rw-rw-   0        0        0       23 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/settings_templates/__init__.py
+-rw-rw-rw-   0        0        0       43 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/settings_templates/github_api_keys_template.py
+-rw-rw-rw-   0        0        0       69 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/settings_templates/smtp_account_template.py
+-rw-rw-rw-   0        0        0       81 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/settings_templates/smtp_settings_template.py
+-rw-rw-rw-   0        0        0      583 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/sqlite_database.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.885760 djangoautoconf-2.0.9/djangoautoconf/templates/
+-rw-rw-rw-   0        0        0       74 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/templates/base.html
+-rw-rw-rw-   0        0        0      760 2022-08-30 06:27:17.000000 djangoautoconf-2.0.9/djangoautoconf/templates/base_with_nav.html
+-rw-rw-rw-   0        0        0     1608 2022-06-20 01:51:52.000000 djangoautoconf-2.0.9/djangoautoconf/templates/detail_with_inline_view.html
+-rw-rw-rw-   0        0        0     1933 2022-06-20 03:12:14.000000 djangoautoconf-2.0.9/djangoautoconf/urls.py
+drwxrwxrwx   0        0        0        0 2023-07-06 06:53:44.238776 djangoautoconf-2.0.9/djangoautoconf.egg-info/
+-rw-rw-rw-   0        0        0     4059 2023-07-06 06:53:42.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5082 2023-07-06 06:53:43.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 06:53:42.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-20 03:18:26.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      235 2023-07-06 06:53:42.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-07-06 06:53:42.000000 djangoautoconf-2.0.9/djangoautoconf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-06 06:53:44.897785 djangoautoconf-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3203 2022-06-20 03:23:46.000000 djangoautoconf-2.0.9/setup.py
```

### Comparing `djangoautoconf-2.0.8/CONTRIBUTING.rst` & `djangoautoconf-2.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/LICENSE` & `djangoautoconf-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/PKG-INFO` & `djangoautoconf-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djangoautoconf
-Version: 2.0.8
+Version: 2.0.9
 Summary: Create a package to ease setting django project settings.
 Home-page: https://github.com/weijia/djangoautoconf
 Author: Richard Wang
 Author-email: richardwangwang@gmail.com
 License: BSD
 Description: ===============================
         Django AutoConf
```

### Comparing `djangoautoconf-2.0.8/README.rst` & `djangoautoconf-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/ajax_select_channel_generator.py` & `djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/ajax_select_channel_generator.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/ajax_select_utils/channel_creator_for_model.py` & `djangoautoconf-2.0.9/djangoautoconf/ajax_select_utils/channel_creator_for_model.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auth/ldap_backend_wrapper.py` & `djangoautoconf-2.0.9/djangoautoconf/auth/ldap_backend_wrapper.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auth/login.py` & `djangoautoconf-2.0.9/djangoautoconf/auth/login.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auth/req_auth.py` & `djangoautoconf-2.0.9/djangoautoconf/auth/req_auth.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auth/req_auth_super_password_backend.py` & `djangoautoconf-2.0.9/djangoautoconf/auth/req_auth_super_password_backend.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auth/username_password_backend.py` & `djangoautoconf-2.0.9/djangoautoconf/auth/username_password_backend.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/action_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/action_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/additional_attr.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/additional_attr.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_attr_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_attr_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_feature_base.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_feature_base.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/admin_tagging_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/admin_tagging_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_features/foreign_key_sort.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_features/foreign_key_sort.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/admin_register.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/admin_register.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/filter_horizontal_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/filter_horizontal_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/filter_item_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/filter_item_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/foreign_key_auto_complete.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/foreign_key_auto_complete.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/guardian_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/guardian_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/import_export_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/import_export_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/list_and_search.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/list_and_search.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/model_with_full_permission_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/model_with_full_permission_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_admin_tools/reversion_feature.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_admin_tools/reversion_feature.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_signals.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_signals.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_urls.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_urls.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_conf_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_conf_utils.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/auto_detection/routing_auto_detection.py` & `djangoautoconf-2.0.9/djangoautoconf/auto_detection/routing_auto_detection.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/base_setting_storage.py` & `djangoautoconf-2.0.9/djangoautoconf/base_setting_storage.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/base_settings.py` & `djangoautoconf-2.0.9/djangoautoconf/base_settings.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/class_based_views/ajax_views.py` & `djangoautoconf-2.0.9/djangoautoconf/class_based_views/ajax_views.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/class_based_views/create_view_factory.py` & `djangoautoconf-2.0.9/djangoautoconf/class_based_views/create_view_factory.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/class_based_views/detail_with_inline_view.py` & `djangoautoconf-2.0.9/djangoautoconf/class_based_views/detail_with_inline_view.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/class_based_views/form_factory.py` & `djangoautoconf-2.0.9/djangoautoconf/class_based_views/form_factory.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/class_based_views/template_view_factory.py` & `djangoautoconf-2.0.9/djangoautoconf/class_based_views/template_view_factory.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/database_connection_maintainer.py` & `djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/database_connection_maintainer.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/cmd_handler_base/msg_process_cmd_base.py` & `djangoautoconf-2.0.9/djangoautoconf/cmd_handler_base/msg_process_cmd_base.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_adv_zip_template_loader.py` & `djangoautoconf-2.0.9/djangoautoconf/django_adv_zip_template_loader.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_autoconf.py` & `djangoautoconf-2.0.9/djangoautoconf/django_autoconf.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_dev_server_auto_conf.py` & `djangoautoconf-2.0.9/djangoautoconf/django_dev_server_auto_conf.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_rest_framework_utils/serializer_generator.py` & `djangoautoconf-2.0.9/djangoautoconf/django_rest_framework_utils/serializer_generator.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_setting_manager.py` & `djangoautoconf-2.0.9/djangoautoconf/django_setting_manager.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/django_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import mimetypes
 from django.http import HttpResponse
 import os
 try:
     from django.core.servers.basehttp import FileWrapper
 except:
     from wsgiref.util import FileWrapper
-from django.utils.http import urlquote
+
+from urllib.parse import quote
+django.utils.http.urlquote = quote
 
 
 def get_new_uuid():
     return str(uuid.uuid4())
 
 
 def retrieve_param(request):
```

### Comparing `djangoautoconf-2.0.8/djangoautoconf/django_zip_template_loader.py` & `djangoautoconf-2.0.9/djangoautoconf/django_zip_template_loader.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/djangoautoconf_settings.py` & `djangoautoconf-2.0.9/djangoautoconf/djangoautoconf_settings.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/local_key_manager.py` & `djangoautoconf-2.0.9/djangoautoconf/local_key_manager.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/management/commands/create_default_super_user.py` & `djangoautoconf-2.0.9/djangoautoconf/management/commands/create_default_super_user.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/management/commands/dump_settings.py` & `djangoautoconf-2.0.9/djangoautoconf/management/commands/dump_settings.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/management/commands/remove_app_tables.py` & `djangoautoconf-2.0.9/djangoautoconf/management/commands/remove_app_tables.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/adv_tastypie_resource.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/adv_tastypie_resource.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/import_export_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/import_export_utils.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/model_attr_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/model_attr_utils.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/model_duplicator.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/model_duplicator.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/model_reversion.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/model_reversion.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/tastypie_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/tastypie_utils.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/model_utils/url_for_models.py` & `djangoautoconf-2.0.9/djangoautoconf/model_utils/url_for_models.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/object_copier.py` & `djangoautoconf-2.0.9/djangoautoconf/object_copier.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/obs/auto_conf_admin_utils.py` & `djangoautoconf-2.0.9/djangoautoconf/obs/auto_conf_admin_utils.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/obs/version_mismatch_work_around.py` & `djangoautoconf-2.0.9/djangoautoconf/obs/version_mismatch_work_around.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/req_with_auth.py` & `djangoautoconf-2.0.9/djangoautoconf/req_with_auth.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/setting_utils/app_folders.py` & `djangoautoconf-2.0.9/djangoautoconf/setting_utils/app_folders.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/sqlite_database.py` & `djangoautoconf-2.0.9/djangoautoconf/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/templates/base_with_nav.html` & `djangoautoconf-2.0.9/djangoautoconf/templates/base_with_nav.html`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/templates/detail_with_inline_view.html` & `djangoautoconf-2.0.9/djangoautoconf/templates/detail_with_inline_view.html`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf/urls.py` & `djangoautoconf-2.0.9/djangoautoconf/urls.py`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/djangoautoconf.egg-info/PKG-INFO` & `djangoautoconf-2.0.9/djangoautoconf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: djangoautoconf
-Version: 2.0.8
+Version: 2.0.9
 Summary: Create a package to ease setting django project settings.
 Home-page: https://github.com/weijia/djangoautoconf
 Author: Richard Wang
 Author-email: richardwangwang@gmail.com
 License: BSD
 Description: ===============================
         Django AutoConf
```

### Comparing `djangoautoconf-2.0.8/djangoautoconf.egg-info/SOURCES.txt` & `djangoautoconf-2.0.9/djangoautoconf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoautoconf-2.0.8/setup.py` & `djangoautoconf-2.0.9/setup.py`

 * *Files identical despite different names*

