# Comparing `tmp/troi-2024.2.9.0.tar.gz` & `tmp/troi-2024.4.26.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troi-2024.2.9.0.tar", last modified: Fri Feb  9 11:47:46 2024, max compression
+gzip compressed data, was "troi-2024.4.26.0.tar", last modified: Fri Apr 26 10:21:36 2024, max compression
```

## Comparing `troi-2024.2.9.0.tar` & `troi-2024.4.26.0.tar`

### file list

```diff
@@ -1,170 +1,161 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.329097 troi-2024.2.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.301097 troi-2024.2.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.305097 troi-2024.2.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-09 11:47:03.000000 troi-2024.2.9.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-02-09 11:47:03.000000 troi-2024.2.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-09 11:47:03.000000 troi-2024.2.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-09 11:47:03.000000 troi-2024.2.9.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-09 11:47:03.000000 troi-2024.2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-02-09 11:47:46.329097 troi-2024.2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-02-09 11:47:03.000000 troi-2024.2.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-09 11:47:03.000000 troi-2024.2.9.0/TODO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-09 11:47:03.000000 troi-2024.2.9.0/config.py.sample
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.305097 troi-2024.2.9.0/docker/
--rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docker/endless.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.305097 troi-2024.2.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.305097 troi-2024.2.9.0/docs/dev/
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/dev/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.305097 troi-2024.2.9.0/docs/elements/
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/elements/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3804 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/elements/listenbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/elements/musicbrainz.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/entities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/lb_radio.rst
--rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/listenbrainz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/patches.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/troi-arguments.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-02-09 11:47:03.000000 troi-2024.2.9.0/docs/user-guide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-09 11:47:03.000000 troi-2024.2.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 11:47:46.329097 troi-2024.2.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.309097 troi-2024.2.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.309097 troi-2024.2.9.0/tests/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/listenbrainz/test_area_random_recordings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/listenbrainz/test_recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/listenbrainz/test_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.309097 troi-2024.2.9.0/tests/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_ac_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_genre_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/musicbrainz/test_year_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_sorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_splitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_tag_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.309097 troi-2024.2.9.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-09 11:47:03.000000 troi-2024.2.9.0/tests/tools/test_area_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.313097 troi-2024.2.9.0/troi/
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8841 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.317097 troi-2024.2.9.0/troi/content_resolver/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2553 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/artist_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7839 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9400 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/content_resolver.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    17637 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/database.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3837 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/duplicates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.317097 troi-2024.2.9.0/troi/content_resolver/formats/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      914 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/flac.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1204 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/m4a.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/mp3.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/ogg_opus.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      918 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/ogg_vorbis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/tag_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      983 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/formats/wma.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/fuzzy_index.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2801 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/lb_radio.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5708 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/metadata_lookup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.317097 troi-2024.2.9.0/troi/content_resolver/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/model/unresolved_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/py_sonic_fix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9988 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/subsonic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5443 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/tag_search.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/top_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6282 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/unresolved_recording.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3432 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/content_resolver/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1698 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13195 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/filters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.317097 troi-2024.2.9.0/troi/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/internal/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     3370 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/internal/top_new_recordings_you_listened_to_for_year.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2689 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/internal/top_recordings_for_year.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2569 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/internal/top_sitewide_recordings_for_year.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2961 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/internal/yim_patch_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.321097 troi-2024.2.9.0/troi/listenbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/area_random_recordings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/dataset_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/listens.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/recs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/listenbrainz/yim_user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.321097 troi-2024.2.9.0/troi/local/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1270 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/local/periodic_jams_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/local/recording_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/loops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.321097 troi-2024.2.9.0/troi/musicbrainz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/artist_credit_id_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/genre_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/mbid_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/mbid_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/recording_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/related_artist_credits.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/musicbrainz/year_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6149 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/operations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5635 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/parse_prompt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9246 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.325097 troi-2024.2.9.0/troi/patches/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2570 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/area_random_recordings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8945 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.325097 troi-2024.2.9.0/troi/patches/lb_radio_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7367 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/artist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3441 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/blend.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/collection.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1543 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2874 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/recs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2544 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/stats.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7386 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/lb_radio_classes/tag.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6984 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/periodic_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/periodic_jams_local.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2004 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/playlist_from_listenbrainz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1200 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/playlist_from_mbids.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3898 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/recs_to_playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2376 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/top_discoveries_for_year.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5881 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/top_missed_recordings_for_year.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3982 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/weekly_flashback_jams.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5776 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/patches/world_trip.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    20649 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/playlist.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4874 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/print_recording.py
--rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/recording_search_service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/sorts.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8076 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.325097 troi-2024.2.9.0/troi/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/tools/area_lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/tools/spotify_lookup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2793 2024-02-09 11:47:03.000000 troi-2024.2.9.0/troi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 11:47:46.325097 troi-2024.2.9.0/troi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7783 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-09 11:47:46.000000 troi-2024.2.9.0/troi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.236178 troi-2024.4.26.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.240178 troi-2024.4.26.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-26 10:21:02.000000 troi-2024.4.26.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-26 10:21:02.000000 troi-2024.4.26.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-26 10:21:36.264179 troi-2024.4.26.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5832 2024-04-26 10:21:02.000000 troi-2024.4.26.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-26 10:21:02.000000 troi-2024.4.26.0/config.py.sample
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.240178 troi-2024.4.26.0/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       54 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docker/endless.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/dev/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.244179 troi-2024.4.26.0/docs/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/listenbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/elements/musicbrainz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/entities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/lb_radio.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    19960 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/listenbrainz-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/patches.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/troi-arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7903 2024-04-26 10:21:02.000000 troi-2024.4.26.0/docs/user-guide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-26 10:21:02.000000 troi-2024.4.26.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:21:36.264179 troi-2024.4.26.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/listenbrainz/test_recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/listenbrainz/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14691 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/musicbrainz/test_related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11684 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8199 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7819 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_plist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_sorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_tag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.248179 troi-2024.4.26.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-26 10:21:02.000000 troi-2024.4.26.0/tests/tools/test_area_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.252179 troi-2024.4.26.0/troi/
+-rw-r--r--   0 runner    (1001) docker     (127)    13635 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9616 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.252179 troi-2024.4.26.0/troi/content_resolver/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4411 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/artist_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8637 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9460 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/content_resolver.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    18059 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/database.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3647 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/duplicates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/content_resolver/formats/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      899 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/flac.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1189 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/m4a.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1977 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/mp3.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      913 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/ogg_opus.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      903 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/ogg_vorbis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/tag_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      968 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/formats/wma.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3345 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/fuzzy_index.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2677 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/lb_radio.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6199 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/metadata_lookup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/content_resolver/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/model/unresolved_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/py_sonic_fix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10148 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/subsonic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5400 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/tag_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1230 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/top_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6273 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/unresolved_recording.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/content_resolver/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1714 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/external/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/external/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/filters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.256178 troi-2024.4.26.0/troi/listenbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/listens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/recs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/listenbrainz/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/unused/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/unused/dataset_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/listenbrainz/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/local/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1388 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/local/periodic_jams_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/local/recording_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/loops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/musicbrainz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/mbid_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/mbid_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/recording_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/musicbrainz/related_artist_credits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/operations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6070 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/parse_prompt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8787 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.260179 troi-2024.4.26.0/troi/patches/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1442 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/ai_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10520 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/patches/lb_radio_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3041 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/artist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3457 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/blend.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1643 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/country.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1543 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2880 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/recs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2850 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4118 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/lb_radio_classes/tag.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6880 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/periodic_jams.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3150 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/periodic_jams_local.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2022 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/playlist_from_listenbrainz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1180 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/playlist_from_mbids.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3878 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/recs_to_playlist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/patches/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/unused/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2550 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/patches/unused/area_random_recordings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    20763 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/playlist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2747 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/plist.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4866 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/print_recording.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/recording_search_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      682 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/sorts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/area_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/tools/spotify_lookup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2912 2024-04-26 10:21:02.000000 troi-2024.4.26.0/troi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:21:36.264179 troi-2024.4.26.0/troi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7784 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-26 10:21:36.000000 troi-2024.4.26.0/troi.egg-info/top_level.txt
```

### Comparing `troi-2024.2.9.0/.github/workflows/cd.yml` & `troi-2024.4.26.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/.github/workflows/ci.yml` & `troi-2024.4.26.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/LICENSE` & `troi-2024.4.26.0/LICENSE`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/PKG-INFO` & `troi-2024.4.26.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 2024.2.9.0
+Version: 2024.4.26.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-2024.2.9.0/README.md` & `troi-2024.4.26.0/README.md`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/Makefile` & `troi-2024.4.26.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/conf.py` & `troi-2024.4.26.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/dev/index.rst` & `troi-2024.4.26.0/docs/dev/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/elements/index.rst` & `troi-2024.4.26.0/docs/elements/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/elements/listenbrainz.rst` & `troi-2024.4.26.0/docs/elements/listenbrainz.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 ListenBrainz Elements
 =====================
 
 The following elements fetch data from ListenBrainz:
 
-troi.listenbrainz.area_random_recordings
-----------------------------------------
-
-This Element is more a proof-of-concept for a fun discovery tool: Give me random recordings from a country during
-a specific time period. Fun for making wild exploration playlists!
-
-.. autoclass:: troi.listenbrainz.area_random_recordings.AreaRandomRecordingsElement
-
-
 troi.listenbrainz.dataset_fetcher.DataSetFetcherElement
 -------------------------------------------------------
 
 ListenBrainz has developed a tool called the `dataset hoster <https://github.com/metabrainz/data-set-hoster>`_ which allows
 us to quickly host SQL queries on the web. This Element is a shortcut for fetching data from one of these endpoints
 and to return a list of Recordings.
```

### Comparing `troi-2024.2.9.0/docs/elements/musicbrainz.rst` & `troi-2024.4.26.0/docs/elements/musicbrainz.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,13 @@
 MusicBrainz Elements
 ====================
 
 The following elements fetch data from MusicBrainz:
 
 
-troi.musicbrainz.artist_credit_id_lookup
-----------------------------------------
-
-Load artist_credit_name and artist_credit_mbids for Artist objects that have an artist_credit_id:
-
-.. autoclass:: troi.musicbrainz.artist_credit_id_lookup.ArtistCreditIdLookupElement
-
-
-troi.musicbrainz.genre_lookup
------------------------------
-
-Retrieve genre tags for Recordings that have their mbid set correctly:
-
-.. autoclass:: troi.musicbrainz.genre_lookup.GenreLookupElement
-
-The Recordings passed into this Element will have the "tags" and "genres" fields in the Recording.musicbrainz dict
-that contain lists of tags and genres. If one of these list is empty, there are no tags/genres for this Recording.
-
-
 troi.musicbrainz.mbid_mapping
 -----------------------------
 
 Look up a Recording in the ListenBrainz MBID mapper from only an Artist.artsit_credit_name and a Recording.name.
 
 
 .. autoclass:: troi.musicbrainz.mbid_mapping.MBIDMappingLookupElement
```

### Comparing `troi-2024.2.9.0/docs/entities.rst` & `troi-2024.4.26.0/docs/entities.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/index.rst` & `troi-2024.4.26.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/installation.rst` & `troi-2024.4.26.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/introduction.rst` & `troi-2024.4.26.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/lb_radio.rst` & `troi-2024.4.26.0/docs/lb_radio.rst`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 #. **artist**: Play tracks from this artists and similar artists
 #. **tag**: Play tracks from one of more tags
 #. **collection**: Use a MusicBrainz collection as a source of recordings. (mode does not apply to collections)
 #. **playlist**: Use a ListenBrainz playlist as a source of recordings. (mode also does not apply to playlists)
 #. **stats**: Use a ListenBrainz user's statistics as a source of recordings.
 #. **recs**: Use a ListenBrainz user's recommended recordings as a source of recordings.
+#. **country**: Select recordings from artists who are from the given country.
 
 Options
 -------
 
 All terms have the following options:
 
 #. **easy**: Use easy mode for this term. See modes below.
@@ -161,29 +162,29 @@
 
   tag:(trip hop, downtempo)
 
 If LB-radio does not find your artist, you can specify an artist using an Artist MBID:
 
 ::
 
-  artist:8f6bd1e4-fbe1-4f50-aa9b-94c450ec0f11
+  artist:(8f6bd1e4-fbe1-4f50-aa9b-94c450ec0f11)
 
 LB-radio also supports MusicBrainz collections as sources:
 
 ::
 
-  collection:8be1a919-a386-45f3-8cc2-0d9249b02aa4
+  collection:(8be1a919-a386-45f3-8cc2-0d9249b02aa4)
 
 Will select random recordings from a MusicBrainz recording collection -- the modes wont have any affect on collections, since
 collections have no inherent ranking that could be used to select recordings according to mode. :(
 
 
 ::
 
-  playlist:8be1a919-a386-45f3-8cc2-0d9249b02aa4
+  playlist:(8be1a919-a386-45f3-8cc2-0d9249b02aa4)
 
 Will select random recordings from a ListenBrainz playlist -- the modes wont have any affect on collections, since
 plylists have no inherent ranking that could be used to select recordings according to mode. :(
 
 
 ::
 
@@ -194,14 +195,22 @@
 
 ::
 
   recs:mr_monkey::unlistened
 
 Will select random recordings from the ListenBrainz user mr_monkey's recommended recordings that mr_monkey hasn't listened to.
 
+::
+
+  country:(Mali)
+
+Will select random recordings from artists who are from the given country. While this features generally represents music from
+that selected country, some artists leave their home country and don't perform music representative of their country, so 
+this element may not always be 100% on point. But it can still create some very interesting playlists!
+
 
 More complex examples
 ---------------------
 
 ::
 
   artist:(pretty lights):3:easy tag:(trip hop):2 artist:(morcheeba)::nosim
```

### Comparing `troi-2024.2.9.0/docs/listenbrainz-logo.svg` & `troi-2024.4.26.0/docs/listenbrainz-logo.svg`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/make.bat` & `troi-2024.4.26.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/patches.rst` & `troi-2024.4.26.0/docs/patches.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/troi-arguments.rst` & `troi-2024.4.26.0/docs/troi-arguments.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/docs/user-guide.rst` & `troi-2024.4.26.0/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/pyproject.toml` & `troi-2024.4.26.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/tests/listenbrainz/test_recs.py` & `troi-2024.4.26.0/tests/listenbrainz/test_recs.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/tests/listenbrainz/test_stats.py` & `troi-2024.4.26.0/tests/listenbrainz/test_stats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from unittest.mock import patch
 
-from troi import Artist, Release, Recording
+from troi import Artist, ArtistCredit, Release, Recording
 import troi.listenbrainz.stats
 
 artist_ret = {
     'payload': {
         'artists': [
             {
                  'artist_mbids': [], 
@@ -62,35 +62,35 @@
     def test_user_artist_stats(self, stats_mock):
 
         stats_mock.return_value = artist_ret
         u = troi.listenbrainz.stats.UserArtistsElement("rob", 1, 1, "week")
         entities = u.read()
         stats_mock.assert_called_with("rob", 1, 1, "week")
         assert len(entities) == 1
-        assert isinstance(entities[0], Artist)
-        assert entities[0].mbids is None
+        assert isinstance(entities[0], ArtistCredit)
         assert entities[0].name == 'Pretty Lights'
+        assert len(entities[0].artists) == 0
 
     @patch('liblistenbrainz.ListenBrainz.get_user_releases')
     def test_user_release_stats(self, stats_mock):
 
         stats_mock.return_value = release_ret
         u = troi.listenbrainz.stats.UserReleasesElement("rob", 1, 1, "all_time")
         entities = u.read()
         stats_mock.assert_called_with("rob", 1, 1, "all_time")
         assert len(entities) == 1
         assert isinstance(entities[0], Release)
-        assert entities[0].artist.name == 'Saltillo'
+        assert entities[0].artist_credit.name == 'Saltillo'
         assert entities[0].name == 'Ganglion'
 
     @patch('liblistenbrainz.ListenBrainz.get_user_recordings')
     def test_user_recording_stats(self, stats_mock):
 
         stats_mock.return_value = recording_ret
         u = troi.listenbrainz.stats.UserRecordingElement("rob", 1, 1, "all_time")
         entities = u.read()
         stats_mock.assert_called_with("rob", 1, 1, "all_time")
         assert len(entities) == 1
         assert isinstance(entities[0], Recording)
-        assert entities[0].artist.name == 'Woolfy'
+        assert entities[0].artist_credit.name == 'Woolfy'
         assert entities[0].release.name == 'Stations'
         assert entities[0].name == 'Tangiers'
```

### Comparing `troi-2024.2.9.0/tests/musicbrainz/test_mbid_mapping.py` & `troi-2024.4.26.0/tests/musicbrainz/test_mbid_mapping.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "artist_credit_name": "Morcheeba",
         "index": 0,
         "recording_arg": "trigger hippie",
         "recording_mbid": "97e69767-5d34-4c97-b36a-f3b2b1ef9dae",
         "recording_name": "Trigger Hippie",
         "release_mbid": "9db51cd6-38f6-3b42-8ad5-559963d68f35",
         "release_name": "Who Can You Trust?",
-        "year": 1996
+        "artist_mbids": ["067102ea-9519-4622-9077-57ca4164cfbb"]
     }
 ]
 
 
 def mocked_requests_post(*args, **kwargs):
     class MockResponse:
         def __init__(self, json_data, status_code):
@@ -40,33 +40,32 @@
 class TestMBIDMapping(unittest.TestCase):
 
     @unittest.mock.patch('requests.post', side_effect=mocked_requests_post)
     def test_read(self, req):
 
         e = troi.musicbrainz.mbid_mapping.MBIDMappingLookupElement()
 
-        r = [ troi.Recording("trigger hippie", artist=troi.Artist("morcheeba")) ]
+        r = [ troi.Recording("trigger hippie", artist_credit=troi.ArtistCredit(name="morcheeba")) ]
         entities = e.read([r])
         req.assert_called_with(e.SERVER_URL, json=[{'[artist_credit_name]': 'morcheeba', '[recording_name]': 'trigger hippie'}])
 
         assert len(entities) == 1
-        assert entities[0].artist.artist_credit_id == 963
-        assert entities[0].artist.name == "Morcheeba"
+        assert entities[0].artist_credit.artist_credit_id == 963
+        assert entities[0].artist_credit.name == "Morcheeba"
+        assert entities[0].artist_credit.artists[0].mbid == "067102ea-9519-4622-9077-57ca4164cfbb"
         assert entities[0].release.mbid == "9db51cd6-38f6-3b42-8ad5-559963d68f35"
         assert entities[0].release.name == "Who Can You Trust?"
         assert entities[0].mbid == "97e69767-5d34-4c97-b36a-f3b2b1ef9dae"
         assert entities[0].name == "Trigger Hippie"
-        assert entities[0].year == 1996
-
 
     @unittest.mock.patch('requests.post')
     def test_read_remove_unmatched(self, req):
 
         mock = unittest.mock.MagicMock()
         mock.status_code = 200
         mock.text = "{}"
         req.return_value = mock
         e = troi.musicbrainz.mbid_mapping.MBIDMappingLookupElement(True)
 
-        r = [ troi.Recording("track not found", artist=troi.Artist("artist not found")) ]
+        r = [ troi.Recording("track not found", artist_credit=troi.ArtistCredit(name="artist not found")) ]
         entities = e.read([r])
         assert len(entities) == 0
```

### Comparing `troi-2024.2.9.0/tests/musicbrainz/test_related_artist_credits.py` & `troi-2024.4.26.0/tests/musicbrainz/test_related_artist_credits.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 
         mock = unittest.mock.MagicMock()
         mock.status_code = 200
         mock.text = return_json
         req.return_value = mock
         e = troi.musicbrainz.related_artist_credits.RelatedArtistCreditsElement()
 
-        inputs = [ troi.Artist(artist_credit_id=65), 
-                   troi.Artist(artist_credit_id=963) ]
+        inputs = [ troi.ArtistCredit(artist_credit_id=65), 
+                   troi.ArtistCredit(artist_credit_id=963) ]
         entities = e.read([inputs])
         req.assert_called_with(e.SERVER_URL, params={'[artist_credit_id]': '65,963', 'threshold': 0})
 
         assert len(entities) == 2
         assert entities[0].artist_credit_id == 65
         assert entities[1].artist_credit_id == 963
         assert len(entities[0].musicbrainz['related_artist_credit_ids']) == 1
```

### Comparing `troi-2024.2.9.0/tests/test_entities.py` & `troi-2024.4.26.0/tests/test_entities.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 import unittest
 
-from troi import Artist, Release, Recording, Playlist
+from troi import Artist, ArtistCredit, Release, Recording, Playlist
 
 
 class TestEntities(unittest.TestCase):
 
     def test_artist(self):
 
         a = Artist()
-        assert a.mbids is None
+        assert a.mbid is None
+        assert a.name is None
+
+        a = Artist("Portishead", mbid="8fe3f1d4-b6d5-4726-89ad-926e3420b9e3", ranking=1.0)
+        assert a.name == "Portishead"
+        assert a.mbid == "8fe3f1d4-b6d5-4726-89ad-926e3420b9e3"
+        assert a.ranking == 1.0
+
+        a = Artist(listenbrainz={ 1 : 2}, musicbrainz={ 3 : 4}, acousticbrainz={ 5 : 6})
+        assert a.lb[1] == 2
+        assert a.mb[3] == 4
+        assert a.ab[5] == 6
+        assert a.name is None
+        assert a.mbid is None
+
+    def test_artist_credit(self):
+
+        a = ArtistCredit()
+        assert a.artists == []
         assert a.name is None
         assert a.artist_credit_id is None
         with self.assertRaises(TypeError):
-            a = Artist(mbids="not a list")
+            a = Artist(artists="not a list")
 
-        a = Artist("Portishead", ["8fe3f1d4-b6d5-4726-89ad-926e3420b9e3"], ranking=1.0)
+        a = ArtistCredit("Portishead", artists=[Artist(name="Portishead", mbid="8fe3f1d4-b6d5-4726-89ad-926e3420b9e3")], ranking=1.0)
         assert a.name == "Portishead"
-        assert a.mbids == ["8fe3f1d4-b6d5-4726-89ad-926e3420b9e3"]
+        assert len(a.artists) == 1
         assert a.ranking == 1.0
 
-        a = Artist("Portishead", ["afe3f1d4-b6d5-4726-89ad-926e3420b9e3", "97b01626-65fc-4c32-b30c-c4d7eab1b339"])
-        assert len(a.mbids)
-        assert a.mbids[0] == "97b01626-65fc-4c32-b30c-c4d7eab1b339"
-        assert a.mbids[1] == "afe3f1d4-b6d5-4726-89ad-926e3420b9e3"
-
-        a = Artist("Portishead", artist_credit_id=65)
+        a = ArtistCredit("Portishead", artist_credit_id=65)
         assert a.artist_credit_id == 65
 
         a = Artist(listenbrainz={ 1 : 2}, musicbrainz={ 3 : 4}, acousticbrainz={ 5 : 6})
         assert a.lb[1] == 2
         assert a.mb[3] == 4
         assert a.ab[5] == 6
         assert a.name is None
```

### Comparing `troi-2024.2.9.0/tests/test_filters.py` & `troi-2024.4.26.0/tests/test_filters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 import unittest
 
 import requests_mock
 
-from troi import Artist, Recording, Playlist
+from troi import Artist, ArtistCredit, Recording, Playlist
 import troi.filters
 from troi.musicbrainz.recording import RecordingListElement
 from troi.listenbrainz.feedback import ListensFeedbackLookup
 
 
 class TestArtistCreditFilterElement(unittest.TestCase):
 
     def test_artist_credit_filter_include(self):
         rlist = [
-            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist=Artist(artist_credit_id=65)),
-            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist=Artist(artist_credit_id=197))
+            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist_credit=ArtistCredit(artist_credit_id=65)),
+            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist_credit=ArtistCredit(artist_credit_id=197))
         ]
         alist = [197]
 
         e = troi.filters.ArtistCreditFilterElement(alist, include=True)
         flist = e.read([rlist])
         assert len(flist) == 1
-        assert flist[0].artist.artist_credit_id == 197
+        assert flist[0].artist_credit.artist_credit_id == 197
         assert flist[0].mbid == "73a9d0db-0ec7-490e-9a85-0525a5ccef8e"
 
         alist = [1]
         e = troi.filters.ArtistCreditFilterElement(alist, include=True)
         flist = e.read([rlist])
         assert len(flist) == 0
 
     def test_artist_credit_filter_exclude(self):
         rlist = [
-            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist=Artist(artist_credit_id=65)),
-            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist=Artist(artist_credit_id=197))
+            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist_credit=ArtistCredit(artist_credit_id=65)),
+            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist_credit=ArtistCredit(artist_credit_id=197))
         ]
         alist = [197]
 
         e = troi.filters.ArtistCreditFilterElement(alist)
         flist = e.read([rlist])
         assert len(flist) == 1
-        assert flist[0].artist.artist_credit_id == 65
+        assert flist[0].artist_credit.artist_credit_id == 65
         assert flist[0].mbid == "8756f690-18ca-488d-a456-680fdaf234bd"
 
         alist = [1]
         e = troi.filters.ArtistCreditFilterElement(alist)
         flist = e.read([rlist])
         assert len(flist) == 2
 
 
 class TestArtistCreditLimiterElement(unittest.TestCase):
 
     def test_artist_credit_limiter_higher_ranked(self):
         rlist = [
-            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist=Artist(artist_credit_id=65), ranking=1.0),
-            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist=Artist(artist_credit_id=65), ranking=.5),
-            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist=Artist(artist_credit_id=197), ranking=.1)
+            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist_credit=ArtistCredit(artist_credit_id=65), ranking=1.0),
+            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist_credit=ArtistCredit(artist_credit_id=65), ranking=.5),
+            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist_credit=ArtistCredit(artist_credit_id=197), ranking=.1)
         ]
 
         e = troi.filters.ArtistCreditLimiterElement(1)
         flist = e.read([rlist])
         assert len(flist) == 2
-        assert flist[0].artist.artist_credit_id == 65
+        assert flist[0].artist_credit.artist_credit_id == 65
         assert flist[0].mbid == "8756f690-18ca-488d-a456-680fdaf234bd"
-        assert flist[1].artist.artist_credit_id == 197
+        assert flist[1].artist_credit.artist_credit_id == 197
         assert flist[1].mbid == "73a9d0db-0ec7-490e-9a85-0525a5ccef8e"
 
         e = troi.filters.ArtistCreditLimiterElement(1, exclude_lower_ranked=False)
         flist = e.read([rlist])
         assert len(flist) == 2
-        assert flist[0].artist.artist_credit_id == 65
+        assert flist[0].artist_credit.artist_credit_id == 65
         assert flist[0].mbid == "139654ae-2c02-4e0f-aee0-c47da6e59ff1"
-        assert flist[1].artist.artist_credit_id == 197
+        assert flist[1].artist_credit.artist_credit_id == 197
         assert flist[1].mbid == "73a9d0db-0ec7-490e-9a85-0525a5ccef8e"
 
     def test_artist_credit_limiter_playlist(self):
         p = Playlist("test playlist")
         p.recordings = [
-            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist=Artist(artist_credit_id=65), ranking=1.0),
-            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist=Artist(artist_credit_id=65), ranking=.5),
-            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist=Artist(artist_credit_id=197), ranking=.1)
+            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist_credit=ArtistCredit(artist_credit_id=65), ranking=1.0),
+            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist_credit=ArtistCredit(artist_credit_id=65), ranking=.5),
+            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist_credit=ArtistCredit(artist_credit_id=197), ranking=.1)
         ]
 
         p2 = Playlist("test playlist 2")
         p2.recordings = [
-            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist=Artist(artist_credit_id=48), ranking=1.0),
-            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist=Artist(artist_credit_id=197), ranking=.1),
-            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist=Artist(artist_credit_id=48), ranking=.5)
+            Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd', artist_credit=ArtistCredit(artist_credit_id=48), ranking=1.0),
+            Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e', artist_credit=ArtistCredit(artist_credit_id=197), ranking=.1),
+            Recording(mbid='139654ae-2c02-4e0f-aee0-c47da6e59ff1', artist_credit=ArtistCredit(artist_credit_id=48), ranking=.5)
         ]
 
         e = troi.filters.ArtistCreditLimiterElement(1)
         plist = e.read([[p, p2]])
         assert len(plist) == 2
         assert len(plist[0].recordings) == 2
-        assert plist[0].recordings[0].artist.artist_credit_id == 65
+        assert plist[0].recordings[0].artist_credit.artist_credit_id == 65
         assert plist[0].recordings[0].mbid == "8756f690-18ca-488d-a456-680fdaf234bd"
-        assert plist[0].recordings[1].artist.artist_credit_id == 197
+        assert plist[0].recordings[1].artist_credit.artist_credit_id == 197
         assert plist[0].recordings[1].mbid == "73a9d0db-0ec7-490e-9a85-0525a5ccef8e"
         assert len(plist[1].recordings) == 2
-        assert plist[1].recordings[0].artist.artist_credit_id == 48
+        assert plist[1].recordings[0].artist_credit.artist_credit_id == 48
         assert plist[1].recordings[0].mbid == "8756f690-18ca-488d-a456-680fdaf234bd"
-        assert plist[1].recordings[1].artist.artist_credit_id == 197
+        assert plist[1].recordings[1].artist_credit.artist_credit_id == 197
         assert plist[1].recordings[1].mbid == "73a9d0db-0ec7-490e-9a85-0525a5ccef8e"
 
 
 class TestDuplicateRecordingMBIDFilterElement(unittest.TestCase):
 
     def test_duplicate_recording_filter_element(self):
         rlist = [
@@ -211,15 +211,15 @@
             Recording(mbid="8e7a9ff8-c31d-4ac0-a01d-20a7fcc28c8f")
         ])
         feedback_lookup = ListensFeedbackLookup(user_name="lucifer")
         feedback_lookup.set_sources(recordings)
         filter_element = troi.filters.HatedRecordingsFilterElement()
         filter_element.set_sources(feedback_lookup)
 
-        received = filter_element.generate()
+        received = filter_element.generate(quiet=True)
         expected = [
             Recording(mbid="53969964-673a-4407-9396-3087be9245f6", listenbrainz={"score": 1}),
             Recording(mbid="8e7a9ff8-c31d-4ac0-a01d-20a7fcc28c8f", listenbrainz={"score": 0})
         ]
         self.assertEqual(expected[0].mbid, received[0].mbid)
         self.assertEqual(expected[0].listenbrainz, received[0].listenbrainz)
         self.assertEqual(expected[1].mbid, received[1].mbid)
```

### Comparing `troi-2024.2.9.0/tests/test_operations.py` & `troi-2024.4.26.0/tests/test_operations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import unittest
 
-from troi import Artist, Release, Recording
+from troi import Artist, ArtistCredit, Release, Recording
 import troi.operations 
 
 
 class TestOperations(unittest.TestCase):
 
     def test_is_homogeneous(self):
         alist = [ ]
@@ -14,38 +14,38 @@
         assert troi.operations.is_homogeneous(alist) == True
 
         alist = [ Artist(), Release() ]
         assert troi.operations.is_homogeneous(alist) == False
 
     def test_unique(self):
         # Test artists
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['a1c35a51-d102-4ce7-aefb-79a361e843b6']) ]
-        e = troi.operations.UniqueElement('mbids')
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
+        e = troi.operations.UniqueElement('mbid')
         u_alist = e.read([alist])
         assert len(u_alist) == 2
 
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']) ]
-        e = troi.operations.UniqueElement('mbids')
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
+        e = troi.operations.UniqueElement('mbid')
         u_alist = e.read([alist])
         assert len(u_alist) == 1
-        assert u_alist[0].mbids == ['8756f690-18ca-488d-a456-680fdaf234bd']
+        assert u_alist[0].mbid == '8756f690-18ca-488d-a456-680fdaf234bd'
 
-        alist = [ Artist(artist_credit_id=65),
-                  Artist(artist_credit_id=65) ]
+        alist = [ ArtistCredit(artist_credit_id=65),
+                  ArtistCredit(artist_credit_id=65) ]
         e = troi.operations.UniqueElement('artist_credit_id')
         u_alist = e.read([alist])
         assert len(u_alist) == 1
         assert u_alist[0].artist_credit_id == 65
 
         # Test recording (not testing release since rel and rec use same code)
         rlist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
                   Recording(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
-        e = troi.operations.UniqueElement('mbids')
+        e = troi.operations.UniqueElement('foo')
         with self.assertRaises(ValueError):
             u_rlist = e.read([rlist])
 
         e = troi.operations.UniqueElement('mbid')
         u_rlist = e.read([rlist])
         assert len(u_rlist) == 2
 
@@ -53,21 +53,21 @@
                   Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
         u_rlist = e.read([rlist])
         assert len(u_rlist) == 1
         assert u_rlist[0].mbid == '8756f690-18ca-488d-a456-680fdaf234bd'
 
     def test_ensure_conformity(self):
         # Test artists
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
-        blist = [ Artist(mbids=['a1c35a51-d102-4ce7-aefb-79a361e843b6']) ]
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
+        blist = [ Artist(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         assert troi.operations._ensure_conformity(alist, blist) == True
 
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
         blist = [ Release(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         with self.assertRaises(TypeError):
             troi.operations._ensure_conformity(alist, blist)
 
         # Test recording (not testing release since rel and rec use same code)
         alist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
                   Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
@@ -78,46 +78,46 @@
                   Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
         blist = [ Release(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         with self.assertRaises(TypeError):
             troi.operations._ensure_conformity(alist, blist)
 
     def test_union(self):
         # Test artists
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']) ]
-        blist = [ Artist(mbids=['a1c35a51-d102-4ce7-aefb-79a361e843b6']) ]
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
+        blist = [ Artist(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         e = troi.operations.UnionElement()
         ulist = e.read([alist, blist])
         assert len(ulist) == 2
-        assert ulist[0].mbids == ['8756f690-18ca-488d-a456-680fdaf234bd']
-        assert ulist[1].mbids == ['a1c35a51-d102-4ce7-aefb-79a361e843b6']
+        assert ulist[0].mbid == '8756f690-18ca-488d-a456-680fdaf234bd'
+        assert ulist[1].mbid == 'a1c35a51-d102-4ce7-aefb-79a361e843b6'
 
         # Test recording (not testing release since rel and rec use same code)
         alist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
         blist = [ Recording(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         ulist = e.read([alist, blist])
         assert len(ulist) == 2
         assert ulist[0].mbid == '8756f690-18ca-488d-a456-680fdaf234bd'
         assert ulist[1].mbid == 'a1c35a51-d102-4ce7-aefb-79a361e843b6'
 
     def test_intersection(self):
         # Test artists
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
-        blist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']) ]
-        e = troi.operations.IntersectionElement('mbid')
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
+        blist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
+        e = troi.operations.IntersectionElement('meh')
         with self.assertRaises(ValueError):
             ilist = e.read([alist, blist])
 
-        e = troi.operations.IntersectionElement('mbids')
+        e = troi.operations.IntersectionElement('mbid')
         ilist = e.read([alist, blist])
         assert len(ilist) == 1
-        assert ilist[0].mbids == blist[0].mbids
+        assert ilist[0].mbid == blist[0].mbid
 
-        alist = [ Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
-        blist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']) ]
+        alist = [ Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
+        blist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
         ilist = e.read([alist, blist])
         assert len(ilist) == 0
 
         # Test recording (not testing release since rel and rec use same code)
         alist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
                   Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
         blist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
@@ -133,33 +133,33 @@
         alist = [ Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
         blist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
         ilist = e.read([alist, blist])
         assert len(ilist) == 0
 
     def test_difference(self):
         # Test artists
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
-        blist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']) ]
-        e = troi.operations.DifferenceElement('mbid')
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
+        blist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
+        e = troi.operations.DifferenceElement('mbids')
         with self.assertRaises(ValueError):
             ilist = e.read([alist, blist])
 
-        e = troi.operations.DifferenceElement('mbids')
+        e = troi.operations.DifferenceElement('mbid')
         ilist = e.read([alist, blist])
         assert len(ilist) == 1
-        assert ilist[0].mbids == ['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']
+        assert ilist[0].mbid == '73a9d0db-0ec7-490e-9a85-0525a5ccef8e'
 
-        alist = [ Artist(mbids=['8756f690-18ca-488d-a456-680fdaf234bd']), 
-                  Artist(mbids=['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']) ]
-        blist = [ Artist(mbids=['a1c35a51-d102-4ce7-aefb-79a361e843b6']) ]
+        alist = [ Artist(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
+                  Artist(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
+        blist = [ Artist(mbid='a1c35a51-d102-4ce7-aefb-79a361e843b6') ]
         dlist = e.read([alist, blist])
         assert len(dlist) == 2
-        assert dlist[0].mbids == ['8756f690-18ca-488d-a456-680fdaf234bd']
-        assert dlist[1].mbids == ['73a9d0db-0ec7-490e-9a85-0525a5ccef8e']
+        assert dlist[0].mbid == '8756f690-18ca-488d-a456-680fdaf234bd'
+        assert dlist[1].mbid == '73a9d0db-0ec7-490e-9a85-0525a5ccef8e'
 
         # Test recording (not testing release since rel and rec use same code)
         alist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd'), 
                   Recording(mbid='73a9d0db-0ec7-490e-9a85-0525a5ccef8e') ]
         blist = [ Recording(mbid='8756f690-18ca-488d-a456-680fdaf234bd') ]
         e = troi.operations.DifferenceElement('mbids')
         with self.assertRaises(ValueError):
```

### Comparing `troi-2024.2.9.0/tests/test_parser.py` & `troi-2024.4.26.0/tests/test_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 from troi.parse_prompt import PromptParser, ParseError
 
 
 class TestParser(unittest.TestCase):
 
     def test_basic_entities(self):
         pp = PromptParser()
-        r = pp.parse("artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        r = pp.parse("artist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
         assert r[0] == {"entity": "artist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
 
-        r = pp.parse("artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        r = pp.parse("artist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
         assert r[0] == {"entity": "artist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
 
         self.assertRaises(ParseError, pp.parse, "wrong:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        self.assertRaises(ParseError, pp.parse, "artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
 
         r = pp.parse("artist:(the knife)")
         assert r[0] == {"entity": "artist", "values": ["the knife"], "weight": 1, "opts": []}
 
         self.assertRaises(ParseError, pp.parse, "artist:u2:nosim")
         self.assertRaises(ParseError, pp.parse, "artists:u2:nosim")
+        self.assertRaises(ParseError, pp.parse, "country:andorra")
 
     def test_tags(self):
         pp = PromptParser()
         r = pp.parse("tag:abstract tag:rock tag:blues")
         assert r[0] == {"entity": "tag", "values": ["abstract"], "weight": 1, "opts": []}
         assert r[1] == {"entity": "tag", "values": ["rock"], "weight": 1, "opts": []}
         assert r[2] == {"entity": "tag", "values": ["blues"], "weight": 1, "opts": []}
@@ -48,14 +50,17 @@
 
         r = pp.parse("tag:(blümchen)")
         assert r[0] == {"entity": "tag", "values": ["blümchen"], "weight": 1, "opts": []}
 
         r = pp.parse("tag:(モーニング娘。)")
         assert r[0] == {"entity": "tag", "values": ["モーニング娘。"], "weight": 1, "opts": []}
 
+        r = pp.parse("tag:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
+        assert r[0] == {"entity": "tag", "values": ["57baa3c6-ee43-4db3-9e6a-50bbc9792ee4"], "weight": 1, "opts": []}
+
     def test_tag_errors(self):
         pp = PromptParser()
         self.assertRaises(ParseError, pp.parse, "t:(abstract rock blues):bork")
         self.assertRaises(ParseError, pp.parse, "tag:(foo")
         self.assertRaises(ParseError, pp.parse, "tag:foo)")
 
     def test_shortcuts(self):
@@ -69,33 +74,33 @@
 
         pp = PromptParser()
         r = pp.parse("amy winehouse")
         assert r[0] == {"entity": "artist", "values": ["amy winehouse"], "weight": 1, "opts": []}
 
     def test_compound(self):
         pp = PromptParser()
-        r = pp.parse('artist:05319f96-e409-4199-b94f-3cabe7cc188a:2 tag:(downtempo):1 tag:(trip hop, abstract):2')
+        r = pp.parse('artist:(05319f96-e409-4199-b94f-3cabe7cc188a):2 tag:(downtempo):1 tag:(trip hop, abstract):2')
         assert r[0] == {"entity": "artist", "values": [UUID("05319f96-e409-4199-b94f-3cabe7cc188a")], "weight": 2, "opts": []}
         assert r[1] == {"entity": "tag", "values": ["downtempo"], "weight": 1, "opts": []}
         assert r[2] == {"entity": "tag", "values": ["trip hop", "abstract"], "weight": 2, "opts": []}
 
     def test_weights(self):
         pp = PromptParser()
-        r = pp.parse("artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4:1 artist:f54ba4c6-12dd-4358-9136-c64ad89420c5:2")
+        r = pp.parse("artist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4):1 artist:(f54ba4c6-12dd-4358-9136-c64ad89420c5):2")
         assert r[0] == {"entity": "artist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
         assert r[1] == {"entity": "artist", "values": [UUID("f54ba4c6-12dd-4358-9136-c64ad89420c5")], "weight": 2, "opts": []}
 
         self.assertRaises(ParseError, pp.parse,
                           "artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4:1 artist:f54ba4c6-12dd-4358-9136-c64ad89420c5:fussy")
         self.assertRaises(ParseError, pp.parse, "artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4:1 artist:f54ba4c6-12dd-4358-9136-c64ad89420c5:.5")
 
-        r = pp.parse("artist:portishead::easy")
+        r = pp.parse("artist:(portishead)::easy")
         assert r[0] == {"entity": "artist", "values": ["portishead"], "weight": 1, "opts": ["easy"]}
 
-        r = pp.parse("artist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4::easy")
+        r = pp.parse("artist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)::easy")
         assert r[0] == {"entity": "artist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": ["easy"]}
 
     def test_opts(self):
         pp = PromptParser()
         r = pp.parse("stats:(mr_monkey)::month")
         print(r[0])
         assert r[0] == {"entity": "stats", "values": ["mr_monkey"], "weight": 1, "opts": ["month"]}
@@ -108,21 +113,21 @@
         pp = PromptParser()
         self.assertRaises(ParseError, pp.parse, 'artist:adfadf(meh)')
         self.assertRaises(ParseError, pp.parse, 'artist:adfadf(meh')
         self.assertRaises(ParseError, pp.parse, 'artist:adfadf)meh')
 
     def test_collection_playlist(self):
         pp = PromptParser()
-        r = pp.parse("collection:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        r = pp.parse("collection:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
         assert r[0] == {"entity": "collection", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
 
-        r = pp.parse("playlist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        r = pp.parse("playlist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
         assert r[0] == {"entity": "playlist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
 
-        r = pp.parse("playlist:57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")
+        r = pp.parse("playlist:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
         assert r[0] == {"entity": "playlist", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
 
     def test_stats(self):
         pp = PromptParser()
         r = pp.parse("stats:mr_monkey:1:year")
         assert r[0] == {"entity": "stats", "values": ["mr_monkey"], "weight": 1, "opts": ["year"]}
 
@@ -152,7 +157,15 @@
         assert r[0] == {"entity": "recs", "values": ["mr_monkey"], "weight": 1, "opts": ["listened"]}
 
         r = pp.parse("recs:(mr_monkey):2:unlistened")
         assert r[0] == {"entity": "recs", "values": ["mr_monkey"], "weight": 2, "opts": ["unlistened"]}
 
         r = pp.parse("recs:(rob zombie)")
         assert r[0] == {"entity": "recs", "values": ["rob zombie"], "weight": 1, "opts": []}
+
+    def test_country(self):
+        pp = PromptParser()
+        r = pp.parse("country:(57baa3c6-ee43-4db3-9e6a-50bbc9792ee4)")
+        assert r[0] == {"entity": "country", "values": [UUID("57baa3c6-ee43-4db3-9e6a-50bbc9792ee4")], "weight": 1, "opts": []}
+
+        r = pp.parse("country:(mali)")
+        assert r[0] == {"entity": "country", "values": ["mali"], "weight": 1, "opts": []}
```

### Comparing `troi-2024.2.9.0/tests/test_playlist.py` & `troi-2024.4.26.0/tests/test_playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/tests/test_sorts.py` & `troi-2024.4.26.0/tests/test_sorts.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/tests/test_tag_utils.py` & `troi-2024.4.26.0/tests/test_tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/tests/tools/test_area_lookup.py` & `troi-2024.4.26.0/tests/tools/test_area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/__init__.py` & `troi-2024.4.26.0/troi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from abc import ABC, abstractmethod
 import logging
 import random
+from abc import ABC, abstractmethod
 from typing import Dict
 
 from troi.utils import recursively_update_dict
 
+logger = logging.getLogger(__name__)
+logger.setLevel(logging.INFO)
+_handler = logging.StreamHandler()
+_handler.setFormatter(logging.Formatter("%(message)s"))
+logger.addHandler(_handler)
+
 DEVELOPMENT_SERVER_URL = "https://datasets.listenbrainz.org"
 
 # Number of recordings that each patch should aim to generate
 TARGET_NUMBER_OF_RECORDINGS = 50
 
 
 class Element(ABC):
     """
         Base class for elements
     """
 
     def __init__(self, patch=None):
         self.sources = []
-        self.logger = logging.getLogger(type(self).__name__)
         self.patch = patch
 
     def set_patch_object(self, patch):
         """
             Set patch object -- this is so that each element has a reference to the 
             parent Patch. To keep pipeline construction easy, this is done automatically
             once the pipeline starts executing.
@@ -34,97 +39,82 @@
         if self.patch is None:
             raise RuntimeError("This Element does not have a patch set. Pass in the patch to the constructor " +
                                "if you need the patch (for local storage) to be available before the pipeline " +
                                "starts executing.")
 
         return self.patch.local_storage
 
-
-    def log(self, msg):
-        '''
-            Log a message with the info log level, which is the default for troi.
-        '''
-        self.logger.info(msg)
-
-    def debug(self, msg):
-        '''
-            Log a message with debug log level. These messages will only be shown when debugging is enabled.
-        '''
-        self.logger.debug(msg)
-
     def set_sources(self, sources):
         """
            Set the source elements for this element.
 
            :param sources: A list of objects derived from the Element class, containing at least 1 class. When the pipeline is executed the output of the provided class(es) read function will become the input to this class.
         """
 
         if not isinstance(sources, list):
-            sources = [ sources ]
+            sources = [sources]
 
         self.sources = sources
 
         # type check the source
         if len(self.inputs()) > 0:
             for source in sources:
                 matched = False if len(source.outputs()) > 0 else True
                 for output_type in source.outputs() or []:
                     if output_type in self.inputs():
                         matched = True
                         break
 
                 if not matched:
-                    raise RuntimeError("Element %s cannot accept any of %s as input." %
-                                       (type(self).__name__, self.inputs())) 
-
+                    raise RuntimeError("Element %s cannot accept any of %s as input." % (type(self).__name__, self.inputs()))
 
     def check(self):
         """
             Check to see if the necessary connections are in place
             and that types match correctly.
         """
 
         if not self.sources:
             raise PipelineError("element %s has no sources defined." % str(type(self)))
 
         for source in self.sources:
             source.check()
 
-
-    def generate(self):
+    def generate(self, quiet):
         """
             Generate output from the pipeline. This should be called on
             the last element in the pipeline and no where else. At the root
             node generate returns the results, but on interior nodes it
             returns data to be used as input in the next level.
         """
 
         source_lists = []
         if self.sources:
             for source in self.sources:
-                result = source.generate()
+                result = source.generate(quiet)
                 if result is None:
                     return None
 
                 if len(self.inputs()) > 0 and \
                     len(result) > 0 and type(result[0]) not in self.inputs() and \
                     len(source.outputs()) > 0:
-                    raise RuntimeError("Element %s was expected to output %s, but actually output %s" % 
+                    raise RuntimeError("Element %s was expected to output %s, but actually output %s" %
                                        (type(source).__name__, source.outputs()[0], type(result[0])))
 
                 source_lists.append(result)
 
         items = self.read(source_lists)
         if items is None:
             return None
 
-        if len(items) > 0 and type(items[0]) == Playlist:
-            print("  %-50s %d items" % (type(self).__name__[:49], len(items[0].recordings or [])))
-        else:
-            print("  %-50s %d items" % (type(self).__name__[:49], len(items or [])))
+        if not quiet:
+            if len(items) > 0 and type(items[0]) == Playlist:
+                logger.info("  %-50s %d items" % (type(self).__name__[:49], len(items[0].recordings or [])))
+            else:
+                logger.info("  %-50s %d items" % (type(self).__name__[:49], len(items or [])))
 
         return items
 
     def run(self):
         """
             This function should be called on the very last element of the
             pipeline to generate output from the timeline. Run will santiy
@@ -132,40 +122,39 @@
         """
         self.check()
         return self.generate()
 
     @staticmethod
     def inputs():
         """
-            Return a list of Artist, Release or Recording classes that define
-            the type and number of input lists to this element.
-            e.g. [ Artist, Recording ] means that this element expects
-            a list of artists and a list of recordings for inputs.
+            Return a list of Artist, ArtistCredit, Release or Recording classes
+            that define the type and number of input lists to this element.
+            e.g. [ Artist, ArtistCredit, Recording ] means that this element expects
+            a list of artist credits and a list of recordings for inputs.
         """
         return None
 
     @staticmethod
     def outputs():
         """
-            Return a list of Artist, Release or Recording classes that define
-            the type and number of output lists returned by this element.
-            e.g. [ Artist, Recording ] means that this element returns
-            a list of artists and a list of recordings.
+            Return a list of Artist, ArtistCreditm Release or Recording classes
+            that define the type and number of output lists returned by this element.
+            e.g. [ Artist, ArtistCredit, Recording ] means that this element returns
+            a list of artist credits and a list of recordings.
         """
         return None
 
     @abstractmethod
     def read(self, source_data_list):
         '''
             This method is where the action happens -- when the consumer wants to
             read data from the pipeline, it calls read() on the last element in
             the pipeline and this casues the while pipeline to generate result.
             If the initializers of other objects in the pipeline are updated,
-            calling read() again will generate the set new. Passing True for
-            debug should print helpful debug statements about its progress.
+            calling read() again will generate the set new.
 
             Note: This function should not be called directly by the user.
         '''
 
         pass
 
 
@@ -176,17 +165,18 @@
         three dicts named musicbrainz, listenbrainz and acousticbrainz that will
         contain collected metadata respective of each project.
 
         For instance, the musicbrainz dict might have keys that shows the type
         of an artist or the listenbrainz dict might contain the BPM for a track.
         How exactly these dicts will be organized is TDB.
     """
-    def __init__(self, ranking=None, musicbrainz=None, listenbrainz=None, acousticbrainz=None):
+
+    def __init__(self, mbid=None, ranking=None, musicbrainz=None, listenbrainz=None, acousticbrainz=None):
         self.name = None
-        self.mbid = None
+        self.mbid = mbid
         self.musicbrainz = musicbrainz or {}
         self.listenbrainz = listenbrainz or {}
         self.acousticbrainz = acousticbrainz or {}
         self.notes = []
         self.ranking = ranking
 
     @property
@@ -211,67 +201,126 @@
         return "<Entity()>"
 
 
 class Area(Entity):
     """
         The class that represents an area.
     """
+
     def __init__(self, id=id, name=None):
         Entity.__init__(self)
         self.name = name
         self.id = id
 
     def __str__(self):
         return "<Area('%s', %d)>" % (self.name, self.id)
 
 
 class Artist(Entity):
     """
         The class that represents an artist.
     """
-    def __init__(self, name=None, mbids=None, artist_credit_id=None, ranking=None,
-                 musicbrainz=None, listenbrainz=None, acousticbrainz=None):
-        Entity.__init__(self, ranking=ranking, musicbrainz=musicbrainz, listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
+
+    def __init__(self,
+                 name=None,
+                 mbid=None,
+                 artist_id=None,
+                 join_phrase=None,
+                 ranking=None,
+                 musicbrainz=None,
+                 listenbrainz=None,
+                 acousticbrainz=None):
+        Entity.__init__(self, mbid=mbid, ranking=ranking, musicbrainz=musicbrainz,
+                        listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
         self.name = name
+        self.artist_id = artist_id
+        self.join_phrase = join_phrase
+
+    def __str__(self):
+        return "<Artist('%s', [%s], %s)>" % (self.name, self.mbid, self.artist_id)
+
+
+class ArtistCredit(Entity):
+    """
+        The class that represents an artist credit.
+    """
+
+    def __init__(self,
+                 name=None,
+                 artists=None,
+                 artist_credit_id=None,
+                 ranking=None,
+                 musicbrainz=None,
+                 listenbrainz=None,
+                 acousticbrainz=None):
+        Entity.__init__(self, ranking=ranking, musicbrainz=musicbrainz,
+                        listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
+        self.name = name
+        self.artists = []
         self.artist_credit_id = artist_credit_id
-        if mbids:
-            if not isinstance(mbids, list) and not isinstance(mbids, tuple):
-                raise TypeError("Artist mbids must be a list.")
-            self.mbids = sorted(mbids)
-        else:
-            self.mbids = None
+        if artists:
+            if not isinstance(artists, list) and not isinstance(artists, tuple):
+                raise TypeError("Artists must be a list.")
+            self.artists = artists
 
     def __str__(self):
-        return "<Artist('%s', [%s], %s)>" % (self.name, ",".join(self.mbids or []), self.artist_credit_id)
+        return "<ArtistCredit('%s', [%s], %s)>" % (self.name, ",".join([ a.mbid for a in self.artists ]), self.artist_credit_id)
 
 
 class Release(Entity):
     """
         The class that represents a release.
     """
-    def __init__(self, name=None, mbid=None, artist=None, ranking=None,
-                 musicbrainz=None, listenbrainz=None, acousticbrainz=None):
-        Entity.__init__(self, ranking=ranking, musicbrainz=musicbrainz, listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
-        self.artist = artist
+
+    def __init__(self,
+                 name=None,
+                 mbid=None,
+                 artist_credit=None,
+                 ranking=None,
+                 caa_id=None,
+                 caa_release_mbid=None,
+                 musicbrainz=None,
+                 listenbrainz=None,
+                 acousticbrainz=None):
+        Entity.__init__(self,
+                        ranking=ranking,
+                        musicbrainz=musicbrainz,
+                        listenbrainz=listenbrainz,
+                        acousticbrainz=acousticbrainz)
+        self.artist_credit = artist_credit
         self.name = name
         self.mbid = mbid
+        self.caa_id = caa_id
+        self.caa_release_mbid = caa_release_mbid
 
     def __str__(self):
         return "<Release('%s', %s)>" % (self.name, self.mbid)
 
 
 class Recording(Entity):
     """
         The class that represents a recording.
     """
-    def __init__(self, name=None, mbid=None, msid=None, duration=None, artist=None, release=None,
-                 ranking=None, year=None, spotify_id=None, musicbrainz=None, listenbrainz=None, acousticbrainz=None):
+
+    def __init__(self,
+                 name=None,
+                 mbid=None,
+                 msid=None,
+                 duration=None,
+                 artist_credit=None,
+                 release=None,
+                 ranking=None,
+                 year=None,
+                 spotify_id=None,
+                 musicbrainz=None,
+                 listenbrainz=None,
+                 acousticbrainz=None):
         Entity.__init__(self, ranking=ranking, musicbrainz=musicbrainz, listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
-        self.duration = duration # track duration in ms
-        self.artist = artist
+        self.duration = duration  # track duration in ms
+        self.artist_credit = artist_credit
         self.release = release
         self.name = name
         self.mbid = mbid
         self.msid = msid
         self.year = year
         self.spotify_id = spotify_id
 
@@ -285,16 +334,28 @@
         different from the PlaylistElement, which is normally uses to terminate a pipeline for submitting or
         saving result playlists to disk.
 
         The arguments are the same as the other entities, except that mbid in this case refers to a playlist_mbid
         and that filename is the suggested filename that this playlist should be saved as, if the user asked to 
         do that and didn't provide a different filename.
     """
-    def __init__(self, name=None, mbid=None, filename=None, recordings=None, description=None, ranking=None,
-                 year=None, musicbrainz=None, listenbrainz=None, acousticbrainz=None, patch_slug=None, user_name=None,
+
+    def __init__(self,
+                 name=None,
+                 mbid=None,
+                 filename=None,
+                 recordings=None,
+                 description=None,
+                 ranking=None,
+                 year=None,
+                 musicbrainz=None,
+                 listenbrainz=None,
+                 acousticbrainz=None,
+                 patch_slug=None,
+                 user_name=None,
                  additional_metadata=None):
         Entity.__init__(self, ranking=ranking, musicbrainz=musicbrainz, listenbrainz=listenbrainz, acousticbrainz=acousticbrainz)
         self.name = name
         self.filename = filename
         self.mbid = mbid
         self.recordings = recordings
         self.description = description
@@ -319,14 +380,15 @@
         random.shuffle(self.recordings)
 
 
 class User(Entity):
     """
         The class that represents a ListenBrainz user.
     """
+
     def __init__(self, user_name=None, user_id=None):
         Entity.__init__(self)
         self.user_name = user_name
         self.user_id = user_id
 
     def __str__(self):
         return "<User('%s', %d)>" % (self.user_name, self.user_id or -1)
```

### Comparing `troi-2024.2.9.0/troi/cli.py` & `troi-2024.4.26.0/troi/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 #!/usr/bin/env python3
-
+import logging
 import sys
+
 import click
 
+from troi.logging_utils import set_log_level
 from troi.utils import discover_patches
 from troi.core import list_patches, patch_info, convert_patch_to_command
 from troi.content_resolver.cli import cli as resolver_cli, db_file_check, output_playlist
 from troi.content_resolver.subsonic import SubsonicDatabase
 from troi.content_resolver.lb_radio import ListenBrainzRadioLocal
 from troi.content_resolver.playlist import read_jspf_playlist
 from troi.local.periodic_jams_local import PeriodicJamsLocal
 
+logger = logging.getLogger(__name__)
+
 try:
     sys.path.insert(1, ".")
     import config
 except ImportError as err:
     config = None
 
 
@@ -26,16 +30,15 @@
 # Add the "db" submenu
 resolver_cli.short_help = "database and content resolution commands sub menu"
 cli.add_command(resolver_cli, name="db")
 
 
 @cli.command(context_settings=dict(ignore_unknown_options=True, ))
 @click.argument('patch', type=str)
-@click.option('--debug/--no-debug', help="Turn on/off debug statements")
-@click.option('--print', '-p', 'echo', help="Show the generated playlist", required=False, is_flag=True)
+@click.option('--quiet', '-q', 'quiet', help="Do no print out anything", required=False, is_flag=True)
 @click.option('--save', '-s', help="Save the generated playlist", required=False, is_flag=True)
 @click.option(
     '--token',
     '-t',
     help="Specify the ListenBrainz user token to upload playlist. See https://listenbrainz.org/profile to get your user token.",
     required=False,
     type=click.UUID)
@@ -55,34 +58,36 @@
               required=False)
 @click.option('--spotify-url',
               help="instead of creating a new spotify playlist, update the existing playlist at this url",
               type=str,
               required=False,
               multiple=True)
 @click.argument('args', nargs=-1, type=click.UNPROCESSED)
-def playlist(patch, debug, echo, save, token, upload, args, created_for, name, desc, min_recordings, spotify_user_id, spotify_token,
+def playlist(patch, quiet, save, token, upload, args, created_for, name, desc, min_recordings, spotify_user_id, spotify_token,
              spotify_url):
     """
     Generate a global MBID based playlist using a patch
     """
+
+    set_log_level(quiet)
     patchname = patch
     patches = discover_patches()
     if patchname not in patches:
-        print("Cannot load patch '%s'. Use the list command to get a list of available patches." % patchname, file=sys.stderr)
+        logger.info("Cannot load patch '%s'. Use the list command to get a list of available patches." % patchname)
         return None
 
     patch_args = {
-        "echo": echo,
         "save": save,
         "token": token,
         "created_for": created_for,
         "upload": upload,
         "name": name,
         "desc": desc,
-        "min_recordings": min_recordings
+        "min_recordings": min_recordings,
+        "quiet": quiet,
     }
     if spotify_token:
         patch_args["spotify"] = {
             "user_id": spotify_user_id,
             "token": spotify_token,
             "is_public": True,
             "is_collaborative": False,
@@ -93,76 +98,89 @@
         args = []
 
     cmd = convert_patch_to_command(patches[patchname])
     context = cmd.make_context(patchname, list(args))
     patch_args.update(context.forward(cmd))
 
     # Create the actual patch, finally
-    patch = patches[patchname](patch_args, debug)
-    ret = patch.generate_playlist()
+    patch = patches[patchname](patch_args)
+    if patch.is_local():
+        logger.info(
+            "This is a local patch and should be invoked via the specific troi function, rather than the playlist function.")
+        return None
+
+    try:
+        ret = patch.generate_playlist()
+    except RuntimeError as err:
+        logger.error(err)
+        ret = 0
 
     user_feedback = patch.user_feedback()
     if len(user_feedback) > 0:
-        print("User feedback:")
+        logger.info("User feedback:")
         for feedback in user_feedback:
-            print(f"  * {feedback}")
-        print()
+            logger.info(f"  * {feedback}")
+        logger.info("")
 
     sys.exit(0 if ret else -1)
 
 
 @cli.command(name="list")
 def list_patches_cli():
     """List all available patches"""
     ret = list_patches()
     sys.exit(0 if ret else -1)
 
 
 @cli.command(name="info")
 @click.argument("patch", nargs=1)
-def info(patch):
+def info_cmd(patch):
     """Get info for a given patch"""
     ret = patch_info(patch)
     sys.exit(0 if ret else -1)
 
 
 @cli.command(name="resolve", context_settings=dict(ignore_unknown_options=True, ))
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.option('-t', '--threshold', default=.80, help="Minimum match percentage for metadata matches. Must be 0.0 - 1.0")
 @click.option('-u', '--upload-to-subsonic', required=False, is_flag=True, help="upload playlist via subsonic API")
 @click.option('-m', '--save-to-m3u', required=False, help="save to specified m3u playlist")
 @click.option('-j', '--save-to-jspf', required=False, help="save to specified JSPF playlist")
 @click.option('-y', '--dont-ask', required=False, is_flag=True, help="save playlist without asking user")
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
 @click.argument('jspf_playlist')
-def resolve(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, jspf_playlist):
+def resolve(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, quiet, jspf_playlist):
     """ Resolve a global JSPF playlist with MusicBrainz MBIDs to files in the local collection"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = SubsonicDatabase(db_file, config)
+    db = SubsonicDatabase(db_file, config, quiet)
     db.open()
-    lbrl = ListenBrainzRadioLocal()
+    lbrl = ListenBrainzRadioLocal(quiet)
     playlist = read_jspf_playlist(jspf_playlist)
     lbrl.resolve_playlist(threshold, playlist)
     output_playlist(db, playlist, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask)
 
 
 @cli.command(name="lb-radio", context_settings=dict(ignore_unknown_options=True, ))
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.option('-t', '--threshold', default=.80, help="Minimum match percentage for metadata matches. Must be 0.0 - 1.0")
 @click.option('-u', '--upload-to-subsonic', required=False, is_flag=True, help="upload playlist via subsonic API")
 @click.option('-m', '--save-to-m3u', required=False, help="save to specified m3u playlist")
 @click.option('-j', '--save-to-jspf', required=False, help="save to specified JSPF playlist")
 @click.option('-y', '--dont-ask', required=False, is_flag=True, help="save playlist without asking user")
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
 @click.argument('mode')
 @click.argument('prompt')
-def lb_radio(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, mode, prompt):
+def lb_radio(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, quiet, mode, prompt):
     """Use LB Radio to create a playlist from a prompt, using a local music collection"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = SubsonicDatabase(db_file, config)
+    db = SubsonicDatabase(db_file, config, quiet)
     db.open()
-    r = ListenBrainzRadioLocal()
+    r = ListenBrainzRadioLocal(quiet)
     playlist = r.generate(mode, prompt, threshold)
     try:
         _ = playlist.playlists[0].recordings[0]
     except (KeyError, IndexError, AttributeError):
         db.metadata_sanity_check(include_subsonic=upload_to_subsonic)
         return
 
@@ -172,22 +190,24 @@
 @cli.command("weekly-jams", context_settings=dict(ignore_unknown_options=True, ))
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.option('-t', '--threshold', default=.80, help="Minimum match percentage for metadata matches. Must be 0.0 - 1.0")
 @click.option('-u', '--upload-to-subsonic', required=False, is_flag=True, help="upload playlist via subsonic API")
 @click.option('-m', '--save-to-m3u', required=False, help="save to specified m3u playlist")
 @click.option('-j', '--save-to-jspf', required=False, help="save to specified JSPF playlist")
 @click.option('-y', '--dont-ask', required=False, is_flag=True, help="save playlist without asking user")
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
 @click.argument('user_name')
-def periodic_jams(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, user_name):
+def periodic_jams(db_file, threshold, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask, quiet, user_name):
     "Generate a weekly jams playlist for your local collection"
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = SubsonicDatabase(db_file, config)
+    db = SubsonicDatabase(db_file, config, quiet)
     db.open()
 
-    pj = PeriodicJamsLocal(user_name, threshold)
+    pj = PeriodicJamsLocal(user_name, threshold, quiet)
     playlist = pj.generate()
     try:
         _ = playlist.playlists[0].recordings[0]
     except (KeyError, IndexError, AttributeError):
         db.metadata_sanity_check(include_subsonic=upload_to_subsonic)
         return
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/artist_search.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/artist.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,77 @@
-import os
-from collections import defaultdict
-import datetime
-import sys
-
-import peewee
 import requests
 
-from troi.content_resolver.model.database import db
-from troi.content_resolver.model.recording import Recording, RecordingMetadata
-from troi.content_resolver.utils import select_recordings_on_popularity
+import troi
+from troi import Recording, Artist
+from troi.plist import plist
+from troi import TARGET_NUMBER_OF_RECORDINGS
+from troi.utils import interleave
 from troi.recording_search_service import RecordingSearchByArtistService
-from troi.splitter import plist
-
 
-class LocalRecordingSearchByArtistService(RecordingSearchByArtistService):
-    '''
-    Given the local database, search for artists that meet given tag criteria
-    '''
-
-    def __init__(self):
-        RecordingSearchByArtistService.__init__(self)
-
-    def search(self, artist_mbids, begin_percent, end_percent, num_recordings):
-        """
-        Perform an artist search. Parameters:
-
-        tags - a list of artist_mbids for which to search recordings
-        begin_percent - if many recordings match the above parameters, return only
-                        recordings that have a minimum popularity percent score
-                        of begin_percent.
-        end_percent - if many recordings match the above parameters, return only
-                      recordings that have a maximum popularity percent score
-                      of end_percent.
-        num_recordings - ideally return these many recordings
-
-        If only few recordings match, the begin_percent and end_percent are
-        ignored.
-        """
-
-        query = """SELECT popularity
-                        , recording_mbid
-                        , artist_mbid
-                        , file_id
-                        , file_id_type
-                     FROM recording
-                     JOIN recording_metadata
-                       ON recording.id = recording_metadata.recording_id
-                    WHERE artist_mbid in (%s)
-                 ORDER BY artist_mbid
-                        , popularity"""
-
-        placeholders = ",".join(("?", ) * len(artist_mbids))
-        cursor = db.execute_sql(query % placeholders, params=tuple(artist_mbids))
-
-        artists = defaultdict(list)
-        for rec in cursor.fetchall():
-            artists[rec[2]].append({
-                "popularity": rec[0],
-                "recording_mbid": rec[1],
-                "artist_mbid": rec[2],
-                "file_id": rec[3],
-                "file_id_type": rec[4]
-            })
 
-        for artist in artists:
-            artists[artist] = select_recordings_on_popularity(artists[artist], begin_percent, end_percent, num_recordings)
+class LBRadioArtistRecordingElement(troi.Element):
+    """
+        Given an artist, find its similar artists and their popular tracks and return one 
+        stream of recodings from it.
+    """
+
+    MAX_TOP_RECORDINGS_PER_ARTIST = 35  # should lower this when other sources of data get added
+    MAX_NUM_SIMILAR_ARTISTS = 8
+
+    def __init__(self, artist_mbid, artist_name, mode="easy", include_similar_artists=True):
+        troi.Element.__init__(self)
+        self.artist_mbid = str(artist_mbid)
+        self.artist_name = artist_name
+        self.mode = mode
+        self.include_similar_artists = include_similar_artists
+        if include_similar_artists:
+            self.max_top_recordings_per_artist = self.MAX_TOP_RECORDINGS_PER_ARTIST * 2
+        else:
+            self.max_top_recordings_per_artist = self.MAX_TOP_RECORDINGS_PER_ARTIST * 3
+
+    def inputs(self):
+        return []
+
+    def outputs(self):
+        return [Recording]
+
+    def read(self, entities):
+
+        self.data_cache = self.local_storage["data_cache"]
+
+        # Fetch our mode ranges
+        start, stop = self.local_storage["modes"][self.mode]
+        self.recording_search_by_artist = self.patch.get_service("recording-search-by-artist")
+        (artist_recordings, msgs) = self.recording_search_by_artist.search(self.mode, self.artist_mbid, start, stop,
+                                                                           self.max_top_recordings_per_artist,
+                                                                           self.MAX_NUM_SIMILAR_ARTISTS)
+        # Collect the names of the similar artists
+        similar_artist_names = []
+        for mbid in artist_recordings:
+            if mbid == self.artist_mbid:
+                continue
+
+            try:
+                similar_artist_names.append(artist_recordings[mbid][0].artist_credit.name)
+            except IndexError:
+                pass
+
+        # craft user feedback messages
+        if not artist_recordings:
+            msgs.append(f"The seed artist %s has no similar artists, nor top recordings. Too niche?" % self.artist_name)
+        else:
+            msg = "Using seed artist %s" % self.artist_name
+            if self.include_similar_artists:
+                if similar_artist_names:
+                    msg += " and similar artists: " + ", ".join(similar_artist_names)
+                else:
+                    msg += " only, since this artist has no similar artists (yet)."
+            else:
+                msg += " only"
+
+            msgs.insert(0, msg)
+
+        for msg in msgs:
+            self.local_storage["user_feedback"].append(msg)
+        self.data_cache["element-descriptions"].append("artist %s" % self.artist_name)
 
-        return artists
+        return interleave([artist_recordings[mbid] for mbid in artist_recordings])
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/cli.py` & `troi-2024.4.26.0/troi/content_resolver/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,91 +1,87 @@
 #!/usr/bin/env python3
-
-import os
-import sys 
+import logging
 import sys
 
 import click
 
-from troi.content_resolver.content_resolver import ContentResolver
+from troi.logging_utils import set_log_level
 from troi.content_resolver.database import Database
-from troi.content_resolver.model.recording import FileIdType
 from troi.content_resolver.subsonic import SubsonicDatabase
 from troi.content_resolver.metadata_lookup import MetadataLookup
 from troi.content_resolver.utils import ask_yes_no_question
 from troi.content_resolver.top_tags import TopTags
 from troi.content_resolver.duplicates import FindDuplicates
 from troi.content_resolver.playlist import write_m3u_playlist, write_jspf_playlist
 from troi.content_resolver.unresolved_recording import UnresolvedRecordingTracker
-from troi.playlist import PLAYLIST_TRACK_EXTENSION_URI
+
+logger = logging.getLogger(__name__)
 
 # TODO: Soon we will need a better configuration file, so we can get rid of this hack
 try:
     sys.path.insert(1, ".")
     import config
 except ImportError as err:
-    print(err)
     config = None
 
-
 DEFAULT_CHUNKSIZE = 100
 
 
 def output_playlist(db, playlist, upload_to_subsonic, save_to_m3u, save_to_jspf, dont_ask):
     try:
         recording = playlist.playlists[0].recordings[0]
     except (KeyError, IndexError):
-        print("Cannot save empty playlist.")
+        logger.error("Cannot save empty playlist.")
         return
 
     if upload_to_subsonic and config:
         if recording and config.SUBSONIC_HOST:
             try:
                 _ = recording.musicbrainz["subsonic_id"]
             except KeyError:
-                print("Playlist does not appear to contain subsonic ids. Can't upload to subsonic.")
+                logger.info("Playlist does not appear to contain subsonic ids. Can't upload to subsonic.")
                 return
 
             if dont_ask or ask_yes_no_question("Upload via subsonic? (Y/n)"):
-                print("uploading playlist")
+                logger.info("uploading playlist")
                 db.upload_playlist(playlist)
             return
 
     if save_to_m3u or save_to_jspf:
         try:
             _ = recording.musicbrainz["filename"]
         except KeyError:
-            print("Playlist does not appear to contain file paths. Can't write a local playlist.")
+            logger.error("Playlist does not appear to contain file paths. Can't write a local playlist.")
             return
 
     if save_to_m3u:
         if dont_ask or ask_yes_no_question(f"Save to '{save_to_m3u}'? (Y/n)"):
-            print("saving playlist")
+            logger.info("saving playlist")
             write_m3u_playlist(save_to_m3u, playlist)
         return
 
     if save_to_jspf:
         if dont_ask or ask_yes_no_question(f"Save to '{save_to_jspf}'? (Y/n)"):
-            print("saving playlist")
+            logger.info("saving playlist")
             write_jspf_playlist(save_to_jspf, playlist)
         return
 
-    print("Playlist displayed, but not saved. Use -j, -m or -u options to save/upload playlists.")
+    logger.info("Playlist displayed, but not saved. Use -j, -m or -u options to save/upload playlists.")
 
 
 def db_file_check(db_file):
     """ Check the db_file argument and give useful user feedback. """
 
     if not db_file:
         if not config:
-            print("Database file not specified with -d (--db_file) argument. Consider adding it to config.py for ease of use.")
+            logger.info("Database file not specified with -d (--db_file) argument. Consider adding it to config.py for ease of use.")
             sys.exit(-1)
 
         if not config.DATABASE_FILE:
-            print("config.py found, but DATABASE_FILE is empty. Please add it or use -d option to specify it.")
+            logger.info("config.py found, but DATABASE_FILE is empty. Please add it or use -d option to specify it.")
             sys.exit(-1)
 
         return config.DATABASE_FILE
     else:
         return db_file
 
 
@@ -101,111 +97,127 @@
 @click.group()
 def cli():
     pass
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
-def create(db_file):
+@click.option('--quiet', '-q', 'quiet', help="Do no print out anything", required=False, is_flag=True)
+def create(db_file, quiet):
     """Create a new database to track a music collection"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, quiet)
     db.create()
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.option('-c', '--chunksize', default=DEFAULT_CHUNKSIZE, help="Number of files to add/update at once")
 @click.option("-f", "--force", required=False, is_flag=True, default=False, help="Force scanning, ignoring any cache")
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
 @click.argument('music_dirs', nargs=-1, type=click.Path())
-def scan(db_file, music_dirs, chunksize=DEFAULT_CHUNKSIZE, force=False):
+def scan(db_file, music_dirs, quiet, chunksize=DEFAULT_CHUNKSIZE, force=False):
     """Scan one or more directories and their subdirectories for music files to add to the collection.
        If no path is passed, check for MUSIC_DIRECTORIES in config instead.
     """
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, quiet)
     db.open()
     if not music_dirs:
         music_dirs = music_directories_from_config()
     db.scan(music_dirs, chunksize=chunksize, force=force)
 
     # Remove any recordings from the unresolved recordings that may have just been added.
     urt = UnresolvedRecordingTracker()
     releases = urt.cleanup()
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.option("-r", "--remove", help="Without this flag, no files are removed.", required=False, is_flag=True, default=True)
-def cleanup(db_file, remove):
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
+def cleanup(db_file, remove, quiet):
     """Perform a database cleanup. Check that files exist and if they don't remove from the index"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, quiet)
     db.open()
     db.database_cleanup(remove)
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
-def metadata(db_file):
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
+def metadata(db_file, quiet):
     """Lookup metadata (popularity and tags) for recordings"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, quiet)
     db.open()
-    lookup = MetadataLookup()
+    lookup = MetadataLookup(quiet)
     lookup.lookup()
 
-    print("\nThese top tags describe your collection:")
+    logger.info("\nThese top tags describe your collection:")
     tt = TopTags()
     tt.print_top_tags_tightly(100)
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
-def subsonic(db_file):
+@click.option('-q', '--quiet', 'quiet', help="Do no print out anything", required=False, is_flag=True)
+def subsonic(db_file, quiet):
     """Scan a remote subsonic music collection"""
+    set_log_level(quiet)
     db_file = db_file_check(db_file)
-    db = SubsonicDatabase(db_file, config)
+    db = SubsonicDatabase(db_file, config, quiet)
     db.open()
     db.sync()
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 @click.argument('count', required=False, default=250)
 def top_tags(db_file, count):
     "Display the top most used tags in the music collection. Useful for writing LB Radio tag prompts"
+    set_log_level(False)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, False)
     db.open()
     tt = TopTags()
     tt.print_top_tags_tightly(count)
 
 
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
-@click.option('-e', '--exclude-different-release', help="Exclude duplicates that appear on different releases",
-                    required=False, default=False, is_flag=True)
+@click.option('-e',
+              '--exclude-different-release',
+              help="Exclude duplicates that appear on different releases",
+              required=False,
+              default=False,
+              is_flag=True)
 @click.option('-v', '--verbose', help="Display extra info about found files", required=False, default=False, is_flag=True)
 def duplicates(db_file, exclude_different_release, verbose):
     "Print all the tracks in the DB that are duplicated as per recording_mbid"
+    set_log_level(False)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, False)
     db.open()
     fd = FindDuplicates(db)
     fd.print_duplicate_recordings(exclude_different_release, verbose)
 
 
-
 @click.command()
 @click.option("-d", "--db_file", help="Database file for the local collection", required=False, is_flag=False)
 def unresolved(db_file):
     "Show the top unresolved releases"
+    set_log_level(False)
     db_file = db_file_check(db_file)
-    db = Database(db_file)
+    db = Database(db_file, False)
     db.open()
     urt = UnresolvedRecordingTracker()
     releases = urt.get_releases()
     urt.print_releases(releases)
 
 
 cli.add_command(create)
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/content_resolver.py` & `troi-2024.4.26.0/troi/content_resolver/content_resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-import os
-import datetime
-import sys
-from uuid import UUID
+import logging
 
-import peewee
-
-from troi.content_resolver.model.database import db, setup_db
 from troi.content_resolver.model.recording import Recording, FileIdType
 from troi.content_resolver.unresolved_recording import UnresolvedRecordingTracker
 from troi.content_resolver.fuzzy_index import FuzzyIndex
 from lb_matching_tools.cleaner import MetadataCleaner
-from troi.content_resolver.playlist import read_jspf_playlist
 from troi.content_resolver.utils import bcolors
-from troi.playlist import PlaylistElement
-from troi import Playlist
+
+logger = logging.getLogger(__name__)
 
 
 class ContentResolver:
     '''
     Scan a given path and enter/update the metadata in the search index
     '''
 
-    def __init__(self):
+    def __init__(self, quiet):
         self.fuzzy_index = None
+        self.quiet = quiet
 
     def get_artist_recording_metadata(self):
         """
             Fetch the metadata needed to build a fuzzy search index.
         """
 
         artist_recording_data = []
@@ -156,15 +150,15 @@
         # Check to make sure we have at least one recording
         try:
             _ = playlist.playlists[0].recordings[0]
         except (KeyError, IndexError):
             return playlist
 
         for rec in playlist.playlists[0].recordings:
-            artist_recording_data.append({"artist_name": rec.artist.name,
+            artist_recording_data.append({"artist_name": rec.artist_credit.name,
                                           "recording_name": rec.name,
                                           "recording_mbid": rec.mbid})
 
         # See what we can resolve using MBIDs
         artist_recording_data = self.resolve_recording_by_mbid(artist_recording_data)
 
         self.build_index()
@@ -179,23 +173,23 @@
             .select(Recording) \
             .where(Recording.id.in_(recording_ids)) \
             .dicts()
 
         # Build index based on recording.id
         rec_index = {r["id"]: r for r in local_recordings}
 
-        print("       %-40s %-40s %-40s" % ("RECORDING", "RELEASE", "ARTIST"))
+        logger.info("       %-40s %-40s %-40s" % ("RECORDING", "RELEASE", "ARTIST"))
         unresolved_recordings = []
         target_recordings = playlist.playlists[0].recordings
         resolved = 0
         failed = 0
         for i, artist_recording in enumerate(artist_recording_data):
             if i not in hit_index:
-                print(bcolors.FAIL + "FAIL " + bcolors.ENDC + "  %-40s %-40s %-40s" % (artist_recording["recording_name"][:39], "",
-                                                                                       artist_recording["artist_name"][:39]))
+                logger.info(bcolors.FAIL + "FAIL " + bcolors.ENDC + "  %-40s %-40s %-40s" % (artist_recording["recording_name"][:39], "",
+                                                                                           artist_recording["artist_name"][:39]))
                 unresolved_recordings.append(artist_recording["recording_mbid"])
                 failed += 1
                 continue
 
             hit = hit_index[i]
             local_recording = rec_index[hit["recording_id"]]   # type content resolver recording
             target = target_recordings[hit["index"]]           # troi recordings
@@ -203,21 +197,27 @@
             if local_recording["file_id_type"] == FileIdType.FILE_PATH:
                 target.musicbrainz["filename"] = local_recording["file_id"]
             if local_recording["file_id_type"] == FileIdType.SUBSONIC_ID:
                 target.musicbrainz["subsonic_id"] = local_recording["file_id"]
             if local_recording["duration"] is not None:
                 target.duration = local_recording["duration"]
 
-            print(bcolors.OKGREEN + ("%-5s" % hit["method"]) + bcolors.ENDC +
-                  "  %-40s %-40s %-40s" % (artist_recording["recording_name"][:39], "",
-                                           artist_recording["artist_name"][:39]))
-            print("       %-40s %-40s %-40s" % (local_recording["recording_name"][:39],
-                                                local_recording["release_name"][:39],
-                                                local_recording["artist_name"][:39]))
+            if not self.quiet:
+                logger.info(bcolors.OKGREEN + ("%-5s" % hit["method"]) + bcolors.ENDC +
+                            "  %-40s %-40s %-40s" % (artist_recording["recording_name"][:39], "",
+                                                     artist_recording["artist_name"][:39]))
+                logger.info("       %-40s %-40s %-40s" % (local_recording["recording_name"][:39],
+                                                          local_recording["release_name"][:39],
+                                                          local_recording["artist_name"][:39]))
             resolved += 1
 
+        ur = UnresolvedRecordingTracker()
+        ur.add(unresolved_recordings)
+
         if resolved == 0:
-            print("Sorry, but no tracks could be resolved, no playlist generated.")
+            logger.info("Sorry, but no tracks could be resolved, no playlist generated.")
             return []
 
-        print(f'\n{resolved} recordings resolved, {failed} not resolved.')
+        if not self.quiet:
+            logger.info(f'\n{resolved} recordings resolved, {failed} not resolved.')
+
         return playlist
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/database.py` & `troi-2024.4.26.0/troi/content_resolver/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+import logging
 from abc import abstractmethod
 from collections import namedtuple
 from enum import IntEnum
 import os
 import datetime
 from mutagen import MutagenError
 from pathlib import Path
 import sys
-from time import time
 from types import SimpleNamespace
 from uuid import UUID
 
-from unidecode import unidecode
 import peewee
 from tqdm import tqdm
 
 from troi.content_resolver.model.database import db, setup_db
 from troi.content_resolver.model.recording import Recording, RecordingMetadata, FileIdType
 from troi.content_resolver.model.unresolved_recording import UnresolvedRecording
 from troi.content_resolver.model.tag import Tag, RecordingTag
 from troi.content_resolver.model.directory import Directory
 from troi.content_resolver.formats import mp3, m4a, flac, ogg_opus, ogg_vorbis, wma
 
 from troi.content_resolver.utils import existing_dirs
 
+logger = logging.getLogger(__name__)
+
 SUPPORTED_FORMATS = (
     flac,
     m4a,
     mp3,
     ogg_opus,
     ogg_vorbis,
     wma,
@@ -93,18 +94,19 @@
 
 
 class Database:
     '''
     Keep a database with metadata for a collection of local music files.
     '''
 
-    def __init__(self, db_file):
+    def __init__(self, db_file, quiet):
         self.db_file = db_file
         self.fuzzy_index = None
         self.forced_scan = False
+        self.quiet = quiet
 
     def create(self):
         """
             Create the database. Can be run again to create tables that have been recently added to the code,
             but don't exist in the DB yet.
         """
         try:
@@ -117,63 +119,69 @@
                 RecordingMetadata,
                 Tag,
                 RecordingTag,
                 UnresolvedRecording,
                 Directory,
             ))
         except Exception as e:
-            print("Failed to create db file %r: %s" % (self.db_file, e))
+            logger.error("Failed to create db file %r: %s" % (self.db_file, e))
 
     def open(self):
         """
             Open the database file and connect to the db.
         """
         try:
             setup_db(self.db_file)
             db.connect()
         except peewee.OperationalError:
-            print("Cannot open database index file: '%s'" % self.db_file)
+            logger.error("Cannot open database index file: '%s'" % self.db_file)
             sys.exit(-1)
 
     def close(self):
         """ Close the db."""
         db.close()
 
     def scan(self, music_dirs, chunksize=100, force=False):
         """
             Scan music directories and add tracks to sqlite.
         """
         if not music_dirs:
-            print("No directory to scan")
+            logger.error("No directory to scan")
             return
 
         self.forced_scan = force
 
         self.music_dirs = tuple(sorted(set(existing_dirs(music_dirs))))
         if not self.music_dirs:
-            print("No valid directories to scan")
+            logger.error("No valid directories to scan")
             return
 
         self.chunksize = chunksize
 
         # Keep some stats
         self.counters = ScanCounters()
         self.skip_dirs = set()
 
-        print("Check collection size...")
-        print("Counting candidates in %s ..." % ", ".join(self.music_dirs))
+        if not self.quiet:
+            logger.info("Check collection size...")
+            logger.info("Counting candidates in %s ..." % ", ".join(self.music_dirs))
         self.traverse(dry_run=True)
-        print(self.counters.dry_run_stats())
+        if not self.quiet:
+            logger.info(self.counters.dry_run_stats())
 
-        with tqdm(total=self.counters.audio_files) as self.progress_bar:
-            print("Scanning ...")
+        if not self.quiet:
+            with tqdm(total=self.counters.audio_files) as self.progress_bar:
+                logger.info("Scanning ...")
+                self.traverse()
+        else:
             self.traverse()
 
         self.close()
-        print(self.counters.stats())
+        if not self.quiet:
+            logger.info(self.counters.stats())
 
     def traverse(self, dry_run=False):
         """
             This function searches for audio files and descends into sub directories
         """
         seen = set()
         changed_dirs = []
@@ -233,15 +241,15 @@
         try:
             stats = os.stat(dir_path)
             mtime = datetime.datetime.fromtimestamp(stats[8])
             directory = Directory.get_or_none(Directory.dir_path == dir_path)
             if directory is None or directory.mtime != mtime:
                 return mtime
         except Exception as e:
-            print("Can't stat dir %r: %s" % (dir_path, e))
+            logger.error("Can't stat dir %r: %s" % (dir_path, e))
         return False
 
     def read_metadata(self, file_path, mtime):
         """
             Read metadata from audio file
             On error, returns None, error msg
             On success, returns metadata dict, StatusDetails
@@ -341,25 +349,27 @@
         return s
 
     def update_status(self, statusdata):
         """
             Update status counter and display matching progress
         """
         self.counters.status[statusdata.status] += 1
-        self.progress_bar.write(self.fmtdetails(statusdata))
+        if not self.quiet:
+            self.progress_bar.write(self.fmtdetails(statusdata))
 
     def add(self, file_path, audio_file_count):
         """
             Given a file, check to see if we already have it and if we do,
             if it has changed since the last time we read it. If it is new
             or has been changed, update in the DB.
         """
 
         # update the progress bar
-        self.progress_bar.update(1)
+        if not self.quiet:
+            self.progress_bar.update(1)
 
         self.counters.total += 1
 
         # Check to see if the file in question has changed since the last time
         # we looked at it.
         try:
             stats = os.stat(file_path)
@@ -415,56 +425,55 @@
             PathId(r.file_id, r.id)
             for r in Recording.select(Recording.file_id, Recording.id).where(Recording.file_id_type == FileIdType.FILE_PATH)
             if not os.path.isfile(r.file_id))
         directories = tuple(
             PathId(d.dir_path, d.id) for d in Directory.select(Directory.dir_path, Directory.id) if not os.path.isdir(d.dir_path))
 
         if not recordings and not directories:
-            print("No cleanup needed.")
+            logger.error("No cleanup needed.")
             return
 
         for elem in sorted(recordings + directories):
-            print("RM %s" % elem.path)
+            logger.info("RM %s" % elem.path)
 
-        print("%d recordings and %d directory entries to remove from database" % (len(recordings), len(directories)))
+        logger.info("%d recordings and %d directory entries to remove from database" % (len(recordings), len(directories)))
         if not dry_run:
             with db.atomic():
                 ids = tuple(r.id for r in recordings)
                 query = Recording.delete().where(Recording.id.in_(ids))
                 count = query.execute()
-                print("%d recordings removed" % count)
+                logger.info("%d recordings removed" % count)
                 ids = tuple(d.id for d in directories)
                 query = Directory.delete().where(Directory.id.in_(ids))
                 count = query.execute()
-                print("%d directory entries removed" % count)
-            print("Vacuuming database...")
+                logger.info("%d directory entries removed" % count)
+            logger.info("Vacuuming database...")
             db.execute_sql('VACUUM')
-            print("Done.")
+            logger.info("Done.")
         else:
-            print("Use command cleanup --remove to actually remove those.")
+            logger.info("Use command cleanup --remove to actually remove those.")
 
     def metadata_sanity_check(self, include_subsonic=False):
         """
         Run a sanity check on the DB to see if data is missing that is required for LB Radio to work.
         """
 
         num_recordings = db.execute_sql("SELECT COUNT(*) FROM recording").fetchone()[0]
         num_metadata = db.execute_sql("SELECT COUNT(*) FROM recording_metadata").fetchone()[0]
         num_file_path = Recording.select(peewee.fn.Count(
             Recording.file_id_type).alias('count')).where(Recording.file_id_type == FileIdType.FILE_PATH)[0].count
         num_subsonic = Recording.select(peewee.fn.Count(
             Recording.file_id_type).alias('count')).where(Recording.file_id_type == FileIdType.SUBSONIC_ID)[0].count
 
         if num_metadata == 0:
-            print("sanity check: You have not downloaded metadata for your collection. Run the metadata command.")
+            logger.info("sanity check: You have not downloaded metadata for your collection. Run the metadata command.")
         elif num_metadata < num_recordings // 2:
-            print("sanity check: Only %d of your %d recordings have metadata information available. Run the metdata command." %
-                  (num_metadata, num_recordings))
+            logger.info("sanity check: Only %d of your %d recordings have metadata information available."
+                        " Run the metdata command." % (num_metadata, num_recordings))
 
         if include_subsonic:
             if num_subsonic == 0 and include_subsonic:
-                print(
-                    "sanity check: You have not matched your collection against the collection in subsonic. Run the subsonic command."
-                )
+                logger.info("sanity check: You have not matched your collection against the collection in subsonic."
+                            " Run the subsonic command.")
             elif num_subsonic < num_recordings // 2:
-                print("sanity check: Only %d of your %d recordings have subsonic matches. Run the subsonic command." %
-                      (num_subsonic, num_recordings))
+                logger.info("sanity check: Only %d of your %d recordings have subsonic matches."
+                            " Run the subsonic command." % (num_subsonic, num_recordings))
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/duplicates.py` & `troi-2024.4.26.0/troi/content_resolver/duplicates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,16 @@
+import logging
 import os
 import json
-from collections import defaultdict
-import datetime
 import hashlib
 import mutagen
-import sys
-
-import peewee
-import requests
 
 from troi.content_resolver.model.database import db
-from troi.content_resolver.model.recording import Recording, RecordingMetadata
-from troi.recording_search_service import RecordingSearchByTagService
-from troi.splitter import plist
+
+logger = logging.getLogger(__name__)
 
 
 class FindDuplicates:
     '''
        Class to fetch recordings that are duplicate in the database.
     '''
 
@@ -69,24 +63,24 @@
         total = 0
         recordings_count = 0
 
         def indent(n, s=''):
             return ' ' * (4 * n) + str(s)
 
         def print_error(e):
-            print(indent(2, "error: %s" % e))
+            logger.info(indent(2, "error: %s" % e))
 
         def print_info(title, content):
-            print(indent(2, "%s: %s" % (title, content)))
+            logger.info(indent(2, "%s: %s" % (title, content)))
 
         for dup in self.get_duplicate_recordings(include_different_releases):
             recordings_count += 1
-            print("%d duplicates of '%s' by '%s'" % (dup[5], dup[0], dup[2]))
+            logger.info("%d duplicates of '%s' by '%s'" % (dup[5], dup[0], dup[2]))
             for file_id in dup[4]:
-                print(indent(1, file_id))
+                logger.info(indent(1, file_id))
                 if verbose:
                     error = False
                     try:
                         file_stats = os.stat(file_id)
                         print_info("size", "%d bytes" % file_stats.st_size)
                     except Exception as e:
                         print_error(e)
@@ -103,12 +97,11 @@
                         try:
                             mf = mutagen.File(file_id)
                             print_info("format", mf.info.pprint())
                         except mutagen.MutagenError as e:
                             print_error(e)
 
                 total += 1
-            print()
+            logger.info("")
 
-        print()
-        print("%d recordings had a total of %d duplicates." %
-              (recordings_count, total))
+        logger.info("")
+        logger.info("%d recordings had a total of %d duplicates." % (recordings_count, total))
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/flac.py` & `troi-2024.4.26.0/troi/content_resolver/formats/flac.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mutagen
 import mutagen.flac
 
 from troi.content_resolver.formats.tag_utils import get_tag_value, extract_track_number
 
 
 EXTENSIONS = {'.flac'}
 READER = mutagen.flac.FLAC
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/m4a.py` & `troi-2024.4.26.0/troi/content_resolver/formats/m4a.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mutagen
 import mutagen.mp4
 
 from troi.content_resolver.formats.tag_utils import get_tag_value, extract_track_number
 
 
 EXTENSIONS = {'.m4a', '.m4b', '.m4p', '.m4v', '.m4r', '.mp4'}
 READER = mutagen.mp4.MP4
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/mp3.py` & `troi-2024.4.26.0/troi/content_resolver/formats/mp3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mutagen
 import mutagen.mp3
 
 from troi.content_resolver.formats.tag_utils import get_tag_value, extract_track_number
 
 
 EXTENSIONS = {'.mp3', '.mp2', '.m2a'}
 READER = mutagen.mp3.MP3
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/ogg_opus.py` & `troi-2024.4.26.0/troi/content_resolver/formats/ogg_opus.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/ogg_vorbis.py` & `troi-2024.4.26.0/troi/content_resolver/formats/ogg_vorbis.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mutagen
 import mutagen.oggvorbis
 
 from troi.content_resolver.formats.tag_utils import get_tag_value, extract_track_number
 
 
 EXTENSIONS = {'.ogg'}
 READER = mutagen.oggvorbis.OggVorbis
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/tag_utils.py` & `troi-2024.4.26.0/troi/content_resolver/formats/tag_utils.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/formats/wma.py` & `troi-2024.4.26.0/troi/content_resolver/formats/wma.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import mutagen
 import mutagen.asf
 
 from troi.content_resolver.formats.tag_utils import get_tag_value, extract_track_number
 
 
 EXTENSIONS = {'.wma'}
 READER = mutagen.asf.ASF
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/fuzzy_index.py` & `troi-2024.4.26.0/troi/content_resolver/fuzzy_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import os
 import datetime
+import logging
 from math import fabs
 from time import time
 import re
 import sys
 
 from sklearn.feature_extraction.text import TfidfVectorizer
 from unidecode import unidecode
 
 try:
     import nmslib
     have_nmslib = True
 except ImportError:
     have_nmslib = False
 
+logger = logging.getLogger(__name__)
 
 def ngrams(string, n=3):
     """ Take a lookup string (noise removed, lower case, etc) and turn into a list of trigrams """
 
     string = ' ' + string + ' '  # pad names for ngrams...
     ngrams = zip(*[string[i:] for i in range(n)])
     return [''.join(ngram) for ngram in ngrams]
@@ -67,14 +69,15 @@
         self.index.createIndex()
 
     def search(self, query_data):
         """
             Return IDs for the matches in a list. Returns a list of dicts with keys of lookup_string, confidence and recording_id.
         """
         if not self.have_nmslib:
+            logger.warn("nmslib not installed and trying fuzzy search, but nothing will match. Install nmslib!")
             return []
 
         query_strings = []
         for data in query_data:
             if data["artist_name"] is None or data["recording_name"] is None:
                 continue
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/lb_radio.py` & `troi-2024.4.26.0/troi/content_resolver/lb_radio.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import datetime
-import os
+import logging
 
 from troi import Playlist
 from troi.playlist import PlaylistElement
-from troi.patches.lb_radio_classes.tag import LBRadioTagRecordingElement
 from troi.patches.lb_radio import LBRadioPatch
-from troi.splitter import plist
 
 from troi.content_resolver.tag_search import LocalRecordingSearchByTagService
 from troi.content_resolver.artist_search import LocalRecordingSearchByArtistService
-from troi.content_resolver.model.database import db
-from troi.content_resolver.model.recording import FileIdType
 from troi.content_resolver.content_resolver import ContentResolver
 
+logger = logging.getLogger(__name__)
+
 
 class ListenBrainzRadioLocal:
     '''
        Generate local playlists against a music collection available via subsonic.
     '''
 
+    def __init__(self, quiet):
+        self.quiet = quiet
+
     def generate(self, mode, prompt, match_threshold):
         """
            Generate a playlist given the mode and prompt. Optional match_threshold, a value from
            0 to 1.0 allows the use to control how well local resolution tracks must match before
            being considered a match.
 
            Returns a troi playlist object.
         """
 
-        patch = LBRadioPatch({"mode": mode, "prompt": prompt, "echo": True, "debug": True, "min_recordings": 1})
+        patch = LBRadioPatch({"mode": mode, "prompt": prompt, "quiet": self.quiet, "min_recordings": 1})
         patch.register_service(LocalRecordingSearchByTagService())
         patch.register_service(LocalRecordingSearchByArtistService())
 
         # Now generate the playlist
         try:
             playlist = patch.generate_playlist()
         except RuntimeError as err:
-            print(f"LB Radio generation failed: {err}")
+            logger.info(f"LB Radio generation failed: {err}")
             return None
 
-        if playlist == None:
+        if playlist is None:
             return playlist
 
         # Resolve any tracks that have not been resolved to a subsonic_id or a local file
         self.resolve_playlist(match_threshold, playlist)
 
         return playlist
 
@@ -58,15 +58,15 @@
 
             recordings.append(recording)
 
         if not recordings:
             return
 
         # Use the content resolver to resolve the recordings in situ
-        cr = ContentResolver()
+        cr = ContentResolver(self.quiet)
         pe = PlaylistElement()
         pe.playlists = [ Playlist(recordings=recordings) ]
         cr.resolve_playlist(match_threshold, pe)
 
         # Now filter out the tracks that were not matched
         filtered = []
         for rec in playlist.playlists[0].recordings:
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/metadata_lookup.py` & `troi-2024.4.26.0/troi/content_resolver/metadata_lookup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-import os
+import logging
 from collections import defaultdict, namedtuple
 import datetime
-import sys
 
-import peewee
 import requests
 from tqdm import tqdm
 
 from troi.content_resolver.model.database import db
 from troi.content_resolver.model.recording import Recording, RecordingMetadata
 from troi.content_resolver.model.tag import RecordingTag
 
+logger = logging.getLogger(__name__)
+
 
 RecordingRow = namedtuple('RecordingRow', ('id', 'mbid', 'metadata_id'))
 
 
 class MetadataLookup:
     '''
     Given the local database, lookup metadata from MusicBrainz to allow local playlist resolution.
     '''
 
     BATCH_SIZE = 1000
 
+    def __init__(self, quiet):
+        self.quiet = quiet
+
     def lookup(self):
         """
         Iterate over all recordings in the database and call lookup_chunk for chunks of recordings.
         """
 
         cursor = db.execute_sql("""SELECT recording.id, recording.recording_mbid, recording_metadata.id
                                      FROM recording
@@ -34,18 +37,24 @@
                                     WHERE recording_mbid IS NOT NULL
                                  ORDER BY artist_name, release_name""")
         recordings = tuple(
             RecordingRow(id=row[0], mbid=str(row[1]), metadata_id=row[2])
             for row in cursor.fetchall()
         )
 
-        print("[ %d recordings to lookup ]" % len(recordings))
+        logger.info("[ %d recordings to lookup ]" % len(recordings))
 
         offset = 0
-        with tqdm(total=len(recordings)) as self.pbar:
+
+        if not self.quiet:
+            with tqdm(total=len(recordings)) as self.pbar:
+                while offset <= len(recordings):
+                    self.process_recordings(recordings[offset:offset+self.BATCH_SIZE])
+                    offset += self.BATCH_SIZE
+        else:
             while offset <= len(recordings):
                 self.process_recordings(recordings[offset:offset+self.BATCH_SIZE])
                 offset += self.BATCH_SIZE
 
     def process_recordings(self, recordings):
         """
             This function carries out the actual lookup of the metadata and inserting the
@@ -54,29 +63,37 @@
 
         args = []
         mbid_to_recording = {}
         for rec in recordings:
             mbid_to_recording[rec.mbid] = rec
             args.append({"[recording_mbid]": rec.mbid})
 
-        r = requests.post("https://labs.api.listenbrainz.org/bulk-tag-lookup/json", json=args)
-        if r.status_code != 200:
-            print("Fail: %d %s" % (r.status_code, r.text))
-            return False
+        while True:
+            r = requests.post("https://labs.api.listenbrainz.org/bulk-tag-lookup/json", json=args)
+            if r.status_code == 429:
+                sleep(2)
+                continue
+
+            if r.status_code != 200:
+                logger.info("Fail: %d %s" % (r.status_code, r.text))
+                return False
+
+            break
 
         recording_pop = {}
         recording_tags = defaultdict(lambda: defaultdict(list))
         tags = set()
         for row in r.json():
             mbid = str(row["recording_mbid"])
             recording_pop[mbid] = row["percent"]
             recording_tags[mbid][row["source"]].append(row["tag"])
             tags.add(row["tag"])
 
-        self.pbar.update(len(recordings))
+        if not self.quiet:
+            self.pbar.update(len(recordings))
 
         with db.atomic():
 
             # This DB code is pretty messy -- things I take for granted with Postgres are not
             # available in SQLite or the PeeWee ORM. But, this might be ok, since we're not
             # updating millions of rows constantly.
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/model/recording.py` & `troi-2024.4.26.0/troi/content_resolver/model/recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/model/tag.py` & `troi-2024.4.26.0/troi/content_resolver/model/tag.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/model/unresolved_recording.py` & `troi-2024.4.26.0/troi/content_resolver/model/unresolved_recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/playlist.py` & `troi-2024.4.26.0/troi/content_resolver/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/py_sonic_fix.py` & `troi-2024.4.26.0/troi/content_resolver/py_sonic_fix.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/content_resolver/subsonic.py` & `troi-2024.4.26.0/troi/content_resolver/subsonic.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import datetime
-import os
-import sys
-from uuid import UUID
+import logging
 
 import peewee
 from tqdm import tqdm
 
 from troi.content_resolver.database import Database
 from troi.content_resolver.model.database import db
 from troi.content_resolver.model.recording import Recording, FileIdType
 from troi.content_resolver.utils import bcolors
 from troi.content_resolver.py_sonic_fix import FixedConnection
 
+logger = logging.getLogger(__name__)
+
 
 class SubsonicDatabase(Database):
     '''
     Add subsonic sync capabilities to the Database
     '''
 
     # Determined by the number of albums we can fetch in one go
     BATCH_SIZE = 500
 
-    def __init__(self, index_dir, config):
+    def __init__(self, index_dir, config, quiet):
         self.config = config
-        Database.__init__(self, index_dir)
+        Database.__init__(self, index_dir, quiet)
+        self.quiet = quiet
 
     def sync(self):
         """
             Scan the subsonic client specified in config.py
         """
 
         # Keep some stats
         self.total = 0
         self.matched = 0
         self.error = 0
 
         self.run_sync()
-
-        print("Checked %s albums:" % self.total)
-        print("  %5d albums matched" % self.matched)
-        print("  %5d recordings with errors" % self.error)
+        
+        logger.info("Checked %s albums:" % self.total)
+        logger.info("  %5d albums matched" % self.matched)
+        logger.info("  %5d recordings with errors" % self.error)
 
     def connect(self):
         if not self.config:
-            print("Missing credentials to connect to subsonic")
+            logger.error("Missing credentials to connect to subsonic")
             return None
 
-        print("[ connect to subsonic ]")
+        logger.info("[ connect to subsonic ]")
 
         return FixedConnection(
             self.config.SUBSONIC_HOST,
             self.config.SUBSONIC_USER,
             self.config.SUBSONIC_PASSWORD,
             self.config.SUBSONIC_PORT,
         )
@@ -62,31 +63,32 @@
 
         conn = self.connect()
         if not conn:
             return
 
         cursor = db.connection().cursor()
 
-        print("[ load albums ]")
+        logger.info("[ load albums ]")
         album_ids = set()
         albums = []
         offset = 0
         while True:
             results = conn.getAlbumList2(ltype="alphabeticalByArtist", size=self.BATCH_SIZE, offset=offset)
             albums.extend(results["albumList2"]["album"])
             album_ids.update([r["id"] for r in results["albumList2"]["album"]])
 
             album_count = len(results["albumList2"]["album"])
             offset += album_count
             if album_count < self.BATCH_SIZE:
                 break
 
-        print("[ loaded %d albums ]" % len(album_ids))
+        logger.info("[ loaded %d albums ]" % len(album_ids))
 
-        pbar = tqdm(total=len(album_ids))
+        if not self.quiet:
+            pbar = tqdm(total=len(album_ids))
         recordings = []
 
         # cross reference subsonic artist id to artitst_mbid
         artist_id_index = {}
 
         for album in albums:
             album_info = conn.getAlbum(id=album["id"])
@@ -94,16 +96,17 @@
             # Some servers might already include the MBID in the list or album response
             album_mbid = album_info.get("musicBrainzId", album.get("musicBrainzId"))
             if not album_mbid:
                 album_info2 = conn.getAlbumInfo2(aid=album["id"])
                 try:
                     album_mbid = album_info2["albumInfo"]["musicBrainzId"]
                 except KeyError:
-                    pbar.write(bcolors.FAIL + "FAIL " + bcolors.ENDC + "subsonic album '%s' by '%s' has no MBID" %
-                               (album["name"], album["artist"]))
+                    if not self.quiet:
+                        pbar.write(bcolors.FAIL + "FAIL " + bcolors.ENDC + "subsonic album '%s' by '%s' has no MBID" %
+                                   (album["name"], album["artist"]))
                     self.error += 1
                     continue
 
 
             recordings = []
             for song in album_info["album"]["song"]:
                 album = album_info["album"]
@@ -114,43 +117,42 @@
                     artist_id = album["artistId"]
 
                 if artist_id not in artist_id_index:
                     artist = conn.getArtistInfo2(artist_id)
                     try:
                         artist_id_index[artist_id] = artist["artistInfo2"]["musicBrainzId"]
                     except KeyError:
-                        pbar.write(bcolors.FAIL + "FAIL " + bcolors.ENDC + "recording '%s' by '%s' has no artist MBID" %
-                                (album["name"], album["artist"]))
-                        pbar.write("Consider retagging this file with Picard! ( https://picard.musicbrainz.org )")
+                        if not self.quiet:
+                            pbar.write(bcolors.FAIL + "FAIL " + bcolors.ENDC + "recording '%s' by '%s' has no artist MBID" %
+                                    (album["name"], album["artist"]))
+                            pbar.write("Consider retagging this file with Picard! ( https://picard.musicbrainz.org )")
                         self.error += 1
                         continue
 
-#                if "musicBrainzId" not in song:
-#                    song_details = conn.getSong(song["id"])
-#                    ic(song_details)
-
                 self.add_subsonic({
                     "artist_name": song["artist"],
                     "release_name": song["album"],
                     "recording_name": song["title"],
                     "artist_mbid": artist_id_index[artist_id],
                     "release_mbid": album_mbid,
                     "recording_mbid": song["musicBrainzId"],
                     "duration": song["duration"] * 1000,
                     "track_num": song["track"],
                     "disc_num": song["discNumber"],
                     "subsonic_id": song["id"],
                     "mtime": datetime.datetime.now()
                     })
 
-            pbar.write(bcolors.OKGREEN + "OK   " + bcolors.ENDC + "album %-50s %-50s" %
-                       (album["name"][:49], album["artist"][:49]))
+            if not self.quiet:
+                pbar.write(bcolors.OKGREEN + "OK   " + bcolors.ENDC + "album %-50s %-50s" %
+                           (album["name"][:49], album["artist"][:49]))
             self.matched += 1
             self.total += 1
-            pbar.update(1)
+            if not self.quiet:
+                pbar.update(1)
 
         if len(recordings) >= self.BATCH_SIZE:
             self.update_recordings(recordings)
 
     def add_subsonic(self, mdata):
         """ 
             Given recording metadata, add it to the database or update it if it already exists
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/tag_search.py` & `troi-2024.4.26.0/troi/content_resolver/tag_search.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 import peewee
 import requests
 
 from troi.content_resolver.model.database import db
 from troi.content_resolver.model.recording import Recording, RecordingMetadata
 from troi.content_resolver.utils import select_recordings_on_popularity
 from troi.recording_search_service import RecordingSearchByTagService
-from troi.splitter import plist
+from troi.plist import plist
 
 
 class LocalRecordingSearchByTagService(RecordingSearchByTagService):
     '''
     Given the local database, search for recordings that meet given tag criteria
     '''
 
     def __init__(self):
         RecordingSearchByTagService.__init__(self)
 
-    def search(self, tags, operator, begin_percent, end_percent, num_recordings):
+    def search(self, tags, operator, pop_begin, pop_end, num_recordings):
         """
         Perform a tag search. Parameters:
 
         tags - a list of string tags to search for
         operator - a string specifying "or" or "and"
-        begin_percent - if many recordings match the above parameters, return only
+        pop_begin - if many recordings match the above parameters, return only
                         recordings that have a minimum popularity percent score
-                        of begin_percent.
-        end_percent - if many recordings match the above parameters, return only
+                        of pop_begin.
+        pop_end - if many recordings match the above parameters, return only
                       recordings that have a maximum popularity percent score
-                      of end_percent.
+                      of pop_end.
 
-        If only few recordings match, the begin_percent and end_percent are
+        If only few recordings match, the pop_begin and pop_end are
         ignored.
         """
 
         # Search for all recordings that match the given tags with given operator
         if operator == "or":
             query, params, pop_clause = self.or_search(tags)
         else:
@@ -47,15 +47,15 @@
         placeholders = ",".join(("?", ) * len(tags))
         cursor = db.execute_sql(query % (placeholders, pop_clause), params)
 
         recordings = []
         for rec in cursor.fetchall():
             recordings.append({"recording_mbid": rec[0], "popularity": rec[1], "file_id": rec[2], "file_id_type": rec[3]})
 
-        return select_recordings_on_popularity(recordings, begin_percent, end_percent, num_recordings)
+        return select_recordings_on_popularity(recordings, pop_begin, pop_end, num_recordings)
 
     def or_search(self, tags, min_popularity=None, max_popularity=None):
         """
             Return the sql query that finds recordings using the OR operator
         """
 
         query = """WITH recording_ids AS (
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/top_tags.py` & `troi-2024.4.26.0/troi/content_resolver/top_tags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-import os
-from collections import defaultdict
-import datetime
-import sys
-
-import peewee
-import requests
+import logging
 
 from troi.content_resolver.model.database import db
-from troi.content_resolver.model.recording import Recording, RecordingMetadata
-from troi.recording_search_service import RecordingSearchByTagService
-from troi.splitter import plist
+
+logger = logging.getLogger(__name__)
 
 
 class TopTags:
     '''
        Class to fetch top tags
     '''
 
@@ -40,15 +33,15 @@
 
         return top_tags
 
     def print_top_tags(self, limit=50):
 
         top_tags = self.get_top_tags(limit)
         for tt in top_tags:
-            print("%-40s %d" % (tt["tag"], tt["count"]))
-        print()
+            logger.info("%-40s %d" % (tt["tag"], tt["count"]))
+        logger.info("")
 
     def print_top_tags_tightly(self, limit=250):
 
         top_tags = self.get_top_tags(limit)
 
-        print("; ".join(["%s %s" % (tt["tag"], tt["count"]) for tt in top_tags]))
+        logger.info("; ".join(["%s %s" % (tt["tag"], tt["count"]) for tt in top_tags]))
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/unresolved_recording.py` & `troi-2024.4.26.0/troi/content_resolver/unresolved_recording.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from collections import defaultdict
 import datetime
-from math import ceil
+import logging
+from collections import defaultdict
 from operator import itemgetter
-import requests
+from time import sleep
 
-import peewee
+import requests
 
 from troi.content_resolver.model.database import db
-from troi.content_resolver.model.unresolved_recording import UnresolvedRecording
+
+logger = logging.getLogger(__name__)
 
 
 class UnresolvedRecordingTracker:
     '''
         This class keeps track of recordings that were not resolved when
         a playlist was resolved. This will allow us to give recommendations
         on which albums to add to their collection to resolve more recordings.
@@ -96,15 +97,15 @@
         for chunk in self.chunks(recording_mbids, self.LOOKUP_BATCH_SIZE):
             args = ",".join(chunk)
 
             params = {"recording_mbids": args, "inc": "artist release"}
             while True:
                 r = requests.get("https://api.listenbrainz.org/1/metadata/recording", params=params)
                 if r.status_code != 200:
-                    print("Failed to fetch metadata for recordings: ", r.text)
+                    logger.info("Failed to fetch metadata for recordings: ", r.text)
                     return []
 
                 if r.status_code == 429:
                     sleep(1)
                     continue
 
                 break
@@ -137,20 +138,20 @@
             })
 
         return self.multisort(release_list, (("lookup_count", True), ("artist_name", False), ("release_name", False)))
 
     def print_releases(self, releases):
         """ Neatly print all the release/recordings returned from the get_releases function """
 
-        print("%-60s %-50s" % ("RELEASE", "ARTIST"))
+        logger.info("%-60s %-50s" % ("RELEASE", "ARTIST"))
         for release in releases:
-            print("%-60s %-50s" % (release["release_name"][:59], release["artist_name"][:49]))
+            logger.info("%-60s %-50s" % (release["release_name"][:59], release["artist_name"][:49]))
             for rec in release["recordings"]:
-                print("   %-57s %d lookups" % (rec["recording_name"][:56], rec["lookup_count"]))
-            print()
+                logger.info("   %-57s %d lookups" % (rec["recording_name"][:56], rec["lookup_count"]))
+            logger.info("")
 
     def cleanup(self):
         """
             Check the local collection and remove any recordings from unresolved recordings that have
             been added to the DB.
         """
```

### Comparing `troi-2024.2.9.0/troi/content_resolver/utils.py` & `troi-2024.4.26.0/troi/content_resolver/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,64 +1,67 @@
+import logging
 import os
 
-from troi.splitter import plist
+from troi.plist import plist
 from troi import Recording as TroiRecording
 from troi.content_resolver.model.recording import FileIdType
 
+logger = logging.getLogger(__name__)
+
 
 def ask_yes_no_question(prompt):
 
     while True:
         resp = input(prompt)
         resp = resp.strip()
         if resp == "":
             resp = 'y'
 
         if resp == 'y':
             return True
         elif resp == 'n':
             return False
         else:
-            print("eh? try again.")
+            logging.info("eh? try again.")
 
 
-def select_recordings_on_popularity(recordings, begin_percent, end_percent, num_recordings):
+def select_recordings_on_popularity(recordings, pop_begin, pop_end, num_recordings):
     """
        Given dicts of recording data, select up to num_recordings recordings randomly
-       from the recordings that ideally lie in popularity between begin_percent and end_percent.
+       from the recordings that ideally lie in popularity between pop_begin and pop_end.
 
        If too little data is found in the percent range, select recordings that are the closest
        to the disired range.
     """
 
     matching_recordings = []
     over_recordings = []
     under_recordings = []
     for rec in recordings:
-        if rec["popularity"] >= begin_percent:
-            if rec["popularity"] < end_percent:
+        if rec["popularity"] >= pop_begin:
+            if rec["popularity"] < pop_end:
                 matching_recordings.append(rec)
             else:
                 over_recordings.append(rec)
         else:
             under_recordings.append(rec)
 
     # If we have enough recordings, skip the extending part
     if len(matching_recordings) < num_recordings:
         # We don't have enough recordings, see if we can pick the ones outside
         # of our desired range in a best effort to make a playlist.
         # Keep adding the best matches until we (hopefully) get our desired number of recordings
         while len(matching_recordings) < num_recordings:
             if under_recordings:
-                under_diff = begin_percent - under_recordings[-1]["popularity"]
+                under_diff = pop_begin - under_recordings[-1]["popularity"]
             else:
                 under_diff = None
 
             if over_recordings:
-                over_diff = over_recordings[-1]["popularity"] - end_percent
+                over_diff = over_recordings[-1]["popularity"] - pop_end
             else:
                 over_diff = None
 
             if over_diff == None and under_diff == None:
                 break
 
             if over_diff is not None and under_diff is not None and under_diff < over_diff:
```

### Comparing `troi-2024.2.9.0/troi/core.py` & `troi-2024.4.26.0/troi/core.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 #!/usr/bin/env python3
+import logging
 import sys
-from typing import Dict
 
 import click
 
 import troi
 import troi.playlist
 import troi.utils
-from troi.patch import Patch
 
 
+logger = logging.getLogger(__name__)
+
 
 def list_patches():
     """
         Print a list of all available patches
     """
     patches = troi.utils.discover_patches()
 
-    print("Available patches:")
+    logger.info("Available patches:")
     size = max([len(k) for k in patches])
     for slug in sorted(patches or []):
-        print("%s:%s %s" % (slug, " " * (size - len(slug)), patches[slug]().description()))
+        patch = patches[slug]
+        print("%s:%s %s" % (slug, " " * (size - len(slug)), patch.description()))
 
 
 def patch_info(patch):
     """
         Get info for a given patch
 
         :param patch: the patch to get info for.
     """
 
     patches = troi.utils.discover_patches()
     if patch not in patches:
-        print("Cannot load patch '%s'. Use the list command to get a list of available patches." % patch, file=sys.stderr)
+        logger.error("Cannot load patch '%s'. Use the list command to get a list of available patches." % patch)
         sys.exit(1)
 
     apatch = patches[patch]
     cmd = convert_patch_to_command(apatch)
     context = click.Context(cmd, info_name=patch)
     click.echo(cmd.get_help(context))
```

### Comparing `troi-2024.2.9.0/troi/filters.py` & `troi-2024.4.26.0/troi/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,22 @@
             try:
                 ac_index[ac] = 1
             except KeyError:
                 raise PipelineError(self.__name__ + " needs to have all input recordings to have artist.artist_credit_id defined!")
 
         results = []
         for r in recordings:
-            if not r.artist or not r.artist.artist_credit_id:
-                self.debug("recording %s has not artist credit id" % (r.mbid))
+            if not r.artist_credit or not r.artist_credit.artist_credit_id:
                 continue
 
             if self.include:
-                if r.artist.artist_credit_id in ac_index:
+                if r.artist_credit.artist_credit_id in ac_index:
                     results.append(r)
             else:
-                if r.artist.artist_credit_id not in ac_index:
+                if r.artist_credit.artist_credit_id not in ac_index:
                     results.append(r)
 
         return results
 
 
 class ArtistCreditLimiterElement(troi.Element):
     '''
@@ -93,15 +92,15 @@
             Carry out the actual artist limiting.
         """
 
         ac_index = defaultdict(list)
         all_have_rankings = True
         for rec in recordings:
             try:
-                ac_index[rec.artist.artist_credit_id].append((rec.mbid, rec.ranking))
+                ac_index[rec.artist_credit.artist_credit_id].append((rec.mbid, rec.ranking))
                 if rec.ranking is None:
                     all_have_rankings = False
             except KeyError:
                 raise PipelineError(self.__name__ + " needs to have all input recordings to have artist.artist_credit_id defined!")
 
         for key in ac_index:
             if all_have_rankings:
@@ -153,15 +152,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
         recordings = inputs[0]
         output = []
         seen = set()
         for rec in recordings:
             if rec.mbid not in seen:
                 seen.add(rec.mbid)
                 output.append(rec)
@@ -179,20 +178,19 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
         recordings = inputs[0]
         index = {}
         for rec in recordings:
             if rec.name is None or rec.name == "" or rec.artist is None or rec.artist.name is None or rec.artist.name == "":
-                self.debug("Recording %s has insufficient metadata, removing" % rec.mbid)
                 continue
 
             k = rec.name + rec.artist.name
             if k not in index:
                 index[k] = rec
 
         return [ index[k] for k in index ]  
@@ -209,15 +207,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
         recordings = inputs[0]
         output = []
         last_mbid = None
         for rec in recordings:
             if rec.mbid != last_mbid:
                 output.append(rec)
             last_mbid = rec.mbid
@@ -234,22 +232,19 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, input):
         recordings = inputs[0]
         output = []
         for rec in recordings:
-            if rec.name is None or (rec.artist and rec.artist.name is None) or rec.mbid is None:
-                if debug:
-                    print(f"recording {rec.mbid} has no metadata, filtering")
-            else:
+            if rec.name is not None and (rec.artist and rec.artist.name is not None) and rec.mbid is not None:
                 output.append(rec)
 
         return output
 
 
 class YearRangeFilterElement(troi.Element):
     '''
@@ -274,15 +269,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
 
         recordings = inputs[0]
 
         results = []
         for r in recordings:
             if not r.year:
                 continue
@@ -318,15 +313,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
 
         recordings = inputs[0]
 
         results = []
         for r in recordings:
             if "tags" not in r.musicbrainz:
                 continue
@@ -356,15 +351,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
 
         recordings = inputs[0]
 
         results = []
         now = datetime.datetime.now()
         for r in recordings:
             if "latest_listened_at" in r.listenbrainz and r.listenbrainz["latest_listened_at"] is not None:
@@ -395,15 +390,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
 
         recordings = inputs[0]
 
         results = []
         for r in recordings:
             # has this track never been listened to before?
             if "latest_listened_at" in r.listenbrainz and r.listenbrainz["latest_listened_at"]:
@@ -428,15 +423,15 @@
     def inputs():
         return [Recording]
 
     @staticmethod
     def outputs():
         return [Recording]
 
-    def read(self, inputs, debug=False):
+    def read(self, inputs):
         results = []
         for r in inputs[0]:
             score = r.listenbrainz.get("score", 0)
             if score < 0:
                 continue
             results.append(r)
         return results
```

### Comparing `troi-2024.2.9.0/troi/internal/top_sitewide_recordings_for_year.py` & `troi-2024.4.26.0/troi/patches/periodic_jams_local.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,84 @@
-from datetime import datetime
+from datetime import datetime, timedelta
 
-from troi import Recording
-import troi.listenbrainz.stats
-import troi.filters
-import troi.sorts
+import troi.listenbrainz.recs
 import troi.musicbrainz.recording_lookup
-import troi.musicbrainz.mbid_reader
-import troi.playlist
+from troi import Playlist
+from troi.playlist import PlaylistMakerElement
 
+from troi.local.recording_resolver import RecordingResolverElement
+from troi.content_resolver.model.database import db
 
-class TopSitewideRecordingsPatch(troi.patch.Patch):
+DAYS_OF_RECENT_LISTENS_TO_EXCLUDE = 60  # Exclude tracks listened in last X days from the daily jams playlist
+DAILY_JAMS_MIN_RECORDINGS = 25  # the minimum number of recordings we aspire to have in a daily jam, this is not a hard limit
+BATCH_SIZE_RECS = 1000  # the number of recommendations fetched in 1 go
+MAX_RECS_LIMIT = 1000  # the maximum of recommendations available in LB
+
+
+class PeriodicJamsLocalPatch(troi.patch.Patch):
     """
-        See below for description
     """
 
-    NAME = "Most Listened to Recordings for %d"
-    DESC = """<p>
-              This playlist is comprised of the top recordings that ListenBrainz users listened to at least once in %d.
-              </p>
-              <p>
-              This playlist serves as an insight to what other users on ListenBrainz are listening to. There is
-              very little guarantee that you may like any of these tracks, so we consider this playlist to be a discovery
-              playlist.  Because of this, it may require more active listening since it may contain tracks
-              that are not fully to your taste.
-              </p>
-           """
-
-    def __init__(self, debug=False, max_num_recordings=50):
-        troi.patch.Patch.__init__(self, debug)
-        self.max_num_recordings = max_num_recordings
+    def __init__(self, args):
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
-        Generate the ListenBrainz site wide top recordings for year playlist.
+        Generate a periodic playlist from the ListenBrainz recommended recordings.
 
         \b
-        FILE_NAME: The filename that contains the recording_mbids for this playlist.
+        USER_NAME is a MusicBrainz user name that has an account on ListenBrainz.
         """
-        return [{"type": "argument", "args": ["file_name"]}]
+        return [{
+            "type": "argument",
+            "args": ["user_name"]
+        }]
 
     @staticmethod
     def outputs():
-        return [Recording]
+        return [Playlist]
 
     @staticmethod
     def slug():
-        return "top-sitewide-recordings-for-year"
+        return "periodic-jams-local"
 
     @staticmethod
     def description():
-        return "Generate top sitewide recorings for year playlist"
-
-    def create(self, inputs):
-        file_name = inputs['file_name']
-        year = datetime.now().year
+        return "Generate a localized periodic playlist from the ListenBrainz recommended recordings."
 
-        recs = troi.musicbrainz.mbid_reader.MBIDReaderElement(file_name)
+    def is_local(self):
+        return True
 
-        rec_lookup = troi.musicbrainz.recording_lookup.RecordingLookupElement()
-        rec_lookup.set_sources(recs)
-
-        remove_empty = troi.filters.EmptyRecordingFilterElement()
-        remove_empty.set_sources(rec_lookup)
-
-        pl_maker = troi.playlist.PlaylistMakerElement(self.NAME % (year,),
-                                                      self.DESC % (year,),
-                                                      patch_slug=self.slug())
-        pl_maker.set_sources(remove_empty)
+    def create(self, inputs):
+        user_name = inputs['user_name']
 
-        shaper = troi.playlist.PlaylistRedundancyReducerElement(max_artist_occurrence=1, max_num_recordings=self.max_num_recordings)
-        shaper.set_sources(pl_maker)
+        recs = troi.listenbrainz.recs.UserRecordingRecommendationsElement(user_name,
+                                                                          "raw",
+                                                                          count=1000)
+
+        recent_listens_lookup = troi.listenbrainz.listens.RecentListensTimestampLookup(user_name,
+                                                                                       days=2)
+        recent_listens_lookup.set_sources(recs)
+
+        latest_filter = troi.filters.LatestListenedAtFilterElement(DAYS_OF_RECENT_LISTENS_TO_EXCLUDE)
+        latest_filter.set_sources(recent_listens_lookup)
+
+        feedback_lookup = troi.listenbrainz.feedback.ListensFeedbackLookup(user_name, auth_token=inputs.get("token"))
+        feedback_lookup.set_sources(latest_filter)
+
+        recs_lookup = troi.musicbrainz.recording_lookup.RecordingLookupElement()
+        recs_lookup.set_sources(feedback_lookup)
+
+        resolve = RecordingResolverElement(.8, self.quiet)
+        resolve.set_sources(recs_lookup)
+
+        pl_maker = PlaylistMakerElement(name="Weekly Jams for %s" % (user_name),
+                                        desc="test playlist!",
+                                        patch_slug="periodic-jams",
+                                        max_num_recordings=50,
+                                        max_artist_occurrence=2,
+                                        shuffle=True,
+                                        expires_at=datetime.utcnow() + timedelta(weeks=2))
+        pl_maker.set_sources(resolve)
 
-        return shaper
+        return pl_maker
```

### Comparing `troi-2024.2.9.0/troi/listenbrainz/dataset_fetcher.py` & `troi-2024.4.26.0/troi/listenbrainz/unused/dataset_fetcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from troi import Element, Artist, Recording, Playlist, PipelineError
 
 
 class DataSetFetcherElement(Element):
     '''
         Fetch a dataset from the ListenBrainz experimental APIs that contains at least a recording_mbid.
-        Recording.name, listenbrainz.listen_count and Artist.artist_credit_name will also be filled out
+        Recording.name, listenbrainz.listen_count and ArtistCredit.name will also be filled out
         if it is available in the returned data.
 
         :param server_url: the URL to POST to
         :param json_post_data: the dict data that will be POSTed as JSON
     '''
 
     def __init__(self, server_url, json_post_data, max_num_items=None):
@@ -25,19 +25,14 @@
 
     @staticmethod
     def outputs():
         return [Recording, Artist]
 
     def create_recording(self, row):
 
-        r = Recording(mbid=row['recording_mbid'])
-        if 'artist_credit_name' in row:
-            if 'artist_credit_id' in row:
-                r.artist.artist_credit_id = row['artist_credit_id']
-
         r.artist = self.create_artist(row)
 
         if 'recording_name' in row:
             r.name = row['recording_name']
 
         if 'year' in row:
             r.year = row['year']
@@ -83,13 +78,13 @@
             if "recordind_mbid" in row:
                 r = self.create_recording(row)
             elif "artist_mbid" in row:
                 r = self.create_artist(row)
             else:
                 continue
 
+        r = Recording(mbid=row['recording_mbid'])
+        if 'artist_credit_name' in row:
+            if 'artist_credit_id' in row:
+                r.artist_credit = ArtistCredit(artist_credit_id = row['artist_credit_id'],
+                                               name = row['artist_credit_name'])
             output.append(r)
-
-        if self.max_num_items is not None:
-            output = output[:self.max_num_items]
-
-        return output
```

### Comparing `troi-2024.2.9.0/troi/listenbrainz/feedback.py` & `troi-2024.4.26.0/troi/listenbrainz/feedback.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/listenbrainz/listens.py` & `troi-2024.4.26.0/troi/listenbrainz/listens.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/listenbrainz/recs.py` & `troi-2024.4.26.0/troi/listenbrainz/recs.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/listenbrainz/stats.py` & `troi-2024.4.26.0/troi/listenbrainz/stats.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from troi import Element, Artist, Release, Recording
+import logging
+
+from troi import Element, Artist, ArtistCredit, Release, Recording
 import liblistenbrainz
 import liblistenbrainz.errors
 
+logger = logging.getLogger(__name__)
+
 
 class UserArtistsElement(Element):
     '''
         Fetch artist statistics from ListenBrainz.
 
         :param user_name: The ListenBrainz user for whom to fetch statistics.
         :param time_range: The time range for which to fetch stats.
@@ -20,22 +24,24 @@
             self.client.set_auth_token(auth_token)
         self.user_name = user_name
         self.count = count
         self.offset = offset
         self.time_range = time_range
 
     def outputs(self):
-        return [Artist]
+        return [ArtistCredit]
 
-    def read(self, inputs = []):
+    def read(self, inputs=[]):
 
         artist_list = []
         artists = self.client.get_user_artists(self.user_name, self.count, self.offset, self.time_range)
+        artist_credits = []
         for a in artists['payload']['artists']:
-            artist_list.append(Artist(a['artist_name'], mbids=a['artist_mbids']))
+            artists = [Artist(mbid=mbid) for mbid in a['artist_mbids']]
+            artist_list.append(ArtistCredit(name=a['artist_name'], artists=artists))
 
         return artist_list
 
 
 class UserReleasesElement(Element):
     '''
         Fetch release statistics from ListenBrainz
@@ -55,21 +61,24 @@
         self.count = count
         self.offset = offset
         self.time_range = time_range
 
     def outputs(self):
         return [Release]
 
-    def read(self, inputs = []):
+    def read(self, inputs=[]):
 
         release_list = []
         releases = self.client.get_user_releases(self.user_name, self.count, self.offset, self.time_range)
         for r in releases['payload']['releases']:
-            artist = Artist(r['artist_name'], mbids=r['artist_mbids'])
-            release_list.append(Release(r['release_name'], mbid=r['release_mbid'], artist=artist))
+            artists = [Artist(mbid=mbid) for mbid in r['artist_mbids']]
+            release_list.append(
+                Release(r['release_name'],
+                        mbid=r['release_mbid'],
+                        artist_credit=ArtistCredit(name=r['artist_name'], artists=artists)))
 
         return release_list
 
 
 class UserRecordingElement(Element):
     '''
         Fetch release statistics from ListenBrainz
@@ -87,24 +96,26 @@
         self.count = count
         self.offset = offset
         self.time_range = time_range
 
     def outputs(self):
         return [Recording]
 
-    def read(self, inputs = []):
+    def read(self, inputs=[]):
         recording_list = []
         try:
             recordings = self.client.get_user_recordings(self.user_name, self.count, self.offset, self.time_range)
         except liblistenbrainz.errors.ListenBrainzAPIException as err:
-            print("Cannot fetch recording stats for user %s" % self.user_name)
+            logger.info("Cannot fetch recording stats for user %s" % self.user_name)
             return []
 
         if recordings is None or "recordings" not in recordings['payload']:
             return []
 
         for r in recordings['payload']['recordings']:
-            artist = Artist(r['artist_name'], mbids=r['artist_mbids'])
+            artists = [Artist(mbid=mbid) for mbid in r['artist_mbids']]
+            artist_credit = ArtistCredit(r['artist_name'], artists=artists)
             release = Release(r['release_name'], mbid=r['release_mbid'])
-            recording_list.append(Recording(r['track_name'], mbid=r['recording_mbid'], artist=artist, release=release))
+            recording_list.append(Recording(r['track_name'], mbid=r['recording_mbid'], artist_credit=artist_credit,
+                                            release=release))
 
         return recording_list
```

### Comparing `troi-2024.2.9.0/troi/listenbrainz/user.py` & `troi-2024.4.26.0/troi/listenbrainz/user.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/local/periodic_jams_local.py` & `troi-2024.4.26.0/troi/local/periodic_jams_local.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,46 @@
+import logging
+
 from troi.content_resolver.lb_radio import ListenBrainzRadioLocal
 from troi.patches.periodic_jams_local import PeriodicJamsLocalPatch
 
+logger = logging.getLogger(__name__)
+
 
 class PeriodicJamsLocal(ListenBrainzRadioLocal):
     '''
        Generate local playlists against a music collection available via subsonic.
     '''
 
-    def __init__(self, user_name, match_threshold):
-        ListenBrainzRadioLocal.__init__(self)
+    def __init__(self, user_name, match_threshold, quiet):
+        ListenBrainzRadioLocal.__init__(self, quiet)
         self.user_name = user_name
         self.match_threshold = match_threshold
+        self.quiet = quiet
 
     def generate(self):
         """
            Generate a periodic jams playlist
         """
-
+    
         patch = PeriodicJamsLocalPatch({
             "user_name": self.user_name,
-            "echo": True,
+            "quiet": self.quiet,
             "debug": True,
             "min_recordings": 1
         })
 
         # Now generate the playlist
         try:
             playlist = patch.generate_playlist()
         except RuntimeError as err:
-            print(f"LB Radio generation failed: {err}")
+            logger.info(f"LB Radio generation failed: {err}")
             return None
 
-        if playlist == None:
-            print("Your prompt generated an empty playlist.")
+        if playlist is None:
+            logger.info("Your prompt generated an empty playlist.")
             return {"playlist": {"track": []}}
 
         # Resolve any tracks that have not been resolved to a subsonic_id or a local file
         self.resolve_playlist(self.match_threshold, playlist)
 
         return playlist
```

### Comparing `troi-2024.2.9.0/troi/local/recording_resolver.py` & `troi-2024.4.26.0/troi/local/recording_resolver.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,47 +8,50 @@
 
 class RecordingResolverElement(Element):
     """
         This Troi element takes in a list of recordings, which *must* have artist name and recording
         name set and resolves them to a local collection by using the ContentResolver class
     """
 
-    def __init__(self, match_threshold):
+    def __init__(self, match_threshold, quiet):
         """ Match threshold: The value from 0 to 1.0 on how sure a match must be to be accepted.
         """
         Element.__init__(self)
         self.match_threshold = match_threshold
-        self.resolve = ContentResolver()
+        self.resolve = ContentResolver(quiet)
 
     @staticmethod
     def inputs():
         return []
 
     @staticmethod
     def outputs():
         return [Recording]
 
     def read(self, inputs):
 
         # Build the fuzzy index
         lookup_data = []
         for recording in inputs[0]:
-            if recording.artist is None or recording.artist.name is None or recording.name is None:
+            if recording.artist_credit is None or recording.artist_credit.name is None or recording.name is None:
                 raise RuntimeError("artist name and recording name are needed for RecordingResolverElement.")
 
-            lookup_data.append({"artist_name": recording.artist.name,
+            lookup_data.append({"artist_name": recording.artist_credit.name,
                                 "recording_name": recording.name,
                                 "recording_mbid": recording.mbid})
 
         self.resolve.build_index()
 
         # Resolve the recordings
         resolved = self.resolve.resolve_recordings(lookup_data, self.match_threshold)
         recording_ids = tuple([result["recording_id"] for result in resolved])
 
+        if not recording_ids:
+            return []
+
         # Could also be done with, but for some reason it fails when using IN. <shrug>
         # Recording.select().where(Recording.id.in_(recording_ids))
 
         # Fetch the recordings to lookup file ids
         query = """SELECT recording.id
                         , file_id
                         , file_id_type
```

### Comparing `troi-2024.2.9.0/troi/loops.py` & `troi-2024.4.26.0/troi/loops.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from collections import defaultdict
+import logging
 from copy import copy
-import sys
 
 import troi
-from troi import PipelineError, Element, User
+from troi import PipelineError, User
 from troi.utils import discover_patches
 
+logger = logging.getLogger(__name__)
+
 
 class ForLoopElement(troi.Element):
     '''
         An element that receives items from a pipeline and for each item in the pipeline it instantiates a new patch and executes that patch. A normal use case might include taking a list of users and running the specified patch for each user.
 
         As of right now, only User objects can be processed with this element.
 
@@ -43,41 +44,41 @@
             for user in inputs[0]:
                 args = copy(self.patch_args)
                 args["user_name"] = user.user_name
                 pipeline = patch.create(args)
                 self.patch_args["created_for"] = user.user_name
 
                 try:
-                    print("generate %s for %s" % (patch_slug, user.user_name))
+                    logger.info("generate %s for %s" % (patch_slug, user.user_name))
                     playlist = troi.playlist.PlaylistElement()
                     playlist.set_sources(pipeline)
                     playlist.generate()
 
                     if self.patch_args["min_recordings"] is not None and \
                         len(playlist.playlists[0].recordings) < self.patch_args["min_recordings"]:
-                        print("Playlist does not have at least %d recordings, not submitting.\n" % self.patch_args["min_recordings"])
+                        logger.info("Playlist does not have at least %d recordings, not submitting.\n" % self.patch_args["min_recordings"])
                         continue
 
-                    if self.patch_args["echo"]:
+                    if not self.patch_args["quiet"]:
                         playlist.print()
                     playlist.add_metadata({"algorithm_metadata": {"source_patch": patch_slug}})
                     if self.patch_args["upload"]:
                         if not self.patch_args["token"] or self.patch_args["token"] == "":
                             raise PipelineError("In order to upload a playlist an auth token must be provided. Use --token")
 
                         try:
                             if self.patch_args["created_for"] and self.patch_args["created_for"] != "":
                                 playlist.submit(self.patch_args["token"], self.patch_args["created_for"])
                             else:
                                 playlist.submit(self.patch_args["token"])
                         except troi.PipelineError as err:
-                            print("Failed to submit playlist: %s, continuing..." % err, file=sys.stderr)
+                            logger.error("Failed to submit playlist: %s, continuing..." % err)
                             continue
 
                     outputs.append(playlist.playlists[0])
-                    print()
+                    logger.info("")
                 except troi.PipelineError as err:
-                    print("Failed to generate playlist: %s" % err, file=sys.stderr)
+                    logger.info("Failed to generate playlist: %s" % err)
                     raise
 
         # Return None if you want to stop processing this pipeline
         return outputs
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/artist_credit_id_lookup.py` & `troi-2024.4.26.0/troi/musicbrainz/related_artist_credits.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,53 @@
+import copy
+from collections import defaultdict
+
 import requests
-import ujson
 
-from troi import Element, Artist, PipelineError, DEVELOPMENT_SERVER_URL
+from troi import Element, Recording, PipelineError, DEVELOPMENT_SERVER_URL
 
 
-class ArtistCreditIdLookupElement(Element):
+class RelatedArtistCreditsElement(Element):
     '''
-       Look up artist_credit_name and artist_credit_mbids for the Artists that have artist_credit_id defined.
-
-       No parameters needed for objection creation.
-
+        Look up related artist_credits, given a list of artists_credits
     '''
 
-    SERVER_URL = DEVELOPMENT_SERVER_URL + "/artist-credit-id-lookup/json"
+    SERVER_URL = DEVELOPMENT_SERVER_URL + "/artist-credit-similarity/json"
 
-    def __init__(self):
+    def __init__(self, threshold=0):
         super().__init__()
+        self.threshold = threshold
 
     @staticmethod
     def inputs():
-        return [Artist]
+        return [Recording]
 
     @staticmethod
     def outputs():
-        return [Artist]
+        return [Recording]
 
     def read(self, inputs):
 
-        ac_ids = []
-        index = {}
-        for a in inputs[0]:
-            ac_ids.append(str(a.artist_credit_id))
-            index[a.artist_credit_id] = a
-
-        params = {"[artist_credit_id]": ",".join(ac_ids)}
+        artists = inputs[0]
+        ac_ids = ",".join([ str(a.artist_credit_id) for a in artists ])
+        params = {"[artist_credit_id]": ac_ids,
+                  "threshold": self.threshold}
         r = requests.get(self.SERVER_URL, params=params)
         if r.status_code != 200:
-            raise PipelineError("Cannot fetch artist credits from ListenBrainz: HTTP code %d" % r.status_code)
+            raise PipelineError("Cannot fetch related artist credits from ListenBrainz: HTTP code %d" % r.status_code)
 
         try:
-            artists = ujson.loads(r.text)
-        except Exception as err:
-            raise PipelineError("Cannot fetch artist credits from ListenBrainz: Invalid JSON returned: " + str(err))
+            relations = r.text
+        except ValueError as err:
+            raise PipelineError("Cannot fetch related artist credits from ListenBrainz: Invalid JSON returned: " + str(err))
+
+        index = defaultdict(list)
+        for row in relations:
+            index[row['artist_credit_id']].append(row)
 
         entities = []
-        for row in artists:
-            a = index[row['artist_credit_id']]
-            a.name = row['artist_credit_name']
-            a.mbids = row['artist_credit_mbids']
+        for artist in artists:
+            a = copy.deepcopy(artist)
+            a.mb['related_artist_credit_ids'] = index[artist.artist_credit_id]
             entities.append(a)
 
         return entities
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/genre_lookup.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/recs.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,83 @@
-import requests
+import troi
+from random import randint, shuffle
+from uuid import UUID
+
+import troi
+import liblistenbrainz
+import liblistenbrainz.errors
+from troi import Artist, Recording
+from troi import TARGET_NUMBER_OF_RECORDINGS
+from troi.parse_prompt import TIME_RANGES
 
-from troi import Element, Recording, PipelineError
 
-MAX_MBIDS_PER_CALL = 20
-
-
-class GenreLookupElement(Element):
+class LBRadioRecommendationRecordingElement(troi.Element):
     """
-        Look up musicbrainz tags and genres for a list of Recordings, based on recording mbid.
-
-        :param count_threshold: This integer parameter controls which tags/genres to load. If the tag_count (the number of times a tag/genre has been applied to this Recording) is greate or equal to count_threshold, then the tag/genre will be kept and returned. Use 0 to return all tags/genres.
+        Given a LB user, fetch their recommended recordings and then include recordings from it.
     """
 
-    SERVER_URL = "https://api.listenbrainz.org/1/metadata/recording"
+    MAX_RECOMMENDED_RECORDINGS = 1000
+    MAX_RECORDINGS_TO_FETCH_PER_CALL = 100
 
-    def __init__(self, count_threshold=3):
-        Element.__init__(self)
-        self.count_threshold = count_threshold
+    def __init__(self, user_name, listened="all", mode="easy"):
+        troi.Element.__init__(self)
+        self.user_name = user_name
+        self.listened = listened
+        self.mode = mode
+        self.client = liblistenbrainz.ListenBrainz()
 
-    @staticmethod
-    def inputs():
-        return [Recording]
+    def inputs(self):
+        return []
 
-    @staticmethod
-    def outputs():
+    def outputs(self):
         return [Recording]
 
-    def read(self, inputs):
+    def read(self, entities):
 
-        recordings = inputs[0]
-        if not recordings:
-            return []
-
-        mbid_sets = []
-        mbids = []
-        for r in recordings:
-            mbids.append(r.mbid)
-            if len(mbids) >= MAX_MBIDS_PER_CALL:
-                mbid_sets.append(mbids)
-                mbids = []
+        if self.mode == "easy":
+            offset = 0
+        elif self.mode == "medium":
+            offset = self.MAX_RECOMMENDED_RECORDINGS // 3
         else:
-            mbid_sets.append(mbids)
-            
-        output = []
-
-        data = {}
-        for mbid_set in mbid_sets:
-            r = requests.get(self.SERVER_URL, params={ "recording_mbids" : ",".join(mbid_set), "inc": "tag" })
-            if r.status_code != 200:
-                raise PipelineError("Cannot fetch tags from ListenBrainz: HTTP code %d" % r.status_code)
-
-            data = {**data, **r.json()}
-
-        for r in recordings:
-
-            if r.mbid not in data:
-                continue
-
-            # Save the whole MB metadata tag info
-            r.musicbrainz["tag_metadata"] = data[r.mbid]["tag"]
-
-            genres = []
-            tags = []
-            for genre in data[r.mbid]["tag"]["recording"]:
-                if genre["count"] >= self.count_threshold:
-                    if "genre_mbid" in genre:
-                        genres.append(genre["tag"])
+            offset = self.MAX_RECOMMENDED_RECORDINGS * 2 // 3
+
+        added = 0
+        skipped = 0
+        recordings = []
+        count = self.MAX_RECOMMENDED_RECORDINGS // 3
+        while count > 0:
+            # Fetch the user recs
+            try:
+                result = self.client.get_user_recommendation_recordings(self.user_name, "raw",
+                                                                        min(self.MAX_RECORDINGS_TO_FETCH_PER_CALL, count), offset)
+            except liblistenbrainz.errors.ListenBrainzAPIException as err:
+                raise RuntimeError("Cannot fetch recording stats for user %s" % self.user_name)
+
+            if result is None or len(result['payload']['mbids']) == 0:
+                break
+
+            # Turn them into recordings
+            for r in result['payload']['mbids']:
+                if r['recording_mbid'] is not None:
+                    offset += 1
+                    latest = r.get("latest_listened_at", None)
+                    if self.listened == "all" or (self.listened == "unlistened" and latest is None) or \
+                            (self.listened == "listened" and latest is not None):
+                        count -= 1
+                        recordings.append(Recording(mbid=r['recording_mbid']))
+                        added += 1
                     else:
-                        tags.append(genre["tag"])
+                        skipped += 1
 
-            r.musicbrainz["genre"] = genres
-            r.musicbrainz["tag"] = tags
+            # Shuffle the recordings
+            shuffle(recordings)
 
-            if r.artist is not None and "artist" in data[r.mbid]["tag"]:
-                artist_genres = []
-                artist_tags = []
-                for genre in data[r.mbid]["tag"]["artist"]:
-                    if genre["count"] >= self.count_threshold:
-                        if "genre_mbid" in genre:
-                            artist_genres.append(genre["tag"])
-                        else:
-                            artist_tags.append(genre["tag"])
+        # Give feedback on what we collected
+        listened = ""
+        if self.listened != "all":
+            listened = f"previously {self.listened} "
 
-                r.artist.musicbrainz["genre"] = artist_genres
-                r.artist.musicbrainz["tag"] = artist_tags
+        self.local_storage["data_cache"]["element-descriptions"].append(f"{self.user_name}'s {listened}recommended songs")
 
-            output.append(r)
+        # TODO: How do we prevent sequential tracks by the same artist?
 
-        return output
+        return recordings
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/mbid_mapping.py` & `troi-2024.4.26.0/troi/musicbrainz/mbid_mapping.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import ujson
 
-from troi import Element, Artist, Recording, Release, PipelineError
+from troi import Element, Artist, ArtistCredit, Recording, Release, PipelineError
 
 
 class MBIDMappingLookupElement(Element):
     '''
        Look up MBIDs for the given recordings, if possible. If recordings
        are not found, their data remains unchanged.
 
@@ -26,17 +26,16 @@
     def outputs():
         return [Recording]
 
     def read(self, inputs):
 
         params = []
         for r in inputs[0]:
-            if r.artist is not None and r.name is not None:
-                params.append({"[artist_credit_name]": r.artist.name,
-                               "[recording_name]": r.name})
+            if r.artist_credit is not None and r.name is not None:
+                params.append({"[artist_credit_name]": r.artist_credit.name, "[recording_name]": r.name})
 
         if not params:
             return []
 
         r = requests.post(self.SERVER_URL, json=params)
         if r.status_code != 200:
             raise PipelineError("Cannot fetch MBID mapping rows from ListenBrainz: HTTP code %d (%s)" % (r.status_code, r.text))
@@ -47,31 +46,22 @@
 
             if not row['artist_credit_name']:
                 if not self.remove_unmatched:
                     entities.append(r)
                 continue
 
             if r.mbid:
-                r.add_note("recording mbid %s overwritten by mbid_lookup" % (r.mbid))
+                r.add_note("recording mbid %s overwritten by mbid_lookup" % (r.mbid,))
             r.mbid = row['recording_mbid']
             r.name = row['recording_name']
-            r.year = row['year']
 
-            if r.artist is None:
-                r.artist = Artist(artist_credit_id=row['artist_credit_id'], name=row['artist_credit_name'])
-            else:
-                if r.artist.artist_credit_id:
-                    r.artist.add_note("artist_credit_id %d overwritten by mbid_lookup" % (r.artist.artist_credit_id))
-                r.artist.artist_credit_id = row['artist_credit_id']
-                r.artist.name = row['artist_credit_name']
-
-            if r.release:
-                if r.release.mbid:
-                    r.release.add_note("mbid %d overwritten by mbid_lookup" % (r.release.mbid))
-                r.release.mbid = row['release_mbid']
-                r.release.name = row['release_name']
-            else:
-                r.release = Release(row['release_name'], mbid=row['release_mbid'])
+            r.artist_credit = ArtistCredit(
+                artist_credit_id=row['artist_credit_id'],
+                name=row['artist_credit_name'],
+                artists=[ Artist(mbid=mbid) for mbid in row['artist_mbids'] ] 
+            )
+
+            r.release = Release(row['release_name'], mbid=row['release_mbid'])
 
             entities.append(r)
 
         return entities
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/mbid_reader.py` & `troi-2024.4.26.0/troi/musicbrainz/mbid_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 import ujson
 
-from troi import Element, Artist, PipelineError, Recording
+from troi import Element, Recording
 
 
 class MBIDReaderElement(Element):
     '''
         Read MBIDs from a file, one per line and return Recording objects with the MBID field filled out.
 
         :param filename: The name (with full path) of the file to read recording MBIDs from.
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/recording.py` & `troi-2024.4.26.0/troi/musicbrainz/recording.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/musicbrainz/recording_lookup.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/blend.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,107 @@
-from time import sleep
+from collections import defaultdict
+import troi
+from random import randint
+from troi import Recording
+from troi import TARGET_NUMBER_OF_RECORDINGS
 
-import requests
-import ujson
 
-from troi import Element, Artist, PipelineError, Recording, Playlist, Release
+class InterleaveRecordingsElement(troi.Element):
+    """
+        This element round-robins the various input sources into one list until all sources are all empty.
+    """
 
+    def __init__(self):
+        troi.Element.__init__(self)
 
-class RecordingLookupElement(Element):
-    '''
-        Look up a musicbrainz data for a list of recordings, based on MBID.
+    def inputs(self):
+        return [Recording]
 
-        :param skip_not_found: If skip_not_found is set to True (the default) then Recordings that cannot be found in MusicBrainz will not be returned from this Element.
-    '''
+    def outputs(self):
+        return [Recording]
 
-    SERVER_URL = "https://labs.api.listenbrainz.org/recording-mbid-lookup/json?count=%d"
-
-    def __init__(self, skip_not_found=True):
-        Element.__init__(self)
-        self.skip_not_found = skip_not_found
-
-    @staticmethod
-    def inputs():
-        return [ Recording, Playlist ]
-
-    @staticmethod
-    def outputs():
-        return [ Recording, Playlist ]
-
-    def read(self, inputs):
-
-        if isinstance(inputs[0], Playlist):
-            recordings = inputs[0].recordings
-        else:
-            recordings = inputs[0]
-        if not recordings:
-            return []
-
-        data = []
-        for r in recordings:
-            if r.artist is None or r.artist.name is None or len(r.artist.mbids) == 0 or r.name is None:
-                data.append({ '[recording_mbid]': r.mbid })
-
-        # If we have all the data for all the recordings, no need to lookup anything and simply pass the data along
-        if len(data) == 0:
-            return inputs[0]
-
-        self.debug("- debug %d recordings" % len(recordings))
+    def read(self, entities):
 
+        recordings = []
         while True:
-            r = requests.post(self.SERVER_URL % len(recordings), json=data)
-            if r.status_code == 429:
-                sleep(2)
-                continue
-
-            if r.status_code != 200:
-                raise PipelineError("Cannot fetch recordings from ListenBrainz: HTTP code %d (%s)" % (r.status_code, r.text))
-
-            break
-
-        try:
-            rows = ujson.loads(r.text)
-            self.debug("- debug %d rows in response" % len(rows))
-        except ValueError as err:
-            raise PipelineError("Cannot fetch recordings from ListenBrainz: " + str(err))
-
-        mbid_index = {}
-        for row in rows:
-            mbid_index[row['original_recording_mbid']] = row
-
-        output = []
-        for r in recordings:
+            empty = 0
+            for entity in entities:
+                try:
+                    recordings.append(entity.pop(0))
+                except IndexError:
+                    empty += 1
+
+            # Did we process all the recordings?
+            if empty == len(entities):
+                break
+
+        return recordings
+
+
+class WeighAndBlendRecordingsElement(troi.Element):
+    """
+        This element will weight all the given sources according to weights passed to __init__ and
+        then combine all the input sources into one weighted output stream.
+
+        A source that has a weight of 2 will be chosen 2 times more often than a source with weight 1.
+    """
+
+    def __init__(self, weights, max_num_recordings=TARGET_NUMBER_OF_RECORDINGS, max_artist_occurrence=None):
+        troi.Element.__init__(self)
+        self.weights = weights
+        self.max_num_recordings = max_num_recordings
+        self.max_artist_occurrence = max_artist_occurrence
+
+    def inputs(self):
+        return [Recording]
+
+    def outputs(self):
+        return [Recording]
+
+    def read(self, entities):
+
+        total_available = sum([len(e) for e in entities])
+
+        # prepare the weights
+        total = sum(self.weights)
+        summed = []
+        acc = 0
+        for i in self.weights:
+            acc += i
+            summed.append(acc)
+
+        # Ensure seed artists are the first tracks -- doing this for all recording elements work in this case.
+        recordings = []
+        for element in entities:
             try:
-                row = mbid_index[r.mbid]
-                if row["recording_mbid"] is None:
-                    continue
-            except KeyError:
-                if self.skip_not_found:
-                    self.debug("- debug recording MBID %s not found, skipping." % r.mbid)
-                else:
-                    output.append(r)
-                continue
-
-            if r.artist:
-                r.artist.name = row['artist_credit_name']
-                r.artist.mbids = row.get('[artist_credit_mbids]', [])
-                r.artist.artist_credit_id = row['artist_credit_id']
-            else:
-                a = Artist(name=row['artist_credit_name'],
-                           mbids=row.get('[artist_credit_mbids]', []),
-                           artist_credit_id=row['artist_credit_id'])
-                r.artist = a
-
-            if r.release:
-                r.release.name = row["release_name"]
-                r.release.mbid = row["release_mbid"]
-            else:
-                r.release = Release(name=row["release_name"],
-                                    mbid=row["release_mbid"])
-
-            r.name = row['recording_name']
-            r.duration = row['length']
-            r.mbid = row['recording_mbid']
-
-            r.listenbrainz["canonical_recording_mbid"] = row["canonical_recording_mbid"]
-
-            output.append(r)
-
-        if isinstance(inputs[0], Playlist):
-            inputs[0].recordings = output
-            output = inputs[0]
+                recordings.append(element.pop(0))
+            except IndexError:
+                pass
+
+        # This still allows sequential tracks to be from the same artists. I'll wait for feedback to see if this
+        # is a problem.
+        artist_counts = defaultdict(int)
+        dedup_set = set()
+        while True:
+            r = randint(0, total)
+            for i, s in enumerate(summed):
+                if r < s:
+                    while True:
+                        if len(entities[i]) > 0:
+                            rec = entities[i].pop(0)
+                            if rec.mbid in dedup_set:
+                                total_available -= 1
+                                continue
+                            if self.max_artist_occurrence is not None and \
+                                    artist_counts[rec.artist_credit.artist_credit_id] == self.max_artist_occurrence:
+                                total_available -= 1
+                                continue
+
+                            recordings.append(rec)
+                            dedup_set.add(rec.mbid)
+                            artist_counts[rec.artist_credit.artist_credit_id] += 1
+                        break
+
+            if len(recordings) >= self.max_num_recordings or len(recordings) == total_available:
+                break
 
-        return output
+        return recordings
```

### Comparing `troi-2024.2.9.0/troi/musicbrainz/year_lookup.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/stats.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-import re
-import sys
-import uuid
-from urllib.parse import quote
-
-import requests
-import ujson
-
-from troi import Element, Artist, Recording, PipelineError
-
-class YearLookupElement(Element):
-    '''
-        Look up musicbrainz earliest release year for a list of recordings, based on artist credit name and recording name.
-
-        By default items that are not found in the year lookup are not returned by this element. Pass
-        skip_not_found=False to init to keep tracks that failed the year lookup.
-
-        :param skip_not_found: If this is True (the default) then any Recordings for which the year could not be lookd up will not be returned from this Element.
-    '''
-
-    SERVER_URL = "https://labs.api.listenbrainz.org/year-artist-recording-year-lookup/json"
-
-    def __init__(self, skip_not_found=True):
-        Element.__init__(self)
-        self.skip_not_found = skip_not_found
-
-    @staticmethod
-    def inputs():
-        return [ Recording ]
-
-    @staticmethod
-    def outputs():
-        return [ Recording ]
-
-    def read(self, inputs):
-
-        recordings = inputs[0]
-        if not recordings:
-            return []
-
-        data = []
-        for r in recordings:
-            try:
-                data.append({ '[recording_name]': r.name, 
-                              '[artist_credit_name]': r.artist.name })
-            except AttributeError:
-                raise PipelineError("YearLookupElement requires artist_credit_name and recording_name to exist.")
-
-        r = requests.post(self.SERVER_URL, json=data)
-        if r.status_code != 200:
-            raise PipelineError("Cannot fetch recording years from MusicBrainz: HTTP code %d" % r.status_code)
+import troi
+from random import randint, shuffle
+from uuid import UUID
+
+import troi
+import liblistenbrainz
+import liblistenbrainz.errors
+from troi import Artist, ArtistCredit, Recording
+from troi import TARGET_NUMBER_OF_RECORDINGS
+from troi.parse_prompt import TIME_RANGES
+
+
+class LBRadioStatsRecordingElement(troi.Element):
+    """
+        Given a LB user, fetch their recording stats and then include recordings from it.
+    """
+
+    NUM_RECORDINGS_TO_COLLECT = TARGET_NUMBER_OF_RECORDINGS * 2
+
+    def __init__(self, user_name, time_range, mode="easy"):
+        troi.Element.__init__(self)
+        self.user_name = user_name
+        self.time_range = time_range
+        self.mode = mode
+        self.client = liblistenbrainz.ListenBrainz()
+
+        if time_range not in TIME_RANGES:
+            raise RuntimeError("entity stats must specify one of the following time range options: " + ", ".join(TIME_RANGES))
+
+    def inputs(self):
+        return []
+
+    def outputs(self):
+        return [Recording]
+
+    def read(self, entities):
+
+        if self.mode == "easy":
+            offset = 0
+        elif self.mode == "medium":
+            offset = 100
+        else:
+            offset = 200
 
+        # Fetch the user stats
         try:
-            rows = ujson.loads(r.text)
-        except ValueError as err:
-            raise PipelineError("Cannot fetch recording years from MusicBrainz: " + str(err))
-
-        mbid_index = {}
-        for row in rows:
-            mbid_index[row['artist_credit_name'] + row['recording_name']] = row['year']
+            result = self.client.get_user_recordings(self.user_name, 100, offset, self.time_range)
+        except liblistenbrainz.errors.ListenBrainzAPIException as err:
+            raise RuntimeError("Cannot fetch recording stats for user %s" % self.user_name)
+
+        if result is None or "recordings" not in result["payload"]:
+            raise RuntimeError("There are no stats available for user '%s' for the %s time_range." %
+                               (self.user_name, self.time_range))
+
+        # Give feedback on what we collected
+        self.local_storage["data_cache"]["element-descriptions"].append(f"{self.user_name}'s stats for {self.time_range}")
+
+        # Turn them into recordings
+        recordings = []
+        for r in result['payload']['recordings']:
+            if r['recording_mbid'] is not None:
+                artists = [Artist(mbid=mbid) for mbid in r["artist_mbids"]]
+                artist_credit = ArtistCredit(artists=artists, musicbrainz={"artist_mbids": r["artist_mbids"]})
+                recordings.append(Recording(mbid=r['recording_mbid'], artist_credit=artist_credit))
 
-        output = []
-        for r in recordings:
-            try:
-                r.year = mbid_index[r.artist.name + r.name]
-            except KeyError:
-                if self.skip_not_found:
-                    self.debug("recording (%s %s) not found, skipping." % (r.artist.name, r.name))
-                else:
-                    output.append(r)
-                continue
+        # Shuffle the recordings
+        shuffle(recordings)
 
-            output.append(r)
+        # Check to make sure we're not going to have tracks by the same artist sequentially
+        for i in range(len(recordings), 0, -1):
+            try:
+                if recordings[i].artist_credit.musicbrainz["artist_mbids"] == recordings[
+                        i + 1].artist_credit.musicbrainz["artist_mbids"]:
+                    recordings.pop(i)
+            except IndexError:
+                pass
 
-        return output
+        return recordings
```

### Comparing `troi-2024.2.9.0/troi/operations.py` & `troi-2024.4.26.0/troi/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,19 @@
 
     return True
 
 
 def _check_key_for_set_op(entities, key):
     """ Check the key based on which set operation is to be performed is valid for given entity """
     if isinstance(entities[0], troi.Artist):
-        if key not in ['mbids', 'name', 'artist_credit_id']:
-            raise ValueError("key must be one of mbids, msid, name or artist_credit_id.")
+        if key not in ['mbid', 'name']:
+            raise ValueError("key must be one of mbid, name.")
+    if isinstance(entities[0], troi.ArtistCredit):
+        if key not in ['name', 'artists', 'artist_credit_id']:
+            raise ValueError("key must be one of name, artists or artist_credit_id.")
     elif isinstance(entities[0], troi.Recording):
         if key not in ['mbid', 'msid', 'name']:
             raise ValueError("key must be one of mbid, msid or name.")
     else:
         if key not in ['mbid', 'name']:
             raise ValueError("key must be one of mbid or name.")
 
@@ -71,15 +74,15 @@
 
         if not is_homogeneous(entities):
             raise TypeError("entity list not homogenous")
         _check_key_for_set_op(entities, self.key)
 
         entity_dict = {}
         for e in entities:
-            if isinstance(e, troi.Artist) and self.key == "mbids":
+            if isinstance(e, troi.ArtistCredit) and self.key == "artists":
                 entity_dict[",".join(getattr(e, self.key))] = e
             else:
                 entity_dict[getattr(e, self.key)] = e
 
         return list(entity_dict.values())
```

### Comparing `troi-2024.2.9.0/troi/parse_prompt.py` & `troi-2024.4.26.0/troi/parse_prompt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from uuid import UUID
 import re
 
 TIME_RANGES = ["week", "month", "quarter", "half_yearly", "year", "all_time", "this_week", "this_month", "this_year"]
-ELEMENTS = ["artist", "tag", "collection", "playlist", "stats", "recs"]
+ELEMENTS = ["artist", "tag", "collection", "playlist", "stats", "recs", "country"]
 
 ELEMENT_OPTIONS = {
     "artist": ["nosim", "easy", "medium", "hard"],
     "tag": ["nosim", "and", "or", "easy", "medium", "hard"],
     "collection": ["easy", "medium", "hard"],
     "playlist": ["easy", "medium", "hard"],
     "stats": TIME_RANGES,
-    "recs": ["easy", "medium", "hard", "listened", "unlistened"]
+    "recs": ["easy", "medium", "hard", "listened", "unlistened"],
+    "country": ["easy", "medium", "hard"]
 }
 
 OPTIONS = set()
 for eo in ELEMENT_OPTIONS:
     OPTIONS.update(ELEMENT_OPTIONS[eo])
 
 OPTIONS = list(OPTIONS)
@@ -61,22 +62,24 @@
 
         return prompt
 
     def set_block_values(self, name, values, weight, opts, text, block):
         """Parse, process and sanity check data for an element"""
 
         if values is None:
-            try:
-                values = [UUID(text)]
-            except ValueError:
-                if name == "tag":
-                    values = text.split(",")
-                    values = [v.strip() for v in values]
-                else:
+            if name in ("artist", "country", "collection", "playlist"):
+                try:
+                    values = [UUID(text)]
+                except ValueError:
                     values = [text]
+            elif name == "tag":
+                values = text.split(",")
+                values = [v.strip() for v in values]
+            else:
+                values = [text]
         elif weight is None:
             if not text:
                 weight = 1
             else:
                 try:
                     weight = int(text)
                 except ValueError:
@@ -138,14 +141,18 @@
                     continue
 
                 if block[i] == ':' and parens == 0:
                     values, weight, opts = self.set_block_values(name, values, weight, opts, text, block)
                     text = ""
                     continue
 
+                # Check to make sure that some values are in ()
+                if name in ("artist", "country", "collection", "playlist") and i == 0 and not block[i] == "(":
+                    raise ParseError("Element value must be enclosed in ( ). Try: %s:(name)" % (name))
+
                 if block[i] == ' ' and parens == 0:
                     break
 
                 text += block[i]
 
             # Now that we've parsed a block, do some sanity checking
             values, weight, opts = self.set_block_values(name, values, weight, opts, text, block)
```

### Comparing `troi-2024.2.9.0/troi/patch.py` & `troi-2024.4.26.0/troi/patch.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,47 @@
 import logging
+
 import troi
 from abc import ABC, abstractmethod
 
+from troi.logging_utils import set_log_level
 from troi.recording_search_service import RecordingSearchByTagService, RecordingSearchByArtistService
 
-default_patch_args = dict(debug=False,
-                          echo=True,
-                          save=False,
+logger = logging.getLogger(__name__)
+
+default_patch_args = dict(save=False,
                           token=None,
                           upload=False,
                           args=None,
                           created_for=None,
                           name=None,
                           desc=None,
                           min_recordings=10,
-                          spotify=None)
+                          spotify=None,
+                          quiet=False)
 
 
 class Patch(ABC):
 
-    def __init__(self, args, debug=False):
+    def __init__(self, args):
+        self.quiet = False
         self.args = args
-        if debug:
-            level = logging.DEBUG
-        else:
-            level = logging.INFO
-        logging.basicConfig(level=level)
-        self.logger = logging.getLogger(type(self).__name__)
 
         # Dict used for local storage
         self.local_storage = {}
 
         self.patch_args = {**default_patch_args, **args}
         self.pipeline = self.create(self.patch_args)
         self._set_element_patch(self.pipeline)
 
         # Setup extensible services
         self.services = {}
         self.register_service(RecordingSearchByTagService())
         self.register_service(RecordingSearchByArtistService())
 
-    def log(self, msg):
-        '''
-            Log a message with the info log level, which is the default for troi. 
-
-            :param msg: The message to log.
-        '''
-        self.logger.info(msg)
-
-    def debug(self, msg):
-        '''
-            Log a message with debug log level. These messages will only be shown when debugging is enabled.
-        '''
-        self.logger.debug(msg)
-
     @staticmethod
     def inputs():
         """
             This function should return a list of dicts that defined the type (argument or option), args, and kwargs to be passed to the click function. MusicBrainz entities and python base types can all be used. The documentation of the method is used as the help returned by the command. Example:
 
             .. code-block:: json
 
@@ -117,14 +101,21 @@
         """
            Given a service slug, return the class registered for this service. 
 
            Raises IndexError if no such service is registered.
         """
         return self.services[slug]
 
+    def is_local(self):
+        """
+            If this function returns True, it means that the patch expects to use the local database, so Troi should
+            setup the local database before running this patch. Returns False unless overridden by a deriving patch.
+        """
+        return False
+
     def post_process(self):
         """
             This function is called once the pipeline has produced its playlist, just before the Playlist object is created.
             This function could be used to inspect data in patch local storage to create the detailed playlist name
             and descriptionm which may not be available when the pipeline is constructed.
         """
         return
@@ -140,90 +131,83 @@
 
     def generate_playlist(self):
         """
         Generate a playlist 
 
         The args parameter is a dict and may containt the following keys:
 
-        * debug: Print debug information or not
-        * print: This option causes the generated playlist to be printed to stdout.
+        * quiet: Do not print out anything
         * save: The save option causes the generated playlist to be saved to disk.
         * token: Auth token to use when using the LB API. Required for submitting playlists to the server. See https://listenbrainz.org/profile to get your user token.
         * upload: Whether or not to submit the finished playlist to the LB server. Token must be set for this to work.
         * created-for: If this option is specified, it must give a valid user name and the TOKEN argument must specify a user who is whitelisted as a playlist bot at listenbrainz.org .
         * name: Override the algorithms that generate a playlist name and use this name instead.
         * desc: Override the algorithms that generate a playlist description and use this description instead.
         * min-recordings: The minimum number of recordings that must be present in a playlist to consider it complete. If it doesn't have sufficient numbers of tracks, ignore the playlist and don't submit it. Default: Off, a playlist with at least one track will be considere complete.
         * spotify: if present, attempt to submit the playlist to spotify as well. should be a dict and contain the spotify user id, spotify auth token with appropriate permissions, whether the playlist should be public, private or collaborative. it can also optionally have the existing urls to update playlists instead of creating new ones.
 
         :param args: the arguments to pass to the patch, may contain one of more of the following keys:
 
         """
 
         try:
+            set_log_level(self.patch_args.get("quiet", False))
             playlist = troi.playlist.PlaylistElement()
             playlist.set_sources(self.pipeline)
-            print("Troi playlist generation starting...")
-            result = playlist.generate()
+            logger.info("Troi playlist generation starting...")
+            result = playlist.generate(self.quiet)
 
             name = self.patch_args["name"]
             if name:
                 playlist.playlists[0].name = name
 
             desc = self.patch_args["desc"]
             if desc:
                 playlist.playlists[0].descripton = desc
 
-            print("done.")
+            logger.info("done.")
         except troi.PipelineError as err:
-            print("Failed to generate playlist: %s" % err, file=sys.stderr)
-            return None
+            raise RuntimeError("Playlist generation failed: %s" % err)
 
         upload = self.patch_args["upload"]
         token = self.patch_args["token"]
         spotify = self.patch_args["spotify"]
         if upload and not token and not spotify:
-            print("In order to upload a playlist, you must provide an auth token. Use option --token.")
-            return None
+            raise RuntimeError("In order to upload a playlist, you must provide an auth token. Use option --token.")
 
         min_recordings = self.patch_args["min_recordings"]
         if min_recordings is not None and \
                 (len(playlist.playlists) == 0 or len(playlist.playlists[0].recordings) < min_recordings):
-            print("Playlist does not have at least %d recordings, stopping." % min_recordings)
-            return None
+            raise RuntimeError("Playlist does not have at least %d recordings" % min_recordings)
 
         save = self.patch_args["save"]
         if result is not None and spotify and upload:
             for url, _ in playlist.submit_to_spotify(spotify["user_id"], spotify["token"], spotify["is_public"],
                                                      spotify["is_collaborative"], spotify.get("existing_urls", [])):
-                print("Submitted playlist to spotify: %s" % url)
+                logger.info("Submitted playlist to spotify: %s" % url)
 
         created_for = self.patch_args["created_for"]
         if result is not None and token and upload:
             for url, _ in playlist.submit(token, created_for):
-                print("Submitted playlist: %s" % url)
+                logger.info("Submitted playlist: %s" % url)
 
         if result is not None and save:
             playlist.save()
-            print("playlist saved.")
+            logger.info("playlist saved.")
 
-        echo = self.patch_args["echo"]
-        if result is not None and (echo or not token):
-            print()
+        if not self.quiet and result is not None:
+            logger.info("")
             playlist.print()
 
-        if not echo and not save and not token:
-            if result is None:
-                print("Patch executed successfully.")
-            elif len(playlist.playlists) == 0:
-                print("No playlists were generated. :(")
-            elif len(playlist.playlists) == 1:
-                print("A playlist with %d tracks was generated." % len(playlist.playlists[0].recordings))
-            else:
-                print("%d playlists were generated." % len(playlist.playlists))
+        if len(playlist.playlists) == 0:
+            logger.info("No playlists were generated. :(")
+        elif len(playlist.playlists) == 1:
+            logger.info("A playlist with %d tracks was generated." % len(playlist.playlists[0].recordings))
+        else:
+            logger.info("%d playlists were generated." % len(playlist.playlists))
 
         return playlist
 
     def _set_element_patch(self, element):
         """ 
             Go through the pipeline, setting the patch objects for each Element
         """
```

### Comparing `troi-2024.2.9.0/troi/patches/area_random_recordings.py` & `troi-2024.4.26.0/troi/patches/unused/area_random_recordings.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from troi.listenbrainz.dataset_fetcher import DataSetFetcherElement
 
 
 class AreaRandomRecordingsPatch(troi.patch.Patch):
 
     SERVER_URL = DEVELOPMENT_SERVER_URL + "/area-random-recordings/json"
 
-    def __init__(self, args, debug=False):
-        super().__init__(args, debug)
+    def __init__(self, args):
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
         Generate a list of random recordings from a given area.
 
         \b
```

### Comparing `troi-2024.2.9.0/troi/patches/lb_radio.py` & `troi-2024.4.26.0/troi/patches/lb_radio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from time import sleep
 from random import randint, shuffle
 from uuid import UUID
 
 import requests
 from urllib.parse import quote
 
 import troi.patch
@@ -15,32 +16,33 @@
 from troi.patches.lb_radio_classes.artist import LBRadioArtistRecordingElement
 from troi.patches.lb_radio_classes.blend import InterleaveRecordingsElement, WeighAndBlendRecordingsElement
 from troi.patches.lb_radio_classes.collection import LBRadioCollectionRecordingElement
 from troi.patches.lb_radio_classes.playlist import LBRadioPlaylistRecordingElement
 from troi.patches.lb_radio_classes.tag import LBRadioTagRecordingElement
 from troi.patches.lb_radio_classes.stats import LBRadioStatsRecordingElement
 from troi.patches.lb_radio_classes.recs import LBRadioRecommendationRecordingElement
+from troi.patches.lb_radio_classes.country import LBRadioCountryRecordingElement
 from troi import TARGET_NUMBER_OF_RECORDINGS, Playlist
 from troi.utils import interleave
 
 
 class LBRadioPatch(troi.patch.Patch):
     """
        ListenBrainz radio experimentation.
     """
 
     # If the user specifies no time_range, default to this one
     DEFAULT_TIME_RANGE = "month"
 
-    def __init__(self, args, debug=False):
+    def __init__(self, args):
         self.artist_mbids = []
         self.mode = None
 
         # Remember, the create function for this class will be called in the super() init.
-        super().__init__(args, debug)
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
         Generate a playlist from one or more Artist MBIDs
 
         \b
@@ -71,42 +73,67 @@
     def slug():
         return "lb-radio"
 
     @staticmethod
     def description():
         return "Given an LB radio prompt, generate a playlist for that prompt."
 
-    def lookup_artist_name(self, artist_name):
+    def lookup_artist(self, artist_name):
         """ Fetch artist names for validation purposes """
 
+        if isinstance(artist_name, UUID):
+            return self.lookup_artist_from_mbid(artist_name)
+
         err_msg = f"Artist {artist_name} could not be looked up. Please use exact spelling."
 
-        r = requests.get(
-            f"https://musicbrainz.org/ws/2/artist?query={quote(artist_name)}&fmt=json"
-        )
-        if r.status_code == 404:
-            raise RuntimeError(err_msg)
+        while True:
+            r = requests.get( f"https://musicbrainz.org/ws/2/artist?query={quote(artist_name)}&fmt=json")
+            if r.status_code == 404:
+                raise RuntimeError(err_msg)
+
+            if r.status_code == 429:
+                sleep(2)
+                continue
 
-        if r.status_code != 200:
-            raise RuntimeError(
-                f"Could not resolve artist name {artist_name}. Error {r.status_code}"
-            )
+            if r.status_code != 200:
+                raise RuntimeError( f"Could not resolve artist name {artist_name}. Error {r.status_code} {r.text}")
+
+            break
 
         data = r.json()
         try:
             fetched_name = data["artists"][0]["name"]
             mbid = data["artists"][0]["id"]
         except (IndexError, KeyError):
             raise RuntimeError(err_msg)
 
         if fetched_name.lower() == artist_name.lower():
-            return mbid
+            return fetched_name, mbid
 
         raise RuntimeError(err_msg)
 
+    def lookup_artist_from_mbid(self, artist_mbid):
+        """ Fetch artist names for validation purposes """
+
+        while True:
+            r = requests.get(f"https://musicbrainz.org/ws/2/artist/%s?fmt=json" % str(artist_mbid))
+            if r.status_code == 404:
+                raise RuntimeError(f"Could not resolve artist mbid {artist_mbid}. Error {r.status_code} {r.text}")
+
+            if r.status_code == 429:
+                sleep(2)
+                continue
+
+            if r.status_code != 200:
+                raise RuntimeError(f"Could not resolve artist name {artist_mbid}. Error {r.status_code} {r.text}")
+
+            break
+
+        return r.json()["name"], artist_mbid
+
     def create(self, inputs):
         self.prompt = inputs["prompt"]
         self.mode = inputs["mode"]
 
         # First parse the prompt
         pp = PromptParser()
         try:
@@ -115,19 +142,21 @@
             raise RuntimeError(f"cannot parse prompt: '{err}'")
 
         if self.mode not in ("easy", "medium", "hard"):
             raise RuntimeError(
                 "Argument mode must be one one easy, medium or hard.")
 
         # Lookup artist names embedded in the prompt
+        artist_names = {}
         for element in prompt_elements:
-            if element["entity"] == "artist" and isinstance(
-                    element["values"][0], str):
-                element["values"][0] = UUID(
-                    self.lookup_artist_name(element["values"][0]))
+            if element["entity"] == "artist":
+                name, mbid = self.lookup_artist(element["values"][0])
+                print(name, mbid)
+                element["values"][0] = mbid
+                artist_names[mbid] = name
 
         # Save descriptions to local storage
         self.local_storage["data_cache"] = {
             "element-descriptions": [],
             "prompt": self.prompt
         }
         self.local_storage["user_feedback"] = []
@@ -158,26 +187,37 @@
                 "hard": (66, 100)
             }
 
             if element["entity"] == "artist":
                 include_sim = False if "nosim" in element["opts"] else True
                 source = LBRadioArtistRecordingElement(
                     element["values"][0],
+                    artist_name=artist_names[element["values"][0]],
                     mode=mode,
                     include_similar_artists=include_sim)
 
             if element["entity"] == "tag":
                 include_sim = False if "nosim" in element["opts"] else True
                 operator = "or" if "or" in element["opts"] else "and"
                 source = LBRadioTagRecordingElement(
-                    element["values"],
+                    [ t.lower() for t in element["values"]],
                     mode=mode,
                     operator=operator,
                     include_similar_tags=include_sim)
 
+            if element["entity"] == "country":
+                if isinstance(element["values"][0], UUID):
+                    source = LBRadioCountryRecordingElement(
+                        mode, 
+                        area_mbid=element["values"][0])
+                else:
+                    source = LBRadioCountryRecordingElement(
+                        mode, 
+                        area_name=element["values"][0])
+
             if element["entity"] == "collection":
                 source = LBRadioCollectionRecordingElement(
                     element["values"][0], mode=mode)
 
             if element["entity"] == "playlist":
                 source = LBRadioPlaylistRecordingElement(element["values"][0],
                                                          mode=mode)
@@ -216,15 +256,15 @@
 
             hate_filter = troi.filters.HatedRecordingsFilterElement()
             hate_filter.set_sources(recs_lookup)
 
             elements.append(hate_filter)
 
         # Finish the pipeline with the element that blends and weighs the streams
-        blend = WeighAndBlendRecordingsElement(weights, max_num_recordings=100)
+        blend = WeighAndBlendRecordingsElement(weights, max_num_recordings=100, max_artist_occurrence=3)
         blend.set_sources(elements)
 
         pl_maker = PlaylistMakerElement(
             patch_slug=self.slug(),
             max_num_recordings=TARGET_NUMBER_OF_RECORDINGS)
         pl_maker.set_sources(blend)
```

### Comparing `troi-2024.2.9.0/troi/patches/lb_radio_classes/collection.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/collection.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/patches/lb_radio_classes/playlist.py` & `troi-2024.4.26.0/troi/patches/lb_radio_classes/playlist.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/patches/periodic_jams.py` & `troi-2024.4.26.0/troi/patches/periodic_jams.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import datetime, timedelta
 
+from troi.patch import Patch
 import troi.filters
 import troi.listenbrainz.feedback
 import troi.listenbrainz.listens
 import troi.listenbrainz.recs
 import troi.musicbrainz.recording_lookup
 from troi import Playlist
 from troi.playlist import PlaylistMakerElement
@@ -30,28 +31,28 @@
     <p>The playlist contains tracks that you've not listened to before (as far as ListenBrainz knows) and that our
     collaborative filtering algorithm believes that you might like.</p>
 
     <p>ListenBrainz creates the Weekly Exploration playlist every monday morning, according to the users' timezone setting.</p>
 """
 
 
-class PeriodicJamsPatch(troi.patch.Patch):
+class PeriodicJamsPatch(Patch):
     """
        Create either daily-jams, weekly-jams or weekly-exploration with this patch.
 
        First, fetch the top recommendations. For daily-jams and weekly-jams, filter out the recently listened tracks.
        For weekly-exploration, filter out tracks that have been listened to.
 
        Then filter out hated tracks and make the playlist.
     """
 
     JAM_TYPES = ("daily-jams", "weekly-jams", "weekly-exploration")
 
-    def __init__(self, args, debug=False):
-        super().__init__(args, debug)
+    def __init__(self, args):
+        super().__init__(args)
 
     @staticmethod
     def inputs():
         """
         Generate a periodic playlist from the ListenBrainz recommended recordings.
 
         \b
@@ -94,22 +95,21 @@
         jam_date = inputs.get('jam_date')
         if jam_date is None:
             jam_date = datetime.utcnow().strftime("%Y-%m-%d %a")
         jam_type = inputs.get('type')
         if jam_type is None:
             jam_type = self.JAM_TYPES[0]
         else:
-            jam_types = jam_type.lower()
+            jam_type = jam_type.lower()
             if jam_type not in self.JAM_TYPES:
-                raise RuntimeError("Jam type must be one of %s" % ", ".join(jam_types))
+                raise RuntimeError("Jam type must be one of %s" % ", ".join(self.JAM_TYPES))
 
         recs = troi.listenbrainz.recs.UserRecordingRecommendationsElement(user_name,
                                                                           "raw",
-                                                                          count=1000,
-                                                                          auth_token=inputs.get("token"))
+                                                                          count=1000)
 
         recent_listens_lookup = troi.listenbrainz.listens.RecentListensTimestampLookup(user_name,
                                                                                        days=2,
                                                                                        auth_token=inputs.get("token"))
         recent_listens_lookup.set_sources(recs)
 
         if jam_type in ("daily-jams", "weekly-jams"):
```

### Comparing `troi-2024.2.9.0/troi/patches/playlist_from_listenbrainz.py` & `troi-2024.4.26.0/troi/patches/playlist_from_listenbrainz.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 
 from troi import Playlist
+from troi.patch import Patch
 from troi.playlist import PlaylistFromJSPFElement
 import troi.musicbrainz.recording_lookup
 
 
-class TransferPlaylistPatch(troi.patch.Patch):
+class TransferPlaylistPatch(Patch):
 
     @staticmethod
     def inputs():
         """
         A dummy patch that retrieves an existing playlist from ListenBrainz or raw JSPF for use in Troi.
 
         \b
```

### Comparing `troi-2024.2.9.0/troi/patches/playlist_from_mbids.py` & `troi-2024.4.26.0/troi/patches/playlist_from_mbids.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from troi.playlist import PlaylistMakerElement
 
 
 class PlaylistFromMBIDsPatch(troi.patch.Patch):
     """
     """
 
-    def __init__(self, args, debug=False):
-        troi.patch.Patch.__init__(self, args, debug)
+    def __init__(self, args):
+        troi.patch.Patch.__init__(self, args)
 
     @staticmethod
     def inputs():
         """
         Make a playlist from a file containing one MBID per line.
 
         \b
```

### Comparing `troi-2024.2.9.0/troi/patches/recs_to_playlist.py` & `troi-2024.4.26.0/troi/patches/recs_to_playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 
 
 class RecommendationsToPlaylistPatch(troi.patch.Patch):
     """
         See below for description
     """
 
-    def __init__(self, args, debug=False):
-        troi.patch.Patch.__init__(self, args, debug)
+    def __init__(self, args):
+        troi.patch.Patch.__init__(self, args)
 
     @staticmethod
     def inputs():
         """
         Save the current recommended tracks for a given user and type (top or similar).
 
         \b
```

### Comparing `troi-2024.2.9.0/troi/patches/top_discoveries_for_year.py` & `troi-2024.4.26.0/troi/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,70 +1,99 @@
-from datetime import datetime
+import importlib
+import inspect
+import logging
+import os
+import traceback
+import sys
 
-import troi.filters
-import troi.listenbrainz.recs
-import troi.musicbrainz.recording_lookup
-import troi.musicbrainz.year_lookup
-import troi.sorts
-from troi import Recording
-from troi.listenbrainz.dataset_fetcher import DataSetFetcherElement
-from troi.playlist import PlaylistShuffleElement, PlaylistMakerElement
+logger = logging.getLogger(__name__)
 
 
-class TopDiscoveries(troi.patch.Patch):
+def discover_patches():
     """
-        See below for description
+        Attempt to load patches from the installed patches dir as well as any patches directory in the current dir.
     """
 
-    NAME = "Top Discoveries of %d for %s"
-    DESC = """<p>
-              This playlist contains the top tracks for %s that were first listened to in %d.
-              </p>
-              <p>
-                For more information on how this playlist is generated, please see our
-                <a href="https://musicbrainz.org/doc/YIM2022Playlists">Year in Music 2022 Playlists</a> page.
-              </p>
-           """
-
-    def __init__(self, args, debug=False):
-        troi.patch.Patch.__init__(self, args, debug)
-
-    @staticmethod
-    def inputs():
-        """
-        Generate a top discoveries playlist for a user.
-
-        \b
-        USER_ID: is a MusicBrainz userid that has an account on ListenBrainz.
-        USER_NAME: is a MusicBrainz username that has an account on ListenBrainz.
-        """
-        return [{"type": "argument", "args": ["user_id"]},
-                {"type": "argument", "args": ["user_name"]}]
-
-    @staticmethod
-    def outputs():
-        return [Recording]
-
-    @staticmethod
-    def slug():
-        return "top-discoveries-for-year"
-
-    @staticmethod
-    def description():
-        return "Generate a top discoveries playlist for a user."
-
-    def create(self, inputs):
-        recs = DataSetFetcherElement(server_url="https://datasets.listenbrainz.org/top-discoveries/json",
-                                     json_post_data=[{ 'user_id': inputs['user_id'] }])
-
-        year = datetime.now().year
-        pl_maker = PlaylistMakerElement(self.NAME % (year, inputs['user_name']),
-                                        self.DESC % (inputs['user_name'], year),
-                                        patch_slug=self.slug(),
-                                        user_name=inputs['user_name'],
-                                        max_artist_occurrence=2)
-        pl_maker.set_sources(recs)
+    patches = discover_patches_from_dir("troi.patches.", os.path.join(os.path.dirname(__file__), "patches"))
+    try:
+        local_patches = discover_patches_from_dir("patches.", "./patches", True)
+    except FileNotFoundError:
+        local_patches = {}
 
-        shuffle = PlaylistShuffleElement()
-        shuffle.set_sources(pl_maker)
+    return  {**patches, **local_patches}
+
+
+def discover_patches_from_dir(module_path, patch_dir, add_dot=False):
+    """
+        Load patches given the appropriate python module path and then file system path. 
+        If add_dot = True, add . to the sys.path and then remove it before this function exists.
+    """
+
+    # This is here to avoid a circular import
+    import troi.patch
+    if add_dot:
+        sys.path.append(".")
+
+    patch_dict = {}
+    for path in os.listdir(patch_dir):
+        if path in ['.', '..']:
+            continue
+
+        if os.path.isdir(os.path.join(patch_dir, path)):
+            continue
+
+        if path.endswith(".py"):
+            try:
+                patch = importlib.import_module(module_path + path[:-3])
+            except ImportError as err:
+                logger.info("Cannot import %s, skipping:" % (path), file=sys.stderr)
+                traceback.print_exc()
+                continue
+
+            for member in inspect.getmembers(patch):
+                if inspect.isclass(member[1]):
+                    if issubclass(member[1], troi.patch.Patch):
+                        if member[1].slug() is not None:
+                            patch_dict[member[1].slug()] = member[1]
+
+    if add_dot:
+        sys.path.pop(-1)
+
+    return patch_dict
+
+
+def recursively_update_dict(source, overrides):
+    """ Updates the `source` dictionary in place and in a recursive fashion. That is unlike
+    dict1.update(dict2) which would simply replace values of keys even in case one of the
+    values is dict, this method will attempt to merge the nested dicts.
+
+    Eg: dict1 - {"a": {"b": 1}}, dict2 - {"a": {"c": 2}}
+    dict1.update(dict2) - {"a": {"c": 2}}
+    recursively_update_dict(dict1, dict2) - {"a": {"b": 1, "c": 2}}
+    """
+    for key, value in overrides.items():
+        if isinstance(value, dict) and value:
+            source[key] = recursively_update_dict(source.get(key, {}), value)
+        else:
+            source[key] = overrides[key]
+    return source
+
+
+def interleave(lists):
+    """ Return a list with all items from the given lists."""
+
+    result = []
+
+    while True:
+        added = False
+        for l in lists:
+            try:
+                result.append(l.pop(0))
+                added = True
+            except IndexError:
+                pass
+
+        if not added:
+            break
+
+    return result
 
-        return shuffle
```

### Comparing `troi-2024.2.9.0/troi/playlist.py` & `troi-2024.4.26.0/troi/playlist.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import logging
 from collections import defaultdict
 import json
 
 
 import requests
 import spotipy
 
 from troi import Recording, Playlist, PipelineError, Element, Artist, Release
 from troi.operations import is_homogeneous
 from troi.print_recording import PrintRecordingList
 from troi.tools.spotify_lookup import submit_to_spotify
-from troi.playlist import PrintRecordingList
+
+logger = logging.getLogger(__name__)
 
 LISTENBRAINZ_SERVER_URL = "https://listenbrainz.org"
 LISTENBRAINZ_API_URL = "https://api.listenbrainz.org"
 LISTENBRAINZ_PLAYLIST_FETCH_URL = LISTENBRAINZ_API_URL + "/1/playlist/"
 LISTENBRAINZ_PLAYLIST_CREATE_URL = LISTENBRAINZ_API_URL + "/1/playlist/create"
 PLAYLIST_TRACK_URI_PREFIX = "https://musicbrainz.org/recording/"
 PLAYLIST_ARTIST_URI_PREFIX = "https://musicbrainz.org/artist/"
@@ -24,14 +26,15 @@
 SUBSONIC_URI_PREFIX = "https://subsonic.org/entity/song/"
 
 # TODO: When resolving a playlist, insert "location" into existing playlist, don't create a new one
 #       And recording lookup needs to be replace with metadata lookup. retire the labs API endpoint!
 #       Artist.mbids is totatlly stupid (see ^^). We need [artists] with "join_phrase" in musicbrainz hash.
 #       All this for the next PR.
 
+
 def _serialize_to_jspf(playlist, created_for=None, track_count=None):
     """
         Serialize a playlist to JSPF.
 
         Arguments:
             created_for: The user name of the user for whom this playlist
                          was created.
@@ -57,17 +60,17 @@
     if not track_count or track_count < 0 or track_count > len(playlist.recordings):
         track_count = len(playlist.recordings)
 
     tracks = []
     for e in playlist.recordings[:track_count]:
         track = {}
         artist_mbids = []
-        if e.artist is not None:
-            artist_mbids = [str(mbid) for mbid in e.artist.mbids or []]
-            track["creator"] = e.artist.name if e.artist else ""
+        if e.artist_credit is not None:
+            artist_mbids = [str(artist.mbid) for artist in e.artist_credit.artists or []]
+            track["creator"] = e.artist_credit.name if e.artist_credit else ""
 
         track["title"] = e.name
         track["identifier"] = "https://musicbrainz.org/recording/" + str(e.mbid)
 
         loc = e.musicbrainz.get("filename", None)
         if loc is not None:
             track["location"] = loc
@@ -175,15 +178,15 @@
     def __str__(self):
         return str(self.playlists)
 
     def read(self, inputs):
 
         for input in inputs:
             if len(input) == 0:
-                print("No recordings or playlists generated to save.")
+                logger.info("No recordings or playlists generated to save.")
                 continue
 
             if isinstance(input[0], Recording):
                 if not is_homogeneous(input):
                     raise TypeError("entity list not homogeneous")
                 self.playlists.append(Playlist(recordings=input))
             elif isinstance(input[0], Playlist):
@@ -195,26 +198,26 @@
 
         return inputs[0]
 
     def print(self):
         """Prints the resultant playlists, one after another."""
 
         if not self.playlists:
-            print("[no playlist(s) generated yet]")
+            logger.error("[no playlist(s) generated yet]")
             return
 
         for i, playlist in enumerate(self.playlists):
             if playlist.name:
-                print("playlist: '%s'" % playlist.name)
+                logger.info("playlist: '%s'" % playlist.name)
             else:
-                print("playlist: %d" % i)
+                logger.info("playlist: %d" % i)
 
             for recording in playlist.recordings:
                 if not recording:
-                    print("[invalid Recording]")
+                    logger.info("[invalid Recording]")
                     continue
                 self.print_recording.print(recording)
 
     def save(self, track_count=None, file_obj=None):
         """Save each playlist to disk, giving each playlist a unique name if none was provided.
 
            Arguments:
@@ -253,15 +256,15 @@
             raise PipelineError("Playlists have not been generated yet.")
 
         playlist_mbids = []
         for playlist in self.playlists:
             if len(playlist.recordings) == 0:
                 continue
 
-            print("submit %d tracks" % len(playlist.recordings))
+            logger.info("submit %d tracks" % len(playlist.recordings))
             if playlist.patch_slug is not None:
                 playlist.add_metadata({"algorithm_metadata": {"source_patch": playlist.patch_slug}})
             r = requests.post(LISTENBRAINZ_PLAYLIST_CREATE_URL,
                               json=_serialize_to_jspf(playlist, created_for),
                               headers={"Authorization": "Token " + str(token)})
             if r.status_code != 200:
                 try:
@@ -468,15 +471,15 @@
             max_num_recordings = self.max_num_recordings
 
         if self.max_artist_occurrence is not None:
             kept = []
             artists = defaultdict(int)
             for r in recordings:
                 keep = True
-                for mbid in r.artist.mbids:
+                for mbid in [ a.mbid for a in r.artist_credit.artists ]:
                     if artists[mbid] >= self.max_artist_occurrence:
                         keep = False
                         break
                     artists[mbid] += 1
 
                 if keep:
                     kept.append(r)
```

### Comparing `troi-2024.2.9.0/troi/service.py` & `troi-2024.4.26.0/troi/service.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/sorts.py` & `troi-2024.4.26.0/troi/sorts.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/tools/area_lookup.py` & `troi-2024.4.26.0/troi/tools/area_lookup.py`

 * *Files identical despite different names*

### Comparing `troi-2024.2.9.0/troi/tools/spotify_lookup.py` & `troi-2024.4.26.0/troi/tools/spotify_lookup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import logging
 from collections import defaultdict
 
 import requests
 import spotipy
 from more_itertools import chunked
 from spotipy import SpotifyException
 
+logger = logging.getLogger(__name__)
+
 SPOTIFY_IDS_LOOKUP_URL = "https://labs.api.listenbrainz.org/spotify-id-from-mbid/json"
 
 
 def lookup_spotify_ids(recordings):
     """ Given a list of Recording elements, try to find spotify track ids from labs api spotify lookup using mbids
     and add those to the recordings. """
     response = requests.post(
@@ -125,26 +128,26 @@
     filtered_recordings = [r for r in playlist.recordings if r.mbid]
 
     _, mbid_spotify_index, spotify_mbid_index = lookup_spotify_ids(filtered_recordings)
     spotify_track_ids = [r.spotify_id for r in filtered_recordings if r.spotify_id]
     if len(spotify_track_ids) == 0:
         return None, None
 
-    print("submit %d tracks" % len(spotify_track_ids))
+    logger.info("submit %d tracks" % len(spotify_track_ids))
 
     playlist_id, playlist_url = None, None
     if existing_url:
         # update existing playlist
         playlist_url = existing_url
         playlist_id = existing_url.split("/")[-1]
         try:
             spotify.playlist_change_details(playlist_id=playlist_id, name=playlist.name, description=playlist.description)
         except SpotifyException as err:
             # one possibility is that the user has deleted the spotify from playlist, so try creating a new one
-            print("provided playlist url has been unfollowed/deleted by the user, creating a new one")
+            logger.info("provided playlist url has been unfollowed/deleted by the user, creating a new one")
             playlist_id, playlist_url = None, None
 
     if not playlist_id:
         # create new playlist
         spotify_playlist = spotify.user_playlist_create(
             user=spotify_user_id,
             name=playlist.name,
```

### Comparing `troi-2024.2.9.0/troi.egg-info/PKG-INFO` & `troi-2024.4.26.0/troi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troi
-Version: 2024.2.9.0
+Version: 2024.4.26.0
 Summary: ListenBrainz' empathic music recommendation/playlisting engine
 Author-email: MetaBrainz Foundation <support@metabrainz.org>
 Project-URL: Homepage, https://github.com/metabrainz/troi-recommendation-playground
 Project-URL: Documentation, https://troi.readthedocs.io/en/latest/
 Project-URL: Releases, https://github.com/metabrainz/troi-recommendation-playground/releases
 Project-URL: Issues, https://tickets.metabrainz.org/secure/RapidBoard.jspa?rapidView=14&projectKey=LB#
 Classifier: Programming Language :: Python :: 3
```

### Comparing `troi-2024.2.9.0/troi.egg-info/SOURCES.txt` & `troi-2024.4.26.0/troi.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
-TODO
 config.py.sample
 pyproject.toml
 .github/workflows/cd.yml
 .github/workflows/ci.yml
 docker/endless.py
 docs/Makefile
 docs/conf.py
@@ -14,54 +13,52 @@
 docs/index.rst
 docs/installation.rst
 docs/introduction.rst
 docs/lb_radio.rst
 docs/listenbrainz-logo.svg
 docs/make.bat
 docs/patches.rst
+docs/requirements.txt
 docs/troi-arguments.rst
 docs/user-guide.rst
 docs/dev/index.rst
 docs/elements/index.rst
 docs/elements/listenbrainz.rst
 docs/elements/musicbrainz.rst
 tests/__init__.py
 tests/test_entities.py
 tests/test_filters.py
 tests/test_operations.py
 tests/test_parser.py
 tests/test_playlist.py
+tests/test_plist.py
 tests/test_sorts.py
-tests/test_splitter.py
 tests/test_tag_utils.py
 tests/test_utils.py
-tests/listenbrainz/test_area_random_recordings.py
 tests/listenbrainz/test_recs.py
 tests/listenbrainz/test_stats.py
-tests/musicbrainz/test_ac_id_lookup.py
-tests/musicbrainz/test_genre_lookup.py
 tests/musicbrainz/test_mbid_mapping.py
 tests/musicbrainz/test_recording_lookup.py
 tests/musicbrainz/test_related_artist_credits.py
-tests/musicbrainz/test_year_lookup.py
 tests/tools/test_area_lookup.py
 troi/__init__.py
 troi/cli.py
 troi/core.py
 troi/filters.py
+troi/logging_utils.py
 troi/loops.py
 troi/operations.py
 troi/parse_prompt.py
 troi/patch.py
 troi/playlist.py
+troi/plist.py
 troi/print_recording.py
 troi/recording_search_service.py
 troi/service.py
 troi/sorts.py
-troi/splitter.py
 troi/utils.py
 troi.egg-info/PKG-INFO
 troi.egg-info/SOURCES.txt
 troi.egg-info/dependency_links.txt
 troi.egg-info/entry_points.txt
 troi.egg-info/requires.txt
 troi.egg-info/top_level.txt
@@ -91,55 +88,47 @@
 troi/content_resolver/formats/wma.py
 troi/content_resolver/model/__init__.py
 troi/content_resolver/model/database.py
 troi/content_resolver/model/directory.py
 troi/content_resolver/model/recording.py
 troi/content_resolver/model/tag.py
 troi/content_resolver/model/unresolved_recording.py
-troi/internal/README.md
-troi/internal/top_new_recordings_you_listened_to_for_year.py
-troi/internal/top_recordings_for_year.py
-troi/internal/top_sitewide_recordings_for_year.py
-troi/internal/yim_patch_runner.py
+troi/external/__init__.py
+troi/external/gpt.py
 troi/listenbrainz/__init__.py
-troi/listenbrainz/area_random_recordings.py
-troi/listenbrainz/dataset_fetcher.py
 troi/listenbrainz/feedback.py
 troi/listenbrainz/listens.py
 troi/listenbrainz/recs.py
 troi/listenbrainz/stats.py
 troi/listenbrainz/user.py
-troi/listenbrainz/yim_user.py
+troi/listenbrainz/unused/README.txt
+troi/listenbrainz/unused/dataset_fetcher.py
 troi/local/periodic_jams_local.py
 troi/local/recording_resolver.py
 troi/musicbrainz/__init__.py
-troi/musicbrainz/artist_credit_id_lookup.py
-troi/musicbrainz/genre_lookup.py
 troi/musicbrainz/mbid_mapping.py
 troi/musicbrainz/mbid_reader.py
 troi/musicbrainz/recording.py
 troi/musicbrainz/recording_lookup.py
 troi/musicbrainz/related_artist_credits.py
-troi/musicbrainz/year_lookup.py
 troi/patches/__init__.py
-troi/patches/area_random_recordings.py
+troi/patches/ai_jams.py
 troi/patches/lb_radio.py
 troi/patches/periodic_jams.py
 troi/patches/periodic_jams_local.py
 troi/patches/playlist_from_listenbrainz.py
 troi/patches/playlist_from_mbids.py
 troi/patches/recs_to_playlist.py
-troi/patches/top_discoveries_for_year.py
-troi/patches/top_missed_recordings_for_year.py
-troi/patches/weekly_flashback_jams.py
-troi/patches/world_trip.py
 troi/patches/lb_radio_classes/__init__.py
 troi/patches/lb_radio_classes/artist.py
 troi/patches/lb_radio_classes/blend.py
 troi/patches/lb_radio_classes/collection.py
+troi/patches/lb_radio_classes/country.py
 troi/patches/lb_radio_classes/playlist.py
 troi/patches/lb_radio_classes/recs.py
 troi/patches/lb_radio_classes/stats.py
 troi/patches/lb_radio_classes/tag.py
+troi/patches/unused/README.txt
+troi/patches/unused/area_random_recordings.py
 troi/tools/__init__.py
 troi/tools/area_lookup.py
 troi/tools/spotify_lookup.py
```

### Comparing `troi-2024.2.9.0/troi.egg-info/requires.txt` & `troi-2024.4.26.0/troi.egg-info/requires.txt`

 * *Files identical despite different names*

