# Comparing `tmp/lumapps_sdk-1.2.6.tar.gz` & `tmp/lumapps_sdk-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumapps_sdk-1.2.6.tar", max compression
+gzip compressed data, was "lumapps_sdk-1.2.7.tar", max compression
```

## Comparing `lumapps_sdk-1.2.6.tar` & `lumapps_sdk-1.2.7.tar`

### file list

```diff
@@ -1,127 +1,126 @@
--rw-r--r--   0        0        0     1087 2023-02-23 09:50:15.949000 lumapps_sdk-1.2.6/LICENSE.md
--rw-r--r--   0        0        0     2772 2023-02-23 09:50:15.949000 lumapps_sdk-1.2.6/README.md
--rw-r--r--   0        0        0       71 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/__init__.py
--rw-r--r--   0        0        0      192 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/__init__.py
--rw-r--r--   0        0        0     6129 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/authlib_helpers.py
--rw-r--r--   0        0        0    19579 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/base_client.py
--rwxr-xr-x   0        0        0     6444 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/cli.py
--rw-r--r--   0        0        0    67431 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/client.py
--rw-r--r--   0        0        0       59 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/conf.py
--rw-r--r--   0        0        0     5439 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/decorators.py
--rw-r--r--   0        0        0     2935 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/errors.py
--rw-r--r--   0        0        0      449 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/helpers/__init__.py
--rw-r--r--   0        0        0     6225 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/helpers/medias.py
--rw-r--r--   0        0        0     5263 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/helpers/widgets.py
--rw-r--r--   0        0        0     4574 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/lumapps_jwt.py
--rw-r--r--   0        0        0     6825 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/api/utils.py
--rw-r--r--   0        0        0        0 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/__init__.py
--rw-r--r--   0        0        0        0 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/__init__.py
--rw-r--r--   0        0        0      609 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/article.py
--rw-r--r--   0        0        0       40 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/__init__.py
--rw-r--r--   0        0        0       38 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/__init__.py
--rw-r--r--   0        0        0      817 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/gateway.py
--rw-r--r--   0        0        0     4662 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/__init__.py
--rw-r--r--   0        0        0     2816 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/all_of_i18n_string_lang.py
--rw-r--r--   0        0        0    10368 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article.py
--rw-r--r--   0        0        0     6099 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_preview.py
--rw-r--r--   0        0        0     4206 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_share.py
--rw-r--r--   0        0        0     5041 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_with_layout.py
--rw-r--r--   0        0        0     6122 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/attached_link.py
--rw-r--r--   0        0        0     3737 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/base_block.py
--rw-r--r--   0        0        0     5031 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_cascade.py
--rw-r--r--   0        0        0     5714 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_client_computed.py
--rw-r--r--   0        0        0    13428 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_community_preview.py
--rw-r--r--   0        0        0    12003 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_directory_entry.py
--rw-r--r--   0        0        0    16471 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_event_metadata.py
--rw-r--r--   0        0        0     3557 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_featured_image.py
--rw-r--r--   0        0        0     3587 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_generic_container.py
--rw-r--r--   0        0        0     7231 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_generic_resource.py
--rw-r--r--   0        0        0     5103 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_grid.py
--rw-r--r--   0        0        0     4174 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_html.py
--rw-r--r--   0        0        0    13922 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_image.py
--rw-r--r--   0        0        0     6230 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_inappropriate.py
--rw-r--r--   0        0        0     3517 2023-02-23 09:50:15.953001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_intro.py
--rw-r--r--   0        0        0     5271 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_list.py
--rw-r--r--   0        0        0     3745 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_no_results.py
--rw-r--r--   0        0        0    13970 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_page_preview.py
--rw-r--r--   0        0        0    27724 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_post.py
--rw-r--r--   0        0        0     8890 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_reactions.py
--rw-r--r--   0        0        0     6783 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_remote.py
--rw-r--r--   0        0        0     6795 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_resource_creation_info.py
--rw-r--r--   0        0        0     8781 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_slideshow.py
--rw-r--r--   0        0        0     4887 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_structured_content.py
--rw-r--r--   0        0        0     4462 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tab_filtered_container.py
--rw-r--r--   0        0        0     4560 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tag_filter.py
--rw-r--r--   0        0        0     3605 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tag_reference_list.py
--rw-r--r--   0        0        0     4949 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_title.py
--rw-r--r--   0        0        0     3629 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_type.py
--rw-r--r--   0        0        0     9964 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user.py
--rw-r--r--   0        0        0     3532 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user_list.py
--rw-r--r--   0        0        0     6678 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user_profile_preview.py
--rw-r--r--   0        0        0     7893 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_votes.py
--rw-r--r--   0        0        0     7173 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/community_info.py
--rw-r--r--   0        0        0     2605 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_orientation.py
--rw-r--r--   0        0        0     4381 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_reference.py
--rw-r--r--   0        0        0     2567 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_type.py
--rw-r--r--   0        0        0     2585 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_variant.py
--rw-r--r--   0        0        0     3626 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/content_status.py
--rw-r--r--   0        0        0     5339 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_article_in_container_request.py
--rw-r--r--   0        0        0    11093 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_event_in_container_request.py
--rw-r--r--   0        0        0     4859 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_article_request.py
--rw-r--r--   0        0        0    10551 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_event_request.py
--rw-r--r--   0        0        0     4092 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/custom_link_label.py
--rw-r--r--   0        0        0     5502 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/document.py
--rw-r--r--   0        0        0     2477 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/element_style.py
--rw-r--r--   0        0        0     8186 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error.py
--rw-r--r--   0        0        0     3370 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error_links.py
--rw-r--r--   0        0        0     4319 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error_source.py
--rw-r--r--   0        0        0    15016 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event.py
--rw-r--r--   0        0        0     5586 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_link_label.py
--rw-r--r--   0        0        0     4903 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_page.py
--rw-r--r--   0        0        0     4136 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_share.py
--rw-r--r--   0        0        0     6917 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/footer.py
--rw-r--r--   0        0        0     4900 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_attendees_response.py
--rw-r--r--   0        0        0     3594 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_error.py
--rw-r--r--   0        0        0     2481 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_errors.py
--rw-r--r--   0        0        0     5310 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_events_by_ids.py
--rw-r--r--   0        0        0     5309 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/header.py
--rw-r--r--   0        0        0     4416 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/i18n_string.py
--rw-r--r--   0        0        0     3958 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/idea_status.py
--rw-r--r--   0        0        0     3253 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/inline_response401.py
--rw-r--r--   0        0        0     2461 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/language.py
--rw-r--r--   0        0        0     6683 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/layout.py
--rw-r--r--   0        0        0     3870 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/link_label.py
--rw-r--r--   0        0        0     9024 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/media_preview.py
--rw-r--r--   0        0        0     5843 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/metadata_reference.py
--rw-r--r--   0        0        0     5100 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/multilang_document.py
--rw-r--r--   0        0        0     5014 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/multilang_object.py
--rw-r--r--   0        0        0     2629 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_event_in_container_request_external_url_label.py
--rw-r--r--   0        0        0     2617 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_or_update_event_request_external_url_label.py
--rw-r--r--   0        0        0     2533 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_event_external_url_label.py
--rw-r--r--   0        0        0     2489 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_widget_body.py
--rw-r--r--   0        0        0     2477 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/organizer_ids.py
--rw-r--r--   0        0        0     3920 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/play_video_preview.py
--rw-r--r--   0        0        0     8878 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/post_share.py
--rw-r--r--   0        0        0     4803 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/site_reference.py
--rw-r--r--   0        0        0     2623 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/slideshow_variant.py
--rw-r--r--   0        0        0    10038 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/structured_content.py
--rw-r--r--   0        0        0     5057 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/tag_reference.py
--rw-r--r--   0        0        0     6856 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field.py
--rw-r--r--   0        0        0     2797 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field_type.py
--rw-r--r--   0        0        0     2545 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_primary_field_values.py
--rw-r--r--   0        0        0     7221 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_reference.py
--rw-r--r--   0        0        0     9118 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget.py
--rw-r--r--   0        0        0     4824 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget_response.py
--rw-r--r--   0        0        0     2835 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget_type.py
--rw-r--r--   0        0        0    13189 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/api/swagger/serialization.py
--rw-r--r--   0        0        0      162 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/client/__init__.py
--rw-r--r--   0        0        0     2716 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/client/application.py
--rw-r--r--   0        0        0     1097 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/client/base.py
--rw-r--r--   0        0        0       40 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/entities/__init__.py
--rw-r--r--   0        0        0      250 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/entities/article.py
--rw-r--r--   0        0        0      122 2023-02-23 09:50:15.957001 lumapps_sdk-1.2.6/lumapps/latest/entities/translation.py
--rw-r--r--   0        0        0     1670 2023-02-23 09:51:47.308830 lumapps_sdk-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     4003 1970-01-01 00:00:00.000000 lumapps_sdk-1.2.6/setup.py
--rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 lumapps_sdk-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-07-06 15:15:15.662815 lumapps_sdk-1.2.7/LICENSE.md
+-rw-r--r--   0        0        0     2772 2023-07-06 15:15:15.662815 lumapps_sdk-1.2.7/README.md
+-rw-r--r--   0        0        0       71 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/__init__.py
+-rw-r--r--   0        0        0     6129 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/authlib_helpers.py
+-rw-r--r--   0        0        0    19579 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/base_client.py
+-rwxr-xr-x   0        0        0     6444 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/cli.py
+-rw-r--r--   0        0        0    67431 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/client.py
+-rw-r--r--   0        0        0       59 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/conf.py
+-rw-r--r--   0        0        0     5439 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/decorators.py
+-rw-r--r--   0        0        0     2935 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/errors.py
+-rw-r--r--   0        0        0      449 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/helpers/__init__.py
+-rw-r--r--   0        0        0     6225 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/helpers/medias.py
+-rw-r--r--   0        0        0     5263 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/helpers/widgets.py
+-rw-r--r--   0        0        0     4651 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/lumapps_jwt.py
+-rw-r--r--   0        0        0     6825 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/api/utils.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/article.py
+-rw-r--r--   0        0        0       40 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/__init__.py
+-rw-r--r--   0        0        0       38 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/__init__.py
+-rw-r--r--   0        0        0      817 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/gateway.py
+-rw-r--r--   0        0        0     4662 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/__init__.py
+-rw-r--r--   0        0        0     2816 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/all_of_i18n_string_lang.py
+-rw-r--r--   0        0        0    10368 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article.py
+-rw-r--r--   0        0        0     6099 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_preview.py
+-rw-r--r--   0        0        0     4206 2023-07-06 15:15:15.666816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_share.py
+-rw-r--r--   0        0        0     5041 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_with_layout.py
+-rw-r--r--   0        0        0     6122 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/attached_link.py
+-rw-r--r--   0        0        0     3737 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/base_block.py
+-rw-r--r--   0        0        0     5031 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_cascade.py
+-rw-r--r--   0        0        0     5714 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_client_computed.py
+-rw-r--r--   0        0        0    13428 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_community_preview.py
+-rw-r--r--   0        0        0    12003 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_directory_entry.py
+-rw-r--r--   0        0        0    16471 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_event_metadata.py
+-rw-r--r--   0        0        0     3557 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_featured_image.py
+-rw-r--r--   0        0        0     3587 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_generic_container.py
+-rw-r--r--   0        0        0     7231 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_generic_resource.py
+-rw-r--r--   0        0        0     5103 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_grid.py
+-rw-r--r--   0        0        0     4174 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_html.py
+-rw-r--r--   0        0        0    13922 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_image.py
+-rw-r--r--   0        0        0     6230 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_inappropriate.py
+-rw-r--r--   0        0        0     3517 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_intro.py
+-rw-r--r--   0        0        0     5271 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_list.py
+-rw-r--r--   0        0        0     3745 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_no_results.py
+-rw-r--r--   0        0        0    13970 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_page_preview.py
+-rw-r--r--   0        0        0    27724 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_post.py
+-rw-r--r--   0        0        0     8890 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_reactions.py
+-rw-r--r--   0        0        0     6783 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_remote.py
+-rw-r--r--   0        0        0     6795 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_resource_creation_info.py
+-rw-r--r--   0        0        0     8781 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_slideshow.py
+-rw-r--r--   0        0        0     4887 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_structured_content.py
+-rw-r--r--   0        0        0     4462 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tab_filtered_container.py
+-rw-r--r--   0        0        0     4560 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tag_filter.py
+-rw-r--r--   0        0        0     3605 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tag_reference_list.py
+-rw-r--r--   0        0        0     4949 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_title.py
+-rw-r--r--   0        0        0     3629 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_type.py
+-rw-r--r--   0        0        0     9964 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user.py
+-rw-r--r--   0        0        0     3532 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user_list.py
+-rw-r--r--   0        0        0     6678 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user_profile_preview.py
+-rw-r--r--   0        0        0     7893 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_votes.py
+-rw-r--r--   0        0        0     7173 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/community_info.py
+-rw-r--r--   0        0        0     2605 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_orientation.py
+-rw-r--r--   0        0        0     4381 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_reference.py
+-rw-r--r--   0        0        0     2567 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_type.py
+-rw-r--r--   0        0        0     2585 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_variant.py
+-rw-r--r--   0        0        0     3626 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/content_status.py
+-rw-r--r--   0        0        0     5339 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_article_in_container_request.py
+-rw-r--r--   0        0        0    11093 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_event_in_container_request.py
+-rw-r--r--   0        0        0     4859 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_article_request.py
+-rw-r--r--   0        0        0    10551 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_event_request.py
+-rw-r--r--   0        0        0     4092 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/custom_link_label.py
+-rw-r--r--   0        0        0     5502 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/document.py
+-rw-r--r--   0        0        0     2477 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/element_style.py
+-rw-r--r--   0        0        0     8186 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error.py
+-rw-r--r--   0        0        0     3370 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error_links.py
+-rw-r--r--   0        0        0     4319 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error_source.py
+-rw-r--r--   0        0        0    15016 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event.py
+-rw-r--r--   0        0        0     5586 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_link_label.py
+-rw-r--r--   0        0        0     4903 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_page.py
+-rw-r--r--   0        0        0     4136 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_share.py
+-rw-r--r--   0        0        0     6917 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/footer.py
+-rw-r--r--   0        0        0     4900 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_attendees_response.py
+-rw-r--r--   0        0        0     3594 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_error.py
+-rw-r--r--   0        0        0     2481 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_errors.py
+-rw-r--r--   0        0        0     5310 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_events_by_ids.py
+-rw-r--r--   0        0        0     5309 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/header.py
+-rw-r--r--   0        0        0     4416 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/i18n_string.py
+-rw-r--r--   0        0        0     3958 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/idea_status.py
+-rw-r--r--   0        0        0     3253 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/inline_response401.py
+-rw-r--r--   0        0        0     2461 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/language.py
+-rw-r--r--   0        0        0     6683 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/layout.py
+-rw-r--r--   0        0        0     3870 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/link_label.py
+-rw-r--r--   0        0        0     9024 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/media_preview.py
+-rw-r--r--   0        0        0     5843 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/metadata_reference.py
+-rw-r--r--   0        0        0     5100 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/multilang_document.py
+-rw-r--r--   0        0        0     5014 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/multilang_object.py
+-rw-r--r--   0        0        0     2629 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_event_in_container_request_external_url_label.py
+-rw-r--r--   0        0        0     2617 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_or_update_event_request_external_url_label.py
+-rw-r--r--   0        0        0     2533 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_event_external_url_label.py
+-rw-r--r--   0        0        0     2489 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_widget_body.py
+-rw-r--r--   0        0        0     2477 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/organizer_ids.py
+-rw-r--r--   0        0        0     3920 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/play_video_preview.py
+-rw-r--r--   0        0        0     8878 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/post_share.py
+-rw-r--r--   0        0        0     4803 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/site_reference.py
+-rw-r--r--   0        0        0     2623 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/slideshow_variant.py
+-rw-r--r--   0        0        0    10038 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/structured_content.py
+-rw-r--r--   0        0        0     5057 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/tag_reference.py
+-rw-r--r--   0        0        0     6856 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field.py
+-rw-r--r--   0        0        0     2797 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field_type.py
+-rw-r--r--   0        0        0     2545 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_primary_field_values.py
+-rw-r--r--   0        0        0     7221 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_reference.py
+-rw-r--r--   0        0        0     9118 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget.py
+-rw-r--r--   0        0        0     4824 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget_response.py
+-rw-r--r--   0        0        0     2835 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget_type.py
+-rw-r--r--   0        0        0    13189 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/api/swagger/serialization.py
+-rw-r--r--   0        0        0      162 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/client/__init__.py
+-rw-r--r--   0        0        0     2716 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/client/application.py
+-rw-r--r--   0        0        0     1097 2023-07-06 15:15:15.670816 lumapps_sdk-1.2.7/lumapps/latest/client/base.py
+-rw-r--r--   0        0        0       40 2023-07-06 15:15:15.674816 lumapps_sdk-1.2.7/lumapps/latest/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-06 15:15:15.674816 lumapps_sdk-1.2.7/lumapps/latest/entities/__init__.py
+-rw-r--r--   0        0        0      250 2023-07-06 15:15:15.674816 lumapps_sdk-1.2.7/lumapps/latest/entities/article.py
+-rw-r--r--   0        0        0      122 2023-07-06 15:15:15.674816 lumapps_sdk-1.2.7/lumapps/latest/entities/translation.py
+-rw-r--r--   0        0        0     1670 2023-07-06 15:17:01.641322 lumapps_sdk-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3731 1970-01-01 00:00:00.000000 lumapps_sdk-1.2.7/PKG-INFO
```

### Comparing `lumapps_sdk-1.2.6/LICENSE.md` & `lumapps_sdk-1.2.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/README.md` & `lumapps_sdk-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/authlib_helpers.py` & `lumapps_sdk-1.2.7/lumapps/api/authlib_helpers.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/base_client.py` & `lumapps_sdk-1.2.7/lumapps/api/base_client.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/cli.py` & `lumapps_sdk-1.2.7/lumapps/api/cli.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/client.py` & `lumapps_sdk-1.2.7/lumapps/api/client.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/decorators.py` & `lumapps_sdk-1.2.7/lumapps/api/decorators.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/errors.py` & `lumapps_sdk-1.2.7/lumapps/api/errors.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/helpers/medias.py` & `lumapps_sdk-1.2.7/lumapps/api/helpers/medias.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/helpers/widgets.py` & `lumapps_sdk-1.2.7/lumapps/api/helpers/widgets.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/api/lumapps_jwt.py` & `lumapps_sdk-1.2.7/lumapps/api/lumapps_jwt.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "dot-lumapps-core.appspot.com": "https://login.dev.lumapps.com/v1/jwks",
     "dot-lumapps-sa.appspot.com": "https://login.dev.lumapps.com/v1/jwks",
     "dot-lumapps-search.appspot.com": "https://login.dev.lumapps.com/v1/jwks",
     "dot-lumapps-social.appspot.com": "https://login.dev.lumapps.com/v1/jwks",
     "dot-lumapps-dev.appspot.com": "https://login.dev.lumapps.com/v1/jwks",
     "dot-lumapps-sandbox.appspot.com": "https://login-sandbox.dev.lumapps.com/v1/jwks",
     "dot-lumapps-staging.appspot.com": "https://login.stag.lumapps.com/v1/jwks",
+    "lumapps-staging.appspot.com": "https://login.stag.lumapps.com/v1/jwks",
     "sites-staging.lumapps.com": "https://login.stag.lumapps.com/v1/jwks",
     "sites-analytics.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
     "sites-ba.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
     "sites-cms.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
     "sites-core.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
     "sites-sa.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
     "sites-search.lumapps.com": "https://login.dev.lumapps.com/v1/jwks",
```

### Comparing `lumapps_sdk-1.2.6/lumapps/api/utils.py` & `lumapps_sdk-1.2.7/lumapps/api/utils.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/article.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/article.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/gateway.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/gateway.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/__init__.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/all_of_i18n_string_lang.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/all_of_i18n_string_lang.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_share.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_share.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/article_with_layout.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/article_with_layout.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/attached_link.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/attached_link.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/base_block.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/base_block.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_cascade.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_cascade.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_client_computed.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_client_computed.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_community_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_community_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_directory_entry.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_directory_entry.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_event_metadata.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_event_metadata.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_featured_image.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_featured_image.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_generic_container.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_generic_container.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_generic_resource.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_generic_resource.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_grid.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_grid.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_html.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_html.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_image.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_image.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_inappropriate.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_inappropriate.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_intro.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_intro.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_list.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_list.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_no_results.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_no_results.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_page_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_page_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_post.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_post.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_reactions.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_reactions.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_remote.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_remote.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_resource_creation_info.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_resource_creation_info.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_slideshow.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_slideshow.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_structured_content.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_structured_content.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tab_filtered_container.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tab_filtered_container.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tag_filter.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tag_filter.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_tag_reference_list.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_tag_reference_list.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_title.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_title.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_type.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_type.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user_list.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user_list.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_user_profile_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_user_profile_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/block_votes.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/block_votes.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/community_info.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/community_info.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_orientation.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_orientation.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_reference.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_reference.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_type.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_type.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/container_variant.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/container_variant.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/content_status.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/content_status.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_article_in_container_request.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_article_in_container_request.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_event_in_container_request.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_event_in_container_request.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_article_request.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_article_request.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_event_request.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/create_or_update_event_request.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/custom_link_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/custom_link_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/document.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/document.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/element_style.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/element_style.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error_links.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error_links.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/error_source.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/error_source.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_link_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_link_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_page.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_page.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/event_share.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/event_share.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/footer.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/footer.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_attendees_response.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_attendees_response.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_error.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_error.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_errors.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_by_id_errors.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/get_events_by_ids.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/get_events_by_ids.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/header.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/header.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/i18n_string.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/i18n_string.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/idea_status.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/idea_status.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/inline_response401.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/language.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/language.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/layout.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/layout.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/link_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/link_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/media_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/media_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/metadata_reference.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/metadata_reference.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/multilang_document.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/multilang_document.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/multilang_object.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/multilang_object.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_event_in_container_request_external_url_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_event_in_container_request_external_url_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_or_update_event_request_external_url_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_create_or_update_event_request_external_url_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_event_external_url_label.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_event_external_url_label.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/one_of_widget_body.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/one_of_widget_body.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/organizer_ids.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/organizer_ids.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/play_video_preview.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/play_video_preview.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/post_share.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/post_share.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/site_reference.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/site_reference.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/slideshow_variant.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/slideshow_variant.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/structured_content.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/structured_content.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/tag_reference.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/tag_reference.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field_type.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_field_type.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_profile_primary_field_values.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_profile_primary_field_values.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/user_reference.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/user_reference.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget_response.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget_response.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/contribution_v1/models/widget_type.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/contribution_v1/models/widget_type.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/api/swagger/serialization.py` & `lumapps_sdk-1.2.7/lumapps/latest/api/swagger/serialization.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/client/application.py` & `lumapps_sdk-1.2.7/lumapps/latest/client/application.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/lumapps/latest/client/base.py` & `lumapps_sdk-1.2.7/lumapps/latest/client/base.py`

 * *Files identical despite different names*

### Comparing `lumapps_sdk-1.2.6/pyproject.toml` & `lumapps_sdk-1.2.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lumapps-sdk"
-version = "1.2.6"
+version = "1.2.7"
 description = ""
 authors = ["Aurélien Dentan <aurelien@lumapps.com>", "Ludovic Vaugeois <ludovic.vaugeois@lumapps.com>"]
 license = "MIT License"
 readme = "README.md"
 repository = "https://github.com/lumapps/lumapps-sdk"
 homepage = "https://github.com/lumapps/lumapps-sdk"
 keywords = ["lumapps-sdk", "sdk", "python"]
```

### Comparing `lumapps_sdk-1.2.6/PKG-INFO` & `lumapps_sdk-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumapps-sdk
-Version: 1.2.6
+Version: 1.2.7
 Summary: 
 Home-page: https://github.com/lumapps/lumapps-sdk
 License: MIT
 Keywords: lumapps-sdk,sdk,python
 Author: Aurélien Dentan
 Author-email: aurelien@lumapps.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lumapps-sdk Version: 1.2.6 Summary: Home-page:
+Metadata-Version: 2.1 Name: lumapps-sdk Version: 1.2.7 Summary: Home-page:
 https://github.com/lumapps/lumapps-sdk License: MIT Keywords: lumapps-
 sdk,sdk,python Author: AurÃ©lien Dentan Author-email: aurelien@lumapps.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

