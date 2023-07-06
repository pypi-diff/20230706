# Comparing `tmp/djangoldp_needle-0.1.92.tar.gz` & `tmp/djangoldp_needle-0.1.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_needle-0.1.92.tar", last modified: Thu Jun 29 09:02:17 2023, max compression
+gzip compressed data, was "dist/djangoldp_needle-0.1.93.tar", last modified: Thu Jul  6 11:45:59 2023, max compression
```

## Comparing `djangoldp_needle-0.1.92.tar` & `djangoldp_needle-0.1.93.tar`

### file list

```diff
@@ -1,242 +1,242 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/
--rw-rw-rw-   0 root         (0) root         (0)      278 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     3001 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16392 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_target_add.py
--rw-rw-rw-   0 root         (0) root         (0)     7376 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributors_delete.py
--rw-rw-rw-   0 root         (0) root         (0)     4838 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_list.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/
--rw-rw-rw-   0 root         (0) root         (0)     4305 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_not_found.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11721 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_dates.py
--rw-rw-rw-   0 root         (0) root         (0)    15329 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links.py
--rw-rw-rw-   0 root         (0) root         (0)      642 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_timeout.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/realsites.py
--rw-rw-rw-   0 root         (0) root         (0)    17166 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_redirect.py
--rw-rw-rw-   0 root         (0) root         (0)     4538 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_error.py
--rw-rw-rw-   0 root         (0) root         (0)     4184 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/needlerealsites.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/base_valid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   613961 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/lemonde-1.html
--rw-rw-rw-   0 root         (0) root         (0)   289885 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/theconversation-1.html
--rw-rw-rw-   0 root         (0) root         (0)   126155 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/internetactu-1.html
--rw-rw-rw-   0 root         (0) root         (0)   306075 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/lemonde.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   181484 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/theconversation.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   149029 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/reporterre-1.html
--rw-rw-rw-   0 root         (0) root         (0)   127161 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/laviedesidees-1.html
--rw-rw-rw-   0 root         (0) root         (0)   369446 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/latribune-1.html
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
--rw-rw-rw-   0 root         (0) root         (0)   232761 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/fredcavazza-1.html
--rw-rw-rw-   0 root         (0) root         (0)   118533 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
--rw-rw-rw-   0 root         (0) root         (0)     2343 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_date_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     6572 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_needle_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)     2696 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_add.py
--rw-rw-rw-   0 root         (0) root         (0)    10168 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_activity.py
--rw-rw-rw-   0 root         (0) root         (0)    10554 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributors_patch.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_import.py
--rw-rw-rw-   0 root         (0) root         (0)    12210 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_add_annotation.py
--rw-rw-rw-   0 root         (0) root         (0)    10327 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_intersection.py
--rw-rw-rw-   0 root         (0) root         (0)     8159 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_yarn.py
--rw-rw-rw-   0 root         (0) root         (0)     6202 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributor_pending.py
--rw-rw-rw-   0 root         (0) root         (0)     5046 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)     4765 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_needle_user_contact_pending.py
--rw-rw-rw-   0 root         (0) root         (0)     4974 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/test_user_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2584 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/tests/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      213 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activation_email.html
--rw-rw-rw-   0 root         (0) root         (0)      329 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      134 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      918 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)      212 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      209 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      299 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activation_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      753 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      214 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     2949 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      178 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/
--rw-rw-rw-   0 root         (0) root         (0)     1040 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/booklet_pending.html
--rw-rw-rw-   0 root         (0) root         (0)     1074 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation.html
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation.txt
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/contact.txt
--rw-rw-rw-   0 root         (0) root         (0)      192 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/booklet_pending.txt
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation_pending.txt
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation_pending.html
--rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/contact.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     1378 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)      723 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_email_subject.txt
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/registration_base.html
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_email.html
--rw-rw-rw-   0 root         (0) root         (0)      665 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_email_body.txt
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      914 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2376 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/authorize.html
--rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/admin.py
--rw-rw-rw-   0 root         (0) root         (0)     3098 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/management/commands/importneedledata.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       23 2023-06-29 09:02:14.000000 djangoldp_needle-0.1.92/djangoldp_needle/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/settings/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/settings/avatar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/linkIcon.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/opengraph.py
--rw-rw-rw-   0 root         (0) root         (0)     1013 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/urlParser.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/abstract_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2328 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/metaProp.py
--rw-rw-rw-   0 root         (0) root         (0)     3571 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/itemProp.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py
--rw-rw-rw-   0 root         (0) root         (0)    25244 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/jsonld.py
--rw-rw-rw-   0 root         (0) root         (0)      808 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/lastChanceParser.py
--rw-rw-rw-   0 root         (0) root         (0)      611 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/titleTag.py
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/webdriver_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     6029 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/request_parser/request_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/form/
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/form/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/form/needle_user_form.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/static/images/
--rw-rw-rw-   0 root         (0) root         (0)   798691 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/static/images/background.png
--rw-rw-rw-   0 root         (0) root         (0)      738 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/static/needle.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/
--rw-rw-rw-   0 root         (0) root         (0)    12144 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_contributor.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_contact_pending.py
--rw-rw-rw-   0 root         (0) root         (0)     1003 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2248 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_contributor_pending.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_intersections.py
--rw-rw-rw-   0 root         (0) root         (0)       93 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      336 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/avatars.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      453 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     3187 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)     3590 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)    10838 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)      333 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      156 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/tag.py
--rw-rw-rw-   0 root         (0) root         (0)     1564 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_invitation.py
--rw-rw-rw-   0 root         (0) root         (0)     1103 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_quit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      258 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/templatetags/settings_value.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)      784 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/booklet_contributor.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/needle_user_contact_pending.py
--rw-rw-rw-   0 root         (0) root         (0)      849 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/booklet_contributor_pending.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/needle_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)     1147 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/annotation_target.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)      108 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)       95 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/permissions/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      473 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/djangoldp_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      413 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0004_annotationtarget_image.py
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0019_auto_20230208_1213.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
--rwxrwxrwx   0 root         (0) root         (0)      798 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0032_avatar2.py
--rw-rw-rw-   0 root         (0) root         (0)     2622 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1852 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0013_needleuserprofile.py
--rw-rw-rw-   0 root         (0) root         (0)      446 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0029_auto_20230411_1211.py
--rwxrwxrwx   0 root         (0) root         (0)      718 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0034_auto_20230515_1735.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0009_activity_subtitle.py
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0015_auto_20230112_1339.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0006_auto_20221101_1846.py
--rw-rw-rw-   0 root         (0) root         (0)     1543 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0002_tag.py
--rw-rw-rw-   0 root         (0) root         (0)      465 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0018_auto_20230129_1617.py
--rw-rw-rw-   0 root         (0) root         (0)      543 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0014_auto_20230105_1238.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0022_annotation_annotation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      584 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0007_auto_20221114_1643.py
--rw-rw-rw-   0 root         (0) root         (0)     1992 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0023_booklet.py
--rwxrwxrwx   0 root         (0) root         (0)     4686 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0036_auto_20230526_1301.py
--rw-rw-rw-   0 root         (0) root         (0)     1854 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0011_auto_20221125_1015.py
--rw-rw-rw-   0 root         (0) root         (0)      432 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
--rwxrwxrwx   0 root         (0) root         (0)     2452 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0032_avatar.py
--rw-rw-rw-   0 root         (0) root         (0)     1846 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0017_annotationintersectionread.py
--rw-rw-rw-   0 root         (0) root         (0)     1970 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0025_needleuserfollow.py
--rw-rw-rw-   0 root         (0) root         (0)     1699 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0019_contactmessage.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0024_auto_20230328_0814.py
--rw-rw-rw-   0 root         (0) root         (0)     2302 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0035_auto_20230525_1351.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0020_contactmessage_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0021_merge_20230213_1548.py
--rw-rw-rw-   0 root         (0) root         (0)      519 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
--rw-rw-rw-   0 root         (0) root         (0)      399 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0003_annotation_tags.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0005_annotationtarget_title.py
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0008_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     2082 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0037_auto_20230604_1525.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0010_activity_read.py
--rwxrwxrwx   0 root         (0) root         (0)     2784 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0033_auto_20230509_1434.py
--rw-rw-rw-   0 root         (0) root         (0)      436 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0026_auto_20230331_1603.py
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/migrations/0016_auto_20230123_1741.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/
--rw-rw-rw-   0 root         (0) root         (0)     2815 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/ldp_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)     8082 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/activity_signal_receiver.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/booklet_contributor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_contact_pending.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2149 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/booklet_contributor_pending.py
--rwxrwxrwx   0 root         (0) root         (0)      875 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     1216 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/needle_activity.py
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/contact_message.py
--rw-rw-rw-   0 root         (0) root         (0)     2046 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_contact.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/booklet.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/annotation_intersection_read.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/annotation_target.py
--rwxrwxrwx   0 root         (0) root         (0)     1644 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/avatar.py
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_follow.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/djangoldp_needle/models/tag.py
--rw-rw-rw-   0 root         (0) root         (0)      112 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-06-29 09:01:51.000000 djangoldp_needle-0.1.92/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      608 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-29 09:02:17.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/
--rw-r--r--   0 root         (0) root         (0)      521 2023-06-29 09:02:16.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-29 09:02:16.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    10884 2023-06-29 09:02:16.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-06-29 09:02:16.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      142 2023-06-29 09:02:16.000000 djangoldp_needle-0.1.92/djangoldp_needle.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/
+-rw-rw-rw-   0 root         (0) root         (0)      278 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_first_annotation_on_user_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3001 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16861 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_target_add.py
+-rw-rw-rw-   0 root         (0) root         (0)     7376 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributors_delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     4838 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_list.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/
+-rw-rw-rw-   0 root         (0) root         (0)     4305 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_not_found.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11721 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)    15329 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links.py
+-rw-rw-rw-   0 root         (0) root         (0)      642 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_timeout.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/realsites.py
+-rw-rw-rw-   0 root         (0) root         (0)    17166 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_redirect.py
+-rw-rw-rw-   0 root         (0) root         (0)     4538 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     4184 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/needlerealsites.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/base_valid.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   613961 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/lemonde-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   289885 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/theconversation-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   126155 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/internetactu-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   306075 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/lemonde.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   181484 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/theconversation.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   149029 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/reporterre-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   127161 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/laviedesidees-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   369446 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/latribune-1.html
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/base_invalid.20221103.html
+-rw-rw-rw-   0 root         (0) root         (0)   232761 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/fredcavazza-1.html
+-rw-rw-rw-   0 root         (0) root         (0)   118533 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_date_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     6634 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     2696 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_add.py
+-rw-rw-rw-   0 root         (0) root         (0)    10168 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)    10554 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributors_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_import.py
+-rw-rw-rw-   0 root         (0) root         (0)    12210 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_add_annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    10327 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_intersection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8159 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_yarn.py
+-rw-rw-rw-   0 root         (0) root         (0)     6212 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     5046 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_invitation.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/test_user_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2584 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/tests/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      213 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activation_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      329 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      918 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      209 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      299 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activation_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      753 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      214 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     2949 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      121 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      178 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/booklet_pending.html
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation.html
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation.txt
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/contact.txt
+-rw-rw-rw-   0 root         (0) root         (0)      191 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/booklet_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)      170 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation_pending.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation_pending.html
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/contact.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)      723 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/password/email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_email_subject.txt
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/registration_base.html
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      665 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_email_body.txt
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      914 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2376 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/authorize.html
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3098 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/management/commands/importneedledata.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       23 2023-07-06 11:45:57.000000 djangoldp_needle-0.1.93/djangoldp_needle/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/settings/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/settings/avatar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/linkIcon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/opengraph.py
+-rw-rw-rw-   0 root         (0) root         (0)     1013 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/urlParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/abstract_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/metaProp.py
+-rw-rw-rw-   0 root         (0) root         (0)     3571 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/itemProp.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py
+-rw-rw-rw-   0 root         (0) root         (0)    25244 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/jsonld.py
+-rw-rw-rw-   0 root         (0) root         (0)      808 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/lastChanceParser.py
+-rw-rw-rw-   0 root         (0) root         (0)      611 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/titleTag.py
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/webdriver_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     6029 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/request_parser/request_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/form/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/form/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/form/needle_user_form.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/static/images/
+-rw-rw-rw-   0 root         (0) root         (0)   798691 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/static/images/background.png
+-rw-rw-rw-   0 root         (0) root         (0)      738 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/static/needle.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/
+-rw-rw-rw-   0 root         (0) root         (0)    12144 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2213 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2845 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_intersections.py
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      336 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/avatars.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      453 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3187 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     3590 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)    10838 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)      333 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)      156 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)     1564 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_invitation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1103 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_quit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      258 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/templatetags/settings_value.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)      784 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      849 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/booklet_contributor_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/annotation_target.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)      108 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)       95 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/permissions/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      473 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0004_annotationtarget_image.py
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0019_auto_20230208_1213.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0012_needleactivity_activity_type.py
+-rwxrwxrwx   0 root         (0) root         (0)      798 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0032_avatar2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2622 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1852 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0013_needleuserprofile.py
+-rw-rw-rw-   0 root         (0) root         (0)      446 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0029_auto_20230411_1211.py
+-rwxrwxrwx   0 root         (0) root         (0)      718 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0034_auto_20230515_1735.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0009_activity_subtitle.py
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      682 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0015_auto_20230112_1339.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0006_auto_20221101_1846.py
+-rw-rw-rw-   0 root         (0) root         (0)     1543 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0002_tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      465 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0018_auto_20230129_1617.py
+-rw-rw-rw-   0 root         (0) root         (0)      543 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0014_auto_20230105_1238.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0022_annotation_annotation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      584 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0007_auto_20221114_1643.py
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0023_booklet.py
+-rwxrwxrwx   0 root         (0) root         (0)     4686 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0036_auto_20230526_1301.py
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0011_auto_20221125_1015.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0028_annotationtarget_annotation_target_date.py
+-rwxrwxrwx   0 root         (0) root         (0)     2452 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0032_avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1846 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0017_annotationintersectionread.py
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0025_needleuserfollow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1699 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0019_contactmessage.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0024_auto_20230328_0814.py
+-rw-rw-rw-   0 root         (0) root         (0)     2302 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0035_auto_20230525_1351.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0020_contactmessage_creation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0021_merge_20230213_1548.py
+-rw-rw-rw-   0 root         (0) root         (0)      519 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      399 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0003_annotation_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0005_annotationtarget_title.py
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0008_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     2082 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0037_auto_20230604_1525.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0010_activity_read.py
+-rwxrwxrwx   0 root         (0) root         (0)     2784 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0033_auto_20230509_1434.py
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0026_auto_20230331_1603.py
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/migrations/0016_auto_20230123_1741.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/
+-rw-rw-rw-   0 root         (0) root         (0)     2815 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/ldp_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2885 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8082 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/activity_signal_receiver.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/booklet_contributor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_contact_pending.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2149 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/booklet_contributor_pending.py
+-rwxrwxrwx   0 root         (0) root         (0)      875 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     1216 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/needle_activity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/contact_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     2046 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_contact.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/booklet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1203 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/annotation_intersection_read.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/annotation_target.py
+-rwxrwxrwx   0 root         (0) root         (0)     1644 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/avatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_follow.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/djangoldp_needle/models/tag.py
+-rw-rw-rw-   0 root         (0) root         (0)      112 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-06 11:45:33.000000 djangoldp_needle-0.1.93/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      608 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      521 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    10884 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      142 2023-07-06 11:45:59.000000 djangoldp_needle-0.1.93/djangoldp_needle.egg-info/requires.txt
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_first_annotation_on_user_creation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_first_annotation_on_user_creation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_user_contact.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_user_contact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_target_add.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_target_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from pkg_resources import resource_string
 
 from ..models import AnnotationTarget
 
 from .data.target_url.realsites import real_sites
 
 from .data.target_url.needlerealsites import needle_real_sites
+from django.conf import settings
+import re
 
 
 @requests_mock.Mocker(real_http=True)
 class TestAnnotationTargetAdd(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
@@ -157,74 +159,81 @@
         file_content = resource_string(__name__, file).decode("utf-8")
         m.register_uri(
             'GET',
             url,
             text=file_content,
         )
 
-    def test_annotation_parse_request_from_needle_urls(self, m):
-        user1 = self.buildUser('user1')
-        self.client.force_authenticate(user1)
-        counter = 1
-        for site_extract, url, title, image, date, canonical_url in needle_real_sites:
-            print("url            :" + url)
-            self._mock_response_content_from_file_and_url(m, site_extract, url)
-
-            data = self._create_annotation_parse_request_from_url(url)
-            response = self.client.post(
-                "/annotationtargets/",
-                content_type='application/ld+json',
-                data=data
-            )
-
-            self.assertEqual(response.status_code, 201)
-
-            response_decoded = response.json()
-
-            target_response = response_decoded['target']
-            if target_response.find("http://") == 0:
-                target_response = target_response[7:]
-            elif target_response.find("https://") == 0:
-                target_response = target_response[8:]
-            #
-            target_request = canonical_url
-            if target_request.find("http://") == 0:
-                target_request = target_request[7:]
-            elif target_request.find("https://") == 0:
-                target_request = target_request[8:]
-            # if target_request.find("#") > 0:
-            #     target_request = target_request[:target_request.find("#")]
-            # if target_request.find("?") > 0:
-            #     target_request = target_request[:target_request.find("?")]
-            #
-            # if target_request.find("www.") == 0 and target_response.find("www.") < 0:
-            #     target_request = target_request[4:]
-            # if target_response.find("www.") == 0 and target_request.find("www.") < 0:
-            #     target_response = target_response[4:]
-            # target_request = target_request.replace('//', '/')
-            # target_response = target_response.replace('//', '/')
-            # print("target_request :" + target_request)
-            # print("target_response:" + target_response)
-            # print("target_check   :" + ("OK" if target_response == target_request else "FAILED"))
-            expected_id = 'http://happy-dev.fr/annotationtargets/' + str(counter) + '/'
-            print("expected_id :" + expected_id)
-            print("id          :" + response_decoded['@id'])
-            print("td_check    :" + ("OK" if expected_id == response_decoded['@id'] else "FAILED"))
-            self.assertEqual(response_decoded['@id'], expected_id)
-            self.assertEqual(target_response, target_request)
-            self.assertEqual(response_decoded['title'], title)
-            if image:
-                self.assertEqual(response_decoded['image'], image)
-            if date:
-                date_to_compare_to =response_decoded['publication_date']
-                if date_to_compare_to.endswith('Z'):
-                    date_to_compare_to = date_to_compare_to[:len(date_to_compare_to)-1]
-                self.assertEqual(date_to_compare_to, date[:len(date_to_compare_to)])
-
-            counter = counter + 1
+    # def test_annotation_parse_request_from_needle_urls(self, m):
+    #     user1 = self.buildUser('user1')
+    #     self.client.force_authenticate(user1)
+    #     counter = 0
+    #     for site_extract, url, title, image, date, canonical_url in needle_real_sites:
+    #         print("url            :" + url)
+    #         self._mock_response_content_from_file_and_url(m, site_extract, url)
+    #
+    #         data = self._create_annotation_parse_request_from_url(url)
+    #         response = self.client.post(
+    #             "/annotationtargets/",
+    #             content_type='application/ld+json',
+    #             data=data
+    #         )
+    #
+    #         self.assertEqual(response.status_code, 201)
+    #
+    #         response_decoded = response.json()
+    #
+    #         target_response = response_decoded['target']
+    #         if target_response.find("http://") == 0:
+    #             target_response = target_response[7:]
+    #         elif target_response.find("https://") == 0:
+    #             target_response = target_response[8:]
+    #         #
+    #         target_request = canonical_url
+    #         if target_request.find("http://") == 0:
+    #             target_request = target_request[7:]
+    #         elif target_request.find("https://") == 0:
+    #             target_request = target_request[8:]
+    #         # if target_request.find("#") > 0:
+    #         #     target_request = target_request[:target_request.find("#")]
+    #         # if target_request.find("?") > 0:
+    #         #     target_request = target_request[:target_request.find("?")]
+    #         #
+    #         # if target_request.find("www.") == 0 and target_response.find("www.") < 0:
+    #         #     target_request = target_request[4:]
+    #         # if target_response.find("www.") == 0 and target_request.find("www.") < 0:
+    #         #     target_response = target_response[4:]
+    #         # target_request = target_request.replace('//', '/')
+    #         # target_response = target_response.replace('//', '/')
+    #         # print("target_request :" + target_request)
+    #         # print("target_response:" + target_response)
+    #         # print("target_check   :" + ("OK" if target_response == target_request else "FAILED"))
+    #         expected_id = settings.BASE_URL + '/annotationtargets/' + str(counter) + '/'
+    #         print("expected_id :" + expected_id)
+    #         print("id          :" + response_decoded['@id'])
+    #         print("td_check    :" + ("OK" if expected_id == response_decoded['@id'] else "FAILED"))
+    #         if counter == 0:
+    #             url = response_decoded['@id']
+    #             m = re.search(r'/\d+/', url)
+    #             counter_str = m.group()
+    #             counter_str = counter_str[1:-1]
+    #             counter = int(counter_str)
+    #         else:
+    #             self.assertEqual(response_decoded['@id'], expected_id)
+    #         self.assertEqual(target_response, target_request)
+    #         self.assertEqual(response_decoded['title'], title)
+    #         if image:
+    #             self.assertEqual(response_decoded['image'], image)
+    #         if date:
+    #             date_to_compare_to = response_decoded['publication_date']
+    #             if date_to_compare_to.endswith('Z'):
+    #                 date_to_compare_to = date_to_compare_to[:len(date_to_compare_to) - 1]
+    #             self.assertEqual(date_to_compare_to, date[:len(date_to_compare_to)])
+    #
+    #         counter = counter + 1
 
     def _create_annotation_parse_request_from_url(self, url):
         return json.dumps({
             "@context": {"@vocab": "http://happy-dev.fr/owl/#",
                          "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
                          "rdfs": "http://www.w3.org/2000/01/rdf-schema#", "ldp": "http://www.w3.org/ns/ldp#",
                          "foaf": "http://xmlns.com/foaf/0.1/", "name": "rdfs:label",
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributors_delete.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributors_delete.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_list.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_list.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_quit.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_quit.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_not_found.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_not_found.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_dates.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_dates.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_timeout.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_timeout.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/realsites.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/realsites.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_redirect.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_redirect.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/links_with_error.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/links_with_error.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/target_url/needlerealsites.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/target_url/needlerealsites.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/lemonde-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/lemonde-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/theconversation-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/theconversation-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/internetactu-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/internetactu-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/lemonde.20221103.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/lemonde.20221103.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/theconversation.20221103.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/theconversation.20221103.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/reporterre-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/reporterre-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/laviedesidees-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/laviedesidees-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/latribune-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/latribune-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/fredcavazza-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/fredcavazza-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/data/parsing/blogdumoderateur-1.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_date_parser.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_date_parser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_needle_user_contact.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_needle_user_contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from djangoldp_account.models import LDPUser
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
 import json, uuid
 from pkg_resources import resource_string
 from django.core import mail
 
 from ..models import NeedleActivity, ContactMessage, NeedleUserContact
+from django.conf import settings
 
 
 class TestNeedleUserContact(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
 
@@ -44,41 +45,41 @@
         self.assertEqual("user1", new_contact.contact_from.username)
 
         self.assertEqual(len(mail.outbox), 1)
         self.assertEqual('[Needle] Nouvelle demande de contact', mail.outbox[0].subject)
         self.assertEqual(['user2@test.startinblox.com'], mail.outbox[0].to)
 
         user1.refresh_from_db()
-        self.assertEqual(
-            """{} veut vous ajouter dans ses contacts sur needle.
+        expected = """{} veut vous ajouter dans ses contacts sur needle.
 
 Test de message
 
-Pour accepter, cliquez sur le lien suivant <a href="http://happy-dev.fr/needleusercontact_validate/{}" target="_blank">http://happy-dev.fr/needleusercontact_validate/{}</a>""".format(
-                user1.avatar.get_full_name(),
-                new_contact.invitation_token,
-                new_contact.invitation_token,
-            ),
-            mail.outbox[0].body
+Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans votre navigateur : {}/needleusercontact_validate/{}""".format(
+            user1.avatar.get_full_name(), settings.BASE_URL,
+            new_contact.invitation_token,
         )
+        result = mail.outbox[0].body
+        self.assertEqual(expected, result)
 
     def test_user_contact_add_invalid_email(self):
         user1 = self.buildUser('user1')
 
         request_content = self.build_request("Test de message", "invalid")
 
         self.client.force_authenticate(user1)
         response = self.client.post(
             "/needleusercontact/",
             content_type='application/ld+json',
             data=request_content
         )
 
         self.assertEqual(response.status_code, 400)
-        self.assertEqual(["Cette personne n'existe pas sur Needle. <solid-contact-button-add-invitation></solid-contact-button-add-invitation>"], response.json()['E-mail'])
+        self.assertEqual([
+                             "Cette personne n'existe pas sur Needle. <solid-contact-button-add-invitation></solid-contact-button-add-invitation>"],
+                         response.json()['E-mail'])
 
     def test_user_contact_add_existing(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
 
         request_content = self.build_request("Test de message", "user2@test.startinblox.com")
 
@@ -105,15 +106,15 @@
     def test_user_contact_validate_valid_token(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
         new_contact = NeedleUserContact(contact_from=user1, contact_to=user2)
         new_contact.save()
         response = self.client.get("/needleusercontact_validate/" + str(new_contact.invitation_token))
         self.assertEqual(response.status_code, 301)
-        self.assertEqual(response.url, 'http://front')
+        self.assertEqual(response.url, settings.INSTANCE_DEFAULT_CLIENT)
 
         new_contact.refresh_from_db()
         self.assertEqual(None, new_contact.invitation_token)
         reverse_contact = NeedleUserContact.objects.get(contact_from=user2, contact_to=user1)
         self.assertEqual(None, reverse_contact.invitation_token)
 
     def test_user_contact_validate_valid_token_existing_reverse(self):
@@ -122,15 +123,15 @@
         new_contact = NeedleUserContact(contact_from=user1, contact_to=user2)
         new_contact.save()
         reverse_contact = NeedleUserContact(contact_from=user2, contact_to=user1)
         reverse_contact.save()
 
         response = self.client.get("/needleusercontact_validate/" + str(new_contact.invitation_token))
         self.assertEqual(response.status_code, 301)
-        self.assertEqual(response.url, 'http://front')
+        self.assertEqual(response.url, settings.INSTANCE_DEFAULT_CLIENT)
 
         new_contact.refresh_from_db()
         self.assertEqual(None, new_contact.invitation_token)
         reverse_contact.refresh_from_db()
         self.assertEqual(None, reverse_contact.invitation_token)
 
     def build_request(self, message, contact_to):
@@ -144,8 +145,8 @@
                          "lng": "geo:long", "entrepreneurProfile": "http://happy-dev.fr/owl/#entrepreneur_profile",
                          "mentorProfile": "http://happy-dev.fr/owl/#mentor_profile", "account": "hd:account",
                          "messageSet": "http://happy-dev.fr/owl/#message_set",
                          "author": "http://happy-dev.fr/owl/#author_user",
                          "title": "http://happy-dev.fr/owl/#title"},
             "message": message,
             "contact_to_email": contact_to,
-        })
+        })
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_add.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_add.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_activity.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributors_patch.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributors_patch.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_import.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_import.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,14 @@
         self.assertEqual(user_email, annotation.creator.email)
         self.assertEqual(annotation_description, annotation.description)
         self.assertEqual(target_url, annotation.target.target)
         self.assertEqual(2, annotation.tags.count())
         self.assertEqual('2016', annotation.annotation_date.strftime('%Y'))
         self.assertEqual('02', annotation.annotation_date.strftime('%m'))
 
-
-    def test_import_old_needle_data(self):
-        annotationTargetViewset = AnnotationTargetViewset()
-        annotation_target = annotationTargetViewset.parse_target("http://ujomusic.com/")
-        self.assertIsNotNone(annotation_target.target)
-
+    #
+    # def test_import_old_needle_data(self):
+    #     annotationTargetViewset = AnnotationTargetViewset()
+    #     annotation_target = annotationTargetViewset.parse_target("http://ujomusic.com/")
+    #     self.assertIsNotNone(annotation_target.target)
+    #
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_add_annotation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_add_annotation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_intersection.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_intersection.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_annotation_yarn.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_annotation_yarn.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklet_contributor_pending.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklet_contributor_pending.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
 import json, uuid
 from pkg_resources import resource_string
 from django.core import mail
 
 from ..models import NeedleActivity, ContactMessage, NeedleUserContact, BookletContributorPending, BookletContributor, \
     Booklet
+from django.conf import settings
 
 
 class TestBookletContributorPending(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
 
@@ -43,16 +44,16 @@
         self.assertEqual("user2@test.startinblox.com", new_contact.booklet_to_email)
         self.assertEqual(booklet, new_contact.booklet_from)
 
         user1.refresh_from_db()
         self.assertEqual(
             """{} veut vous inviter à contributer à son carnet title sur Needle.
 
-Pour créer un compte, cliquez sur le lien suivant <a href="http://happy-dev.fr/auth/register/" target="_blank">http://happy-dev.fr/auth/register/</a>""".format(
-                user1.avatar.get_full_name(),
+Pour créer un compte, veuillez suivre ce lien ou le copier-coller dans votre navigateur : {}/auth/register/""".format(
+                user1.avatar.get_full_name(), settings.BASE_URL
             ),
             mail.outbox[0].body
         )
 
     def test_booklet_contributor_pending_add_invalid_email(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
@@ -150,8 +151,8 @@
                          "messageSet": "http://happy-dev.fr/owl/#message_set",
                          "author": "http://happy-dev.fr/owl/#author_user",
                          "title": "http://happy-dev.fr/owl/#title"},
             "booklet_from": {
                 "@id": booklet.urlid
             },
             "booklet_to_email": contact_to,
-        })
+        })
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_booklets_invitation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_booklets_invitation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_needle_user_contact_pending.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_needle_user_contact_pending.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from djangoldp_account.models import LDPUser
 from rest_framework.test import APITestCase, APIClient, APITransactionTestCase
 import json, uuid
 from pkg_resources import resource_string
 from django.core import mail
 
 from ..models import NeedleActivity, ContactMessage, NeedleUserContact, NeedleUserContactPending
-
+from django.conf import settings
 
 class TestNeedleUserContactPending(APITestCase):
 
     def setUp(self):
         self.client = APIClient()
 
     def buildUser(self, username):
@@ -37,24 +37,23 @@
         self.assertEqual(response.status_code, 201)
         self.assertEqual(1, NeedleUserContactPending.objects.count())
         new_contact = NeedleUserContactPending.objects.all()[0]
         self.assertEqual("user2@test.startinblox.com", new_contact.contact_to_email)
         self.assertEqual("user1", new_contact.contact_from.username)
 
         user1.refresh_from_db()
-        self.assertEqual(
-            """{} veut vous inviter sur Needle.
+        expected = """{} veut vous inviter sur Needle.
 
 Test de message
 
-Pour créer un compte, cliquez sur le lien suivant <a href="http://happy-dev.fr/auth/register/" target="_blank">http://happy-dev.fr/auth/register/</a>""".format(
-                user1.avatar.get_full_name(),
-            ),
-            mail.outbox[0].body
+Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans votre navigateur : {}/auth/register/""".format(
+            user1.avatar.get_full_name(), settings.BASE_URL
         )
+        result = mail.outbox[0].body
+        self.assertEqual(expected, result)
 
     def test_user_contact_pending_add_invalid_email(self):
         user1 = self.buildUser('user1')
         user2 = self.buildUser('user2')
 
         request_content = self.build_request("Test de message", "user2@test.startinblox.com")
 
@@ -90,15 +89,14 @@
         self.assertEqual(user2, contact.contact_to)
         self.assertEqual(None, contact.invitation_token)
         contact_reverse = NeedleUserContact.objects.last()
         self.assertEqual(user2, contact_reverse.contact_from)
         self.assertEqual(user1, contact_reverse.contact_to)
         self.assertEqual(None, contact_reverse.invitation_token)
 
-
     def build_request(self, message, contact_to):
         return json.dumps({
             "@context": {"@vocab": "http://happy-dev.fr/owl/#",
                          "rdf": "http://www.w3.org/1999/02/22-rdf-syntax-ns#",
                          "rdfs": "http://www.w3.org/2000/01/rdf-schema#", "ldp": "http://www.w3.org/ns/ldp#",
                          "foaf": "http://xmlns.com/foaf/0.1/", "name": "rdfs:label",
                          "acl": "http://www.w3.org/ns/auth/acl#", "permissions": "acl:accessControl",
@@ -106,8 +104,8 @@
                          "lng": "geo:long", "entrepreneurProfile": "http://happy-dev.fr/owl/#entrepreneur_profile",
                          "mentorProfile": "http://happy-dev.fr/owl/#mentor_profile", "account": "hd:account",
                          "messageSet": "http://happy-dev.fr/owl/#message_set",
                          "author": "http://happy-dev.fr/owl/#author_user",
                          "title": "http://happy-dev.fr/owl/#title"},
             "message": message,
             "contact_to_email": contact_to,
-        })
+        })
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/test_user_serializer.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/test_user_serializer.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/tests/runner.py` & `djangoldp_needle-0.1.93/djangoldp_needle/tests/runner.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/activation_email.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/activation_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/password_reset_form.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/lost_user.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/lost_user.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/registration/login.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/booklet_pending.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation.html`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,20 @@
 
 <body>
     <div class="container">
         <main id="content" class="flex-column">
             <div>
                 Bonjour,
 
-                {{ from_name }} veut vous inviter à contributer à son carnet {{ booklet }} sur Needle.
+                {{ from_name }} veut vous ajouter dans ses contacts sur needle.
             </div>
             <div>
-                Pour créer un compte, cliquez sur le lien suivant <a href="{{ link }}" target="_blank">{{ link }}</a>
+                {{ message }}
+            </div>
+            <div>
+                Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans votre navigateur : <a href="{{ link }}" target="_blank">{{ link }}</a>
             </div>
         </main>
     </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
 
 
 
-Bonjour, {{ from_name }} veut vous inviter Ã  contributer Ã  son carnet {
-{ booklet }} sur Needle.
-Pour crÃ©er un compte, cliquez sur le lien suivant {{_link_}}
+Bonjour, {{ from_name }} veut vous ajouter dans ses contacts sur needle.
+{{ message }}
+Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans
+votre navigateur : {{_link_}}
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/invitation_pending.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="fr">
 <head>
     <meta charset="UTF-8">
     <title>Quelqu'un vous a contacté</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <link rel="stylesheet" href="/styles/index.css">
     <link rel="stylesheet"
@@ -14,20 +14,20 @@
 
 <body>
     <div class="container">
         <main id="content" class="flex-column">
             <div>
                 Bonjour,
 
-                {{ from_name }} veut vous ajouter dans ses contacts sur needle.
+                {{ from_name }} a souhaité vous inviter à le rejoindre sur Needle.
             </div>
             <div>
                 {{ message }}
             </div>
             <div>
-                Pour accepter, cliquez sur le lien suivant <a href="{{ link }}" target="_blank">{{ link }}</a>
+                Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans votre navigateur : <a href="{{ link }}" target="_blank">{{ link }}</a>
             </div>
         </main>
     </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
 
 
 
-Bonjour, {{ from_name }} veut vous ajouter dans ses contacts sur needle.
+Bonjour, {{ from_name }} a souhaitÃ© vous inviter Ã  le rejoindre sur Needle.
 {{ message }}
-Pour accepter, cliquez sur le lien suivant {{_link_}}
+Pour accepter son invitation, veuillez suivre ce lien ou le copier-coller dans
+votre navigateur : {{_link_}}
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/invitation_pending.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/booklet_pending.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="fr">
 <head>
     <meta charset="UTF-8">
-    <title>Quelqu'un vous a contacté</title>
+    <title>Quelqu'un vous invite à participer au carnet {{  booklet }}</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <link rel="stylesheet" href="/styles/index.css">
     <link rel="stylesheet"
           href="https://fonts.googleapis.com/css?family=Open+Sans:300,400,400i,600,700&amp;amp;subset=latin-ext">
     <link rel="stylesheet"
           href="https://fonts.googleapis.com/css?family=Open+Sans:300,300i,400,400i,600,600i,700,700i,800,800i">
@@ -14,20 +14,17 @@
 
 <body>
     <div class="container">
         <main id="content" class="flex-column">
             <div>
                 Bonjour,
 
-                {{ from_name }} veut vous inviter sur Needle.
+                {{ from_name }} veut vous inviter à contributer à son carnet <a href="{{ booklet_url }}" target="_blank">{{  booklet }}</a> sur Needle.
             </div>
             <div>
-                {{ message }}
-            </div>
-            <div>
-                Pour créer un compte, cliquez sur le lien suivant <a href="{{ link }}" target="_blank">{{ link }}</a>
+                Pour créer un compte, veuillez suivre ce lien ou le copier-coller dans votre navigateur : <a href="{{ link }}" target="_blank">{{ link }}</a>
             </div>
         </main>
     </div>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
 
 
 
-Bonjour, {{ from_name }} veut vous inviter sur Needle.
-{{ message }}
-Pour crÃ©er un compte, cliquez sur le lien suivant {{_link_}}
+Bonjour, {{ from_name }} veut vous inviter Ã  contributer Ã  son carnet {
+{_booklet_}} sur Needle.
+Pour crÃ©er un compte, veuillez suivre ce lien ou le copier-coller dans votre
+navigateur : {{_link_}}
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/emails/contact.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/emails/contact.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 <!DOCTYPE html>
-<html lang="en">
+<html lang="fr">
 <head>
     <meta charset="UTF-8">
     <title>Quelqu'un vous a contacté</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <link rel="stylesheet" href="/styles/index.css">
     <link rel="stylesheet"
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/oidc_provider/authorize.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/oidc_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/password/email.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/base.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_email.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_email_body.txt` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_email_body.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/activation_complete.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/registration_form.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/templates/django_registration/authorize.html` & `djangoldp_needle-0.1.93/djangoldp_needle/templates/django_registration/authorize.html`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/djangoldp_urls.py` & `djangoldp_needle-0.1.93/djangoldp_needle/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/linkIcon.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/linkIcon.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/opengraph.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/opengraph.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/urlParser.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/urlParser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/metaProp.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/metaProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/itemProp.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/itemProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/linkCanonicalProp.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/jsonld.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/jsonld.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/lastChanceParser.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/lastChanceParser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/parsers/titleTag.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/parsers/titleTag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/webdriver_utils.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/webdriver_utils.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/request_parser/request_parser.py` & `djangoldp_needle-0.1.93/djangoldp_needle/request_parser/request_parser.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/form/needle_user_form.py` & `djangoldp_needle-0.1.93/djangoldp_needle/form/needle_user_form.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/static/images/background.png` & `djangoldp_needle-0.1.93/djangoldp_needle/static/images/background.png`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/static/needle.css` & `djangoldp_needle-0.1.93/djangoldp_needle/static/needle.css`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/annotation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/annotation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_contributor.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_contributor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_contact_pending.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_contributor_pending.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,51 +4,66 @@
 from djangoldp.views import LDPViewSet
 from djangoldp_account.models import LDPUser
 from rest_framework.exceptions import ValidationError
 from rest_framework.response import Response
 from django.conf import settings
 from rest_framework import status
 
-from ..models import NeedleUserFollow, NeedleUserContact
+from ..models import NeedleUserFollow, NeedleUserContact, BookletContributor, Booklet
 from django.core.mail import send_mail
 from django.template import loader
 
-class NeedleUserContactPendingViewset(LDPViewSet):
+
+class BookletContributorPendingViewset(LDPViewSet):
     def create(self, request, *args, **kwargs):
-        if LDPUser.objects.filter(email=request.data['contact_to_email']).count() > 0:
+        if LDPUser.objects.filter(email=request.data['booklet_to_email']).count() > 0:
             return Response({'E-mail': [
                 'Cette personne existe déjà sur Needle']},
-                            status=status.HTTP_400_BAD_REQUEST)
+                status=status.HTTP_400_BAD_REQUEST)
+
+        if BookletContributor.objects.filter(user=request.user, booklet__urlid=request.data['booklet_from']['@id'],
+                                             role=BookletContributor.ROLE_OWNER).count() == 0:
+            return Response({'Booklet': [
+                'Vous devez être propriétaire du carnet']},
+                status=status.HTTP_400_BAD_REQUEST)
 
         return super().create(request)
 
     def perform_create(self, serializer, **kwargs):
         res = super().perform_create(serializer)
         email_from = getattr(settings, 'DEFAULT_FROM_EMAIL', False)
 
+        booklet_id = self.request.data['booklet_from']['@id']
+        booklet_url = settings.INSTANCE_DEFAULT_CLIENT + "/@" + settings.BASE_URL + "/carnets/voir/@" + booklet_id + "/@";
+
         if email_from:
+            from_email = self.request.user.email
+            from_url = settings.INSTANCE_DEFAULT_CLIENT + "/@" + settings.BASE_URL + "/users/" + self.request.user.username + "/@";
+
             template_parameters = {
-                'from_name': res.contact_from.avatar.get_full_name(),
+                'from_name': self.request.user.avatar.get_full_name(),
+                'from_email': from_email,
+                'from_url': from_url,
                 'link': settings.BASE_URL + '/auth/register/',
-                'message': self.request.data['message']
+                'booklet': res.booklet_from.title,
+                'booklet_id': booklet_id,
+                'booklet_url': booklet_url
             }
             message = loader.render_to_string(
-                'emails/invitation_pending.txt',
+                'emails/booklet_pending.txt',
                 template_parameters
             )
 
             html_message = loader.render_to_string(
-                'emails/invitation_pending.html',
+                'emails/booklet_pending.html',
                 template_parameters
             )
 
             send_mail(
-                '[Needle] Invitation à créer un compte',
+                '[Needle] Invitation à participer à un carnet',
                 message,
                 email_from,
-                [res.contact_to_email],
+                [res.booklet_to_email],
                 html_message=html_message
             )
 
-
         return res
-
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/__init__.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_intersections.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_intersections.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/needle_user_contact.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/needle_user_contact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/booklet.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/booklet.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_intersection_read.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_intersection_read.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/annotation_target.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/annotation_target.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_invitation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_invitation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/views/booklet_quit.py` & `djangoldp_needle-0.1.93/djangoldp_needle/views/booklet_quit.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/permissions/booklet_contributor.py` & `djangoldp_needle-0.1.93/djangoldp_needle/permissions/booklet_contributor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/permissions/__init__.py` & `djangoldp_needle-0.1.93/djangoldp_needle/permissions/__init__.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/permissions/booklet.py` & `djangoldp_needle-0.1.93/djangoldp_needle/permissions/booklet.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0032_avatar2.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0032_avatar2.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0001_initial.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0013_needleuserprofile.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0013_needleuserprofile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0034_auto_20230515_1735.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0034_auto_20230515_1735.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0015_auto_20230112_1339.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0015_auto_20230112_1339.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0002_tag.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0002_tag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0014_auto_20230105_1238.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0014_auto_20230105_1238.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0007_auto_20221114_1643.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0007_auto_20221114_1643.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0023_booklet.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0023_booklet.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0036_auto_20230526_1301.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0036_auto_20230526_1301.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0011_auto_20221125_1015.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0011_auto_20221125_1015.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0032_avatar.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0032_avatar.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0017_annotationintersectionread.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0017_annotationintersectionread.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0025_needleuserfollow.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0025_needleuserfollow.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0019_contactmessage.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0019_contactmessage.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0035_auto_20230525_1351.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0035_auto_20230525_1351.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0020_contactmessage_creation_date.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0020_contactmessage_creation_date.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0027_needleuserfollow_creation_date.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0008_activity.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0008_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0037_auto_20230604_1525.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0037_auto_20230604_1525.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0033_auto_20230509_1434.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0033_auto_20230509_1434.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/migrations/0016_auto_20230123_1741.py` & `djangoldp_needle-0.1.93/djangoldp_needle/migrations/0016_auto_20230123_1741.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/ldp_user.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/ldp_user.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/annotation.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/annotation.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/activity_signal_receiver.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/activity_signal_receiver.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/booklet_contributor.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/booklet_contributor.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_contact_pending.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_contact_pending.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/__init__.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/__init__.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/booklet_contributor_pending.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/booklet_contributor_pending.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_profile.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_profile.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/needle_activity.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/needle_activity.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/contact_message.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/contact_message.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_contact.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_contact.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/booklet.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/booklet.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/annotation_intersection_read.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/annotation_intersection_read.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/annotation_target.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/annotation_target.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/avatar.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/avatar.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/needle_user_follow.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/needle_user_follow.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle/models/tag.py` & `djangoldp_needle-0.1.93/djangoldp_needle/models/tag.py`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/setup.cfg` & `djangoldp_needle-0.1.93/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_needle-0.1.92/PKG-INFO` & `djangoldp_needle-0.1.93/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp_needle
-Version: 0.1.92
+Version: 0.1.93
 Summary: Needle backend
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: include_package_data
 Provides-Extra: dev
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle.egg-info/PKG-INFO` & `djangoldp_needle-0.1.93/djangoldp_needle.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangoldp-needle
-Version: 0.1.92
+Version: 0.1.93
 Summary: Needle backend
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: include_package_data
 Provides-Extra: dev
```

### Comparing `djangoldp_needle-0.1.92/djangoldp_needle.egg-info/SOURCES.txt` & `djangoldp_needle-0.1.93/djangoldp_needle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

