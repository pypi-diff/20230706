# Comparing `tmp/markata-0.7.1.dev0.tar.gz` & `tmp/markata-0.7.2.tar.gz`

## Comparing `markata-0.7.1.dev0.tar` & `markata-0.7.2.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/.markataignore
--rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/CHANGELOG.md
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/SECURITY.md
--rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/contributing.md
--rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata.toml
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/404.md
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/color-theme.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/home-page.md
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/index.md
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/nav.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/project-gallery/markata_dev.md
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/docs/project-gallery/waylonwalker.md
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/__about__.py
--rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/__main__.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/background.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/errors.py
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/hookspec.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/lifecycle.py
--rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/standard_config.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/__init__.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/__main__.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/cli.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/header.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/plugins.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/runner.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/server.py
--rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/cli/summary.py
--rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/Karla-Regular.ttf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/__init__.py
--rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/auto_description.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/auto_title.py
--rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/base_cli.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/copy_assets.py
--rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/covers.py
--rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/create_covers.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/datetime.py
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/default_doc_template.md
--rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/default_log_template.html
--rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/default_post_template.html
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/default_redirect_template.html
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/default_service_worker_template.js
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/docs.py
--rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/feeds.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/flat_slug.py
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/generator.py
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/glob.py
--rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/heading_link.py
--rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/icon_resize.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/jinja_md.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/load.py
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/manifest.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/md_it_highlight_code.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/md_it_wikilinks.py
--rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/mdit_details.py
--rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/post_template.py
--rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/prevnext.py
--rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/prevnext_template.html
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/publish_dev_to_source.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/publish_html.py
--rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/publish_source.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/pyinstrument.py
--rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/redirects.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/render_markdown.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/rss.py
--rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/seo.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/service_worker.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/setup_logging.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/sitemap.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/subroute.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/to_json.py
--rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/plugins/tui.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/markata/scripts/migrate_to_slugify.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/_redirects
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/favicon.ico
--rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/markata.dev_.webp
--rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/markata.dev_markata_plugins_base-cli_.webp
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/robots.txt
--rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/waylonwalker.com.webp
--rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/waylonwalker.com_archive.webp
--rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/static/waylonwalker.com_markata-configure-head.webp
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/test_doc_page.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/test_feeds.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/test_one_default_page.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/test_one_default_page_with_path_prefix.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/plugins/conftest.py
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/plugins/test_default_post_template.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/plugins/test_flat_slug.py
--rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/tests/plugins/test_redirects.py
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/.gitignore
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/LICENSE
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/README.md
--rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/pyproject.toml
--rw-r--r--   0        0        0     7881 2020-02-02 00:00:00.000000 markata-0.7.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.2/.markataignore
+-rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 markata-0.7.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 markata-0.7.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 markata-0.7.2/SECURITY.md
+-rw-r--r--   0        0        0     5530 2020-02-02 00:00:00.000000 markata-0.7.2/contributing.md
+-rw-r--r--   0        0        0     7164 2020-02-02 00:00:00.000000 markata-0.7.2/markata.toml
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 markata-0.7.2/docs/404.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 markata-0.7.2/docs/color-theme.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 markata-0.7.2/docs/home-page.md
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 markata-0.7.2/docs/index.md
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 markata-0.7.2/docs/nav.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 markata-0.7.2/docs/project-gallery/markata_dev.md
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 markata-0.7.2/docs/project-gallery/waylonwalker.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__about__.py
+-rw-r--r--   0        0        0    15949 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 markata-0.7.2/markata/__main__.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 markata-0.7.2/markata/background.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 markata-0.7.2/markata/errors.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 markata-0.7.2/markata/hookspec.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 markata-0.7.2/markata/lifecycle.py
+-rw-r--r--   0        0        0     6197 2020-02-02 00:00:00.000000 markata-0.7.2/markata/standard_config.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/__init__.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/__main__.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/cli.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/header.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/plugins.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/runner.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/server.py
+-rw-r--r--   0        0        0     4120 2020-02-02 00:00:00.000000 markata-0.7.2/markata/cli/summary.py
+-rw-r--r--   0        0        0    38304 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/Karla-Regular.ttf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/__init__.py
+-rw-r--r--   0        0        0     4940 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/auto_description.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/auto_title.py
+-rw-r--r--   0        0        0    17051 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/base_cli.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/copy_assets.py
+-rw-r--r--   0        0        0     7472 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/covers.py
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/create_covers.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/datetime.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_doc_template.md
+-rw-r--r--   0        0        0    13176 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_log_template.html
+-rw-r--r--   0        0        0    21666 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_post_template.html
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_redirect_template.html
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/default_service_worker_template.js
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/docs.py
+-rw-r--r--   0        0        0    12989 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/feeds.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/flat_slug.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/generator.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/glob.py
+-rw-r--r--   0        0        0     3659 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/heading_link.py
+-rw-r--r--   0        0        0     1917 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/icon_resize.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/jinja_md.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/load.py
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/manifest.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/md_it_highlight_code.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/md_it_wikilinks.py
+-rw-r--r--   0        0        0     5083 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/mdit_details.py
+-rw-r--r--   0        0        0     4613 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/post_template.py
+-rw-r--r--   0        0        0     4449 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/prevnext.py
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/prevnext_template.html
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_dev_to_source.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_html.py
+-rw-r--r--   0        0        0     2282 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/publish_source.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/pyinstrument.py
+-rw-r--r--   0        0        0     5782 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/redirects.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/render_markdown.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/rss.py
+-rw-r--r--   0        0        0     6855 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/seo.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/service_worker.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/setup_logging.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/sitemap.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/subroute.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/to_json.py
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 markata-0.7.2/markata/plugins/tui.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 markata-0.7.2/markata/scripts/migrate_to_slugify.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 markata-0.7.2/static/_redirects
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 markata-0.7.2/static/favicon.ico
+-rw-r--r--   0        0        0    52806 2020-02-02 00:00:00.000000 markata-0.7.2/static/markata.dev_.webp
+-rw-r--r--   0        0        0    37044 2020-02-02 00:00:00.000000 markata-0.7.2/static/markata.dev_markata_plugins_base-cli_.webp
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 markata-0.7.2/static/robots.txt
+-rw-r--r--   0        0        0    63534 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com.webp
+-rw-r--r--   0        0        0    77848 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com_archive.webp
+-rw-r--r--   0        0        0    41986 2020-02-02 00:00:00.000000 markata-0.7.2/static/waylonwalker.com_markata-configure-head.webp
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_doc_page.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_feeds.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_one_default_page.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 markata-0.7.2/tests/test_one_default_page_with_path_prefix.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/conftest.py
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_default_post_template.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_flat_slug.py
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 markata-0.7.2/tests/plugins/test_redirects.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 markata-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 markata-0.7.2/LICENSE
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 markata-0.7.2/README.md
+-rw-r--r--   0        0        0     4043 2020-02-02 00:00:00.000000 markata-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     7876 2020-02-02 00:00:00.000000 markata-0.7.2/PKG-INFO
```

### Comparing `markata-0.7.1.dev0/CHANGELOG.md` & `markata-0.7.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/CODE_OF_CONDUCT.md` & `markata-0.7.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/contributing.md` & `markata-0.7.2/contributing.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata.toml` & `markata-0.7.2/markata.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/color-theme.md` & `markata-0.7.2/docs/color-theme.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/home-page.md` & `markata-0.7.2/docs/home-page.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/index.md` & `markata-0.7.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/nav.md` & `markata-0.7.2/docs/nav.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/project-gallery/markata_dev.md` & `markata-0.7.2/docs/project-gallery/markata_dev.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/docs/project-gallery/waylonwalker.md` & `markata-0.7.2/docs/project-gallery/waylonwalker.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/__init__.py` & `markata-0.7.2/markata/__init__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/background.py` & `markata-0.7.2/markata/background.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/hookspec.py` & `markata-0.7.2/markata/hookspec.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/lifecycle.py` & `markata-0.7.2/markata/lifecycle.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/standard_config.py` & `markata-0.7.2/markata/standard_config.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/__main__.py` & `markata-0.7.2/markata/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/cli.py` & `markata-0.7.2/markata/cli/cli.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/plugins.py` & `markata-0.7.2/markata/cli/plugins.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/runner.py` & `markata-0.7.2/markata/cli/runner.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/server.py` & `markata-0.7.2/markata/cli/server.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/cli/summary.py` & `markata-0.7.2/markata/cli/summary.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/Karla-Regular.ttf` & `markata-0.7.2/markata/plugins/Karla-Regular.ttf`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/auto_description.py` & `markata-0.7.2/markata/plugins/auto_description.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/base_cli.py` & `markata-0.7.2/markata/plugins/base_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,54 +164,54 @@
         )
     ) -> None:
         """
         Create a new blog from using the template from
         https://github.com/WaylonWalker/markata-blog-starter.
         """
 
-        from copier import run_auto
+        from copier import run_copy
 
         typer.echo(f"creating a new project in {directory.absolute()}")
         url = markata.config.get("starters", {}).get(
             "blog", "git+https://github.com/WaylonWalker/markata-blog-starter"
         )
-        run_auto(url, directory)
+        run_copy(url, directory)
 
     @new_app.command()
     def post() -> None:
         """
         Create new blog post in the pages directory from the template at
         https://github.com/WaylonWalker/markata-post-template.
         """
 
         print("create a new post")
-        from copier import run_auto
+        from copier import run_copy
 
         typer.echo(f"creating a new post in {Path().absolute()}/posts")
         url = markata.config.get("starters", {}).get(
             "post", "git+https://github.com/WaylonWalker/markata-post-template"
         )
-        run_auto(url, Path("."))
+        run_copy(url, Path("."))
 
     @new_app.command()
     def plugin() -> None:
         """
         Create a new plugin using the template at
         https://github.com/WaylonWalker/markata-plugin-template.
         """
-        from copier import run_auto
+        from copier import run_copy
 
         typer.echo(
             f"creating a new plugin in {Path().absolute()}"
             f"/<python-package-name>/plugins"
         )
         url = markata.config.get("starters", {}).get(
             "post", "git+https://github.com/WaylonWalker/markata-plugin-template"
         )
-        run_auto(url, Path("."))
+        run_copy(url, Path("."))
 
     @app.command()
     def build(
         pretty: bool = True,
         quiet: bool = typer.Option(
             False,
             "--quiet",
```

### Comparing `markata-0.7.1.dev0/markata/plugins/copy_assets.py` & `markata-0.7.2/markata/plugins/copy_assets.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/covers.py` & `markata-0.7.2/markata/plugins/covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/create_covers.py` & `markata-0.7.2/markata/plugins/create_covers.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/datetime.py` & `markata-0.7.2/markata/plugins/datetime.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/default_doc_template.md` & `markata-0.7.2/markata/plugins/default_doc_template.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/default_log_template.html` & `markata-0.7.2/markata/plugins/default_log_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/default_post_template.html` & `markata-0.7.2/markata/plugins/default_post_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/default_redirect_template.html` & `markata-0.7.2/markata/plugins/default_redirect_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/default_service_worker_template.js` & `markata-0.7.2/markata/plugins/default_service_worker_template.js`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/docs.py` & `markata-0.7.2/markata/plugins/docs.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/feeds.py` & `markata-0.7.2/markata/plugins/feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/flat_slug.py` & `markata-0.7.2/markata/plugins/flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/generator.py` & `markata-0.7.2/markata/plugins/generator.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/glob.py` & `markata-0.7.2/markata/plugins/glob.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/heading_link.py` & `markata-0.7.2/markata/plugins/heading_link.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/icon_resize.py` & `markata-0.7.2/markata/plugins/icon_resize.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/jinja_md.py` & `markata-0.7.2/markata/plugins/jinja_md.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/load.py` & `markata-0.7.2/markata/plugins/load.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/manifest.py` & `markata-0.7.2/markata/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/md_it_highlight_code.py` & `markata-0.7.2/markata/plugins/md_it_highlight_code.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/md_it_wikilinks.py` & `markata-0.7.2/markata/plugins/md_it_wikilinks.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/mdit_details.py` & `markata-0.7.2/markata/plugins/mdit_details.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/post_template.py` & `markata-0.7.2/markata/plugins/post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/prevnext.py` & `markata-0.7.2/markata/plugins/prevnext.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/prevnext_template.html` & `markata-0.7.2/markata/plugins/prevnext_template.html`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/publish_dev_to_source.py` & `markata-0.7.2/markata/plugins/publish_dev_to_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/publish_html.py` & `markata-0.7.2/markata/plugins/publish_html.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/publish_source.py` & `markata-0.7.2/markata/plugins/publish_source.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/pyinstrument.py` & `markata-0.7.2/markata/plugins/pyinstrument.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/redirects.py` & `markata-0.7.2/markata/plugins/redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/render_markdown.py` & `markata-0.7.2/markata/plugins/render_markdown.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/rss.py` & `markata-0.7.2/markata/plugins/rss.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/seo.py` & `markata-0.7.2/markata/plugins/seo.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/service_worker.py` & `markata-0.7.2/markata/plugins/service_worker.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/setup_logging.py` & `markata-0.7.2/markata/plugins/setup_logging.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/sitemap.py` & `markata-0.7.2/markata/plugins/sitemap.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/subroute.py` & `markata-0.7.2/markata/plugins/subroute.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/plugins/tui.py` & `markata-0.7.2/markata/plugins/tui.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/markata/scripts/migrate_to_slugify.py` & `markata-0.7.2/markata/scripts/migrate_to_slugify.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/_redirects` & `markata-0.7.2/static/_redirects`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/favicon.ico` & `markata-0.7.2/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/markata.dev_.webp` & `markata-0.7.2/static/markata.dev_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/markata.dev_markata_plugins_base-cli_.webp` & `markata-0.7.2/static/markata.dev_markata_plugins_base-cli_.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/waylonwalker.com.webp` & `markata-0.7.2/static/waylonwalker.com.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/waylonwalker.com_archive.webp` & `markata-0.7.2/static/waylonwalker.com_archive.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/static/waylonwalker.com_markata-configure-head.webp` & `markata-0.7.2/static/waylonwalker.com_markata-configure-head.webp`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/test_doc_page.py` & `markata-0.7.2/tests/test_doc_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/test_feeds.py` & `markata-0.7.2/tests/test_feeds.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/test_one_default_page.py` & `markata-0.7.2/tests/test_one_default_page.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/test_one_default_page_with_path_prefix.py` & `markata-0.7.2/tests/test_one_default_page_with_path_prefix.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/plugins/test_default_post_template.py` & `markata-0.7.2/tests/plugins/test_default_post_template.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/plugins/test_flat_slug.py` & `markata-0.7.2/tests/plugins/test_flat_slug.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/tests/plugins/test_redirects.py` & `markata-0.7.2/tests/plugins/test_redirects.py`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/.gitignore` & `markata-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/LICENSE` & `markata-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/README.md` & `markata-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/pyproject.toml` & `markata-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `markata-0.7.1.dev0/PKG-INFO` & `markata-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markata
-Version: 0.7.1.dev0
+Version: 0.7.2
 Summary: Static site generator plugins all the way down.
 Project-URL: Homepage, https://markata.dev
 Project-URL: Changelog, https://markata.dev/CHANGELOG/
 Project-URL: Source, https://github.com/waylonwalker/markata
 Project-URL: Issues, https://github.com/waylonwalker/markata/issues
 Project-URL: Documentation, https://markata.dev
 Author-email: Waylon Walker <waylon@waylonwalker.com>, waylon@markata.dev
```
