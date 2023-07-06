# Comparing `tmp/tekore-5.0.0.tar.gz` & `tmp/tekore-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tekore-5.0.0.tar", last modified: Sun Jun 18 18:59:55 2023, max compression
+gzip compressed data, was "tekore-5.0.1.tar", last modified: Thu Jul  6 17:22:18 2023, max compression
```

## Comparing `tekore-5.0.0.tar` & `tekore-5.0.1.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.744243 tekore-5.0.0/
--rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-5.0.0/LICENSE
--rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-5.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5311 2023-06-18 18:59:55.743743 tekore-5.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4184 2023-06-18 12:22:02.000000 tekore-5.0.0/contributing.rst
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.655228 tekore-5.0.0/docs/
--rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.661728 tekore-5.0.0/docs/src/
--rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/404.rst
--rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/advanced_usage.rst
--rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/auth_guide.rst
--rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-5.0.0/docs/src/conf.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.665229 tekore-5.0.0/docs/src/examples/
--rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-5.0.0/docs/src/examples/artist_follower.rst
--rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-5.0.0/docs/src/examples/async_server.rst
--rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-5.0.0/docs/src/examples/auth_server.rst
--rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-5.0.0/docs/src/examples/creating_scripts.rst
--rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-5.0.0/docs/src/examples/discord_bot.rst
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.670230 tekore-5.0.0/docs/src/examples/scripts/
--rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/albums_top_artist.rst
--rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/analyse_from_playlist.rst
--rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/follow_by_search.rst
--rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/follow_category_playlist.rst
--rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/play_saved_album.rst
--rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/recommended_playlist.rst
--rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/related_artists_top_artist.rst
--rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-5.0.0/docs/src/examples/scripts/scrape_playlists.rst
--rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-5.0.0/docs/src/examples/scripts/tracks_new_release.rst
--rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/examples/scripts.rst
--rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/examples.rst
--rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-5.0.0/docs/src/getting_started.rst
--rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-5.0.0/docs/src/index.rst
--rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-5.0.0/docs/src/logo.png
--rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-5.0.0/docs/src/logo_small.png
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.674231 tekore-5.0.0/docs/src/reference/
--rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-5.0.0/docs/src/reference/auth.rst
--rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference/client.rst
--rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-5.0.0/docs/src/reference/config.rst
--rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-5.0.0/docs/src/reference/conversions.rst
--rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference/errors.rst
--rw-rw-rw-   0        0        0     7553 2023-06-18 17:59:26.000000 tekore-5.0.0/docs/src/reference/models.rst
--rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-5.0.0/docs/src/reference/senders.rst
--rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-5.0.0/docs/src/reference.rst
--rw-rw-rw-   0        0        0    20908 2023-06-18 18:36:40.000000 tekore-5.0.0/docs/src/release_notes.rst
--rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-5.0.0/docs/src/resources.rst
--rw-rw-rw-   0        0        0     2036 2023-06-18 18:52:59.000000 tekore-5.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-5.0.0/readme_pypi.rst
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.676731 tekore-5.0.0/requirements/
--rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/build
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/checks
--rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/dev
--rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/docs
--rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-5.0.0/requirements/tests
--rw-rw-rw-   0        0        0       42 2023-06-18 18:59:55.744243 tekore-5.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.647226 tekore-5.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.678732 tekore-5.0.0/src/tekore/
--rw-rw-rw-   0        0        0     2610 2023-06-18 18:37:26.000000 tekore-5.0.0/src/tekore/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.683732 tekore-5.0.0/src/tekore/_auth/
--rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.685732 tekore-5.0.0/src/tekore/_auth/expiring/
--rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/__init__.py
--rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/client.py
--rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/decor.py
--rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/expiring/token.py
--rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/refreshing.py
--rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/scope.py
--rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_auth/util.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.688733 tekore-5.0.0/src/tekore/_client/
--rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.696234 tekore-5.0.0/src/tekore/_client/api/
--rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/__init__.py
--rw-rw-rw-   0        0        0     1966 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/album.py
--rw-rw-rw-   0        0        0     3160 2023-06-18 17:26:57.000000 tekore-5.0.0/src/tekore/_client/api/artist.py
--rw-rw-rw-   0        0        0     2877 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/audiobook.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.697234 tekore-5.0.0/src/tekore/_client/api/browse/
--rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/browse/__init__.py
--rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/browse/validate.py
--rw-rw-rw-   0        0        0     1772 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/chapter.py
--rw-rw-rw-   0        0        0     1773 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/episode.py
--rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/follow.py
--rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/library.py
--rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/markets.py
--rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/personalisation.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.698735 tekore-5.0.0/src/tekore/_client/api/player/
--rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/player/__init__.py
--rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/player/modify.py
--rw-rw-rw-   0        0        0     4097 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/player/view.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.700735 tekore-5.0.0/src/tekore/_client/api/playlist/
--rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/__init__.py
--rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/items.py
--rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/modify.py
--rw-rw-rw-   0        0        0     7576 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/playlist/view.py
--rw-rw-rw-   0        0        0     3568 2023-06-18 16:08:44.000000 tekore-5.0.0/src/tekore/_client/api/search.py
--rw-rw-rw-   0        0        0     2996 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/show.py
--rw-rw-rw-   0        0        0     2475 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_client/api/track.py
--rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/api/user.py
--rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/base.py
--rw-rw-rw-   0        0        0     4130 2023-06-18 17:26:05.000000 tekore-5.0.0/src/tekore/_client/chunked.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.702235 tekore-5.0.0/src/tekore/_client/decor/
--rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/decor/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/decor/handle.py
--rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_client/full.py
--rw-rw-rw-   0        0        0     4259 2023-06-18 16:19:25.000000 tekore-5.0.0/src/tekore/_client/paging.py
--rw-rw-rw-   0        0        0     1276 2023-06-18 17:38:50.000000 tekore-5.0.0/src/tekore/_client/process.py
--rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_config.py
--rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-5.0.0/src/tekore/_convert.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.712737 tekore-5.0.0/src/tekore/_model/
--rw-rw-rw-   0        0        0     2322 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.714237 tekore-5.0.0/src/tekore/_model/album/
--rw-rw-rw-   0        0        0      857 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/album/__init__.py
--rw-rw-rw-   0        0        0      677 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/album/base.py
--rw-rw-rw-   0        0        0      874 2023-06-18 17:28:56.000000 tekore-5.0.0/src/tekore/_model/album/full.py
--rw-rw-rw-   0        0        0      707 2023-06-18 17:36:38.000000 tekore-5.0.0/src/tekore/_model/artist.py
--rw-rw-rw-   0        0        0     1629 2023-06-18 17:27:56.000000 tekore-5.0.0/src/tekore/_model/audio_analysis.py
--rw-rw-rw-   0        0        0      457 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/audio_features.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.715737 tekore-5.0.0/src/tekore/_model/audiobook/
--rw-rw-rw-   0        0        0      436 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/audiobook/__init__.py
--rw-rw-rw-   0        0        0      743 2023-06-18 17:29:06.000000 tekore-5.0.0/src/tekore/_model/audiobook/base.py
--rw-rw-rw-   0        0        0      184 2023-06-18 14:03:09.000000 tekore-5.0.0/src/tekore/_model/audiobook/full.py
--rw-rw-rw-   0        0        0      250 2023-06-18 13:57:29.000000 tekore-5.0.0/src/tekore/_model/base.py
--rw-rw-rw-   0        0        0      347 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/category.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.717238 tekore-5.0.0/src/tekore/_model/chapter/
--rw-rw-rw-   0        0        0      320 2023-06-18 17:29:11.000000 tekore-5.0.0/src/tekore/_model/chapter/__init__.py
--rw-rw-rw-   0        0        0      640 2023-06-18 17:29:14.000000 tekore-5.0.0/src/tekore/_model/chapter/base.py
--rw-rw-rw-   0        0        0      171 2023-06-18 15:59:39.000000 tekore-5.0.0/src/tekore/_model/chapter/full.py
--rw-rw-rw-   0        0        0      385 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/context.py
--rw-rw-rw-   0        0        0     1804 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/currently_playing.py
--rw-rw-rw-   0        0        0      711 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/device.py
--rw-rw-rw-   0        0        0     1285 2023-06-18 17:28:10.000000 tekore-5.0.0/src/tekore/_model/episode.py
--rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_model/error.py
--rw-rw-rw-   0        0        0     1065 2023-06-18 17:28:13.000000 tekore-5.0.0/src/tekore/_model/local.py
--rw-rw-rw-   0        0        0      941 2023-06-18 16:16:53.000000 tekore-5.0.0/src/tekore/_model/member.py
--rw-rw-rw-   0        0        0      654 2023-06-18 17:17:07.000000 tekore-5.0.0/src/tekore/_model/paging.py
--rw-rw-rw-   0        0        0      726 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/play_history.py
--rw-rw-rw-   0        0        0     2308 2023-06-18 18:18:36.000000 tekore-5.0.0/src/tekore/_model/playlist.py
--rw-rw-rw-   0        0        0      986 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/recommendations.py
--rw-rw-rw-   0        0        0     1812 2023-06-18 17:24:30.000000 tekore-5.0.0/src/tekore/_model/serialise.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.719238 tekore-5.0.0/src/tekore/_model/show/
--rw-rw-rw-   0        0        0      683 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/show/__init__.py
--rw-rw-rw-   0        0        0      507 2023-06-18 17:29:22.000000 tekore-5.0.0/src/tekore/_model/show/base.py
--rw-rw-rw-   0        0        0      343 2023-06-18 14:22:16.000000 tekore-5.0.0/src/tekore/_model/show/full.py
--rw-rw-rw-   0        0        0     2095 2023-06-18 17:28:32.000000 tekore-5.0.0/src/tekore/_model/track.py
--rw-rw-rw-   0        0        0     1209 2023-06-18 17:36:39.000000 tekore-5.0.0/src/tekore/_model/user.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.722239 tekore-5.0.0/src/tekore/_sender/
--rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/__init__.py
--rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/base.py
--rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/client.py
--rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/concrete.py
--rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/error.py
--rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-5.0.0/src/tekore/_sender/extending.py
--rw-rw-rw-   0        0        0     4100 2023-06-18 17:26:16.000000 tekore-5.0.0/src/tekore/model.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.681732 tekore-5.0.0/src/tekore.egg-info/
--rw-rw-rw-   0        0        0     5311 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4979 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-18 18:59:55.000000 tekore-5.0.0/src/tekore.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.725739 tekore-5.0.0/tests/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.0/tests/__init__.py
--rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/_util.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.729740 tekore-5.0.0/tests/auth/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/auth/__init__.py
--rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/expiring.py
--rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/refreshing.py
--rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/scope.py
--rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/auth/util.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.740742 tekore-5.0.0/tests/client/
--rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.0/tests/client/__init__.py
--rw-rw-rw-   0        0        0     2542 2023-05-25 05:51:13.000000 tekore-5.0.0/tests/client/_resources.py
--rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/album.py
--rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/artist.py
--rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-5.0.0/tests/client/audiobook.py
--rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/base.py
--rw-rw-rw-   0        0        0     3444 2023-06-18 15:20:59.000000 tekore-5.0.0/tests/client/browse.py
--rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-5.0.0/tests/client/chapter.py
--rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/episode.py
--rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/follow.py
--rw-rw-rw-   0        0        0    13150 2023-06-18 17:29:58.000000 tekore-5.0.0/tests/client/full.py
--rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/library.py
--rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-5.0.0/tests/client/markets.py
--rw-rw-rw-   0        0        0     3619 2023-06-18 17:20:20.000000 tekore-5.0.0/tests/client/paging.py
--rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/client/personalisation.py
--rw-rw-rw-   0        0        0     6147 2023-06-18 18:52:49.000000 tekore-5.0.0/tests/client/player.py
--rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/playlist.py
--rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/search.py
--rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/show.py
--rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/client/track.py
--rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-5.0.0/tests/client/user.py
--rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/config.py
--rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/conftest.py
--rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/convert.py
--rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/error.py
--rw-rw-rw-   0        0        0     2202 2023-06-18 17:51:35.000000 tekore-5.0.0/tests/model.py
-drwxrwxrwx   0        0        0        0 2023-06-18 18:59:55.743242 tekore-5.0.0/tests/sender/
--rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.0/tests/sender/__init__.py
--rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/base.py
--rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/caching.py
--rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/client.py
--rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-5.0.0/tests/sender/retrying.py
--rw-rw-rw-   0        0        0     2443 2023-06-18 17:19:58.000000 tekore-5.0.0/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:18.020745 tekore-5.0.1/
+-rw-rw-rw-   0        0        0     1096 2023-01-06 17:05:20.000000 tekore-5.0.1/LICENSE
+-rw-rw-rw-   0        0        0      156 2023-01-05 23:44:39.000000 tekore-5.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5311 2023-07-06 17:22:18.020245 tekore-5.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4184 2023-06-18 12:22:02.000000 tekore-5.0.1/contributing.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.815709 tekore-5.0.1/docs/
+-rw-rw-rw-   0        0        0       89 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.852215 tekore-5.0.1/docs/src/
+-rw-rw-rw-   0        0        0      311 2020-06-21 19:25:53.000000 tekore-5.0.1/docs/src/404.rst
+-rw-rw-rw-   0        0        0     8153 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/src/advanced_usage.rst
+-rw-rw-rw-   0        0        0    12443 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/src/auth_guide.rst
+-rw-rw-rw-   0        0        0     1082 2023-01-06 17:05:20.000000 tekore-5.0.1/docs/src/conf.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.875219 tekore-5.0.1/docs/src/examples/
+-rw-rw-rw-   0        0        0     1648 2020-08-27 18:40:55.000000 tekore-5.0.1/docs/src/examples/artist_follower.rst
+-rw-rw-rw-   0        0        0     2177 2020-09-02 16:05:17.000000 tekore-5.0.1/docs/src/examples/async_server.rst
+-rw-rw-rw-   0        0        0     7611 2021-09-08 13:22:42.000000 tekore-5.0.1/docs/src/examples/auth_server.rst
+-rw-rw-rw-   0        0        0     2070 2020-09-02 16:24:55.000000 tekore-5.0.1/docs/src/examples/creating_scripts.rst
+-rw-rw-rw-   0        0        0     2086 2021-01-10 19:32:00.000000 tekore-5.0.1/docs/src/examples/discord_bot.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.910226 tekore-5.0.1/docs/src/examples/scripts/
+-rw-rw-rw-   0        0        0      685 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/albums_top_artist.rst
+-rw-rw-rw-   0        0        0     1073 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/analyse_from_playlist.rst
+-rw-rw-rw-   0        0        0      793 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/follow_by_search.rst
+-rw-rw-rw-   0        0        0      731 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/follow_category_playlist.rst
+-rw-rw-rw-   0        0        0      670 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/play_saved_album.rst
+-rw-rw-rw-   0        0        0     1045 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/recommended_playlist.rst
+-rw-rw-rw-   0        0        0      976 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/related_artists_top_artist.rst
+-rw-rw-rw-   0        0        0     3859 2022-05-02 15:56:27.000000 tekore-5.0.1/docs/src/examples/scripts/scrape_playlists.rst
+-rw-rw-rw-   0        0        0      657 2020-08-27 18:37:41.000000 tekore-5.0.1/docs/src/examples/scripts/tracks_new_release.rst
+-rw-rw-rw-   0        0        0      262 2020-06-21 19:25:53.000000 tekore-5.0.1/docs/src/examples/scripts.rst
+-rw-rw-rw-   0        0        0      183 2020-06-21 19:25:53.000000 tekore-5.0.1/docs/src/examples.rst
+-rw-rw-rw-   0        0        0     5076 2021-10-26 07:09:35.000000 tekore-5.0.1/docs/src/getting_started.rst
+-rw-rw-rw-   0        0        0     2745 2020-09-02 15:00:17.000000 tekore-5.0.1/docs/src/index.rst
+-rw-rw-rw-   0        0        0   143290 2021-01-11 16:43:14.000000 tekore-5.0.1/docs/src/logo.png
+-rw-rw-rw-   0        0        0    22000 2021-01-11 16:43:14.000000 tekore-5.0.1/docs/src/logo_small.png
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.942231 tekore-5.0.1/docs/src/reference/
+-rw-rw-rw-   0        0        0     2435 2021-01-10 19:32:00.000000 tekore-5.0.1/docs/src/reference/auth.rst
+-rw-rw-rw-   0        0        0    12495 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/src/reference/client.rst
+-rw-rw-rw-   0        0        0     1252 2020-06-21 19:25:53.000000 tekore-5.0.1/docs/src/reference/config.rst
+-rw-rw-rw-   0        0        0      823 2020-06-25 21:26:36.000000 tekore-5.0.1/docs/src/reference/conversions.rst
+-rw-rw-rw-   0        0        0     1577 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/src/reference/errors.rst
+-rw-rw-rw-   0        0        0     7553 2023-06-18 17:59:26.000000 tekore-5.0.1/docs/src/reference/models.rst
+-rw-rw-rw-   0        0        0     2003 2020-09-02 14:48:39.000000 tekore-5.0.1/docs/src/reference/senders.rst
+-rw-rw-rw-   0        0        0      618 2022-12-30 08:34:42.000000 tekore-5.0.1/docs/src/reference.rst
+-rw-rw-rw-   0        0        0    21041 2023-07-06 16:33:07.000000 tekore-5.0.1/docs/src/release_notes.rst
+-rw-rw-rw-   0        0        0     1174 2020-09-02 14:48:39.000000 tekore-5.0.1/docs/src/resources.rst
+-rw-rw-rw-   0        0        0     2036 2023-06-18 18:52:59.000000 tekore-5.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     2901 2021-09-09 16:40:04.000000 tekore-5.0.1/readme_pypi.rst
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.945232 tekore-5.0.1/requirements/
+-rw-rw-rw-   0        0        0       14 2023-01-05 23:44:39.000000 tekore-5.0.1/requirements/build
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.1/requirements/checks
+-rw-rw-rw-   0        0        0       50 2023-01-05 23:44:39.000000 tekore-5.0.1/requirements/dev
+-rw-rw-rw-   0        0        0       65 2023-01-05 23:44:39.000000 tekore-5.0.1/requirements/docs
+-rw-rw-rw-   0        0        0       54 2023-01-05 23:44:39.000000 tekore-5.0.1/requirements/tests
+-rw-rw-rw-   0        0        0       42 2023-07-06 17:22:18.020745 tekore-5.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.802706 tekore-5.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.947232 tekore-5.0.1/src/tekore/
+-rw-rw-rw-   0        0        0     2610 2023-07-06 16:33:25.000000 tekore-5.0.1/src/tekore/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.952733 tekore-5.0.1/src/tekore/_auth/
+-rw-rw-rw-   0        0        0      393 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.955234 tekore-5.0.1/src/tekore/_auth/expiring/
+-rw-rw-rw-   0        0        0       72 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/expiring/__init__.py
+-rw-rw-rw-   0        0        0     9619 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/expiring/client.py
+-rw-rw-rw-   0        0        0     1603 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/expiring/decor.py
+-rw-rw-rw-   0        0        0     2869 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/expiring/token.py
+-rw-rw-rw-   0        0        0     9067 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/refreshing.py
+-rw-rw-rw-   0        0        0     5817 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/scope.py
+-rw-rw-rw-   0        0        0     8596 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_auth/util.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.958734 tekore-5.0.1/src/tekore/_client/
+-rw-rw-rw-   0        0        0       27 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.967736 tekore-5.0.1/src/tekore/_client/api/
+-rw-rw-rw-   0        0        0      584 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/__init__.py
+-rw-rw-rw-   0        0        0     1966 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/album.py
+-rw-rw-rw-   0        0        0     3160 2023-06-18 17:26:57.000000 tekore-5.0.1/src/tekore/_client/api/artist.py
+-rw-rw-rw-   0        0        0     2877 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/audiobook.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.968736 tekore-5.0.1/src/tekore/_client/api/browse/
+-rw-rw-rw-   0        0        0     7095 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/browse/__init__.py
+-rw-rw-rw-   0        0        0      663 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/browse/validate.py
+-rw-rw-rw-   0        0        0     1772 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/chapter.py
+-rw-rw-rw-   0        0        0     1773 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/episode.py
+-rw-rw-rw-   0        0        0     5593 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/follow.py
+-rw-rw-rw-   0        0        0     9081 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/library.py
+-rw-rw-rw-   0        0        0      503 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/markets.py
+-rw-rw-rw-   0        0        0     1853 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/personalisation.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.970736 tekore-5.0.1/src/tekore/_client/api/player/
+-rw-rw-rw-   0        0        0      181 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/player/__init__.py
+-rw-rw-rw-   0        0        0     7343 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/player/modify.py
+-rw-rw-rw-   0        0        0     4097 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/player/view.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.972736 tekore-5.0.1/src/tekore/_client/api/playlist/
+-rw-rw-rw-   0        0        0      256 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/playlist/__init__.py
+-rw-rw-rw-   0        0        0     6142 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/playlist/items.py
+-rw-rw-rw-   0        0        0     2770 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/playlist/modify.py
+-rw-rw-rw-   0        0        0     7576 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/playlist/view.py
+-rw-rw-rw-   0        0        0     3568 2023-06-18 16:08:44.000000 tekore-5.0.1/src/tekore/_client/api/search.py
+-rw-rw-rw-   0        0        0     2996 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/show.py
+-rw-rw-rw-   0        0        0     2475 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_client/api/track.py
+-rw-rw-rw-   0        0        0      951 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/api/user.py
+-rw-rw-rw-   0        0        0     4407 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/base.py
+-rw-rw-rw-   0        0        0     4130 2023-06-18 17:26:05.000000 tekore-5.0.1/src/tekore/_client/chunked.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.973737 tekore-5.0.1/src/tekore/_client/decor/
+-rw-rw-rw-   0        0        0     2861 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/decor/__init__.py
+-rw-rw-rw-   0        0        0     1068 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/decor/handle.py
+-rw-rw-rw-   0        0        0     4129 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_client/full.py
+-rw-rw-rw-   0        0        0     4259 2023-06-18 16:19:25.000000 tekore-5.0.1/src/tekore/_client/paging.py
+-rw-rw-rw-   0        0        0     1276 2023-07-06 16:24:46.000000 tekore-5.0.1/src/tekore/_client/process.py
+-rw-rw-rw-   0        0        0     5922 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_config.py
+-rw-rw-rw-   0        0        0     4051 2023-03-26 09:38:45.000000 tekore-5.0.1/src/tekore/_convert.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.986239 tekore-5.0.1/src/tekore/_model/
+-rw-rw-rw-   0        0        0     2322 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.988239 tekore-5.0.1/src/tekore/_model/album/
+-rw-rw-rw-   0        0        0      857 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/album/__init__.py
+-rw-rw-rw-   0        0        0      677 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/album/base.py
+-rw-rw-rw-   0        0        0      874 2023-06-18 17:28:56.000000 tekore-5.0.1/src/tekore/_model/album/full.py
+-rw-rw-rw-   0        0        0      707 2023-06-18 17:36:38.000000 tekore-5.0.1/src/tekore/_model/artist.py
+-rw-rw-rw-   0        0        0     1629 2023-06-18 17:27:56.000000 tekore-5.0.1/src/tekore/_model/audio_analysis.py
+-rw-rw-rw-   0        0        0      457 2023-06-18 14:22:16.000000 tekore-5.0.1/src/tekore/_model/audio_features.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.990239 tekore-5.0.1/src/tekore/_model/audiobook/
+-rw-rw-rw-   0        0        0      436 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/audiobook/__init__.py
+-rw-rw-rw-   0        0        0      743 2023-06-18 17:29:06.000000 tekore-5.0.1/src/tekore/_model/audiobook/base.py
+-rw-rw-rw-   0        0        0      184 2023-06-18 14:03:09.000000 tekore-5.0.1/src/tekore/_model/audiobook/full.py
+-rw-rw-rw-   0        0        0      250 2023-06-18 13:57:29.000000 tekore-5.0.1/src/tekore/_model/base.py
+-rw-rw-rw-   0        0        0      347 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/category.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.991740 tekore-5.0.1/src/tekore/_model/chapter/
+-rw-rw-rw-   0        0        0      340 2023-07-06 16:23:11.000000 tekore-5.0.1/src/tekore/_model/chapter/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-06-18 17:29:14.000000 tekore-5.0.1/src/tekore/_model/chapter/base.py
+-rw-rw-rw-   0        0        0      171 2023-06-18 15:59:39.000000 tekore-5.0.1/src/tekore/_model/chapter/full.py
+-rw-rw-rw-   0        0        0      385 2023-06-18 14:22:16.000000 tekore-5.0.1/src/tekore/_model/context.py
+-rw-rw-rw-   0        0        0     1804 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/currently_playing.py
+-rw-rw-rw-   0        0        0      711 2023-06-18 14:22:16.000000 tekore-5.0.1/src/tekore/_model/device.py
+-rw-rw-rw-   0        0        0     1285 2023-06-18 17:28:10.000000 tekore-5.0.1/src/tekore/_model/episode.py
+-rw-rw-rw-   0        0        0     1747 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_model/error.py
+-rw-rw-rw-   0        0        0     1065 2023-06-18 17:28:13.000000 tekore-5.0.1/src/tekore/_model/local.py
+-rw-rw-rw-   0        0        0      941 2023-06-18 16:16:53.000000 tekore-5.0.1/src/tekore/_model/member.py
+-rw-rw-rw-   0        0        0      654 2023-06-18 17:17:07.000000 tekore-5.0.1/src/tekore/_model/paging.py
+-rw-rw-rw-   0        0        0      726 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/play_history.py
+-rw-rw-rw-   0        0        0     2308 2023-06-18 18:18:36.000000 tekore-5.0.1/src/tekore/_model/playlist.py
+-rw-rw-rw-   0        0        0      986 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/recommendations.py
+-rw-rw-rw-   0        0        0     1812 2023-06-18 17:24:30.000000 tekore-5.0.1/src/tekore/_model/serialise.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.993240 tekore-5.0.1/src/tekore/_model/show/
+-rw-rw-rw-   0        0        0      683 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/show/__init__.py
+-rw-rw-rw-   0        0        0      517 2023-07-06 16:19:52.000000 tekore-5.0.1/src/tekore/_model/show/base.py
+-rw-rw-rw-   0        0        0      343 2023-06-18 14:22:16.000000 tekore-5.0.1/src/tekore/_model/show/full.py
+-rw-rw-rw-   0        0        0     2095 2023-06-18 17:28:32.000000 tekore-5.0.1/src/tekore/_model/track.py
+-rw-rw-rw-   0        0        0     1209 2023-06-18 17:36:39.000000 tekore-5.0.1/src/tekore/_model/user.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.996741 tekore-5.0.1/src/tekore/_sender/
+-rw-rw-rw-   0        0        0      466 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/base.py
+-rw-rw-rw-   0        0        0     3286 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/client.py
+-rw-rw-rw-   0        0        0     3130 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/concrete.py
+-rw-rw-rw-   0        0        0     2881 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/error.py
+-rw-rw-rw-   0        0        0    10259 2023-01-05 23:44:39.000000 tekore-5.0.1/src/tekore/_sender/extending.py
+-rw-rw-rw-   0        0        0     4100 2023-06-18 17:26:16.000000 tekore-5.0.1/src/tekore/model.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:17.950233 tekore-5.0.1/src/tekore.egg-info/
+-rw-rw-rw-   0        0        0     5311 2023-07-06 17:22:17.000000 tekore-5.0.1/src/tekore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4979 2023-07-06 17:22:17.000000 tekore-5.0.1/src/tekore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 17:22:17.000000 tekore-5.0.1/src/tekore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-06 17:22:17.000000 tekore-5.0.1/src/tekore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 17:22:17.000000 tekore-5.0.1/src/tekore.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:18.001241 tekore-5.0.1/tests/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      407 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/_util.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:18.004242 tekore-5.0.1/tests/auth/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.1/tests/auth/__init__.py
+-rw-rw-rw-   0        0        0     8738 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/auth/expiring.py
+-rw-rw-rw-   0        0        0     2880 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/auth/refreshing.py
+-rw-rw-rw-   0        0        0     5793 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/auth/scope.py
+-rw-rw-rw-   0        0        0     5167 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/auth/util.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:18.016744 tekore-5.0.1/tests/client/
+-rw-rw-rw-   0        0        0        0 2020-01-13 21:08:33.000000 tekore-5.0.1/tests/client/__init__.py
+-rw-rw-rw-   0        0        0     2542 2023-05-25 05:51:13.000000 tekore-5.0.1/tests/client/_resources.py
+-rw-rw-rw-   0        0        0     2123 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/album.py
+-rw-rw-rw-   0        0        0     1833 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/artist.py
+-rw-rw-rw-   0        0        0     1640 2023-03-26 09:38:45.000000 tekore-5.0.1/tests/client/audiobook.py
+-rw-rw-rw-   0        0        0     1528 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/base.py
+-rw-rw-rw-   0        0        0     3444 2023-06-18 15:20:59.000000 tekore-5.0.1/tests/client/browse.py
+-rw-rw-rw-   0        0        0     1315 2023-03-26 09:38:45.000000 tekore-5.0.1/tests/client/chapter.py
+-rw-rw-rw-   0        0        0     1079 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/episode.py
+-rw-rw-rw-   0        0        0     2267 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/follow.py
+-rw-rw-rw-   0        0        0    13150 2023-06-18 17:29:58.000000 tekore-5.0.1/tests/client/full.py
+-rw-rw-rw-   0        0        0     3583 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/library.py
+-rw-rw-rw-   0        0        0      130 2021-04-08 08:00:20.000000 tekore-5.0.1/tests/client/markets.py
+-rw-rw-rw-   0        0        0     3619 2023-06-18 17:20:20.000000 tekore-5.0.1/tests/client/paging.py
+-rw-rw-rw-   0        0        0      229 2020-05-21 14:45:59.000000 tekore-5.0.1/tests/client/personalisation.py
+-rw-rw-rw-   0        0        0     6147 2023-06-18 18:52:49.000000 tekore-5.0.1/tests/client/player.py
+-rw-rw-rw-   0        0        0     9110 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/playlist.py
+-rw-rw-rw-   0        0        0     1103 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/search.py
+-rw-rw-rw-   0        0        0      866 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/show.py
+-rw-rw-rw-   0        0        0     3779 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/client/track.py
+-rw-rw-rw-   0        0        0      477 2022-01-14 08:24:39.000000 tekore-5.0.1/tests/client/user.py
+-rw-rw-rw-   0        0        0     6369 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/config.py
+-rw-rw-rw-   0        0        0     3662 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/conftest.py
+-rw-rw-rw-   0        0        0     3731 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/convert.py
+-rw-rw-rw-   0        0        0      450 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/error.py
+-rw-rw-rw-   0        0        0     2229 2023-07-06 15:27:34.000000 tekore-5.0.1/tests/model.py
+drwxrwxrwx   0        0        0        0 2023-07-06 17:22:18.019745 tekore-5.0.1/tests/sender/
+-rw-rw-rw-   0        0        0        0 2020-05-21 14:45:59.000000 tekore-5.0.1/tests/sender/__init__.py
+-rw-rw-rw-   0        0        0      296 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/sender/base.py
+-rw-rw-rw-   0        0        0    10662 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/sender/caching.py
+-rw-rw-rw-   0        0        0     1204 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/sender/client.py
+-rw-rw-rw-   0        0        0     5995 2023-01-05 23:44:39.000000 tekore-5.0.1/tests/sender/retrying.py
+-rw-rw-rw-   0        0        0     2443 2023-06-18 17:19:58.000000 tekore-5.0.1/tox.ini
```

### Comparing `tekore-5.0.0/LICENSE` & `tekore-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/PKG-INFO` & `tekore-5.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 5.0.0
+Version: 5.0.1
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
```

### Comparing `tekore-5.0.0/contributing.rst` & `tekore-5.0.1/contributing.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/advanced_usage.rst` & `tekore-5.0.1/docs/src/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/auth_guide.rst` & `tekore-5.0.1/docs/src/auth_guide.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/conf.py` & `tekore-5.0.1/docs/src/conf.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/artist_follower.rst` & `tekore-5.0.1/docs/src/examples/artist_follower.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/async_server.rst` & `tekore-5.0.1/docs/src/examples/async_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/auth_server.rst` & `tekore-5.0.1/docs/src/examples/auth_server.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/creating_scripts.rst` & `tekore-5.0.1/docs/src/examples/creating_scripts.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/discord_bot.rst` & `tekore-5.0.1/docs/src/examples/discord_bot.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/albums_top_artist.rst` & `tekore-5.0.1/docs/src/examples/scripts/albums_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/analyse_from_playlist.rst` & `tekore-5.0.1/docs/src/examples/scripts/analyse_from_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/follow_by_search.rst` & `tekore-5.0.1/docs/src/examples/scripts/follow_by_search.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/follow_category_playlist.rst` & `tekore-5.0.1/docs/src/examples/scripts/follow_category_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/play_saved_album.rst` & `tekore-5.0.1/docs/src/examples/scripts/play_saved_album.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/recommended_playlist.rst` & `tekore-5.0.1/docs/src/examples/scripts/recommended_playlist.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/related_artists_top_artist.rst` & `tekore-5.0.1/docs/src/examples/scripts/related_artists_top_artist.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/scrape_playlists.rst` & `tekore-5.0.1/docs/src/examples/scripts/scrape_playlists.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/examples/scripts/tracks_new_release.rst` & `tekore-5.0.1/docs/src/examples/scripts/tracks_new_release.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/getting_started.rst` & `tekore-5.0.1/docs/src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/index.rst` & `tekore-5.0.1/docs/src/index.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/logo.png` & `tekore-5.0.1/docs/src/logo.png`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/logo_small.png` & `tekore-5.0.1/docs/src/logo_small.png`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/auth.rst` & `tekore-5.0.1/docs/src/reference/auth.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/client.rst` & `tekore-5.0.1/docs/src/reference/client.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/config.rst` & `tekore-5.0.1/docs/src/reference/config.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/conversions.rst` & `tekore-5.0.1/docs/src/reference/conversions.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/errors.rst` & `tekore-5.0.1/docs/src/reference/errors.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/models.rst` & `tekore-5.0.1/docs/src/reference/models.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference/senders.rst` & `tekore-5.0.1/docs/src/reference/senders.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/reference.rst` & `tekore-5.0.1/docs/src/reference.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/docs/src/release_notes.rst` & `tekore-5.0.1/docs/src/release_notes.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. _release-notes:
 .. currentmodule:: tekore
 
 Release notes
 =============
+5.0.1 (2023-07-06)
+------------------
+Fixed
+*****
+- Add missing ``Optional`` annotations to support Pydantic 2 (:issue:`293`)
+
 5.0.0 (2023-06-18)
 ------------------
 Tekore 5 comes with an overhauled response model system based on Pydantic.
 Although the underlying change is major, the primary usage of models remains
 unchanged. The new models are more robust and easier to maintain.
 However, with more careful data validation new issues may arise. Please submit
 them on `GitHub <https://github.com/felix-hilden/tekore/issues>`_.
```

### Comparing `tekore-5.0.0/docs/src/resources.rst` & `tekore-5.0.1/docs/src/resources.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/pyproject.toml` & `tekore-5.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/readme_pypi.rst` & `tekore-5.0.1/readme_pypi.rst`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/__init__.py` & `tekore-5.0.1/src/tekore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ServerError,
     ServiceUnavailable,
     SyncSender,
     TooManyRequests,
     Unauthorised,
 )
 
-__version__ = "5.0.0"
+__version__ = "5.0.1"
 
 # Change the module of classes to hide module structure
 # and fix Sphinx base class links
 _classes = [
     Spotify,
     Credentials,
     Token,
```

### Comparing `tekore-5.0.0/src/tekore/_auth/expiring/client.py` & `tekore-5.0.1/src/tekore/_auth/expiring/client.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_auth/expiring/decor.py` & `tekore-5.0.1/src/tekore/_auth/expiring/decor.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_auth/expiring/token.py` & `tekore-5.0.1/src/tekore/_auth/expiring/token.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_auth/refreshing.py` & `tekore-5.0.1/src/tekore/_auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_auth/scope.py` & `tekore-5.0.1/src/tekore/_auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_auth/util.py` & `tekore-5.0.1/src/tekore/_auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/__init__.py` & `tekore-5.0.1/src/tekore/_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/album.py` & `tekore-5.0.1/src/tekore/_client/api/album.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/artist.py` & `tekore-5.0.1/src/tekore/_client/api/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/audiobook.py` & `tekore-5.0.1/src/tekore/_client/api/audiobook.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/browse/__init__.py` & `tekore-5.0.1/src/tekore/_client/api/browse/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/browse/validate.py` & `tekore-5.0.1/src/tekore/_client/api/browse/validate.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/chapter.py` & `tekore-5.0.1/src/tekore/_client/api/chapter.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/episode.py` & `tekore-5.0.1/src/tekore/_client/api/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/follow.py` & `tekore-5.0.1/src/tekore/_client/api/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/library.py` & `tekore-5.0.1/src/tekore/_client/api/library.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/personalisation.py` & `tekore-5.0.1/src/tekore/_client/api/personalisation.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/player/modify.py` & `tekore-5.0.1/src/tekore/_client/api/player/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/player/view.py` & `tekore-5.0.1/src/tekore/_client/api/player/view.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/playlist/items.py` & `tekore-5.0.1/src/tekore/_client/api/playlist/items.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/playlist/modify.py` & `tekore-5.0.1/src/tekore/_client/api/playlist/modify.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/playlist/view.py` & `tekore-5.0.1/src/tekore/_client/api/playlist/view.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/search.py` & `tekore-5.0.1/src/tekore/_client/api/search.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/show.py` & `tekore-5.0.1/src/tekore/_client/api/show.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/track.py` & `tekore-5.0.1/src/tekore/_client/api/track.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/api/user.py` & `tekore-5.0.1/src/tekore/_client/api/user.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/base.py` & `tekore-5.0.1/src/tekore/_client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/chunked.py` & `tekore-5.0.1/src/tekore/_client/chunked.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/decor/__init__.py` & `tekore-5.0.1/src/tekore/_client/decor/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/decor/handle.py` & `tekore-5.0.1/src/tekore/_client/decor/handle.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/full.py` & `tekore-5.0.1/src/tekore/_client/full.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/paging.py` & `tekore-5.0.1/src/tekore/_client/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_client/process.py` & `tekore-5.0.1/src/tekore/_client/process.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_config.py` & `tekore-5.0.1/src/tekore/_config.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_convert.py` & `tekore-5.0.1/src/tekore/_convert.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/__init__.py` & `tekore-5.0.1/src/tekore/_model/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/album/__init__.py` & `tekore-5.0.1/src/tekore/_model/album/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/album/base.py` & `tekore-5.0.1/src/tekore/_model/album/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/album/full.py` & `tekore-5.0.1/src/tekore/_model/album/full.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/artist.py` & `tekore-5.0.1/src/tekore/_model/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/audio_analysis.py` & `tekore-5.0.1/src/tekore/_model/audio_analysis.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/audiobook/base.py` & `tekore-5.0.1/src/tekore/_model/audiobook/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/chapter/base.py` & `tekore-5.0.1/src/tekore/_model/chapter/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/currently_playing.py` & `tekore-5.0.1/src/tekore/_model/currently_playing.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/device.py` & `tekore-5.0.1/src/tekore/_model/device.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/episode.py` & `tekore-5.0.1/src/tekore/_model/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/error.py` & `tekore-5.0.1/src/tekore/_model/error.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/local.py` & `tekore-5.0.1/src/tekore/_model/local.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/member.py` & `tekore-5.0.1/src/tekore/_model/member.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/paging.py` & `tekore-5.0.1/src/tekore/_model/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/play_history.py` & `tekore-5.0.1/src/tekore/_model/play_history.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/playlist.py` & `tekore-5.0.1/src/tekore/_model/playlist.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/recommendations.py` & `tekore-5.0.1/src/tekore/_model/recommendations.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/serialise.py` & `tekore-5.0.1/src/tekore/_model/serialise.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/show/__init__.py` & `tekore-5.0.1/src/tekore/_model/show/__init__.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/track.py` & `tekore-5.0.1/src/tekore/_model/track.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_model/user.py` & `tekore-5.0.1/src/tekore/_model/user.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_sender/base.py` & `tekore-5.0.1/src/tekore/_sender/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_sender/client.py` & `tekore-5.0.1/src/tekore/_sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_sender/concrete.py` & `tekore-5.0.1/src/tekore/_sender/concrete.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_sender/error.py` & `tekore-5.0.1/src/tekore/_sender/error.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/_sender/extending.py` & `tekore-5.0.1/src/tekore/_sender/extending.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore/model.py` & `tekore-5.0.1/src/tekore/model.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/src/tekore.egg-info/PKG-INFO` & `tekore-5.0.1/src/tekore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tekore
-Version: 5.0.0
+Version: 5.0.1
 Summary: Client for the Spotify Web API
 Author-email: Felix Hildén <felix.hilden@gmail.com>
 Maintainer-email: Felix Hildén <felix.hilden@gmail.com>
 License: MIT License
         
         Copyright (c) 2019-2023 Felix Hildén
```

### Comparing `tekore-5.0.0/src/tekore.egg-info/SOURCES.txt` & `tekore-5.0.1/src/tekore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/auth/expiring.py` & `tekore-5.0.1/tests/auth/expiring.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/auth/refreshing.py` & `tekore-5.0.1/tests/auth/refreshing.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/auth/scope.py` & `tekore-5.0.1/tests/auth/scope.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/auth/util.py` & `tekore-5.0.1/tests/auth/util.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/_resources.py` & `tekore-5.0.1/tests/client/_resources.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/album.py` & `tekore-5.0.1/tests/client/album.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/artist.py` & `tekore-5.0.1/tests/client/artist.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/audiobook.py` & `tekore-5.0.1/tests/client/audiobook.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/base.py` & `tekore-5.0.1/tests/client/base.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/browse.py` & `tekore-5.0.1/tests/client/browse.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/chapter.py` & `tekore-5.0.1/tests/client/chapter.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/episode.py` & `tekore-5.0.1/tests/client/episode.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/follow.py` & `tekore-5.0.1/tests/client/follow.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/full.py` & `tekore-5.0.1/tests/client/full.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/library.py` & `tekore-5.0.1/tests/client/library.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/paging.py` & `tekore-5.0.1/tests/client/paging.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/player.py` & `tekore-5.0.1/tests/client/player.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/playlist.py` & `tekore-5.0.1/tests/client/playlist.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/search.py` & `tekore-5.0.1/tests/client/search.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/show.py` & `tekore-5.0.1/tests/client/show.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/client/track.py` & `tekore-5.0.1/tests/client/track.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/config.py` & `tekore-5.0.1/tests/config.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/conftest.py` & `tekore-5.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/convert.py` & `tekore-5.0.1/tests/convert.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/model.py` & `tekore-5.0.1/tests/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,16 +64,16 @@
 
 class TestModel:
     def test_enum_in_model(self):
         class C(Model):
             v: E
 
         c = C(v=E.a)
-        assert isinstance(c.dict()["v"], str)
-        assert c.json() == '{"v": "a"}'
+        assert isinstance(c.model_dump()["v"], str)
+        assert c.model_dump_json() == '{"v":"a"}'
 
     def test_timestamps_in_model(self):
         class C(Model):
             v: datetime
 
         C(v="2019-01-01T12:00:00Z")
         C(v="2019-01-01T12:00:00.1234Z")
@@ -83,8 +83,8 @@
             i: int
 
         with pytest.warns(UnknownModelAttributeWarning):
             data = Data(i=1, u=2)
 
         with pytest.raises(AttributeError):
             assert data.u
-        assert "u" not in data.json()
+        assert "u" not in data.model_dump_json()
```

### Comparing `tekore-5.0.0/tests/sender/caching.py` & `tekore-5.0.1/tests/sender/caching.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/sender/client.py` & `tekore-5.0.1/tests/sender/client.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tests/sender/retrying.py` & `tekore-5.0.1/tests/sender/retrying.py`

 * *Files identical despite different names*

### Comparing `tekore-5.0.0/tox.ini` & `tekore-5.0.1/tox.ini`

 * *Files identical despite different names*

