# Comparing `tmp/buildarr_radarr-0.2.5.tar.gz` & `tmp/buildarr_radarr-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildarr_radarr-0.2.5.tar", max compression
+gzip compressed data, was "buildarr_radarr-0.2.6.tar", max compression
```

## Comparing `buildarr_radarr-0.2.5.tar` & `buildarr_radarr-0.2.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0    35149 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/LICENSE
--rw-r--r--   0        0        0    19152 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/README.md
--rw-r--r--   0        0        0      959 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/__init__.py
--rw-r--r--   0        0        0     5409 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/api.py
--rw-r--r--   0        0        0     2853 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/cli.py
--rw-r--r--   0        0        0     6520 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/__init__.py
--rw-r--r--   0        0        0     7751 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/__init__.py
--rw-r--r--   0        0        0     7503 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/__init__.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/__init__.py
--rw-r--r--   0        0        0     4282 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/base.py
--rw-r--r--   0        0        0     1579 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/edition.py
--rw-r--r--   0        0        0     4201 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/indexer_flag.py
--rw-r--r--   0        0        0     3925 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/language.py
--rw-r--r--   0        0        0     3929 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/quality_modifier.py
--rw-r--r--   0        0        0     1646 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/release_group.py
--rw-r--r--   0        0        0     1758 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/release_title.py
--rw-r--r--   0        0        0     3845 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/resolution.py
--rw-r--r--   0        0        0     2184 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/size.py
--rw-r--r--   0        0        0     3713 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/source.py
--rw-r--r--   0        0        0    14236 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/custom_format.py
--rw-r--r--   0        0        0     9107 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/__init__.py
--rw-r--r--   0        0        0     6293 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/base.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/__init__.py
--rw-r--r--   0        0        0     1963 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/aria2.py
--rw-r--r--   0        0        0      897 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/base.py
--rw-r--r--   0        0        0     2385 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/blackhole.py
--rw-r--r--   0        0        0     3302 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/deluge.py
--rw-r--r--   0        0        0     3020 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/downloadstation.py
--rw-r--r--   0        0        0     3758 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/flood.py
--rw-r--r--   0        0        0     3966 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/freebox.py
--rw-r--r--   0        0        0     2606 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/hadouken.py
--rw-r--r--   0        0        0     4880 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/qbittorrent.py
--rw-r--r--   0        0        0     4461 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/rtorrent.py
--rw-r--r--   0        0        0     4806 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/transmission.py
--rw-r--r--   0        0        0     4028 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/utorrent.py
--rw-r--r--   0        0        0     1062 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/vuze.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/__init__.py
--rw-r--r--   0        0        0      843 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/base.py
--rw-r--r--   0        0        0     1567 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/blackhole.py
--rw-r--r--   0        0        0     3010 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/downloadstation.py
--rw-r--r--   0        0        0     3742 2024-03-02 02:54:11.781169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/nzbget.py
--rw-r--r--   0        0        0     3059 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/nzbvortex.py
--rw-r--r--   0        0        0     1627 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/pneumatic.py
--rw-r--r--   0        0        0     4191 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/sabnzbd.py
--rw-r--r--   0        0        0    20652 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/general.py
--rw-r--r--   0        0        0    11560 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/__init__.py
--rw-r--r--   0        0        0    10394 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/base.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/__init__.py
--rw-r--r--   0        0        0     5187 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/base.py
--rw-r--r--   0        0        0     2730 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/filelist.py
--rw-r--r--   0        0        0     3172 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/hdbits.py
--rw-r--r--   0        0        0     1396 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/iptorrents.py
--rw-r--r--   0        0        0     1759 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/nyaa.py
--rw-r--r--   0        0        0     1849 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/passthepopcorn.py
--rw-r--r--   0        0        0     2090 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/rss.py
--rw-r--r--   0        0        0     1724 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/torrentpotato.py
--rw-r--r--   0        0        0     3584 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/torznab.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/usenet/__init__.py
--rw-r--r--   0        0        0      862 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/usenet/base.py
--rw-r--r--   0        0        0     3601 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/usenet/newznab.py
--rw-r--r--   0        0        0     1864 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/util.py
--rw-r--r--   0        0        0    11803 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/__init__.py
--rw-r--r--   0        0        0     7584 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/base.py
--rw-r--r--   0        0        0     2376 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/couchpotato.py
--rw-r--r--   0        0        0     7785 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/exclusions.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/plex/__init__.py
--rw-r--r--   0        0        0      887 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/plex/base.py
--rw-r--r--   0        0        0     1622 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/plex/watchlist.py
--rw-r--r--   0        0        0    16436 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/radarr_import.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/__init__.py
--rw-r--r--   0        0        0     4950 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/base.py
--rw-r--r--   0        0        0     1407 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/list.py
--rw-r--r--   0        0        0     2133 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/popular_list.py
--rw-r--r--   0        0        0     1629 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/user.py
--rw-r--r--   0        0        0    17907 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/media_management.py
--rw-r--r--   0        0        0     8590 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/__init__.py
--rw-r--r--   0        0        0     3485 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/base.py
--rw-r--r--   0        0        0     1165 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/emby_legacy.py
--rw-r--r--   0        0        0     4602 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/kodi_emby.py
--rw-r--r--   0        0        0     1295 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/roksbox.py
--rw-r--r--   0        0        0     1283 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/wdtv.py
--rw-r--r--   0        0        0     9552 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/__init__.py
--rw-r--r--   0        0        0     3835 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/apprise.py
--rw-r--r--   0        0        0     9236 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/base.py
--rw-r--r--   0        0        0     1357 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/boxcar.py
--rw-r--r--   0        0        0     1575 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/custom_script.py
--rw-r--r--   0        0        0     6282 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/discord.py
--rw-r--r--   0        0        0     3341 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/email.py
--rw-r--r--   0        0        0     2492 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/emby_jellyfin.py
--rw-r--r--   0        0        0     2133 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/gotify.py
--rw-r--r--   0        0        0     2474 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/join.py
--rw-r--r--   0        0        0     2558 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/kodi.py
--rw-r--r--   0        0        0     2324 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/mailgun.py
--rw-r--r--   0        0        0     1378 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/notifiarr.py
--rw-r--r--   0        0        0     3821 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/ntfy.py
--rw-r--r--   0        0        0     1781 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/prowl.py
--rw-r--r--   0        0        0     2282 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushbullet.py
--rw-r--r--   0        0        0     3588 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushover.py
--rw-r--r--   0        0        0     4288 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushsafer.py
--rw-r--r--   0        0        0     1984 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/sendgrid.py
--rw-r--r--   0        0        0     2229 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/signal.py
--rw-r--r--   0        0        0     1611 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/simplepush.py
--rw-r--r--   0        0        0     2154 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/slack.py
--rw-r--r--   0        0        0     1414 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/synology_indexer.py
--rw-r--r--   0        0        0     1819 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/telegram.py
--rw-r--r--   0        0        0     2337 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/webhook.py
--rw-r--r--   0        0        0     1107 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/__init__.py
--rw-r--r--   0        0        0    15290 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/delay_profiles.py
--rw-r--r--   0        0        0    26491 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/quality_profiles.py
--rw-r--r--   0        0        0     9661 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/quality.py
--rw-r--r--   0        0        0     2904 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/tags.py
--rw-r--r--   0        0        0     9456 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/settings/ui.py
--rw-r--r--   0        0        0     1012 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/types.py
--rw-r--r--   0        0        0     2061 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/config/util.py
--rw-r--r--   0        0        0     1718 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/exceptions.py
--rw-r--r--   0        0        0      931 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/manager.py
--rw-r--r--   0        0        0     1160 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/plugin.py
--rw-r--r--   0        0        0        0 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/py.typed
--rw-r--r--   0        0        0     5146 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/secrets.py
--rw-r--r--   0        0        0      986 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/types.py
--rw-r--r--   0        0        0     1456 2024-03-02 02:54:11.785169 buildarr_radarr-0.2.5/buildarr_radarr/util.py
--rw-r--r--   0        0        0     2246 2024-03-02 02:54:11.789169 buildarr_radarr-0.2.5/pyproject.toml
--rw-r--r--   0        0        0    20577 1970-01-01 00:00:00.000000 buildarr_radarr-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/LICENSE
+-rw-r--r--   0        0        0    19152 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/README.md
+-rw-r--r--   0        0        0      959 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/__init__.py
+-rw-r--r--   0        0        0     5409 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/api.py
+-rw-r--r--   0        0        0     2853 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/cli.py
+-rw-r--r--   0        0        0     6520 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/config/__init__.py
+-rw-r--r--   0        0        0     7751 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/__init__.py
+-rw-r--r--   0        0        0     7503 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.826120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/__init__.py
+-rw-r--r--   0        0        0     4282 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/base.py
+-rw-r--r--   0        0        0     1579 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/edition.py
+-rw-r--r--   0        0        0     4201 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/indexer_flag.py
+-rw-r--r--   0        0        0     3925 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/language.py
+-rw-r--r--   0        0        0     3929 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/quality_modifier.py
+-rw-r--r--   0        0        0     1646 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/release_group.py
+-rw-r--r--   0        0        0     1758 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/release_title.py
+-rw-r--r--   0        0        0     3845 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/resolution.py
+-rw-r--r--   0        0        0     2184 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/size.py
+-rw-r--r--   0        0        0     3713 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/source.py
+-rw-r--r--   0        0        0    14236 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/custom_format.py
+-rw-r--r--   0        0        0     9107 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/__init__.py
+-rw-r--r--   0        0        0     6293 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/__init__.py
+-rw-r--r--   0        0        0     1963 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/aria2.py
+-rw-r--r--   0        0        0      897 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/base.py
+-rw-r--r--   0        0        0     2385 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/blackhole.py
+-rw-r--r--   0        0        0     3302 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/deluge.py
+-rw-r--r--   0        0        0     3020 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/downloadstation.py
+-rw-r--r--   0        0        0     3758 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/flood.py
+-rw-r--r--   0        0        0     3966 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/freebox.py
+-rw-r--r--   0        0        0     2606 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/hadouken.py
+-rw-r--r--   0        0        0     4880 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/qbittorrent.py
+-rw-r--r--   0        0        0     4461 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/rtorrent.py
+-rw-r--r--   0        0        0     4808 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/transmission.py
+-rw-r--r--   0        0        0     4028 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/utorrent.py
+-rw-r--r--   0        0        0     1062 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/vuze.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/__init__.py
+-rw-r--r--   0        0        0      843 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/base.py
+-rw-r--r--   0        0        0     1567 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/blackhole.py
+-rw-r--r--   0        0        0     3010 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/downloadstation.py
+-rw-r--r--   0        0        0     3742 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/nzbget.py
+-rw-r--r--   0        0        0     3059 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/nzbvortex.py
+-rw-r--r--   0        0        0     1627 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/pneumatic.py
+-rw-r--r--   0        0        0     4191 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/sabnzbd.py
+-rw-r--r--   0        0        0    20644 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/general.py
+-rw-r--r--   0        0        0    11560 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/__init__.py
+-rw-r--r--   0        0        0    10394 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/base.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/__init__.py
+-rw-r--r--   0        0        0     5187 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/base.py
+-rw-r--r--   0        0        0     2730 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/filelist.py
+-rw-r--r--   0        0        0     3172 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/hdbits.py
+-rw-r--r--   0        0        0     1396 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/iptorrents.py
+-rw-r--r--   0        0        0     1759 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/nyaa.py
+-rw-r--r--   0        0        0     1849 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/passthepopcorn.py
+-rw-r--r--   0        0        0     2090 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/rss.py
+-rw-r--r--   0        0        0     1724 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/torrentpotato.py
+-rw-r--r--   0        0        0     3584 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/torznab.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/usenet/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/usenet/base.py
+-rw-r--r--   0        0        0     3601 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/usenet/newznab.py
+-rw-r--r--   0        0        0     1864 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/util.py
+-rw-r--r--   0        0        0    11803 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/__init__.py
+-rw-r--r--   0        0        0     7584 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/base.py
+-rw-r--r--   0        0        0     2376 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/couchpotato.py
+-rw-r--r--   0        0        0     7785 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/exclusions.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/plex/__init__.py
+-rw-r--r--   0        0        0      887 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/plex/base.py
+-rw-r--r--   0        0        0     1622 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/plex/watchlist.py
+-rw-r--r--   0        0        0    16415 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/radarr_import.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/__init__.py
+-rw-r--r--   0        0        0     4950 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/base.py
+-rw-r--r--   0        0        0     1407 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/list.py
+-rw-r--r--   0        0        0     2133 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/popular_list.py
+-rw-r--r--   0        0        0     1629 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/user.py
+-rw-r--r--   0        0        0    17907 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/media_management.py
+-rw-r--r--   0        0        0     8590 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/__init__.py
+-rw-r--r--   0        0        0     3485 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/base.py
+-rw-r--r--   0        0        0     1165 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/emby_legacy.py
+-rw-r--r--   0        0        0     4602 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/kodi_emby.py
+-rw-r--r--   0        0        0     1295 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/roksbox.py
+-rw-r--r--   0        0        0     1283 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/wdtv.py
+-rw-r--r--   0        0        0     9552 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/__init__.py
+-rw-r--r--   0        0        0     3835 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/apprise.py
+-rw-r--r--   0        0        0     9236 2024-04-26 10:57:42.830120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/base.py
+-rw-r--r--   0        0        0     1357 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/boxcar.py
+-rw-r--r--   0        0        0     1575 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/custom_script.py
+-rw-r--r--   0        0        0     6282 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/discord.py
+-rw-r--r--   0        0        0     3341 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/email.py
+-rw-r--r--   0        0        0     2492 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/emby_jellyfin.py
+-rw-r--r--   0        0        0     2133 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/gotify.py
+-rw-r--r--   0        0        0     2474 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/join.py
+-rw-r--r--   0        0        0     2558 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/kodi.py
+-rw-r--r--   0        0        0     2324 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/mailgun.py
+-rw-r--r--   0        0        0     1378 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/notifiarr.py
+-rw-r--r--   0        0        0     3821 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/ntfy.py
+-rw-r--r--   0        0        0     1781 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/prowl.py
+-rw-r--r--   0        0        0     2282 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushbullet.py
+-rw-r--r--   0        0        0     3588 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushover.py
+-rw-r--r--   0        0        0     4288 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushsafer.py
+-rw-r--r--   0        0        0     1984 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/sendgrid.py
+-rw-r--r--   0        0        0     2229 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/signal.py
+-rw-r--r--   0        0        0     1611 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/simplepush.py
+-rw-r--r--   0        0        0     2154 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/slack.py
+-rw-r--r--   0        0        0     1414 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/synology_indexer.py
+-rw-r--r--   0        0        0     1819 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/telegram.py
+-rw-r--r--   0        0        0     2337 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/webhook.py
+-rw-r--r--   0        0        0     1107 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/__init__.py
+-rw-r--r--   0        0        0    15290 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/delay_profiles.py
+-rw-r--r--   0        0        0    26491 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/quality_profiles.py
+-rw-r--r--   0        0        0     9661 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/quality.py
+-rw-r--r--   0        0        0     2904 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/tags.py
+-rw-r--r--   0        0        0     9456 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/settings/ui.py
+-rw-r--r--   0        0        0     1012 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/types.py
+-rw-r--r--   0        0        0     2061 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/config/util.py
+-rw-r--r--   0        0        0     1718 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/exceptions.py
+-rw-r--r--   0        0        0      931 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/manager.py
+-rw-r--r--   0        0        0     1160 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/plugin.py
+-rw-r--r--   0        0        0        0 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/py.typed
+-rw-r--r--   0        0        0     5146 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/secrets.py
+-rw-r--r--   0        0        0      986 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/types.py
+-rw-r--r--   0        0        0     1456 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/buildarr_radarr/util.py
+-rw-r--r--   0        0        0     2246 2024-04-26 10:57:42.834120 buildarr_radarr-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0    20577 1970-01-01 00:00:00.000000 buildarr_radarr-0.2.6/PKG-INFO
```

### Comparing `buildarr_radarr-0.2.5/LICENSE` & `buildarr_radarr-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/README.md` & `buildarr_radarr-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/api.py` & `buildarr_radarr-0.2.6/buildarr_radarr/api.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/cli.py` & `buildarr_radarr-0.2.6/buildarr_radarr/cli.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/edition.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/edition.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/indexer_flag.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/indexer_flag.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/language.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/language.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/quality_modifier.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/quality_modifier.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/release_group.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/release_group.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/release_title.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/release_title.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/resolution.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/resolution.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/size.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/size.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/conditions/source.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/conditions/source.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/custom_formats/custom_format.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/custom_formats/custom_format.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/aria2.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/aria2.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/blackhole.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/blackhole.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/deluge.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/deluge.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/downloadstation.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/downloadstation.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/flood.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/flood.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/freebox.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/freebox.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/hadouken.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/hadouken.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/qbittorrent.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/qbittorrent.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/rtorrent.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/rtorrent.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/transmission.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/transmission.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 
 
 from __future__ import annotations
 
 from typing import Any, List, Literal, Mapping, Optional
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
-from pydantic import validator
+from buildarr.types import BaseEnum, NonEmptyStr, Port
+from pydantic import SecretStr, validator
 
 from .base import TorrentDownloadClient
 
 
 class TransmissionPriority(BaseEnum):
     last = 0
     first = 1
@@ -59,15 +59,15 @@
     """
 
     username: Optional[str] = None
     """
     User name to use when authenticating with the download client, if required.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password to use to authenticate the download client user, if required.
     """
 
     category: Optional[str] = None
     """
     Associate media from Radarr with a category.
```

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/utorrent.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/utorrent.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/torrent/vuze.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/torrent/vuze.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/blackhole.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/blackhole.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/downloadstation.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/downloadstation.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/nzbget.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/nzbget.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/nzbvortex.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/nzbvortex.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/pneumatic.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/pneumatic.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/download_clients/usenet/sabnzbd.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/download_clients/usenet/sabnzbd.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/general.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from ipaddress import IPv4Address
 from typing import Any, Dict, List, Literal, Mapping, Optional, Set, Tuple, Union
 
 import radarr
 
 from buildarr.config import RemoteMapEntry
-from buildarr.types import BaseEnum, NonEmptyStr, Password, Port
+from buildarr.types import BaseEnum, NonEmptyStr, Port
 from packaging.version import Version
 from pydantic import Field, SecretStr
 from typing_extensions import Self
 
 from ...api import radarr_api_client
 from ...secrets import RadarrSecrets
 from ..types import RadarrConfigBase
@@ -262,15 +262,15 @@
     username: Optional[str] = None
     """
     Username for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Radarr to take effect.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the administrator user. Required if authentication is enabled.
 
     Requires a restart of Radarr to take effect.
     """
 
     certificate_validation: CertificateValidation = CertificateValidation.enabled
@@ -357,15 +357,15 @@
 
     username: Optional[str] = None
     """
     Username to authenticate with.
     Only enter if authentication is required by the proxy.
     """
 
-    password: Optional[Password] = None
+    password: Optional[SecretStr] = None
     """
     Password for the proxy user.
     Only enter if authentication is required by the proxy.
     """
 
     ignored_addresses: Set[NonEmptyStr] = set()
     """
```

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/filelist.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/filelist.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/hdbits.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/hdbits.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/iptorrents.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/iptorrents.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/nyaa.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/nyaa.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/passthepopcorn.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/passthepopcorn.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/rss.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/rss.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/torrentpotato.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/torrentpotato.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/torrent/torznab.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/torrent/torznab.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/usenet/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/usenet/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/usenet/newznab.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/usenet/newznab.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/indexers/util.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/indexers/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/couchpotato.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/couchpotato.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/exclusions.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/exclusions.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/plex/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/plex/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/plex/watchlist.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/plex/watchlist.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/radarr_import.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/radarr_import.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,19 @@
 
 from logging import getLogger
 from typing import Any, Dict, Iterable, List, Literal, Mapping, Optional, Set, Union, cast
 
 from buildarr.config import RemoteMapEntry
 from buildarr.state import state
 from buildarr.types import InstanceName, NonEmptyStr
-from pydantic import AnyHttpUrl, Field, PositiveInt, validator
+from pydantic import AnyHttpUrl, Field, PositiveInt, SecretStr, validator
 from typing_extensions import Self
 
 from ....api import api_get
 from ....secrets import RadarrSecrets
-from ....types import ArrApiKey
 from .base import ImportList
 
 logger = getLogger(__name__)
 
 
 class RadarrImportList(ImportList):
     """
@@ -116,15 +115,15 @@
     """
 
     full_url: AnyHttpUrl
     """
     The URL that this Radarr instance will use to connect to the source Radarr instance.
     """
 
-    api_key: Optional[ArrApiKey] = None
+    api_key: Optional[SecretStr] = None
     """
     API key used to access the source Radarr instance.
 
     If a Radarr instance managed by Buildarr is not referenced using `instance_name`,
     this attribute is required.
     """
 
@@ -224,17 +223,17 @@
             List of resource API objects
         """
         return api_get(cls._get_secrets(instance_name), f"/api/v3/{resource_type}")
 
     @validator("api_key", always=True)
     def validate_api_key(
         cls,
-        value: Optional[ArrApiKey],
+        value: Optional[SecretStr],
         values: Mapping[str, Any],
-    ) -> Optional[ArrApiKey]:
+    ) -> Optional[SecretStr]:
         """
         Validate the `api_key` attribute after parsing.
 
         Args:
             value (Optional[str]): `api_key` value.
             values (Mapping[str, Any]): Currently parsed attributes. `instance_name` is checked.
```

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/list.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/list.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/popular_list.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/popular_list.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/lists/trakt/user.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/lists/trakt/user.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/media_management.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/media_management.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/emby_legacy.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/emby_legacy.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/kodi_emby.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/kodi_emby.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/roksbox.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/roksbox.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/metadata/wdtv.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/metadata/wdtv.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/apprise.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/apprise.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/base.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/base.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/boxcar.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/boxcar.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/custom_script.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/custom_script.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/discord.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/discord.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/email.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/email.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/emby_jellyfin.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/emby_jellyfin.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/gotify.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/gotify.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/join.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/join.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/kodi.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/kodi.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/mailgun.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/mailgun.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/notifiarr.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/notifiarr.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/ntfy.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/ntfy.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/prowl.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/prowl.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushbullet.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushbullet.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushover.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushover.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/pushsafer.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/pushsafer.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/sendgrid.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/sendgrid.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/signal.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/signal.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/simplepush.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/simplepush.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/slack.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/slack.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/synology_indexer.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/synology_indexer.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/telegram.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/telegram.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/notifications/webhook.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/notifications/webhook.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/__init__.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/__init__.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/delay_profiles.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/delay_profiles.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/profiles/quality_profiles.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/profiles/quality_profiles.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/quality.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/quality.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/tags.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/tags.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/settings/ui.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/settings/ui.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/types.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/config/util.py` & `buildarr_radarr-0.2.6/buildarr_radarr/config/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/exceptions.py` & `buildarr_radarr-0.2.6/buildarr_radarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/manager.py` & `buildarr_radarr-0.2.6/buildarr_radarr/manager.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/plugin.py` & `buildarr_radarr-0.2.6/buildarr_radarr/plugin.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/secrets.py` & `buildarr_radarr-0.2.6/buildarr_radarr/secrets.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/types.py` & `buildarr_radarr-0.2.6/buildarr_radarr/types.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/buildarr_radarr/util.py` & `buildarr_radarr-0.2.6/buildarr_radarr/util.py`

 * *Files identical despite different names*

### Comparing `buildarr_radarr-0.2.5/pyproject.toml` & `buildarr_radarr-0.2.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [build-system]
 requires = ["poetry-core>=1.3.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "buildarr-radarr"
-version = "0.2.5"
+version = "0.2.6"
 description = "Radarr movie PVR plugin for Buildarr "
 authors = ["Callum Dickinson <callum.dickinson.nz@gmail.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://buildarr.github.io"
 repository = "https://github.com/buildarr/buildarr-radarr"
 documentation = "https://buildarr.github.io/plugins/radarr"
 keywords = [
```

### Comparing `buildarr_radarr-0.2.5/PKG-INFO` & `buildarr_radarr-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildarr-radarr
-Version: 0.2.5
+Version: 0.2.6
 Summary: Radarr movie PVR plugin for Buildarr 
 Home-page: https://buildarr.github.io
 License: GPL-3.0-or-later
 Keywords: buildarr,radarr
 Author: Callum Dickinson
 Author-email: callum.dickinson.nz@gmail.com
 Requires-Python: >=3.8,<4.0
```

