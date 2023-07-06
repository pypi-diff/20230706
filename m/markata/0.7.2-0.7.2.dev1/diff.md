# Comparing `tmp/markata-0.7.2.tar.gz` & `tmp/markata-0.7.2.dev1.tar.gz`

## Comparing `markata-0.7.2.tar` & `markata-0.7.2.dev1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.2/.markataignore
--rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 markata-0.7.2/CHANGELOG.md
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 markata-0.7.2/SECURITY.md
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.2/contributing.md
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.2/markata.toml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.2/docs/404.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.2/docs/color-theme.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.2/docs/home-page.md
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.2/docs/index.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.2/docs/nav.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.2/docs/project-gallery/markata_dev.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.2/docs/project-gallery/waylonwalker.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__about__.py
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__main__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.2/markata/background.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.2/markata/errors.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.2/markata/hookspec.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.2/markata/lifecycle.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.2/markata/standard_config.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/__main__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/cli.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/header.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/plugins.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/runner.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/server.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/summary.py
--rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/Karla-Regular.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/auto_description.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/auto_title.py
--rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/base_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/copy_assets.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/covers.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/create_covers.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/datetime.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_doc_template.md
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_log_template.html
--rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_post_template.html
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_redirect_template.html
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_service_worker_template.js
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/docs.py
--rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/feeds.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/flat_slug.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/generator.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/glob.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/heading_link.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/icon_resize.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/jinja_md.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/load.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/manifest.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/md_it_highlight_code.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/md_it_wikilinks.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/mdit_details.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/post_template.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/prevnext.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/prevnext_template.html
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_dev_to_source.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_html.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_source.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/pyinstrument.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/redirects.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/render_markdown.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/rss.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/seo.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/service_worker.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/setup_logging.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/sitemap.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/subroute.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/to_json.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/tui.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.2/markata/scripts/migrate_to_slugify.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.2/static/_redirects
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.2/static/favicon.ico
--rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.2/static/markata.dev_.webp
--rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.2/static/markata.dev_markata_plugins_base-cli_.webp
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.2/static/robots.txt
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com.webp
--rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com_archive.webp
--rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com_markata-configure-head.webp
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_doc_page.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_feeds.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_one_default_page.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_one_default_page_with_path_prefix.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/conftest.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_default_post_template.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_flat_slug.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_redirects.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.2/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 markata-0.7.2/LICENSE
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 markata-0.7.2/README.md
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 markata-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 markata-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/.markataignore
+-rw-r--r--   0        0        0    17938 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/CHANGELOG.md
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/SECURITY.md
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/contributing.md
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata.toml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/404.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/color-theme.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/home-page.md
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/index.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/nav.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/project-gallery/markata_dev.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/docs/project-gallery/waylonwalker.md
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/__about__.py
+-rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/__main__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/background.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/errors.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/hookspec.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/lifecycle.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/standard_config.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/__main__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/cli.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/header.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/plugins.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/runner.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/server.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/cli/summary.py
+-rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/Karla-Regular.ttf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/auto_description.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/auto_title.py
+-rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/base_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/copy_assets.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/covers.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/create_covers.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/datetime.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/default_doc_template.md
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/default_log_template.html
+-rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/default_post_template.html
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/default_redirect_template.html
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/default_service_worker_template.js
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/docs.py
+-rw-r--r--   0        0        0    13029 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/feeds.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/flat_slug.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/generator.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/glob.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/heading_link.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/icon_resize.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/jinja_md.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/load.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/manifest.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/md_it_highlight_code.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/md_it_wikilinks.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/mdit_details.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/post_template.py
+-rw-r--r--   0        0        0     4463 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/prevnext.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/prevnext_template.html
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/publish_dev_to_source.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/publish_html.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/publish_source.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/pyinstrument.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/redirects.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/render_markdown.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/rss.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/seo.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/service_worker.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/setup_logging.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/sitemap.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/subroute.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/to_json.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/plugins/tui.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/markata/scripts/migrate_to_slugify.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/_redirects
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/favicon.ico
+-rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/markata.dev_.webp
+-rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/markata.dev_markata_plugins_base-cli_.webp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/robots.txt
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/waylonwalker.com.webp
+-rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/waylonwalker.com_archive.webp
+-rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/static/waylonwalker.com_markata-configure-head.webp
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/test_doc_page.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/test_feeds.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/test_one_default_page.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/test_one_default_page_with_path_prefix.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/plugins/test_default_post_template.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/plugins/test_flat_slug.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/tests/plugins/test_redirects.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/README.md
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 markata-0.7.2.dev1/PKG-INFO
```

### Comparing `markata-0.7.2/CHANGELOG.md` & `markata-0.7.2.dev1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Markata Changelog
 
+## 0.7.3
+
+- Fix: broken default feed card template
+- Fix: broken links for index.md in feeds
+
+## 0.7.2
+
+- Fix: broken `markata new` command due to pydantic v2 compatability with copier.
+
 ## 0.7.0
 
 - Adopt ruff linter 0.7.0.dev1 #142
 - add support for markdown_it_py backend #145
 - add trogon tui support 0.7.0.dev6
 
 ### trogon tui support
@@ -16,14 +25,18 @@
 
 usage
 
 ```bash
 markata tui
 ```
 
+## 0.6.3
+
+- Fix: broken `markata new` command due to pydantic v2 compatability with copier.
+
 ## 0.6.1
 
 - Fix: allow feeds to be used from within markdown
 
 ### Feeds in markdown
 
 ```markdown
@@ -75,14 +88,18 @@
 > ProTip: this was highly inspired by the
 > [marksman-lsp](https://github.com/artempyanykh/marksman) by
 > [artempyanykh](https://github.com/artempyanykh/) which can autocomplete post
 > links in this style for you.
 
 [[home-page]]
 
+## 0.5.4
+
+- Fix: broken `markata new` command due to pydantic v2 compatability with copier.
+
 ## 0.5.2
 
 - clean up unnecessary images_url is missing warning #104 0.5.2.dev1
 
 ## 0.5.1
 
 - fix: contrast ratio on admonitions was insufficient for A11y #103 0.5.1.dev0
```

### Comparing `markata-0.7.2/CODE_OF_CONDUCT.md` & `markata-0.7.2.dev1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/contributing.md` & `markata-0.7.2.dev1/contributing.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata.toml` & `markata-0.7.2.dev1/markata.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/color-theme.md` & `markata-0.7.2.dev1/docs/color-theme.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/home-page.md` & `markata-0.7.2.dev1/docs/home-page.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/index.md` & `markata-0.7.2.dev1/docs/index.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/nav.md` & `markata-0.7.2.dev1/docs/nav.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/project-gallery/markata_dev.md` & `markata-0.7.2.dev1/docs/project-gallery/markata_dev.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/docs/project-gallery/waylonwalker.md` & `markata-0.7.2.dev1/docs/project-gallery/waylonwalker.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/__init__.py` & `markata-0.7.2.dev1/markata/__init__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/background.py` & `markata-0.7.2.dev1/markata/background.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/hookspec.py` & `markata-0.7.2.dev1/markata/hookspec.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/lifecycle.py` & `markata-0.7.2.dev1/markata/lifecycle.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/standard_config.py` & `markata-0.7.2.dev1/markata/standard_config.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/__main__.py` & `markata-0.7.2.dev1/markata/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/cli.py` & `markata-0.7.2.dev1/markata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/plugins.py` & `markata-0.7.2.dev1/markata/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/runner.py` & `markata-0.7.2.dev1/markata/cli/runner.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/server.py` & `markata-0.7.2.dev1/markata/cli/server.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/cli/summary.py` & `markata-0.7.2.dev1/markata/cli/summary.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/Karla-Regular.ttf` & `markata-0.7.2.dev1/markata/plugins/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/auto_description.py` & `markata-0.7.2.dev1/markata/plugins/auto_description.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/base_cli.py` & `markata-0.7.2.dev1/markata/plugins/base_cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/copy_assets.py` & `markata-0.7.2.dev1/markata/plugins/copy_assets.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/covers.py` & `markata-0.7.2.dev1/markata/plugins/covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/create_covers.py` & `markata-0.7.2.dev1/markata/plugins/create_covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/datetime.py` & `markata-0.7.2.dev1/markata/plugins/datetime.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/default_doc_template.md` & `markata-0.7.2.dev1/markata/plugins/default_doc_template.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/default_log_template.html` & `markata-0.7.2.dev1/markata/plugins/default_log_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/default_post_template.html` & `markata-0.7.2.dev1/markata/plugins/default_post_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/default_redirect_template.html` & `markata-0.7.2.dev1/markata/plugins/default_redirect_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/default_service_worker_template.js` & `markata-0.7.2.dev1/markata/plugins/default_service_worker_template.js`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/docs.py` & `markata-0.7.2.dev1/markata/plugins/docs.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/feeds.py` & `markata-0.7.2.dev1/markata/plugins/feeds.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
         template = markata.config.get("feeds_config", {}).get("card_template", None)
 
     if template is None:
         if "date" in post.keys():
             return textwrap.dedent(
                 f"""
                 <li class='post'>
-                <a href="/{markata.config.get('path_prefix', '')}{post['slug']}/">
+                <a href="/{markata.config.get('path_prefix', '')}{'' if post['slug'] == 'index' else post['slug'] + '/'}">
                     {post['title']}
                     {post['date'].year}-
                     {post['date'].month}-
                     {post['date'].day}
                 </a>
                 </li>
                 """
```

### Comparing `markata-0.7.2/markata/plugins/flat_slug.py` & `markata-0.7.2.dev1/markata/plugins/flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/generator.py` & `markata-0.7.2.dev1/markata/plugins/generator.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/glob.py` & `markata-0.7.2.dev1/markata/plugins/glob.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/heading_link.py` & `markata-0.7.2.dev1/markata/plugins/heading_link.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/icon_resize.py` & `markata-0.7.2.dev1/markata/plugins/icon_resize.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/jinja_md.py` & `markata-0.7.2.dev1/markata/plugins/jinja_md.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/load.py` & `markata-0.7.2.dev1/markata/plugins/load.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/manifest.py` & `markata-0.7.2.dev1/markata/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/md_it_highlight_code.py` & `markata-0.7.2.dev1/markata/plugins/md_it_highlight_code.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/md_it_wikilinks.py` & `markata-0.7.2.dev1/markata/plugins/md_it_wikilinks.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/mdit_details.py` & `markata-0.7.2.dev1/markata/plugins/mdit_details.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/post_template.py` & `markata-0.7.2.dev1/markata/plugins/post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/prevnext.py` & `markata-0.7.2.dev1/markata/plugins/prevnext.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         post_idx = posts.index(post)
         return PrevNext(prev=posts[post_idx - 1], next=posts[post_idx + 1])
     except ValueError:
         # post is not in posts
         return None
 
 
-TEMPLATE = Path(__file__).parent / "prevnext_template.html"
+TEMPLATE = (Path(__file__).parent / "prevnext_template.html").read_text()
 
 
 @hook_impl
 @register_attr("prevnext")
 def pre_render(markata: "Markata") -> None:
     config = markata.config.get("prevnext", {})
     feed_config = markata.config.get("feeds", {})
```

### Comparing `markata-0.7.2/markata/plugins/prevnext_template.html` & `markata-0.7.2.dev1/markata/plugins/prevnext_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/publish_dev_to_source.py` & `markata-0.7.2.dev1/markata/plugins/publish_dev_to_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/publish_html.py` & `markata-0.7.2.dev1/markata/plugins/publish_html.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/publish_source.py` & `markata-0.7.2.dev1/markata/plugins/publish_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/pyinstrument.py` & `markata-0.7.2.dev1/markata/plugins/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/redirects.py` & `markata-0.7.2.dev1/markata/plugins/redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/render_markdown.py` & `markata-0.7.2.dev1/markata/plugins/render_markdown.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/rss.py` & `markata-0.7.2.dev1/markata/plugins/rss.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/seo.py` & `markata-0.7.2.dev1/markata/plugins/seo.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/service_worker.py` & `markata-0.7.2.dev1/markata/plugins/service_worker.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/setup_logging.py` & `markata-0.7.2.dev1/markata/plugins/setup_logging.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/sitemap.py` & `markata-0.7.2.dev1/markata/plugins/sitemap.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/subroute.py` & `markata-0.7.2.dev1/markata/plugins/subroute.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/plugins/tui.py` & `markata-0.7.2.dev1/markata/plugins/tui.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/markata/scripts/migrate_to_slugify.py` & `markata-0.7.2.dev1/markata/scripts/migrate_to_slugify.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/_redirects` & `markata-0.7.2.dev1/static/_redirects`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/favicon.ico` & `markata-0.7.2.dev1/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/markata.dev_.webp` & `markata-0.7.2.dev1/static/markata.dev_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/markata.dev_markata_plugins_base-cli_.webp` & `markata-0.7.2.dev1/static/markata.dev_markata_plugins_base-cli_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/waylonwalker.com.webp` & `markata-0.7.2.dev1/static/waylonwalker.com.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/waylonwalker.com_archive.webp` & `markata-0.7.2.dev1/static/waylonwalker.com_archive.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/static/waylonwalker.com_markata-configure-head.webp` & `markata-0.7.2.dev1/static/waylonwalker.com_markata-configure-head.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/test_doc_page.py` & `markata-0.7.2.dev1/tests/test_doc_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/test_feeds.py` & `markata-0.7.2.dev1/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/test_one_default_page.py` & `markata-0.7.2.dev1/tests/test_one_default_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/test_one_default_page_with_path_prefix.py` & `markata-0.7.2.dev1/tests/test_one_default_page_with_path_prefix.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/plugins/test_default_post_template.py` & `markata-0.7.2.dev1/tests/plugins/test_default_post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/plugins/test_flat_slug.py` & `markata-0.7.2.dev1/tests/plugins/test_flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/tests/plugins/test_redirects.py` & `markata-0.7.2.dev1/tests/plugins/test_redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/.gitignore` & `markata-0.7.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/LICENSE` & `markata-0.7.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/README.md` & `markata-0.7.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/pyproject.toml` & `markata-0.7.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.2/PKG-INFO` & `markata-0.7.2.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markata
-Version: 0.7.2
+Version: 0.7.2.dev1
 Summary: Static site generator plugins all the way down.
 Project-URL: Homepage, https://markata.dev
 Project-URL: Changelog, https://markata.dev/CHANGELOG/
 Project-URL: Source, https://github.com/waylonwalker/markata
 Project-URL: Issues, https://github.com/waylonwalker/markata/issues
 Project-URL: Documentation, https://markata.dev
 Author-email: Waylon Walker <waylon@waylonwalker.com>, waylon@markata.dev
```

