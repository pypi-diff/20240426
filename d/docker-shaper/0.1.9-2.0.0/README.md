# Comparing `tmp/docker_shaper-0.1.9.tar.gz` & `tmp/docker_shaper-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker_shaper-0.1.9.tar", max compression
+gzip compressed data, was "docker_shaper-2.0.0.tar", max compression
```

## Comparing `docker_shaper-0.1.9.tar` & `docker_shaper-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,12 @@
--rw-r--r--   0        0        0     3084 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/Readme.md
--rw-r--r--   0        0        0        0 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/docker_shaper/__init__.py
--rwxr-xr-x   0        0        0     1459 2023-07-21 09:44:02.034044 docker_shaper-0.1.9/docker_shaper/cli.py
--rw-r--r--   0        0        0    41373 2023-07-21 19:30:35.081819 docker_shaper-0.1.9/docker_shaper/dynamic.py
--rw-r--r--   0        0        0    12075 2023-07-21 19:35:11.395918 docker_shaper-0.1.9/docker_shaper/server.py
--rw-r--r--   0        0        0        0 2023-07-21 09:44:02.038044 docker_shaper-0.1.9/docker_shaper/static/__init__.py
--rw-r--r--   0        0        0   232914 2023-07-21 15:40:59.051386 docker_shaper-0.1.9/docker_shaper/static/bootstrap.min.css
--rw-r--r--   0        0        0   589307 2023-07-21 15:40:59.055386 docker_shaper-0.1.9/docker_shaper/static/bootstrap.min.css.map
--rw-r--r--   0        0        0     1001 2023-07-21 15:40:59.059386 docker_shaper-0.1.9/docker_shaper/static/docker_shaper.js
--rw-r--r--   0        0        0        0 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-21 15:40:59.059386 docker_shaper-0.1.9/docker_shaper/templates/base.html
--rw-r--r--   0        0        0      312 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/containers.html
--rw-r--r--   0        0        0     1362 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/dashboard.html
--rw-r--r--   0        0        0      299 2023-07-21 09:44:02.062044 docker_shaper-0.1.9/docker_shaper/templates/images.html
--rw-r--r--   0        0        0      315 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/messages.html
--rw-r--r--   0        0        0      315 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/rules.html
--rw-r--r--   0        0        0      317 2023-07-21 09:44:02.066044 docker_shaper-0.1.9/docker_shaper/templates/volumes.html
--rw-r--r--   0        0        0     9586 2023-07-21 17:39:57.663751 docker_shaper-0.1.9/docker_shaper/utils.py
--rw-r--r--   0        0        0     2296 2023-07-21 09:44:02.074044 docker_shaper-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3888 1970-01-01 00:00:00.000000 docker_shaper-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     4558 2024-04-19 07:43:31.743076 docker_shaper-2.0.0/Readme.md
+-rw-r--r--   0        0        0       74 2024-04-26 12:49:34.686323 docker_shaper-2.0.0/docker_shaper/__init__.py
+-rwxr-xr-x   0        0        0     1355 2024-04-24 08:49:58.546578 docker_shaper-2.0.0/docker_shaper/cli.py
+-rw-r--r--   0        0        0    48946 2024-04-23 11:24:51.755605 docker_shaper-2.0.0/docker_shaper/docker_state.py
+-rw-r--r--   0        0        0    34839 2024-04-26 13:21:36.086252 docker_shaper-2.0.0/docker_shaper/dynamic.py
+-rwxr-xr-x   0        0        0      709 2023-11-13 15:44:58.815461 docker_shaper-2.0.0/docker_shaper/headless_examples/docker_events.py
+-rwxr-xr-x   0        0        0     6398 2023-10-26 10:22:54.409443 docker_shaper-2.0.0/docker_shaper/headless_examples/docker_prune.py
+-rwxr-xr-x   0        0        0    12458 2024-04-24 09:42:35.488952 docker_shaper-2.0.0/docker_shaper/headless_examples/dockermon.py
+-rw-r--r--   0        0        0    21381 2024-04-26 12:37:07.471713 docker_shaper-2.0.0/docker_shaper/server.py
+-rw-r--r--   0        0        0     7683 2024-04-24 09:42:37.260960 docker_shaper-2.0.0/docker_shaper/utils.py
+-rw-r--r--   0        0        0     2408 2024-04-26 13:22:39.278568 docker_shaper-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5435 1970-01-01 00:00:00.000000 docker_shaper-2.0.0/PKG-INFO
```

### Comparing `docker_shaper-0.1.9/docker_shaper/cli.py` & `docker_shaper-2.0.0/docker_shaper/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 #!/usr/bin/env python3
 
 """Docker Shaper command line interface
 """
 
 from argparse import ArgumentParser
 from argparse import Namespace as Args
-from pathlib import Path
+
+from trickkiste.logging_helper import apply_common_logging_cli_args, setup_logging
 
 from docker_shaper import server
-from docker_shaper.utils import setup_logging
 
 
 def parse_args() -> Args:
     """Cool git like multi command argument parser"""
     parser = ArgumentParser()
-    parser.add_argument(
-        "--log-level",
-        "-l",
-        choices=["ALL_DEBUG", "DEBUG", "INFO", "WARN", "ERROR", "CRITICAL"],
-        help="Sets the logging level - ALL_DEBUG sets all other loggers to DEBUG, too",
-        type=str.upper,
-        default="INFO",
-    )
+
+    apply_common_logging_cli_args(parser)
+
+    # parser.add_argument(
+    # "--log-level",
+    # "-l",
+    # choices=["ALL_DEBUG", "DEBUG", "INFO", "WARN", "WARNING", "ERROR", "CRITICAL"],
+    # help="Sets the logging level - ALL_DEBUG sets all other loggers to DEBUG, too",
+    # type=str.upper,
+    # default="INFO",
+    # )
     parser.set_defaults(func=lambda *_: parser.print_usage())
     subparsers = parser.add_subparsers(help="available commands", metavar="CMD")
 
     parser_serve = subparsers.add_parser("serve")
     parser_serve.set_defaults(func=fn_serve)
 
-    parser_no_serve = subparsers.add_parser("no-serve")
-    parser_no_serve.set_defaults(func=fn_no_serve)
-
     return parser.parse_args()
 
 
 def fn_serve(args: Args) -> None:
     """Entry point for event consistency check"""
     setup_logging(args.log_level)
-    server.serve()
+    # logging.getLogger().setLevel(logging.WARNING)
+    # log().setLevel(logging.DEBUG)
 
-
-def fn_no_serve(args: Args) -> None:
-    """Entry point for event consistency check"""
-    setup_logging(args.log_level)
-    server.no_serve()
+    server.serve()
 
 
 def main() -> int:
     """Entry point for everything else"""
     (args := parse_args()).func(args)
     return 0
```

### Comparing `docker_shaper-0.1.9/docker_shaper/dynamic.py` & `docker_shaper-2.0.0/docker_shaper/docker_state.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,334 +1,86 @@
 #!/usr/bin/env python3
 
 """Functionality that might change during runtime
 """
+# pylint: disable=invalid-name  # names come from aiodocker, not my fault
+# pylint: disable=too-many-instance-attributes,too-few-public-methods
+# pylint: disable=too-many-branches,too-many-return-statements
+# pylint: disable=too-many-lines
+# pylint: disable=too-many-arguments
+# pylint: disable=fixme
+# pylint: disable=import-error  # no clue why..
+
 import asyncio
+import json
 import logging
-import os
 import re
 import time
-from collections import Counter
+from asyncio import StreamReader
+from asyncio.subprocess import PIPE, create_subprocess_exec
+from collections.abc import (
+    AsyncIterator,
+    Iterable,
+    Mapping,
+    MutableMapping,
+    MutableSequence,
+    Sequence,
+)
 from contextlib import suppress
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from datetime import datetime
-from subprocess import CalledProcessError
-from typing import MutableMapping, MutableSequence, Optional, Set, Tuple
+from pathlib import Path
+from typing import Any, ClassVar, Literal, Type, TypeAlias, cast
 
+import aiohttp
 from aiodocker import Docker, DockerError
-from dateutil import tz
-from flask_table import Col, Table
-from quart import redirect, render_template, request, url_for, websocket
-
-from docker_shaper.utils import (
-    age_str,
-    date_from,
-    date_str,
-    dur_str,
-    impatient,
-    process_output,
-    setup_introspection_on_signal,
-)
+from aiodocker.containers import DockerContainer
+from aiodocker.networks import DockerNetwork
+from aiodocker.volumes import DockerVolume
+from pydantic import BaseModel, ConfigDict, Json, model_validator
+from trickkiste.misc import date_from
+
+MessageType: TypeAlias = Literal[
+    "exception",
+    "error",
+    "warning",
+    "info",
+    "client_disconnect",
+    "reference_update",
+    "reference_del",
+    "container_add",
+    "container_del",
+    "container_update",
+    "image_add",
+    "image_del",
+    "image_update",
+    "volume_add",
+    "volume_del",
+    "network_add",
+    "network_del",
+]
+MType: TypeAlias = tuple[MessageType, str, None | object]
+ImageIdent: TypeAlias = str | tuple[None | str, str, str]
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper")
 
 
-@dataclass
-class GlobalState:
-    """The dirty globally shared state of docker-shaper"""
-
-    intervals: MutableMapping[str, float]
-    image_ids: MutableMapping[str, object]
-    images: MutableMapping[str, object]
-    images_crawled: bool
-    containers: MutableMapping[str, object]
-    containers_crawled: bool
-    volumes: MutableMapping[str, object]
-    volumes_crawled: bool
-    event_horizon: int
-    last_referenced: MutableMapping[str, MutableSequence[int]]
-    tag_rules: MutableMapping[str, int]
-    extra_links: MutableMapping[str, int]
-    messages: MutableSequence[Tuple[int, str, str]]
-    switches: MutableMapping[str, bool]
-    hostname: str
-    expiration_ages: MutableMapping[str, int]
-    update_mqueues: Set[asyncio.Queue]
-
-    def __init__(self):
-        self.intervals = {
-            "state": 2,
-            "image_stats": 2,
-            "image_update": 2,
-            "container_update": 2,
-            "container_stats": 2,
-            "cleanup": 3600,
-        }
-        self.cleanup_fuse = 0
-        self.image_ids = {}
-        self.images = {}
-        self.images_crawled = False
-        self.containers = {}
-        self.containers_crawled = False
-        self.volumes = {}
-        self.volumes_crawled = False
-
-        self.event_horizon = int(time.time())
-        self.last_referenced = {}
-        self.tag_rules = {}
-        self.counter = 0
-        self.extra_links = {}
-        self.switches = {}
-        self.messages = []
-        self.hostname = open("/etc/hostname").read().strip()
-        self.expiration_ages = {}
-        self.update_mqueues = set()
-
-    def new_update_queue(self) -> asyncio.Queue:
-        """Creates and returns a new message queue"""
-        mqueue = asyncio.Queue()
-        self.update_mqueues.add(mqueue)
-        log().info("new connection (%d)", len(self.update_mqueues))
-        return mqueue
-
-    def remove_queue(self, mqueue: asyncio.Queue) -> None:
-        """Removes an existing queue from message queues"""
-        self.update_mqueues.remove(mqueue)
-        del mqueue
-        log().info("closed connection (%d)", len(self.update_mqueues))
-
-    async def inform(self, message: str) -> None:
-        """Send a message to all connected message queues"""
-        for mqueue in self.update_mqueues:
-            await mqueue.put(message)
-
-
 def short_id(docker_id: str) -> str:
     """Return the 10-digit variant of a long docker ID
     >>> short_id("sha256:abcdefghijklmnop")
     'abcdefghij'
     """
-    if not docker_id:
+    if not docker_id or not is_uid(docker_id):
         return docker_id
-    assert is_uid(docker_id)
     return docker_id[7:17] if docker_id.startswith("sha256:") else docker_id[:10]
 
 
-@impatient
-def id_from(name: str) -> Optional[str]:
-    """Looks up name using `docker inspect` and returns a 10 digit Docker ID"""
-    with suppress(CalledProcessError):
-        log().debug("resolve %s", name)
-        return short_id(
-            name
-            if name.startswith("sha256:")
-            else process_output(f"docker inspect --format='{{{{.Id}}}}' {name}")
-        )
-    return None
-
-
-def lookup_id(ids: MutableMapping[str, Optional[str]], name: str) -> Optional[str]:
-    """Looks up a given @name in @ids and resolves it first if not yet given"""
-    if name not in ids:
-        ids[name] = id_from(name)
-    return ids[name]
-
-
-def event_from(line: str):
-    """Reads a line from event log and turns it into a tuple containing the data"""
-    match = re.match(r"^(.*) \((.*)\)$", line)
-    assert match, f"line did not match the expected format: {line!r}"
-    cmd, params = match.groups()
-    timestamp, object_type, operator, *cmd, uid = cmd.split(" ")
-    assert len(timestamp) == 35
-    assert (operator in {"exec_create:", "exec_start:", "health_status:"}) == bool(
-        cmd
-    ), f"{operator=} {cmd=} {line=}"
-    assert object_type in {
-        "container",
-        "network",
-        "image",
-        "volume",
-        "builder",
-    }, f"{object_type}"
-    assert operator in {
-        "create",
-        "destroy",
-        "attach",
-        "connect",
-        "disconnect",
-        "start",
-        "die",
-        "pull",
-        "push",
-        "tag",
-        "save",
-        "delete",
-        "untag",
-        "prune",
-        "commit",
-        "unpause",
-        "resize",
-        "exec_die",
-        "exec_create:",
-        "exec_start:",
-        "health_status:",
-        "mount",
-        "unmount",
-        "archive-path",
-        "rename",
-        "kill",
-        "stop",
-        "top",
-        "pause",
-    }, f"{operator}"
-    assert len(uid) == 64 or (object_type, operator) in {
-        ("image", "pull"),
-        ("image", "push"),
-        ("image", "tag"),
-        ("image", "untag"),
-        ("image", "save"),
-        ("image", "delete"),
-        ("image", "prune"),
-        ("volume", "prune"),
-        ("volume", "create"),
-        ("container", "prune"),
-        ("network", "prune"),
-        ("builder", "prune"),
-    }, f"{len(uid)=} {(object_type, operator)}"
-    return (
-        int(
-            datetime.strptime(
-                f"{timestamp[:26]}{timestamp[-6:]}", "%Y-%m-%dT%H:%M:%S.%f%z"
-            ).timestamp()
-        ),
-        object_type,
-        operator,
-        cmd,
-        uid,
-        dict(p.split("=") for p in params.split(", ")),
-    )
-
-
-async def handle_docker_event_line(global_state: GlobalState, line: str, docker_client) -> None:
-    """Read a `docker events` line and maintain the last-used information"""
-
-    tstamp, object_type, operator, _cmd, uid, params = event_from(line)
-
-    # print(f"{object_type} {operator} {uid} {params['name']}")
-    # print("XXXX", line)
-
-    if (object_type, operator) in {
-        ("image", "tag"),
-        ("image", "pull"),
-        ("container", "create"),
-    }:
-        ident = params.get("image") or params["name"]
-        log().info(
-            "docker event %s %s %s ident=%s _uid=%s",
-            datetime.fromtimestamp(tstamp),
-            object_type,
-            operator,
-            ident,
-            uid,
-        )
-        global_state.event_horizon = min(global_state.event_horizon, tstamp)
-        register_reference(ident, tstamp, global_state)
-
-    if object_type == "container":
-        if operator in {
-            "create",
-        }:
-            container = await container_from(docker_client, uid)
-            assert container
-            await register_container(container, global_state)
-            return
-
-        if operator in {
-            "destroy",
-        }:
-            # not needed, since watch_container() already takes care..
-            # unregister_container(uid, global_state)
-
-            if await container_from(docker_client, uid):
-                report(global_state, "error", f"container {uid} still alive after {operator}")
-            return
-
-        if operator in {
-            "exec_create:",
-            "exec_start:",
-            "exec_die",
-            "kill",
-            "start",
-            "attach",
-            "top",
-            "prune",
-            "die",
-            "stop",
-            "resize",
-            "archive-path",
-        }:
-            if (
-                operator not in {"prune", "destroy"}
-                and not await container_from(docker_client, uid)
-                and global_state.containers_crawled
-            ):
-                report(
-                    global_state,
-                    "error",
-                    f"operator is {operator} but container {uid} does not exist",
-                )
-            return
-        # del global_state.images[ident]
-        # del global_state.volumes[ident]
-
-    elif object_type == "image":
-        if operator in {
-            "pull",
-        }:
-            await register_image(global_state, await image_from(docker_client, uid))
-            return
-
-        if operator in {
-            "tag",
-        }:
-            await update_image_registration(global_state, docker_client, params["name"])
-            return
-
-        if operator in {
-            "untag",
-            "prune",
-            "push",
-            "delete",
-        }:
-            await update_image_registration(global_state, docker_client, params["name"])
-            return
-
-    elif object_type == "network":
-        if operator in {
-            "connect",
-            "disconnect",
-        }:
-            return
-
-    elif object_type == "volume":
-        if operator in {
-            "create",
-            "mount",
-            "unmount",
-            "destroy",
-        }:
-            return
-
-    log().warning("unknown type/operator %s %s", object_type, operator)
-
-
 def is_uid(ident: str) -> bool:
     """
     >>> is_uid("sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
     True
     >>> is_uid("48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
     True
     >>> is_uid("48a3535fe2")
@@ -339,866 +91,1379 @@
     return bool(
         ident.startswith("sha256:")
         or re.match("^[0-9a-f]{64}$", ident)
         or re.match("^[0-9a-f]{10}$", ident)
     )
 
 
-def unique_ident(ident: str) -> str:
+def unique_ident(ident: str) -> ImageIdent:
     """Return a short Id if ident is a unique id and leave it as it is otherwise
     >>> unique_ident("sha256:48a3535fe27fea1ac6c2f41547770d081552c54b2391c2dda99e2ad87561a4f2")
     '48a3535fe2'
     >>> unique_ident("914463316976.dkr.ecr.eu-central-1.amazonaws.com/user_admin_panel:958")
-    '914463316976.dkr.ecr.eu-central-1.amazonaws.com/user_admin_panel:958'
+    ('914463316976.dkr.ecr.eu-central-1.amazonaws.com', 'user_admin_panel', '958')
+    >>> unique_ident("https://abcd.def:1234/nested/structure/base_name:12345")
+    ('https://abcd.def:1234/nested/structure', 'base_name', '12345')
     """
-    return short_id(ident) if is_uid(ident) else ident
+    if is_uid(ident):
+        return short_id(ident)
+    *maybe_reg, tagged_name = ident.rsplit("/", maxsplit=1)
+    name, *maybe_tag = tagged_name.split(":")
+    assert len(maybe_tag) in {0, 1}, ident
+    return maybe_reg[0] if maybe_reg else None, name, maybe_tag[0] if maybe_tag else "latest"
+
+
+class Deserializable(BaseModel):
+    """Implements a generic deserializer with explicitly ignorable keys"""
+
+    model_config = ConfigDict(extra="forbid")
+    IgnoreKeys: ClassVar[set[str]] = set()
+
+    @model_validator(mode="before")
+    @classmethod
+    def remove_ignored(
+        cls: Type["Deserializable"], values: Json[dict[str, Any]]
+    ) -> Json[dict[str, Any]]:
+        """Removes unwanted keys"""
+        return {key: value for key, value in values.items() if key not in cls.IgnoreKeys}
+
+
+class ContainerShowConfig(Deserializable):
+    """Wraps information coming from container.show().config"""
+
+    Labels: Mapping[str, str]
+    Volumes: None | Mapping[str, object]
+    Cmd: None | Sequence[str]
+
+    IgnoreKeys = {
+        "User",
+        "AttachStderr",
+        "Env",
+        "AttachStdin",
+        "Domainname",
+        "Tty",
+        "OpenStdin",
+        "WorkingDir",
+        "Hostname",
+        "Entrypoint",
+        "AttachStdout",
+        "OnBuild",
+        "Image",
+        "StdinOnce",
+        "ExposedPorts",
+        "Healthcheck",
+        "Shell",
+    }
 
 
-def register_reference(ident: str, timestamp: int, global_state) -> None:
-    effective_ident = unique_ident(ident)
-    if effective_ident not in global_state.last_referenced:
-        global_state.last_referenced[effective_ident] = [
-            0,
-            expiration_age_from_ident(effective_ident, global_state),
-        ]
-
-    # increase last reference date if applicable
-    global_state.last_referenced[effective_ident][0] = max(
-        global_state.last_referenced[effective_ident][0] or 0, timestamp
-    )
+class ContainerShowState(Deserializable):
+    """Wraps information coming from container.show().state"""
 
+    Running: bool
+    Status: str
+    OOMKilled: bool
+    Dead: bool
+    Error: str
+    Pid: int
+    ExitCode: int
+    StartedAt: datetime
+    FinishedAt: datetime
+    Health: None | Mapping[str, object] = None
+
+    IgnoreKeys = {"Paused", "Restarting"}
+
+
+class ContainerMount(Deserializable):
+    """Wraps information for elements coming from container.show().Mounts"""
+
+    Name: None | str = None
+    Type: str
+    Source: str
+    Destination: str
+    Driver: None | str = None
+    Mode: str
+    RW: bool
+
+    IgnoreKeys = {"Propagation"}
+
+
+class ContainerShow(Deserializable):
+    """Wraps information coming from container.show()"""
+
+    Id: str
+    Name: str
+    Created: datetime
+    Image: str
+    Mounts: Sequence[ContainerMount]
+    State: ContainerShowState
+    Args: Sequence[str]
+    Config: ContainerShowConfig
+    HostConfig: Mapping[str, object]
+    IgnoreKeys = {
+        "RestartCount",
+        "Path",
+        "Platform",
+        "MountLabel",
+        "AppArmorProfile",
+        "ExecIDs",
+        "ProcessLabel",
+        "Driver",
+        "ResolvConfPath",
+        "HostnamePath",
+        "HostsPath",
+        "NetworkSettings",
+        "GraphDriver",
+        "LogPath",
+        "AppArmorLabel",
+    }
 
-def expiration_age_from_ident(ident: str, global_state: GlobalState) -> int:
-    # TODO: distinguish between container, image and volume
-    if is_uid(ident):
-        return global_state.expiration_ages["tag_default"]
+    def __str__(self) -> str:
+        return (
+            f"{self.Id[:10]}{self.Name:<20s}"
+            f" {self.State.Status} {str(self.Created)[:19]} {self.Config.Volumes}"
+        )
 
-    effective_ident = unique_ident(ident)
+    @property
+    def status(self) -> str:
+        """Status shortcut"""
+        return self.State.Status
 
-    matching_rules = tuple(
-        (regex, age)
-        for regex, age in global_state.tag_rules.items()
-        if re.match(regex, effective_ident)
-    )
 
-    if len(matching_rules) == 1:
-        return matching_rules[0][1]
-    if not matching_rules:
-        log().warn("No rule found for %r", ident)
-    else:
-        log().error("Multiple rules found for %s:", ident)
-        for rule in matching_rules:
-            log().error("  %s:", rule[0])
+class ContainerCpuStatsCpuUsage(Deserializable):
+    """Wraps information coming from container.stats().cpu_stats.cpu_usage"""
 
-    return global_state.expiration_ages["tag_unknown"]
+    total_usage: int
+    IgnoreKeys = {"usage_in_kernelmode", "usage_in_usermode"}
 
 
-@impatient
-def expired(ident: str, global_state, now: int, extra_date: int = 0) -> bool:
-    if ident not in global_state.last_referenced:
-        log().debug("expired(%s): no reference yet", ident)
+class ContainerCpuStats(Deserializable):
+    """Wraps information coming from container.stats().cpu_stats"""
 
-    if ident != unique_ident(ident):
-        log().error("expired() called with non-uniform identifier: %s", ident)
+    cpu_usage: ContainerCpuStatsCpuUsage
+    system_cpu_usage: None | int = None
+    online_cpus: None | int = None
+    throttling_data: None | Mapping[str, int]
 
-    # TODO
-    last_referenced, expiration_age = global_state.last_referenced.setdefault(
-        ident, [None, expiration_age_from_ident(ident, global_state)]
-    )
 
-    effective_age = now - max(
-        last_referenced or 0,
-        global_state.event_horizon,
-        extra_date,
-    )
-    return effective_age > expiration_age, last_referenced, expiration_age
+class ContainerMemoryStats(Deserializable):
+    """Wraps information coming from container.stats().memory_stats"""
 
+    stats: None | Mapping[str, int] = None
+    limit: None | int = None
+    usage: None | int = None
 
-def jobname_from(binds):
-    candidates = [
-        d.replace("/home/jenkins/workspace/", "").replace("/checkout", "")
-        for b in binds or []
-        for d in (b.split(":")[0],)
-        if "workspace" in d
-    ]
-    if not len(candidates) == len(set(candidates)):
-        print(binds)
-    return candidates and candidates[0] or "--"
-
-
-def cpu_perc(cpu_stats, last_cpu_stats):
-    if not (
-        cpu_stats
-        and "system_cpu_usage" in cpu_stats
-        and last_cpu_stats
-        and "system_cpu_usage" in last_cpu_stats
-    ):
-        return 0
-    return (
-        (cpu_stats["cpu_usage"]["total_usage"] - last_cpu_stats["cpu_usage"]["total_usage"])
-        / (cpu_stats["system_cpu_usage"] - last_cpu_stats["system_cpu_usage"])
-        * cpu_stats["online_cpus"]
-    )
+
+class ContainerStats(Deserializable):
+    """Wraps information coming from container.show()"""
+
+    cpu_stats: ContainerCpuStats
+    memory_stats: ContainerMemoryStats
+    IgnoreKeys = {
+        "preread",
+        "id",
+        "read",
+        "name",
+        "num_procs",
+        "blkio_stats",
+        "pids_stats",
+        "storage_stats",
+        "precpu_stats",
+        "networks",
+    }
 
 
-def label_filter(label_values):
-    return ",".join(
-        w.replace("artifacts.lan.tribe29.com:4000", "A")
-        for key, l in label_values.items()
-        if key
-        in (
-            "org.tribe29.base_image",
-            "org.tribe29.cmk_branch",
-            "org.tribe29.cmk_edition_short",
-            "org.tribe29.cmk_hash",
-            "org.tribe29.cmk_version",
+@dataclass
+class Container:
+    """Gathers information about a Docker container"""
+
+    raw_container: DockerContainer
+    show: None | ContainerShow = None
+    stats: None | ContainerStats = None
+    last_stats: None | ContainerStats = None
+
+    def __str__(self) -> str:
+        image_str = "" if not self.show else f", image={short_id(self.show.Image)}"
+        status_str = "" if not self.show else f", status={self.show.State.Status}"
+        return f"Container({self.short_id}, name={self.name}{image_str}{status_str})"
+
+    @property
+    def id(self) -> str:
+        """Container ID"""
+        return self.raw_container.id
+
+    @property
+    def short_id(self) -> str:
+        """First 10 digits of Id"""
+        return self.raw_container.id[:10]
+
+    @property
+    def name(self) -> str:
+        """Shortcut for name of image (without leading /)"""
+        if not self.show:
+            return "(unknown)"
+        return self.show.Name[1:]
+
+    @property
+    def status(self) -> str:
+        """Status shortcut"""
+        if not self.show:
+            return "(unknown)"
+        return self.show.State.Status
+
+    @property
+    def created_at(self) -> datetime:
+        """Shortcut to self.show.Created"""
+        assert self.show
+        return self.show.Created
+
+    @property
+    def started_at(self) -> datetime:
+        """Shortcut to self.show.State.StartedAt"""
+        assert self.show
+        return self.show.State.StartedAt
+
+    @property
+    def finished_at(self) -> datetime:
+        """Shortcut to self.show.State.FinishedAt"""
+        assert self.show
+        return self.show.State.FinishedAt
+
+    @property
+    def image(self) -> str:
+        """Shortcut to self.show.State.FinishedAt"""
+        assert self.show
+        return self.show.Image
+
+    @property
+    def pid(self) -> int:
+        """Shortcut to self.show.State.Pid"""
+        assert self.show
+        return self.show.State.Pid
+
+    @property
+    def labels(self) -> Mapping[str, str]:
+        """Shortcut to self.show.State.Pid"""
+        assert self.show
+        return self.show.Config.Labels
+
+    @property
+    def cmd(self) -> None | Sequence[str]:
+        """Shortcut to self.show.State.Pid"""
+        assert self.show
+        return self.show.Config.Cmd
+
+    @property
+    def host_config(self) -> Mapping[str, object]:
+        """Shortcut to self.show.HostConfig"""
+        assert self.show
+        return self.show.HostConfig
+
+    def cpu_usage(self) -> float:
+        """Returns actual CPU usage of container"""
+        if not self.stats or not self.last_stats:
+            return 0
+        cpu_stats, last_cpu_stats = self.stats.cpu_stats, self.last_stats.cpu_stats
+        if (
+            (cpu_stats := self.stats.cpu_stats) is None
+            or (last_cpu_stats := self.last_stats.cpu_stats) is None
+            or cpu_stats.system_cpu_usage is None
+            or last_cpu_stats.system_cpu_usage is None
+            or cpu_stats.online_cpus is None
+        ):
+            return 0
+        return (
+            ((cpu_stats.cpu_usage.total_usage or 0) - (last_cpu_stats.cpu_usage.total_usage or 0))
+            / (cpu_stats.system_cpu_usage - last_cpu_stats.system_cpu_usage)
+            * cpu_stats.online_cpus
         )
-        for w in l.split()
-        if not (w.startswith("sha256") or len(w) == 64)
-    )
 
+    def mem_usage(self) -> int:
+        """Returns actual memory usage of container"""
+        if not self.stats:
+            return 0
+        return self.stats.memory_stats.usage or 0
+
+
+class ImageInspect(Deserializable):
+    """Wraps information docker.image.inspect"""
+
+    Id: str
+    RepoTags: Sequence[str]
+    RepoDigests: Sequence[str]
+    Created: datetime
+    Parent: str
+
+    IgnoreKeys = {
+        "RootFS",
+        "ContainerConfig",
+        "Os",
+        "Author",
+        "Container",
+        "Config",
+        "Comment",
+        "Architecture",
+        "DockerVersion",
+        "Size",
+        "Metadata",
+        "VirtualSize",
+        "GraphDriver",
+    }
 
-async def dump_global_state(global_state: GlobalState):
-    global_state.counter += 1
-    print(f"STATE: ========================================================")
-    print(f"STATE: frame counter: {global_state.counter}")
-    print(
-        f"STATE: intervals:     {', '.join('='.join(map(str, i)) for i in global_state.intervals.items())}"
-    )
-    print(f"STATE: images:        {len(global_state.images)}")
-    print(f"STATE: containers:    {len(global_state.containers)}")
-    print(f"STATE: tag_rules:     {len(global_state.tag_rules)}")
-    print(f"STATE: connections:   {len(global_state.update_mqueues)}")
-    print(
-        f"STATE: tasks: {', '.join('/'.join(map(str, i)) for i in Counter(t.get_coro().__name__ for t in asyncio.all_tasks()).items())}"
-    )
-    print(f"STATE: ========================================================")
+    @property
+    def tags(self) -> set[str]:
+        """All named references to image"""
+        return set(self.RepoTags)  # | set(self.RepoDigests)
 
 
-class BaseTable(Table):
-    allow_sort = True
-    classes = ["table", "table-striped"]
+class ImageHistoryElement(Deserializable):
+    """Wraps information docker.image.history"""
+
+    Id: str
+    CreatedBy: str
+    Created: int
+    Tags: None | Sequence[str]
+    Size: int
+    Comment: str
 
-    def __init__(self, endpoint, items):
-        super().__init__(items)
-        self.endpoint = endpoint
 
-    def get_tr_attrs(self, item):
-        return {"class": item.get("class")}
+@dataclass
+class Image:
+    """Wraps information docker.images
+    Note: images.get() will be deprecated and thereof images.inspect() has to be used. As a result
+    all values also in ImageInspect will be pruned
+    """
 
+    inspect: ImageInspect
+    history: Sequence[ImageHistoryElement]
+    children: set[str] = field(default_factory=set)
+    # containers: set[str] = field(default_factory=set)
+
+    def __str__(self) -> str:
+        return f"{self.short_id} / {list(self.tags)}"
+
+    @property
+    def id(self) -> str:
+        """Image ID"""
+        assert re.match("^sha256:[0-9a-f]{64}$", self.inspect.Id)
+        return self.inspect.Id
+
+    @property
+    def short_id(self) -> str:
+        """First 10 digits of Id"""
+        assert re.match("^sha256:[0-9a-f]{64}$", self.inspect.Id)
+        return self.inspect.Id[7:17]
+
+    @property
+    def parent(self) -> str:
+        """Shortcut to self.inspect.Parent"""
+        return self.inspect.Parent
+
+    @property
+    def created_at(self) -> datetime:
+        """Shortcut to self.inspect.Created"""
+        return self.inspect.Created
+
+    @property
+    def tags(self) -> set[str]:
+        """All named references to image"""
+        return self.inspect.tags
+
+
+class Volume(Deserializable):
+    """Wraps information docker.volumes"""
+
+    Name: str
+    Labels: None | Mapping[str, str]
+    CreatedAt: datetime
+    Mountpoint: str
+    IgnoreKeys = {"Driver", "Scope", "Options"}
+
+    def __str__(self) -> str:
+        return f"{self.Name[:12]} {str(self.CreatedAt)[:19]} {self.Mountpoint}"
+
+
+class Network(Deserializable):
+    """Wraps information docker.networks"""
+
+    Id: str
+    Name: str
+    Created: datetime
+    IgnoreKeys = {
+        "Driver",
+        "Options",
+        "Containers",
+        "Ingress",
+        "Scope",
+        "Attachable",
+        "ConfigFrom",
+        "IPAM",
+        "EnableIPv6",
+        "ConfigOnly",
+        "Internal",
+        "Labels",
+    }
 
-class PlainCol(Col):
-    def td_format(self, content):
-        return f"<tt><b>{content}</b></tt>"
+    def __str__(self) -> str:
+        return f"{self.Id[:12]} {str(self.Created)[:19]}"
 
 
-class ImageTable(BaseTable):
-    short_id = PlainCol("short_id")
-    tags = PlainCol("tags")
-    created_at = PlainCol("created_at")
-    age = PlainCol("age")
+class DockerEventActorAttributes(Deserializable):
+    """Wraps information coming from DockerEvent.Actor"""
 
-    def sort_url(self, col_key, reverse=False):
-        return url_for(
-            self.endpoint,
-            sort_key_images=col_key,
-            sort_direction_images="desc" if reverse else "asc",
-        )
+    image: None | str
+    name: None | str
+    IgnoreKeys = {
+        "maintainer",
+        "execID",
+        "container",
+        "type",
+        "exitCode",
+        "execDuration",
+        "signal",
+        "reclaimed",
+        "driver",
+        "read/write",
+        "destination",
+        "propagation",
+        "version",
+        "comment",
+        "imageID",
+        "imageRef",
+    }
 
-    @staticmethod
-    def html_from(endpoint, global_state, sort, reverse):
-        now = datetime.now(tz=tz.tzutc())
-
-        def dict_from(image):
-            now_timestamp = now.timestamp()
-            # todo: no need for date_from
-            created_timestamp = date_from(image["created_at"]).timestamp()
-
-            def coloured_ident(ident):
-                is_expired, last_referenced, expiration_age = expired(
-                    ident, global_state, now_timestamp, created_timestamp
-                )
-                return (
-                    f"<div class='text-{'danger' if is_expired else 'success'}'>"
-                    f"{ident} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)}) "
-                    f"<a href=remove_image_ident?ident={ident}>del</a>"
-                    f"</div>"
-                )
 
-            return {
-                "short_id": coloured_ident(image["short_id"]),
-                "tags": "".join(map(coloured_ident, image["tags"] or [])),
-                "created_at": date_str(image["created_at"]),
-                "age": age_str(now, image["created_at"], fixed=True),
-                # "last_referenced": last_referenced_str(image["short_id"]),
-                # "class": "text-danger" if would_cleanup_image(image, now, global_state) else "text-success",
-            }
+class DockerEventActor(Deserializable):
+    """Wraps information coming from DockerEvent.Actor"""
 
-        return ImageTable(
-            endpoint,
-            items=sorted(
-                map(dict_from, global_state.images.values()),
-                key=lambda e: e[sort],
-                reverse=reverse,
-            ),
-        ).__html__()
-
-
-class ContainerTable(BaseTable):
-    short_id = PlainCol("short_id")
-    name = PlainCol("name")
-    image = PlainCol("image")
-
-    status = PlainCol("status")
-    created_at = PlainCol("created_at")
-    started_at = PlainCol("started_at")
-    uptime = PlainCol("uptime")
-    pid = PlainCol("pid")
-    mem_usage = PlainCol("mem_usage")
-    cpu = PlainCol("cpu")
-    cmd = PlainCol("cmd")
-
-    job = PlainCol("job")
-    hints = PlainCol("hints")
-    # link = LinkCol('Link', 'route_containers', url_kwargs=dict(id='id'), allow_sort=False)
-
-    def sort_url(self, col_key, reverse=False):
-        return url_for(
-            self.endpoint,
-            sort_key_containers=col_key,
-            sort_direction_containers="desc" if reverse else "asc",
-        )
+    ID: str
+    Attributes: Mapping[str, str]  # DockerEventActorAttributes
 
-    @staticmethod
-    def html_from(endpoint, global_state, sort, reverse):
-        now = datetime.now(tz=tz.tzutc())
-
-        def coloured_ident(cnt):
-            cnt_expired = would_cleanup_container(cnt, now.timestamp(), global_state)
-            return (
-                f"<div class='text-{'danger' if cnt_expired else 'success'}'>"
-                f"{cnt['short_id']} "
-                f"<a href=delete_container?ident={cnt['short_id']}>del</a>"
-                f"</div>"
-            )
 
-        return ContainerTable(
-            endpoint,
-            items=sorted(
-                (
-                    {
-                        "short_id": coloured_ident(cnt),
-                        "name": cnt["name"],
-                        "image": short_id(cnt["image"]) if is_uid(cnt["image"]) else cnt["image"],
-                        "mem_usage": f"{(mem_stats.get('usage', 0)>>20)}MiB",
-                        "cpu": f"{int(cpu_perc(cpu_stats, last_cpu_stats) * 1000) / 10}%",
-                        "cmd": " ".join(cnt["show"]["Config"]["Cmd"])[:100],
-                        "job": jobname_from(
-                            cnt["show"]["HostConfig"]["Binds"]
-                            or list(cnt["show"]["Config"]["Volumes"] or [])
-                        ),
-                        "created_at": date_str(date_from(cnt["show"]["Created"])),
-                        "started_at": date_str(
-                            started_at := date_from(cnt["show"]["State"]["StartedAt"])
-                        ),
-                        "uptime": age_str(now, started_at, fixed=True),
-                        "status": cnt["show"]["State"]["Status"],
-                        "hints": label_filter(cnt["show"]["Config"]["Labels"]),
-                        "pid": int(cnt["show"]["State"]["Pid"]),
-                        # https://getbootstrap.com/docs/4.0/utilities/colors/
-                    }
-                    for cnt, mem_stats, cpu_stats, last_cpu_stats in (
-                        (
-                            c,
-                            c["stats"].get("memory_stats", {}),
-                            c["stats"]["cpu_stats"],
-                            c["last_stats"].get("cpu_stats"),
-                        )
-                        for c in global_state.containers.values()
-                        if c.keys() > {"short_id", "name", "stats"}
-                    )
-                ),
-                key=lambda e: e[sort],
-                reverse=reverse,
-            ),
-        ).__html__()
-
-
-class VolumeTable(BaseTable):
-    name = PlainCol("name")
-    labels = PlainCol("labels")
-    created_at = PlainCol("created_at")
-    age = PlainCol("age")
-    mountpoint = PlainCol("mountpoint")
-
-    def sort_url(self, col_key, reverse=False):
-        return url_for(
-            self.endpoint,
-            sort_key_volumes=col_key,
-            sort_direction_volumes="desc" if reverse else "asc",
-        )
+class DockerEvent(Deserializable):
+    """Wraps a Docker event"""
 
-    @staticmethod
-    def html_from(endpoint, global_state, sort, reverse):
-        now = datetime.now(tz=tz.tzutc())
-
-        def dict_from(volume):
-            now_timestamp = now.timestamp()
-            created_timestamp = date_from(volume["CreatedAt"]).timestamp()
-
-            def coloured_ident(ident: str, formatter=lambda s: s) -> str:
-                is_expired, last_referenced, expiration_age = expired(
-                    ident, global_state, now_timestamp, created_timestamp
-                )
-                return (
-                    f"<div class='text-{'danger' if is_expired else 'success'}'>"
-                    f"{formatter(ident)} ({age_str(now, last_referenced)}/{age_str(expiration_age, 0)})"
-                    f"<a href=delete_volume?ident={ident}>del</a></div>"
-                )
+    timeNano: int
+    Type: str
+    Action: str  # create
+    Actor: DockerEventActor
 
-            return {
-                "name": coloured_ident(volume["Name"], formatter=lambda s: s[:12]),
-                "labels": "".join(map(coloured_ident, volume["Labels"] or [])),
-                "created_at": date_str(date_from(volume["CreatedAt"])),
-                "age": age_str(now, date_from(volume["CreatedAt"])),
-                "mountpoint": volume["Mountpoint"],
-            }
+    # id: None | str # same as event.Actor.ID
+    # status: str    # same as event.Action
+    # from: str      # same as event.Actor.Attributes["image"]
 
-        return VolumeTable(
-            endpoint,
-            items=sorted(
-                map(dict_from, global_state.volumes.values()),
-                key=lambda e: e[sort],
-                reverse=reverse,
-            ),
-        ).__html__()
-
-
-def meta_info(global_state: GlobalState):
-    return {
-        "refresh_interval": global_state.intervals.get("site_refresh", 10),
-        "event_horizon": age_str(time.time(), global_state.event_horizon),
-        "container_count": len(global_state.containers),
-        "image_count": len(global_state.images),
-        "volume_count": len(global_state.volumes),
-        "extra_links": global_state.extra_links,
-        "intervals": {key: dur_str(value) for key, value in global_state.intervals.items()},
-        "next_cleanup": dur_str(global_state.intervals["cleanup"] - global_state.cleanup_fuse),
-        "hostname": global_state.hostname,
-        "switches": global_state.switches,
-        "expiration_ages": {
-            key: dur_str(value) for key, value in global_state.expiration_ages.items()
-        },
-        "self_pid": os.getpid(),
-    }
+    IgnoreKeys = {"id", "time", "scope", "status", "from"}
 
 
-async def response_remove_image_ident(global_state: GlobalState):
-    docker = Docker()
-    try:
-        await remove_image_ident(global_state, docker, request.args.get("ident"))
-    except Exception as exc:
-        return f"Exception raised in remove_image_ident({request.args.get('ident')}): {exc}"
-    finally:
-        await docker.close()
-    return redirect(request.referrer or url_for("route_dashboard"))
+class DockerState:
+    """Gathers all information about local docker service"""
 
+    started_at: int
 
-async def response_delete_container(global_state: GlobalState):
-    docker = Docker()
-    try:
-        await delete_container(global_state, docker, request.args.get("ident"))
-    except Exception as exc:
-        return f"Exception raised in remove_image_ident({request.args.get('ident')}): {exc}"
-    finally:
-        await docker.close()
-    return redirect(request.referrer or url_for("route_dashboard"))
+    containers: MutableMapping[str, Container]
+    containers_crawled: bool
+    containers_crawl_interval: int
 
+    images: MutableMapping[str, Image]
+    images_crawled: bool
+    images_crawl_interval: int
 
-async def response_cleanup(global_state: GlobalState):
-    global_state.cleanup_fuse = global_state.intervals["cleanup"]
-    return redirect(request.referrer or url_for("route_dashboard"))
+    volumes: MutableMapping[str, Volume]
+    volumes_crawled: bool
+    volumes_crawl_interval: int
 
+    networks: MutableMapping[str, Network]
+    networks_crawled: bool
+    networks_crawl_interval: int
 
-async def response_rules(global_state):
-    return "no rules yet"
+    event_horizon: int
+    last_referenced: MutableMapping[ImageIdent, int]
 
+    def __init__(self) -> None:
+        self.started_at = int(time.time())
 
-async def response_messages(global_state):
-    return "no messages yet"
+        self.containers = {}
+        self.containers_crawled = False
+        self.containers_crawl_interval = 120
 
+        self.images = {}
+        self.images_crawled = False
+        self.images_crawl_interval = 120
 
-async def response_volumes(global_state):
-    return await render_template(
-        "volumes.html",
-        meta=meta_info(global_state),
-        volumes_html=VolumeTable.html_from(
-            "route_volumes",
-            global_state,
-            sort=request.args.get("sort_key_volumes", "created_at"),
-            reverse=request.args.get("sort_direction_volumes", "desc") == "desc",
-        ),
-    )
+        self.volumes = {}
+        self.volumes_crawled = False
+        self.volumes_crawl_interval = 120
 
+        self.networks = {}
+        self.networks_crawled = False
+        self.networks_crawl_interval = 120
 
-async def response_containers(global_state):
-    # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
-    return await render_template(
-        "containers.html",
-        meta=meta_info(global_state),
-        containers_html=ContainerTable.html_from(
-            "route_containers",
-            global_state,
-            sort=request.args.get("sort_key_containers", "cpu"),
-            reverse=request.args.get("sort_direction_containers", "desc") == "desc",
-        ),
-    )
+        self.event_horizon = self.started_at
+        self.last_referenced = {}
 
+        self.docker_client: None | Docker = None
+        self.updates = asyncio.Queue[MType]()
 
-async def response_images(global_state):
-    # https://github.com/plumdog/flask_table/blob/master/examples/sortable.py
-    return await render_template(
-        "images.html",
-        meta=meta_info(global_state),
-        images_html=ImageTable.html_from(
-            "route_images",
-            global_state,
-            sort=request.args.get("sort_key_images", "created_at"),
-            reverse=request.args.get("sort_direction_images", "asc") == "desc",
-        ),
-    )
+    def inform(self, mtype: MessageType, mtext: str, mobj: None | object = None) -> None:
+        """Inform about something important has happened"""
+        self.updates.put_nowait((mtype, mtext, mobj))
 
+    async def wait_for_change(self) -> AsyncIterator[MType]:
+        """Pass messages read from message queue"""
+        while True:
+            message = await self.updates.get()
+            yield message
 
-async def response_dashboard(global_state):
-    return await render_template(
-        "dashboard.html",
-        meta=meta_info(global_state),
-        containers_html=ContainerTable.html_from(
-            "route_dashboard",
-            global_state,
-            sort=request.args.get("sort_key_containers", "cpu"),
-            reverse=request.args.get("sort_direction_containers", "desc") == "desc",
-        ),
-        images_html=ImageTable.html_from(
-            "route_dashboard",
-            global_state,
-            sort=request.args.get("sort_key_images", "created_at"),
-            reverse=request.args.get("sort_direction_images", "asc") == "desc",
-        ),
-        messages=[(date_str(m[0]), m[1], m[2]) for m in global_state.messages],
-    )
+    async def run(self) -> None:
+        """Starts and awaits monitoring background tasks"""
+        try:
+
+            def docker_connection(limit: int = 1000) -> Docker:
+                """Creates a Docker connection with a customized Connector in order to
+                increase connection limit"""
+                for sockpath in [Path("/run/docker.sock"), Path("/var/run/docker.sock")]:
+                    if sockpath.is_socket():
+                        return Docker(
+                            "unix://localhost",
+                            aiohttp.UnixConnector(sockpath.as_posix(), limit=limit),
+                        )
+                raise RuntimeError("No path to docker.sock found")
 
+            async with docker_connection() as self.docker_client:
+                await asyncio.gather(
+                    # self.__disconnect(),
+                    self.monitor_events(),
+                    self.run_crawl_containers(),
+                    self.run_crawl_images(),
+                    self.run_crawl_volumes(),
+                    self.run_crawl_networks(),
+                )
+                self.docker_client = None
+        except Exception:  # pylint: disable=broad-except
+            log().exception("in DockerState.run()")
+
+    async def __disconnect(self) -> None:  # pylint: disable=unused-private-member
+        """Simulate a sudden disconnect from Docker socket"""
+        await asyncio.sleep(60)
+        if self.docker_client:
+            log().info("close!")
+            await self.docker_client.close()
+
+    def client(self) -> Docker:
+        """Returns the current Docker client and raises if not available (for typing reasons)"""
+        if not self.docker_client:
+            raise RuntimeError("Wrong state")
+        return self.docker_client
 
-async def container_table_html(global_state):
-    return await response_containers(global_state)
+    async def monitor_events(self) -> None:
+        """Continuously reads and handles Docker events"""
 
+        subscriber = self.client().events.subscribe()  # type: ignore[no-untyped-call]
+        event_buffer: MutableSequence[DockerEvent] = []
 
-async def image_table_html(global_state):
-    return await response_images(global_state)
+        # import json
+        # for _raw_e in map(json.loads, open("docker-events.log")):
+        while True:
+            try:
+                if (_raw_e := await subscriber.get()) is None:
+                    log().error("got None event (probably socket disconnect)")
+                    self.inform("client_disconnect", "docker events yielded None")
+                    continue
 
+                event = DockerEvent(**_raw_e)
 
-async def dashboard(global_state):
-    return await response_dashboard(global_state)
-
-
-# leftover - remove me after restarts
-async def generic_html(generic, global_state):
-    if generic == "favicon.ico":
-        return ""
-    if generic == "volumes":
-        return await response_volumes(global_state)
-    if generic == "rules":
-        return await response_rules(global_state)
-    if generic == "messages":
-        return await response_messages(global_state)
-
-    raise RuntimeError(f"not found: {generic}")
-
-
-async def print_container_stats(global_state):
-    hostname = open("/etc/hostname").read().strip()
-    stats = [
-        {
-            "short_id": cnt["short_id"],
-            "name": cnt["name"],
-            "usage": mem_stats.get("usage", 0),
-            "cmd": " ".join(cnt["show"]["Config"]["Cmd"]),
-            "job": jobname_from(
-                cnt["show"]["HostConfig"]["Binds"] or list(cnt["show"]["Config"]["Volumes"] or [])
-            ),
-            "cpu": cpu_perc(cpu_stats, last_cpu_stats),
-            "created_at": date_from(cnt["show"]["Created"]),
-            "started_at": date_from(cnt["show"]["State"]["StartedAt"]),
-            "status": cnt["show"]["State"]["Status"],
-            "hints": label_filter(cnt["show"]["Config"]["Labels"]),
-            "pid": int(cnt["show"]["State"]["Pid"]),
-            "container": cnt["container"],
-        }
-        for cnt, mem_stats, cpu_stats, last_cpu_stats in (
-            (
-                c,
-                c["stats"].get("memory_stats", {}),
-                c["stats"]["cpu_stats"],
-                c["last_stats"].get("cpu_stats"),
-            )
-            for c in global_state.containers.values()
-            if c.keys() > {"short_id", "name", "stats"}
-        )
-    ]
+                assert not _raw_e.get("id") or _raw_e.get("id") == event.Actor.ID
+                assert not _raw_e.get("status") or _raw_e.get("status") == event.Action
+                assert (
+                    not _raw_e.get("from") or _raw_e.get("from") == event.Actor.Attributes["image"]
+                )
 
-    os.system("clear")
-    print(f"=[ {hostname} ]======================================")
-    print(
-        f"{'ID':<12}  {'NAME':<25}"
-        f" {'PID':>9}"
-        f" {'CPU':>9}"
-        f" {'MEM':>9}"
-        f" {'UP':>9}"
-        f" {'STATE':>9}"
-        f" {'JOB':<60}"
-        f" {'HINTS'}"
-    )
-    now = datetime.now()
-    for s in sorted(stats, key=lambda e: e["pid"]):
-        tds = int((now - (s["started_at"] or s["created_at"])).total_seconds())
-        col_td = "\033[1m\033[91m" if tds // 3600 > 5 else ""
-        dur_str = f"{tds//86400:2d}d+{tds//3600%24:02d}:{tds//60%60:02d}"
-        col_mem = "\033[1m\033[91m" if s["usage"] >> 30 > 2 else ""
-        mem_str = f"{(s['usage']>>20)}MiB"
-        col_cpu = "\033[1m\033[91m" if s["cpu"] > 2 else ""
-        container_is_critical = (
-            (s["started_at"] and tds // 3600 > 5) or s["status"] == "exited" or not s["started_at"]
-        )
-        col_cpu = "\033[1m\033[91m" if s["cpu"] > 2 else ""
-        print(
-            f"{s['short_id']:<12}  {s['name']:<25}"
-            f" {s['pid']:>9}"
-            f" {col_cpu}{int(s['cpu'] * 100):>8}%\033[0m"
-            f" {col_mem}{mem_str:>9}\033[0m"
-            f" {col_td}{dur_str}\033[0m"
-            f" {s['status']:>9}"
-            f" {s['job']:<60}"
-            f" {s['hints']}"
-        )
-        # if (
-        #    (s["started_at"] and tds // 3600 > 5)
-        #    or s["status"] == "exited"
-        #    or not s["started_at"]
-        # ):
-        #    log(f"remove {s['short_id']}")
-        #    await s["container"].delete(force=True)
-    print(
-        f"{'TOTAL':<12}  {len(stats):<25}"
-        f" {'':>9}"
-        f" {int(sum(s['cpu'] for s in stats)*1000) / 10:>8}%\033[0m"
-        f" {int(sum(s['usage'] for s in stats) / (1<<30)*10) / 10:>6}GiB\033[0m"
-        f" {''}"
-        f" {'':>9}"
-        f" {'':<60}"
-        f" {''}"
-    )
+                if all(
+                    (
+                        self.containers_crawled,
+                        self.images_crawled,
+                        self.volumes_crawled,
+                        self.networks_crawled,
+                    )
+                ):
+                    while event_buffer:
+                        await handle_docker_event(self, event_buffer.pop(0))
+                    await handle_docker_event(self, event)
+                else:
+                    log().info(
+                        "postpone event (C: %s, I: %s, V: %s, N: %s)",
+                        self.containers_crawled,
+                        self.images_crawled,
+                        self.volumes_crawled,
+                        self.networks_crawled,
+                    )
+                    event_buffer.append(event)
 
+            except Exception as exc:  # pylint: disable=broad-except
+                log().error("Error while handling event: %s", str(_raw_e))
+                self.inform("exception", "in monitor_events()", exc)
 
-async def watch_container(container, global_state: GlobalState):
-    name = "unknown"
-    containers = global_state.containers
-    try:
-        container_info = containers[container.id]
-        container_info["container"] = container
-        container_info["short_id"] = (short_id_ := short_id(container.id))
-        container_info["show"] = (show := await container.show())
-        container_info["name"] = (name := show["Name"][1:])
-        container_info["image"] = show["Config"]["Image"]
-
-        # wrong - other things could have happened since..
-        # register_reference(image, date_from(show["Created"]).timestamp(), global_state)
-
-        log().info(">> new container: %s %s", short_id_, name)
-
-        async for stats in container.stats():
-            container_info["last_stats"] = container_info.get("stats", {})
-            container_info["stats"] = stats
-            container_info["show"] = await container.show()
+    async def run_crawl_containers(self) -> None:
+        """Continuously updates information about running containers"""
+        while True:
+            try:
+                await crawl_containers(self)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.inform("exception", "in run_crawl_containers()", exc)
+            await asyncio.sleep(self.containers_crawl_interval)
 
-    except DockerError as exc:
-        log().error("DockerError: %s", exc)
-    except Exception:
-        log().exception("Unhandled exception in watch_container()")
-    finally:
-        log().info("<< container terminated: %s %s", short_id_, name)
-        await unregister_container(container.id, global_state)
+    async def run_crawl_images(self) -> None:
+        """Continuously updates information about local images"""
+        while True:
+            try:
+                await crawl_images(self)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.inform("exception", "in run_crawl_images()", exc)
+            await asyncio.sleep(self.images_crawl_interval)
 
+    async def run_crawl_volumes(self) -> None:
+        """Continuously updates information about docker volumes"""
+        while True:
+            try:
+                await crawl_volumes(self)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.inform("exception", "in run_crawl_volumes()", exc)
+            await asyncio.sleep(self.volumes_crawl_interval)
 
-async def unregister_image(global_state: GlobalState, image):
-    ident = image if isinstance(image, str) else image["Id"]
-    # todo? assert image_from() results None
-    if ident in global_state.images:
-        del global_state.images[ident]
-        await global_state.inform("refresh")
+    async def run_crawl_networks(self) -> None:
+        """Continuously updates information about docker networks"""
+        while True:
+            try:
+                await crawl_networks(self)
+            except Exception as exc:  # pylint: disable=broad-except
+                self.inform("exception", "in run_crawl_networks()", exc)
+            await asyncio.sleep(self.networks_crawl_interval)
+
+    async def prune_builder_cache(self) -> tuple[Sequence[str], Sequence[str], int]:
+        """Runs `docker builder prune` in background"""
+        return await prune_builder_cache()
+
+    def export_references(self, filepath: Path) -> None:
+        """Writes event horizon and image references to disk"""
+        export_references(self, filepath)
+
+    def import_references(self, filepath: Path) -> None:
+        """Reads event horizon and image references from disk if applicable"""
+        import_references(self, filepath)
+
+
+async def prune_builder_cache() -> tuple[Sequence[str], Sequence[str], int]:
+    """Runs `docker builder prune` in background"""
+
+    async def acc_stream(stream: StreamReader, prefix: str) -> Sequence[str]:
+        result = []
+        async for line in (raw_line.decode().strip() async for raw_line in stream):
+            log().debug("%s: %s", prefix, line)
+            result.append(line)
+        return result
+
+    cmd = ("docker", "builder", "prune", "--force", "--filter=until=24h", "--keep-storage=50G")
+    process = await create_subprocess_exec(*cmd, stdout=PIPE, stderr=PIPE)
+    assert process.stdout and process.stderr
+    stdout, stderr, returncode = await asyncio.gather(
+        acc_stream(process.stdout, "docker-builder-prune-std"),
+        acc_stream(process.stderr, "docker-builder-prune-err"),
+        process.wait(),
+    )
+    if returncode != 0:
+        log().error("prune_builder_cache failed")
+    return stdout, stderr, returncode
 
 
-async def register_image(global_state: GlobalState, image):
-    global_state.images[image["Id"]] = {
-        "short_id": short_id(image["Id"]),
-        "created_at": date_from(image["Created"]),
-        "tags": [tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"],
-        "size": image["Size"],
-        "parent": short_id(image.get("ParentId", "")),
+async def crawl_containers(state: DockerState) -> None:
+    """Updates set of known containers - first run is allowed to find unknown containers,
+    afterwards the set is expected to be consistent"""
+
+    containers = {
+        cont.id: cont
+        for cont in await state.client().containers.list(all=True)  # type: ignore[no-untyped-call]
     }
-    await global_state.inform("refresh")
+    log().info("crawl (%d) containers..", len(containers))
+    for container in containers.values():
+        if container.id in state.containers:
+            continue
+        log().debug("found unregistered container %s", short_id(container.id))
+        if state.containers_crawled:
+            log().error("%s should have been registered automatically before!", container.id)
+        register_container(state, container)
+
+    if not state.containers_crawled:
+        state.containers_crawled = True
+        log().info("initial container crawl done")
+
+    for container_id in list(state.containers):
+        if container_id not in containers:
+            log().error("registered container %s does not exist anymore", short_id(container_id))
 
 
-async def update_image_registration(global_state: GlobalState, docker_client, image_id):
-    if image := await image_from(docker_client, image_id):
-        if image["Id"] in global_state.images:
-            global_state.images[image["Id"]]["tags"] = [
-                tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"
-            ]
-            await global_state.inform("refresh")
-        else:
-            await register_image(global_state, image)
-    else:
-        await unregister_image(global_state, image_id)
-
+async def container_from(docker_client: Docker, ident: str) -> None | DockerContainer:
+    """Retrieves container instance identified by @ident"""
+    with suppress(DockerError):
+        return cast(
+            DockerContainer,
+            await docker_client.containers.get(ident),  # type: ignore[no-untyped-call]
+        )
 
-async def watch_images(docker_client, global_state: GlobalState) -> None:
-    # TODO: also use events to register
-    log().info("crawl images..")
-    for image in await docker_client.images.list(all=True):
-        if image["Id"] not in global_state.images:
-            log().warning("  found unregistered image %s", image["Id"])
-            await register_image(global_state, image)
+    return None
 
 
-async def register_container(container, global_state: GlobalState) -> None:
-    log().debug("register container %s", container.id)
-    global_state.containers[container.id] = {}
-    asyncio.ensure_future(watch_container(container, global_state))
-    await global_state.inform("refresh")
+def register_container(state: DockerState, container: DockerContainer) -> None:
+    """Put a container into set of known containers"""
+    if container.id in state.containers:
+        return
+    log().debug("register container %s", container.id[:10])
+    state.containers[container.id] = Container(container)
+    asyncio.ensure_future(watch_container(state, container))
 
 
-async def unregister_container(ident, global_state: GlobalState) -> None:
+def unregister_container(state: DockerState, container_id: str) -> None:
+    """Remove a container from set of known containers"""
     try:
-        del global_state.containers[ident]
-        await global_state.inform("refresh")
+        del state.containers[container_id]
     except KeyError:
-        report(global_state, "error", f"tried to remove container {ident} unknown to registry")
+        state.inform("error", f"tried to remove container {short_id(container_id)} unknown to us")
 
 
-async def watch_containers(docker_client, global_state: GlobalState):
-    # TODO: also use events to register
-    log().debug("crawl containers..")
-    for container in await docker_client.containers.list(all=True):
-        if container.id not in global_state.containers:
-            log().debug("  found container %s", container.id)
-            if global_state.containers_crawled:
-                log().error("%s should have been registered automatically before!", container.id)
-            await register_container(container, global_state)
-    global_state.containers_crawled = True
-
-
-async def watch_volumes(docker_client, global_state: GlobalState):
-    # TODO: also use events to register
-    log().info("crawl volumes..")
-    for volume in (await docker_client.volumes.list())["Volumes"]:
-        if volume["Name"] not in global_state.volumes:
-            log().debug("  found volume %s", volume)
-            global_state.volumes[volume["Name"]] = volume
-
-
-def would_cleanup_container(container, now: int, global_state: GlobalState):
-    if "show" not in container:
-        return False
-    status = (show := container["show"])["State"]["Status"]
-    if status == "exited":
-        return (
-            now - date_from(show["State"]["FinishedAt"]).timestamp()
-            > global_state.expiration_ages["container_exited"]
-        )
-    if status == "created":
-        return (
-            now - date_from(show["Created"]).timestamp()
-            > global_state.expiration_ages["container_created"]
-        )
-    if status == "running":
-        return (
-            now - date_from(show["State"]["StartedAt"]).timestamp()
-            > global_state.expiration_ages["container_running"]
+async def watch_container(state: DockerState, container: DockerContainer) -> None:
+    """Continuously monitor a distinct container over time"""
+    name = "unknown"  # have a value for the `except` case
+    normally_terminated = False
+    try:
+        container_info = state.containers[container.id]
+        container_info.show = (
+            show := ContainerShow(**(await container.show()))  # type: ignore[no-untyped-call]
         )
-    return False
+        """
+        if (image := state.images.get(image_id := state.containers[container_id].image)):
+            try:
+                image.containers.remove(container_id)
+            except KeyError:
+                state.inform("warning", f"container {short_id(container_id)} image {image_id} did not know container")
+        else:
+            state.inform("warning", f"container {short_id(container_id)} image {image_id} unknown to us")
+        """
 
+        # todo: wrong - other things could have happened since..
+        register_reference(state, show.Image, show.Created.timestamp())
 
-def expired_idents(image, now, global_state: GlobalState):
-    log().debug("check expiration for image %s, tags=%s", image["short_id"], image["tags"])
+        state.inform("container_add", container.id, container_info)
 
-    # todo: remove date_from
-    created_timestamp = int(date_from(image["created_at"]).timestamp())
+        log().info(">> new container: %s %s", container_info.short_id, name)
 
-    for tag in image["tags"] or []:
-        if expired(tag, global_state, now, created_timestamp)[0]:
-            yield tag
+        last_cpu_usage, last_mem_usage, count = 0.0, 0, 0
 
-    # only remove a container directly if there are no tags we could monitor
-    if not image["tags"]:
-        if expired(image["short_id"], global_state, now, created_timestamp)[0]:
-            yield image["short_id"]
+        async for raw_stats in container.stats():  # type: ignore[no-untyped-call]
+            container_info.last_stats = container_info.stats
+            container_info.stats = ContainerStats(**raw_stats)
+            old_show = container_info.show
+            container_info.show = ContainerShow(
+                **(await container.show())  # type: ignore[no-untyped-call]
+            )
+            cpu_usage = container_info.cpu_usage()
+            mem_usage = container_info.mem_usage()
+            if not old_show and container_info.last_stats:
+                continue
 
+            if update_inform_trigger(
+                count,
+                old_show,
+                container_info.show,
+                cpu_usage,
+                mem_usage,
+                last_cpu_usage,
+                last_mem_usage,
+            ):
+                last_cpu_usage, last_mem_usage = cpu_usage, mem_usage
+                state.inform("container_update", container.id, container_info)
 
-async def image_from(docker_client: Docker, ident: str) -> bool:
-    with suppress(DockerError):
-        return await docker_client.images.get(ident)
-    return None
+            count += 1
 
+        normally_terminated = True
 
-async def container_from(docker_client: Docker, ident: str) -> bool:
-    with suppress(DockerError):
-        return await docker_client.containers.get(ident)
-    return None
+    except DockerError as exc:
+        log().warning("DockerError while watching %s: %s", container.id, exc)
+    except Exception as exc:  # pylint: disable=broad-except
+        state.inform("exception", f"in watch_container() while watching {container.id}", exc)
+    finally:
+        if normally_terminated:
+            log().info("<< container terminated: %s %s", container_info.short_id, name)
+        """
+        if (image := state.images.get(image_id := state.containers[container_id].image)):
+            try:
+                image.containers.remove(container_id)
+            except KeyError:
+                state.inform("warning", f"container {short_id(container_id)} image {image_id} did not know container")
+        else:
+            state.inform("warning", f"container {short_id(container_id)} image {image_id} unknown to us")
+        """
+
+        unregister_container(state, container.id)
+        state.inform("container_del", container.id, container_info)
+
+
+def update_inform_trigger(
+    count: int,
+    old_show: ContainerShow,
+    new_show: ContainerShow,
+    cpu_usage: float,
+    mem_usage: int,
+    last_cpu_usage: float,
+    last_mem_usage: int,
+) -> bool:
+    """Returns wether we should send a container update"""
+    return (
+        count == 0
+        or (new_show.status != old_show.status)
+        or (
+            (count % 10 == 0)
+            and (abs(last_cpu_usage - cpu_usage) > 0.2 or abs(last_mem_usage - mem_usage) > 1 << 20)
+        )
+    )
 
 
-async def volume_from(docker_client: Docker, ident: str) -> bool:
+async def crawl_images(state: DockerState) -> None:
+    """Updates set of known images - first run is allowed to find unknown images,
+    afterwards the set is expected to be consistent"""
+    log().debug("fetch image list..")
+    image_ids = set(image["Id"] for image in await state.client().images.list(all=True))
+    log().info("crawl (%d) images..", len(image_ids))
+
+    for image_id in image_ids:
+        if image_id in state.images:
+            continue
+        if state.images_crawled:
+            log().warning("  found unregistered image %s", short_id(image_id))
+        try:
+            await register_image(state, image_id)
+        except DockerError:
+            log().warning("newly found image %s suddenly disappeared", short_id(image_id))
+
+    if not state.images_crawled:
+        state.images_crawled = True
+        log().info("initial image crawl done")
+
+    # This is only for plausibility - go through all registered images and check if they still
+    # exist and also check their parents having stored a reference
+    for image_id in list(state.images):
+        if image_id in image_ids:
+            # registered image also exists in found images (ok)
+            if not (parent_id := state.images[image_id].parent):
+                continue
+            if parent_id in state.images:
+                # parent is registered (as expected) - now check if it knows it's child
+                if image_id not in state.images[parent_id].children:
+                    log().error(
+                        "parent '%s' of '%s' does not store a reference to its child",
+                        short_id(parent_id),
+                        short_id(image_id),
+                    )
+                    state.images[parent_id].children.add(image_id)
+            else:
+                log().error(
+                    "parent '%s' of '%s' is not registered even after crawls",
+                    short_id(parent_id),
+                    short_id(image_id),
+                )
+                await register_image(state, parent_id)
+                state.images[parent_id].children.add(image_id)
+            await update_image_registration(state, image_id)
+        else:
+            log().error("registered image %s does not exist anymore", short_id(image_id))
+            unregister_image(state, image_id)
+
+
+async def image_from(docker_client: Docker, ident: str) -> None | ImageInspect:
+    """Retrieve image details from an image identifier"""
     with suppress(DockerError):
-        for volume in (await docker_client.volumes.list())["Volumes"]:
-            if volume["Name"].startswith(ident):
-                return volume
+        try:
+            return ImageInspect(**await docker_client.images.inspect(ident))
+        except ValueError as exc:
+            log().error("could not resolve '%s', got '%r'", ident, exc)
+            raise
     return None
 
 
-async def remove_image_ident(global_state: GlobalState, docker_client: Docker, ident: str) -> None:
-    report(global_state, "info", f"remove image/tag {ident}", None)
-    await docker_client.images.delete(ident)
-    await update_image_registration(global_state, docker_client, ident)
+async def register_image(state: DockerState, image_id: str) -> None:
+    """Put an image into set of known images"""
+    if image_id in state.images:
+        return
+    log().debug("image '%s': fetch inspect/history data..", short_id(image_id))
+    inspect = ImageInspect(**await state.client().images.inspect(image_id))
+
+    if inspect.Id in state.images:
+        return
+
+    raw_history = await state.client().images.history(inspect.Id)
+
+    history = []
+    for raw_hist_element in raw_history:
+        hist_element = ImageHistoryElement(**raw_hist_element)
+        # log().debug("found %s | %s", hist_element.Id, hist_element.CreatedBy)
+        history.append(hist_element)
+
+    state.images[inspect.Id] = Image(inspect, history)
+
+    if inspect.Parent:
+        if inspect.Parent not in state.images:
+            log().debug(
+                "image '%s': register parent %s", short_id(image_id), short_id(inspect.Parent)
+            )
+            await register_image(state, inspect.Parent)
+        state.images[inspect.Parent].children.add(inspect.Id)
 
+    log().debug("image '%s': registered", short_id(image_id))
 
-async def delete_container(global_state: GlobalState, docker_client: Docker, container_ident):
-    container = (
-        await container_from(docker_client, container_ident)
-        if isinstance(container_ident, str)
-        else container_ident["container"]
-    )
+    state.inform("image_add", inspect.Id, state.images[inspect.Id])
 
-    report(
-        global_state,
-        "warn",
-        f"force removing container {short_id(container.id)}",
-        container,
+
+def unregister_image(state: DockerState, image_id: str) -> None:
+    """Remove an image from set of known images"""
+    # todo? assert image_from() results None
+    if image_id not in state.images:
+        return
+    for deleted_tag in state.images[image_id].tags:
+        unregister_reference(state, deleted_tag)
+    parent_id = state.images[image_id].parent
+    del state.images[image_id]
+    unregister_reference(state, image_id)
+    if parent_id:
+        try:
+            state.images[parent_id].children.remove(image_id)
+        except KeyError:
+            log().error(
+                "Could not remove %s from it's parent %s: does not exist",
+                short_id(image_id),
+                short_id(parent_id),
+            )
+    state.inform("image_del", image_id)
+
+
+async def update_image_registration(state: DockerState, image_id: str) -> None:
+    """Update internally held information about image with given @image_id"""
+    if inspect := await image_from(state.client(), image_id):
+        if inspect.Id in state.images:
+            image = state.images[inspect.Id]
+            tags_before = image.tags
+            tags_new = inspect.tags
+            for deleted_tag in tags_before - tags_new:
+                unregister_reference(state, deleted_tag)
+            state.images[inspect.Id].inspect = inspect
+            # tag for tag in (image["RepoTags"] or []) if tag != "<none>:<none>"
+            state.inform("image_update", inspect.Id)
+        else:
+            await register_image(state, inspect.Id)
+    else:
+        unregister_image(state, image_id)
+
+
+async def crawl_volumes(state: DockerState) -> None:
+    """Crawls volumes"""
+    raw_volumes = await state.client().volumes.list()  # type: ignore[no-untyped-call]
+    volumes = {vol["Name"]: Volume(**vol) for vol in raw_volumes["Volumes"]}
+    log().info("crawl (%d) volumes..", len(volumes))
+    for volume_name, volume in volumes.items():
+        if volume_name in state.volumes:
+            continue
+        if state.images_crawled:
+            log().error("  found unregistered volume %s", short_id(volume_name))
+        await register_volume(state, volume)
+
+    if not state.volumes_crawled:
+        state.volumes_crawled = True
+        log().info("initial volume crawl done")
+
+    if raw_volumes["Warnings"]:
+        log().warning("  VolumesWarnings: %s", raw_volumes["Warnings"])
+
+    await cleanup_volume_registrations(state, volumes.keys())
+
+
+async def cleanup_volume_registrations(
+    state: DockerState, volume_names: None | Iterable[str] = None
+) -> None:
+    """Cleans up volume registrations"""
+    volumes = volume_names or await state.client().volumes.list()  # type: ignore[no-untyped-call]
+    for volume_name in list(state.volumes):
+        if volume_name not in volumes:
+            # we don't get network delete events, so this is not an 'error'
+            log().debug("registered volume '%s' does not exist anymore", short_id(volume_name))
+            unregister_volume(state, volume_name)
+
+
+async def register_volume(state: DockerState, volume_or_id: str | Volume) -> None:
+    """Put a volume into set of known volumes"""
+    volume_name = volume_or_id.Name if isinstance(volume_or_id, Volume) else volume_or_id
+    if volume_name in state.volumes:
+        return
+
+    log().debug("volume '%s': fetch data..", short_id(volume_name))
+    volume = (
+        volume_or_id
+        if isinstance(volume_or_id, Volume)
+        else Volume(
+            **await DockerVolume(
+                state.client(),
+                volume_or_id,
+            ).show()  # type: ignore[no-untyped-call]
+        )
     )
-    await container.delete(force=True, v=True)
+    state.volumes[volume_name] = volume
 
-    # Container should cleanup itself
+    state.inform("volume_add", volume_name, volume)
 
-    if container := await container_from(docker_client, container_ident):
-        report(
-            global_state,
-            "error",
-            f"container {container_ident} still exists after deletion",
-            container,
+
+def unregister_volume(state: DockerState, volume_id: str) -> None:
+    """Remove a volume from set of known volumes"""
+    try:
+        del state.volumes[volume_id]
+        state.inform("volume_del", volume_id)
+    except KeyError:
+        state.inform("error", f"tried to remove volume {short_id(volume_id)} unknown to us")
+
+
+async def crawl_networks(state: DockerState) -> None:
+    """Crawls networks"""
+    networks = {net["Id"]: Network(**net) for net in await state.client().networks.list()}
+    log().info("crawl (%d) networks..", len(networks))
+    for net_id, network in networks.items():
+        if net_id in state.networks:
+            continue
+        if state.images_crawled:
+            log().error("  found unregistered network %s", short_id(net_id))
+        await register_network(state, network)
+
+    if not state.networks_crawled:
+        state.networks_crawled = True
+        log().info("initial network crawl done")
+
+    await cleanup_network_registrations(state, networks.keys())
+
+
+async def cleanup_network_registrations(
+    state: DockerState, networks: None | Iterable[str] = None
+) -> None:
+    """Cleans up network registrations"""
+    network_ids = networks or await state.client().networks.list()
+    for net_id in list(state.networks):
+        if net_id not in network_ids:
+            # we don't get network delete events, so this is not an 'error'
+            log().debug("registered network %s does not exist anymore", short_id(net_id))
+            unregister_network(state, net_id)
+
+
+async def register_network(state: DockerState, network_or_id: str | Network) -> None:
+    """Put a network into set of known networks"""
+    network_id = network_or_id.Name if isinstance(network_or_id, Network) else network_or_id
+    if network_id in state.networks:
+        return
+
+    log().debug(
+        "network '%s': fetch data..",
+        short_id(network_id),
+    )
+    network = (
+        network_or_id
+        if isinstance(network_or_id, Network)
+        else Network(
+            **await DockerNetwork(
+                state.client(),
+                network_or_id,
+            ).show()  # type: ignore[no-untyped-call]
         )
+    )
+    state.networks[network.Id] = network
 
+    state.inform("network_add", network.Id, network)
 
-async def cleanup(docker_client: Docker, global_state):
-    log().info("Cleanup!..")
 
-    report(global_state, "info", "start cleanup", None)
+def unregister_network(state: DockerState, network_id: str) -> None:
+    """Remove a network from set of known networks"""
     try:
-        now = int(datetime.now().timestamp())
-        # we could go through docker_client.containers, too, but to be more consistent, we work
-        # on one structure only
-        # also, we have to create a list we can operate on, in order to not modify the structure, we're
-        # iterating
-        for container_info in list(
-            filter(
-                lambda cnt: would_cleanup_container(cnt, now, global_state),
-                global_state.containers.values(),
-            )
-        ):
-            if not global_state.switches.get("remove_container"):
-                log().info("skip removal of container %s", container_info["short_id"])
-                continue
-            try:
-                await delete_container(global_state, docker_client, container_info)
-            except DockerError as exc:
-                log().error(
-                    "Could not delete container %s, error was %s", container_info["short_id"], exc
+        del state.networks[network_id]
+        state.inform("network_del", network_id)
+    except KeyError:
+        state.inform("error", f"tried to remove network {short_id(network_id)} unknown to us")
+
+
+def register_reference(state: DockerState, ident: str, timestamp: float) -> None:
+    """Remember the exact time we've last seen @ident"""
+    if "@sha256:" in ident or is_uid(ident):
+        return
+    effective_ident = unique_ident(ident)
+    if timestamp > state.last_referenced.get(effective_ident, 0):
+        state.last_referenced[effective_ident] = int(timestamp)
+        state.inform("reference_update", str(effective_ident), effective_ident)
+
+
+def unregister_reference(state: DockerState, ident: str) -> None:
+    """Forget the time we've last seen @ident"""
+    effective_ident = unique_ident(ident)
+    with suppress(KeyError):
+        del state.last_referenced[effective_ident]
+        state.inform("reference_del", str(effective_ident))
+
+
+async def handle_docker_event(state: DockerState, event: DockerEvent) -> None:
+    """Modify current Docker state based on incoming Docker events"""
+    # tstamp, object_type, operator, _cmd, uid, params = event_from(line)
+    tstamp, event_type, event_action, event_id = (
+        event.timeNano // 1_000_000_000,
+        event.Type,
+        event.Action.split(":", maxsplit=1)[0],
+        event.Actor.ID,
+    )
+    assert tstamp >= state.event_horizon, (
+        f"event timestamp {tstamp}" f" < event horizon {state.event_horizon}"
+    )
+
+    log().debug(
+        "EVENT %d/%s, %s ID=%s",
+        tstamp,
+        date_from(tstamp),
+        f"({event_type:<10s}{event_action:>13s})",
+        unique_ident(event_id),
+    )
+
+    if event_type == "container":
+        if event_action in {
+            "create",
+        }:
+            container = await container_from(state.client(), event_id)
+            if not container:
+                raise RuntimeError(f"Container {event_id} does not exist after 'create'")
+            register_container(state, container)
+            register_reference(state, event.Actor.Attributes["image"], tstamp)
+            return
+
+        if event_action in {
+            "destroy",
+        }:
+            # not needed, since watch_container() already takes care..
+            # unregister_container(uid, global_state)
+
+            if await container_from(state.client(), event_id):
+                state.inform("error", f"container {event_id} still alive after {event_action}")
+            return
+
+        if event_action in {
+            "exec_create",
+            "exec_start",
+            "exec_die",
+            "commit",
+            "pause",
+            "rename",
+            "unpause",
+            "health_status",
+            "kill",
+            "start",
+            "attach",
+            "top",
+            "prune",
+            "die",
+            "stop",
+            "resize",
+            "archive-path",
+        }:
+            if (
+                event_action not in {"prune", "destroy", "die", "stop", "exec_die"}
+                and not await container_from(state.client(), event_id)
+                and state.containers_crawled
+            ):
+                log().warning(
+                    "Event.action is '%s' but container %s does not exist",
+                    event_action,
+                    short_id(event_id),
                 )
+            return
 
-        for image_info in list(global_state.images.values()):
-            for ident in expired_idents(image_info, now, global_state):
-                if not global_state.switches.get("remove_images"):
-                    log().info("skip removal of image/tag %s", ident)
-                    continue
-                try:
-                    await remove_image_ident(global_state, docker_client, ident)
-                except DockerError as exc:
-                    log().error("Could not delete image %s, error was %s", ident, exc)
-
-        for ident in [
-            ident for ident in global_state.images if not await image_from(docker_client, ident)
-        ]:
-            report(global_state, "warn", f"reference to image {ident} has not been cleaned up")
-            await unregister_image(global_state, ident)
-
-        for ident in [
-            ident
-            for ident in global_state.containers
-            if not await container_from(docker_client, ident)
-        ]:
-            report(global_state, "warn", f"reference to container {ident} has not been cleaned up")
-            del global_state.containers[ident]
-
-        for ident in [
-            ident for ident in global_state.volumes if not await volume_from(docker_client, ident)
-        ]:
-            report(global_state, "warn", f"reference to volume {ident} has not been cleaned up")
-            del global_state.volumes[ident]
-    finally:
-        report(global_state, "info", "cleanup done", None)
+    elif event_type == "image":
+        if event_action in {
+            "pull",
+        }:
+            await register_image(state, event_id)
+            return
 
+        if event_action in {
+            "tag",
+            "untag",
+            "prune",
+            "delete",
+        }:
+            if event_action == "prune":
+                if event.Actor.ID == "":
+                    return
+                log().error("Event 'image-prune', but Actor.ID is not empty!")
+
+            # NOTE: image tag/untag has NO REFERENCE to the added/removed tag!!
+            await update_image_registration(state, event_id)
+
+            # if event_action == "tag":
+            #    if 'org.opencontainers.image.ref.name' in event.Actor.Attributes:
+            #        await register_reference(state, (
+            #            f"{event.Actor.Attributes['org.opencontainers.image.ref.name']}:"
+            #            f"{event.Actor.Attributes['org.opencontainers.image.version']}"), tstamp)
 
-def report(global_state, msg_type, message: str, extra=None):
-    """Report an incident - maybe good or bad"""
-    # TODO: cleanup
-    # TODO: persist
-    log().info(message)
-    global_state.messages.insert(0, (datetime.now().timestamp(), msg_type, message, str(extra)))
-    global_state.messages = global_state.messages[
-        : global_state.additional_values.get("message_history_size", 100)
-    ]
+            return
 
+        if event_action in {
+            "push",
+            "save",
+        }:
+            return
 
-def reconfigure(global_state: GlobalState) -> None:
-    """Reacts on changes to the configuration, e.g. applies"""
-    for ident, reference in global_state.last_referenced.items():
-        reference[1] = expiration_age_from_ident(ident, global_state)
+    elif event_type == "network":
+        if event_action == "connect":
+            await register_network(state, event_id)
+            return
 
-    # todo
-    # global_state.inform("refresh")
+        if event_action == "destroy":
+            unregister_network(state, event_id)
+            return
 
+        if event_action == "prune":
+            # cleanup networks - there seems to be no destroy
+            await cleanup_network_registrations(state)
+            return
 
-def setup_introspection():
-    setup_introspection_on_signal()
+        if event_action in {
+            "disconnect",
+        }:
+            return
 
+    elif event_type == "volume":
+        if event_action == "create":
+            await register_volume(state, event_id)
+            return
 
-async def response_control_ws(global_state) -> None:
-    """Provides a way to talk with a connected client"""
-    # Only allow clients we know
-    # user_id = websocket.cookies.get("session")
-    # log().debug(f"/control({user_id})")
-    # if not user_id:
-    # websocket.close()
+        if event_action == "destroy":
+            unregister_volume(state, event_id)
+            return
 
-    mqueue = global_state.new_update_queue()
-    await websocket.accept()
+        if event_action == "mount":
+            # todo: reference
+            return
 
-    try:
-        while True:
-            message = await mqueue.get()
-            await websocket.send(message)
-            reply = await websocket.receive()
-            log().debug("reply to '%s': '%s'", message, reply)
-    except asyncio.CancelledError:
-        raise
-    except Exception:
-        log().exception("Unhandled exception in control")
-    finally:
-        global_state.remove_queue(mqueue)
-        log().info("Connection closed")
+        if event_action == "prune":
+            # cleanup volumes - there seems to be no destroy
+            await cleanup_volume_registrations(state)
+            return
+
+        if event_action in {
+            "unmount",
+        }:
+            return
+
+    elif event_type == "builder":
+        if event_action in {
+            "prune",
+        }:
+            return
+
+    log().warning("unknown type/operator %s %s", event_type, event_action)
+
+
+def export_references(state: DockerState, filepath: Path) -> None:
+    """Write to disk all we need to restart without losing track of image references"""
+    with open(filepath, "w", encoding="utf-8") as eh_file:
+        json.dump(
+            {
+                "created": datetime.now().strftime("%Y.%m.%d-%H.%M.%S"),
+                "event_horizon": state.event_horizon,
+                "references": {
+                    ",".join(map(str, key)) if isinstance(key, tuple) else str: value
+                    for key, value in state.last_referenced.items()
+                },
+            },
+            eh_file,
+            indent=2,
+        )
+        log().info("exported image references")
+
+
+def import_references(state: DockerState, filepath: Path) -> None:
+    """Load image reference information from disk and restore event horizon if not too old"""
+    with suppress(FileNotFoundError):
+        with open(filepath, encoding="utf-8") as eh_file:
+            reference_data = json.load(eh_file)
+            created = datetime.strptime(reference_data["created"], "%Y.%m.%d-%H.%M.%S")
+            references = {
+                splitted[0] if len(splitted) == 1 else tuple(splitted): value
+                for key, value in reference_data["references"].items()
+                for splitted in (key.split(","),)
+            }
+            state.inform("info", "imported image references")
+            state.last_referenced = references
+            if (datetime.now() - created).total_seconds() < 60:
+                state.inform("info", "restored event horizon")
+                state.event_horizon = reference_data["event_horizon"]
+            else:
+                state.inform("warning", "event horizon too old to restore")
+
+
+async def main() -> None:
+    """Only for debugging purposes:
+    Asynchronously run reference application"""
+    from rich.logging import RichHandler  # pylint: disable=import-outside-toplevel
+
+    async def listen_messages(docker_state: DockerState) -> None:
+        """Print messages"""
+        async for mtype, mtext, mobj in docker_state.wait_for_change():
+            if mtype == "exception":
+                try:
+                    raise mobj  # type: ignore[misc]
+                except Exception:  # pylint: disable=broad-except
+                    log().exception(mtext)
+            elif mtype == "error":
+                log().error(mtext)
+            elif mtype == "warning":
+                log().warning(mtext)
+            elif mtype == "info":
+                log().info(mtext)
+            elif mtype == "client_disconnect":
+                raise SystemExit(1)
+            elif mtype in {"container_add", "container_del", "container_update"}:
+                cnt: Container = cast(Container, mobj)
+                log().info(
+                    "container info: %s / %s (%d total)",
+                    cnt.short_id,
+                    mtype,
+                    len(docker_state.containers),
+                )
+            elif mtype in {"image_add", "image_del", "image_update"}:
+                image = docker_state.images[mtext]
+
+                log().info(
+                    "image info: %s / %s (%d total)",
+                    image.short_id,
+                    mtype,
+                    len(docker_state.images),
+                )
+            elif mtype in {"reference_update", "reference_del"}:
+                ident = cast(ImageIdent, mobj)
+                log().info(
+                    "reference updated: %s (%d total)",
+                    ident,
+                    len(docker_state.last_referenced),
+                )
+            else:
+                log().error("don't know message type %s", mtype)
+
+    logging.basicConfig(
+        format="│ %(name)-10s │ %(message)s",
+        handlers=[RichHandler(show_path=False, markup=False, show_time=False)],
+    )
+    logging.getLogger().setLevel(logging.WARNING)
+    log().setLevel(logging.DEBUG)
+
+    await asyncio.gather(
+        (docker_state := DockerState()).run(),
+        listen_messages(docker_state),
+    )
+
+
+if __name__ == "__main__":
+    with suppress(KeyboardInterrupt):
+        asyncio.run(main())
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `docker_shaper-0.1.9/docker_shaper/utils.py` & `docker_shaper-2.0.0/docker_shaper/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,226 +1,140 @@
 #!/usr/bin/env python3
 
 """Common stuff shared among modules"""
 
 import asyncio
 import logging
 import os
-import shlex
+
+# import re
 import signal
 import sys
 import time
 import traceback
-from datetime import datetime
+
+# from datetime import datetime
 from functools import wraps
+from importlib.machinery import SourceFileLoader
+from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
-from subprocess import DEVNULL, check_output
+from types import ModuleType
 
-# we need 3.8 compatible typing (python on build nodes)
-from typing import AsyncIterator, Union, cast
+# from dateutil import tz
+from rich.logging import RichHandler
+from rich.markup import escape as markup_escape
 
-from asyncinotify import Event, Inotify, Mask
-from dateutil import tz
+from docker_shaper.dynamic import Container, short_id
 
-LOG_LEVELS = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
+# LOG_LEVELS = ("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL")
 
 
 def log() -> logging.Logger:
     """Logger for this module"""
     return logging.getLogger("docker-shaper")
 
 
-def setup_logging(level: str = "INFO") -> None:
-    """Make logging fun"""
-    for lev in LOG_LEVELS:
-        logging.addLevelName(getattr(logging, lev), f"{lev[0] * 2}")
-
-    logging.basicConfig(
-        format=(
-            "(%(levelname)s): %(message)s"
-            if os.environ.get("USER") == "root"
-            else "(%(levelname)s) %(asctime)s %(name)s: %(message)s"
-        ),
-        datefmt="%Y-%m-%d %H:%M:%S",
-        level=logging.DEBUG if level == "ALL_DEBUG" else logging.WARNING,
-    )
-    logging.getLogger().setLevel(getattr(logging, level.split("_")[-1]))
-    logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
+# def stack_str(depth: int = 0):
+# def stack_fns():
+# stack = list(
+# reversed(
+# traceback.extract_stack(sys._getframe(depth))  # pylint: disable=protected-access
+# )
+# )
+
+# for site in stack:
+# if site.filename != stack[0].filename or site.name == "<module>":
+# break
+# yield site.name
+
+# return ">".join(reversed(list(stack_fns())))
+
+
+# def setup_logging(level: str = "INFO") -> None:
+# """Make logging fun"""
+
+# class CustomLogger(logging.getLoggerClass()):
+# """Logger with stack information"""
+
+# def makeRecord(  # pylint: disable=too-many-arguments
+# self, name, level, fn, lno, msg, args, exc_info, func=None, extra=None, sinfo=None
+# ):
+# if extra is None:
+# extra = {}
+# extra["stack"] = stack_str(5)
+# return super().makeRecord(name, level, fn, lno, msg, args, exc_info, func, extra, sinfo)
+
+# logging.setLoggerClass(CustomLogger)
+
+# logging.getLogger().setLevel(logging.WARNING)
+# log().setLevel(getattr(logging, level.split("_")[-1]))
+## logging.getLogger("urllib3.connectionpool")
+# ch = RichHandler(show_path=False, markup=True, show_time=False)
+# ch.setLevel(getattr(logging, level.split("_")[-1]))
+# ch.setFormatter(
+# logging.Formatter(
+# "│ %(asctime)s │ [grey]%(stack)-55s[/] │ [bold white]%(message)s[/]",
+# datefmt="%Y-%m-%d %H:%M:%S",
+# )
+# )
+# log().handlers = [ch]
+# logging.getLogger("urllib3.connectionpool").setLevel(logging.INFO)
+
+# def markup_escaper(record: logging.LogRecord) -> bool:
+# record.args = record.args and tuple(
+# markup_escape(arg) if isinstance(arg, str) else arg for arg in record.args
+# )
+# record.msg = markup_escape(record.msg)
+# return True
+
+# ch.addFilter(markup_escaper)
+
+## https://stackoverflow.com/questions/76788727/how-can-i-change-the-debug-level-and-format-for-the-quart-i-e-hypercorn-logge
+## https://pgjones.gitlab.io/hypercorn/how_to_guides/logging.html#how-to-log
+## https://www.phind.com/agent?cache=clkqhh48y001smg0832tvq1rl
+
+## from quart.logging import default_handler
+## logging.getLogger('quart.app').removeHandler(default_handler)
+## logger = logging.getLogger("hypercorn.error")
+## logger.removeHandler(default_handler)
+## logger.addHandler(ch)
+## logger.setLevel(logging.WARNING)
+## logger.propagate = False
 
 
 def impatient(func):
     """Tells us, when a function takes suspiciously long"""
 
     @wraps(func)
     def run(*args: object, **kwargs: object) -> object:
+        t1 = time.time()
         try:
-            t1 = time.time()
             return func(*args, **kwargs)
         finally:
             if (duration := time.time() - t1) > 0.2:
-                log().warn("%s took %.2fs!", func.__name__, duration)
-            # log().info("%s took %.2fs!", func.__name__, duration)
+                log().warning("%s took %.2fs!", func.__name__, duration)
 
     return run
 
 
 def aimpatient(func):
     """Tells us, when a function takes suspiciously long"""
 
     @wraps(func)
     async def run(*args: object, **kwargs: object) -> object:
+        t1 = time.time()
         try:
-            t1 = time.time()
             return await func(*args, **kwargs)
         finally:
             if (duration := time.time() - t1) > 0.1:
                 log().warning("%s took %.2fs!", func.__name__, duration)
-            # log().info("%s took %.2fs!", func.__name__, duration)
 
     return run
 
 
-async def fs_changes(
-    *paths: Path,
-    queue: asyncio.Queue = asyncio.Queue(),
-    mask: Mask = Mask.CLOSE_WRITE | Mask.MOVED_TO | Mask.CREATE,
-    postpone: bool = False,
-    timeout: float = 2,
-) -> AsyncIterator[Path]:
-    """Controllable, timed filesystem watcher"""
-
-    # pylint: disable=too-many-locals
-
-    async def fuse_fn(queue: asyncio.Queue, timeout: float) -> None:
-        await asyncio.sleep(timeout)
-        await queue.put("timeout")
-
-    def task(name: str) -> asyncio.Task:
-        """Creates a task from a name identifying a data source to read from"""
-        return asyncio.create_task(
-            cast(Union[asyncio.Queue, Inotify], {"inotify": inotify, "mqueue": queue}[name]).get(),
-            name=name,
-        )
-
-    with Inotify() as inotify:
-        for path in paths:
-            inotify.add_watch(path, mask)
-        fuse = None
-        changed_files = set()
-        tasks = set(map(task, ("inotify", "mqueue")))
-
-        while True:
-            done, tasks = await asyncio.wait(
-                fs=tasks,
-                return_when=asyncio.FIRST_COMPLETED,
-            )
-            for event in done:
-                event_type, event_value = event.get_name(), event.result()
-                tasks.add(task(event_type))
-                if event_type == "inotify":
-                    assert isinstance(event_value, Event)
-                    if event_value.path:
-                        changed_files.add(event_value.path)
-                    if postpone and fuse:
-                        fuse.cancel()
-                        del fuse
-                        fuse = None
-                    if not fuse:
-                        fuse = asyncio.create_task(fuse_fn(queue, timeout))
-                elif event_type == "mqueue":
-                    if event_value == "timeout":
-                        del fuse
-                        fuse = None
-                        for file in changed_files:
-                            yield file
-                        changed_files.clear()
-
-
-async def read_process_output(cmd: str) -> AsyncIterator[str]:
-    """Run a process asynchronously and handle each line on stdout using provided callback"""
-    process = await asyncio.create_subprocess_exec(
-        *shlex.split(cmd),
-        stdout=asyncio.subprocess.PIPE,
-    )
-    assert process.stdout
-    while True:
-        if not (line := (await process.stdout.readline()).decode().strip("\n")):
-            break
-        yield line
-
-
-def process_output(cmd: str) -> str:
-    """Return command output as one blob"""
-    return check_output(shlex.split(cmd), stderr=DEVNULL, text=True)
-
-
-def dur_str(seconds: int, fixed=False) -> str:
-    """Turns a number of seconds into a string like 1d:2h:3m"""
-    if not fixed and not seconds:
-        return "0s"
-    digits = 2 if fixed else 1
-    days = f"{seconds//86400:0{digits}d}d" if fixed or seconds >= 86400 else ""
-    hours = (
-        f"{seconds//3600%24:0{digits}d}h" if fixed or seconds >= 3600 and (seconds % 86400) else ""
-    )
-    minutes = f"{seconds//60%60:0{digits}d}m" if fixed or seconds >= 60 and (seconds % 3600) else ""
-    seconds_str = (
-        f"{seconds%60:0{digits}d}s" if not fixed and ((seconds % 60) or seconds == 0) else ""
-    )
-    return ":".join(e for e in (days, hours, minutes, seconds_str) if e)
-
-
-def age_str(now: Union[int, datetime], age: Union[int, datetime, None], fixed: bool = False) -> str:
-    """Turn a number of seconds into something human readable"""
-    if age is None:
-        return "--"
-    return dur_str(
-        int(
-            (now.timestamp() if isinstance(now, datetime) else now)
-            - (age.timestamp() if isinstance(age, datetime) else age)
-        ),
-        fixed=fixed,
-    )
-
-
-def date_str(date: datetime) -> str:
-    if not date:
-        return "--"
-    return (date if isinstance(date, datetime) else datetime.fromtimestamp(date)).strftime(
-        "%Y.%m.%d-%H:%M:%S"
-    )
-
-
-def date_from(timestamp: Union[int, float, str]) -> Union[None, datetime]:
-    """
-    >>> date_from("2023-07-14T15:05:32.174200714+02:00")
-    ?
-    """
-    try:
-        if isinstance(timestamp, datetime):
-            return timestamp
-
-        if isinstance(timestamp, (int, float)):
-            return datetime.fromtimestamp(timestamp)
-
-        if timestamp[-1] == "Z":
-            return (
-                datetime.strptime(timestamp[:19], "%Y-%m-%dT%H:%M:%S")
-                .replace(tzinfo=tz.tzutc())
-                .astimezone(tz.tzlocal())
-            )
-        if len(timestamp) == 35:
-            timestamp = timestamp[:19] + timestamp[-6:]
-        return datetime.strptime(timestamp, "%Y-%m-%dT%H:%M:%S%z")
-    except OverflowError:
-        return None
-    except Exception as exc:
-        raise ValueError(f"Could not parse datetime from <{timestamp!r}> ({exc})") from exc
-
-
 def increase_loglevel(*_):
     """Become one level more verbose.
     If level is already DEBUG we go back to WARNING.
     """
     try:
         new_level = {
             logging.WARNING: logging.INFO,
@@ -234,15 +148,15 @@
             logging.CRITICAL: "CRITICAL",
             logging.ERROR: "ERROR",
             logging.WARNING: "WARNING",
             logging.INFO: "INFO",
             logging.DEBUG: "DEBUG",
         }[new_level]
         print(f"increase_loglevel to {level}", file=sys.stderr)
-    except Exception:
+    except Exception:  # pylint: disable=broad-except
         log().exception("Could not fully write application stack trace")
 
 
 def print_stacktrace_on_signal(sig, frame):
     """interrupt running process, and provide a python prompt for
     interactive debugging.
     see http://stackoverflow.com/questions/132058
@@ -261,24 +175,64 @@
             print_stack_frame(frame, file)
             for task in asyncio.all_tasks():
                 print(f"++++++ {task.get_coro().__name__} ++++++++", file=file)
                 for stack in task.get_stack(limit=1000):
                     print_stack_frame(stack, file)
 
         print_stack_frames(sys.stderr)
-        with open(Path("~/.docker_shaper/traceback.log").expanduser(), "w") as trace_file:
+        with open(
+            Path("~/.docker_shaper/traceback.log").expanduser(), "w", encoding="utf-8"
+        ) as trace_file:
             print_stack_frames(trace_file)
-    except Exception:
+            print(f"traceback also written to {trace_file}", file=sys.stderr)
+    except Exception:  # pylint: disable=broad-except
         log().exception("Could not fully write application stack trace")
 
 
 def setup_introspection_on_signal():
     """Install signal handlers for some debug stuff"""
 
     def setup_signal(sig, func, msg):
         signal.signal(sig, func)
         signal.siginterrupt(sig, False)
         sig_str = {signal.SIGUSR1: "USR1", signal.SIGUSR2: "USR2"}.get(sig, sig)
         print(f"Run `kill -{sig_str} {os.getpid()}` to {msg}", file=sys.stderr)
 
     setup_signal(signal.SIGUSR1, increase_loglevel, "increase log level")
     setup_signal(signal.SIGUSR2, print_stacktrace_on_signal, "print stacktrace")
+
+
+def load_module(path: Path) -> ModuleType:
+    """Loads a module from a file path"""
+    spec = spec_from_file_location("dynamic_config", path)
+    if not (spec and spec.loader):
+        raise RuntimeError("Could not load")
+    module = module_from_spec(spec)
+    assert module
+    # assert isinstance(spec.loader, SourceFileLoader)
+    loader: SourceFileLoader = spec.loader
+    loader.exec_module(module)
+    return module
+
+
+def get_hostname() -> str:
+    """Returns local hostname read from /etc/hostname"""
+    with open("/etc/hostname", encoding="utf-8") as hostname_file:
+        return hostname_file.read().strip()
+
+
+def container_markup(container: Container) -> str:
+    status_markups = {"running": "cyan bold"}
+    image_str, status_str = (
+        ("", "")
+        if not container.show
+        else (
+            f" image:[bold]{short_id(container.show.Image)}[/]",
+            f" - [{status_markups.get(container.show.State.Status, 'grey53')}]"
+            f"{container.show.State.Status:7s}[/]",
+        )
+    )
+    return (
+        f"[bold]{container.short_id}[/] / {container.name:<26s}{image_str}{status_str}"
+        f" - {container.cpu_usage() * 100:7.2f}%"
+        f" - {container.mem_usage() >> 20:6d}MiB"
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `docker_shaper-0.1.9/pyproject.toml` & `docker_shaper-2.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,96 @@
 [tool.poetry]
 name = "docker-shaper"
-version = "0.1.9"
+version = "2.0.0"
 description = "Keeps Docker resources in shape based on rules and usage"
 authors = ["Frans Fürst <frans.fuerst@checkmk.com>"]
 repository = "https://github.com/Checkmk/checkmk-dev-tools"
 readme = "Readme.md"
 packages = [
   {include = "docker_shaper/**/*.py"},
-  {include = "docker_shaper/static"},
-  {include = "docker_shaper/templates"},
 ]
 
+
 [tool.poetry.scripts]
-docker-shaper = 'docker_shaper.cli:main'
+docker-shaper = 'docker_shaper.server:main'
+dockermon = 'docker_shaper.headless_examples.dockermon:main'
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<4.0.0"
-aiodocker = "^0.21.0"
-asyncinotify = "^4.0.1"
-quart = "^0.18.4"
-flask-table = "^0.5.0"
-python-dateutil = "^2.8.2"
+python = "^3.10.4"
+aiodocker = "^0"
+
+pytz = "^2023.3.post1"
+apparat = "^0.0.8"
+pydantic = "^2.4"
+rich = "^13"
+textual = "^0"
+psutil = "^5.9.8"
+
+trickkiste = "^0.0.10"
+#trickkiste  = {path = "/home/frafue/_HOME/trickkiste", develop = true}
+python-dateutil = "^2"  # needed by trickkiste but not set as dependency (intentionally)
+
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.6.0"
-isort = "^5.10.1"
-flake8 = "^4.0.1"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-mypy = "^1.2"
-pylint = "^2.15.3"
-ipython = "^8.8.0"
-types-pyyaml = "^6.0.12.6"
-twine = "^4.0.2"
-yamllint = "^1.29.0"
-pylint-per-file-ignores = "^1.2.1"
-types-python-dateutil = "^2.8.19.13"
+black = "*"
+isort = "*"
+flake8 = "*"
+pytest = "*"
+mypy = "*"
+pylint = "*"
+ipython = "*"
+twine = "*"
+yamllint = "*"
+pytest-cov = "*"
+types-pyyaml = "*"
+pylint-per-file-ignores = "*"
+types-python-dateutil = "*"
+pre-commit = "*"
+
+# see https://pypi.org/project/poetry-bumpversion
+[tool.poetry_bumpversion.file."docker_shaper/__init__.py"]
+[tool.poetry_bumpversion.file."docker_shaper/server.py"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ['py311']
 include = '\.pyi?$'
 fast = true
 exclude = '''
 (
   /(                        # exclude a few common directories in the
     \.git                   # root of the project
     | \.pytest_cache
     | untracked
     | \.venv
     | \.container_home_dir
     | dist
   ))
 '''
 
+
 [tool.isort]
 profile = "black"
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.10.12"
 strict="True"
 disallow_untyped_defs = "True"
 disallow_any_unimported = "True"
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
-exclude = [
-    '\.venv',
-    '\.container_home_dir',
-]
+exclude = []
 mypy_path="typeshed"
 
 [tool.pylint]
 #ignore = [".venv", "untracked"]
 
 # Files or directories matching the regular expression patterns are skipped. The
 # regex matches against base names, not paths. The default value ignores Emacs
@@ -87,12 +98,7 @@
 #ignore-patterns = ["^\\.#"]
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
 # number of processors available to use, and will cap the count on Windows to
 # avoid hangs.
 jobs = 0
 
-[tool.pylint.MASTER]
-load-plugins=["pylint_per_file_ignores"]
-
-[tool.pylint-per-file-ignores]
-"pocketrockit/examples/" = "invalid-name"
```

### Comparing `docker_shaper-0.1.9/PKG-INFO` & `docker_shaper-2.0.0/Readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,112 +1,52 @@
-Metadata-Version: 2.1
-Name: docker-shaper
-Version: 0.1.9
-Summary: Keeps Docker resources in shape based on rules and usage
-Home-page: https://github.com/Checkmk/checkmk-dev-tools
-Author: Frans Fürst
-Author-email: frans.fuerst@checkmk.com
-Requires-Python: >=3.8.1,<4.0.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiodocker (>=0.21.0,<0.22.0)
-Requires-Dist: asyncinotify (>=4.0.1,<5.0.0)
-Requires-Dist: flask-table (>=0.5.0,<0.6.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: quart (>=0.18.4,<0.19.0)
-Project-URL: Repository, https://github.com/Checkmk/checkmk-dev-tools
-Description-Content-Type: text/markdown
-
 # Docker Shaper
 
-This repository includes scripts/tools for Checkmk developers.
+This is a spin-off package for the `docker-shaper` tool, which can be used to monitor Docker stuff
+like containers, images and volumes and automatically enforce certain cleanup-rules.
 
 
 ## Installation
 
 ```sh
 [<PYTHON> -m] pip[3] install [--user] [--upgrade] docker-shaper
 ```
 
 
 ## Usage
 
 ```
 docker-shaper serve`
 ```
-Navigate to e.g. http://build-fra-003:5432/
-
 
-## Development & Contribution
+=> Navigate to e.g. http://my-build-node:5432/
 
-### Todo
-
-- [x] pip package
-- [x] Quart interface
-- [x] bring in dockermon
-- [x] auto update
-- [x] outsource config
-- [x] bring in dgcd
-- [x] new: untag certain tags
-- [x] new: container cleanup
-- [x] Fix `none` image lookup
-- [x] Exceptions to messages
-- [x] Clip
-- [x] Increase/decrease logging via web / signal
-- [x] Link: cleanup (images/containers) now
-- [x] Add volumes list (with recent owners)
-- [ ] Bring in `list_volumes` (volume monitoring)
-- [ ] Containers: show total CPU usage
-- [ ] Containers: list volumes
-- [ ] Volumes: list usage
-- [ ] Persist messages
-- [ ] Instructions to readme
-- [ ] List unmatched / overmatched tags
-- [ ] Links to `delete` / `remove`
-- [ ] Links to jobs
-- [ ] Link: inspect
-- [ ] Graph: cpu / containers (idle/up)
-- [ ] Authenticate (at least if we can modify behavior, like stopping/removing images/containers)
-
-
-### Setup
 
+## Development & Contribution
 
 ### Prerequisites
 
-* Python 3.8.10
-* `poetry`
-* `pre-commit`
-
+* Python 3.8.10+ (e.g. via `pyenv`)
+* `poetry` and `pre-commit`
+  `python3 -m pip install --upgrade --user poetry pre-commit`
 
 ```sh
-python3 -m pip install --upgrade --user poetry pre-commit
-git clone ssh://review.lan.tribe29.com:29418/checkmk_ci
-cd checkmk_ci
+git clone https://github.com/Checkmk/checkmk-dev-tools
+cd checkmk-dev-tools/additional_packages/docker_shaper
 pre-commit install
 # if you need a specific version of Python inside your dev environment
 poetry env use ~/.pyenv/versions/3.8.10/bin/python3
 poetry install
 ```
 
 
 ### Workflow
 
-poetry config repositories.checkmk https://upload.pypi.org/legacy/
-poetry config pypi-token.checkmk pypi-
-
-pip3 install --user --upgrade docker-shaper
-~/.local/bin/docker-shaper server
-
-poetry run mypy docker_shaper
-
 * (once and only for publishing to PyPi) Get token on PyPi.org
-* (once and only for publishing to PyPi) `poetry config pypi-token.pypi pypi-<LONG-STRING>`
+* (maybe) setup distinct repository setup `poetry config repositories.checkmk https://upload.pypi.org/legacy/`
+* (once and only for publishing to PyPi) `poetry config pypi-token.checkmk pypi-<LONG-STRING>`
   (will write to `~/.config/pypoetry/auth.toml`)
 * modify and check commits via `pre-commit`
 * after work is done locally:
   - adapt version in `pyproject.toml`
   - build and check a package
 ```sh
 poetry build && \
@@ -116,16 +56,72 @@
 ```
   - check installed package
   - go through review process
   - publish the new package `poetry publish --build --repository checkmk`
   - commit new version && push
 
 
+## Todo
+
+- [x] Fix: stuck auto-reload: was: postpone=True + monitoring log
+- [x] Fix: crawl-images should fix parents not having them listed
+- [-] Fix: stuck crawl images (too many async requests, does not happen in production)
+- [ ] Fix: `'677aff0727' could not be removed: DockerError(404, 'No such image: 677aff0727:latest')`
+- [ ] Fix: `tried to remove container 4f5fb0848c unknown to us`
+- [ ] Fix: Crashes (see runlog)
+- [ ] Image update message only if needed
+- [ ] New TUI
+    - make ongoing progress visible
+- [ ] review log levels (too verbose)
+- [ ] answer https://stackoverflow.com/questions/32723111
+
+- [x] installable via `pip install`
+- [x] Quart interface (instead of `flask`)
+- [x] auto-apply changes to source and configuration files
+- [x] outsourced config file
+- [x] bring in features of former `dgcd`
+- [x] bring in features of former `dockermon`
+- [x] untag certain tags
+- [x] container cleanup
+- [x] Fix `none` image lookup
+- [x] Exceptions to messages
+- [x] Clip
+- [x] Increase/decrease logging via web / signal
+- [x] Link: cleanup (images/containers) now
+- [x] Add volumes list (with recent owners)
+- [x] Containers: Store CPU / Memory usage over time
+- [x] Containers: store history
+- [x] Persist messages
+- [ ] Remove old message/container logs
+- [ ] Show different color for unmatched images
+- [ ] Warn about use of unpinned / upstream images
+- [ ] Handle 'build cache objects' (found on system prune)
+- [ ] Bring in volume monitoring: which volumes have been created and used by which containers?
+- [ ] Containers: show total CPU usage
+- [ ] Containers: list volumes
+- [ ] Images: list parents / children
+- [ ] Volumes: list usage
+- [ ] Instructions to readme
+- [ ] List unmatched / overmatched tags
+- [ ] Links to `delete` / `remove`
+- [ ] Links to jobs
+- [ ] Link: inspect
+- [ ] Graph: cpu / containers (idle/up)
+- [ ] Authenticate (at least if we can modify behavior, like stopping/removing images/containers)
+
+
 ## Knowledge
+
+(just misc links to articles that helped me out)
+* [How to delete docker images from Nexus Repository 3](https://support.sonatype.com/hc/en-us/articles/360009696054-How-to-delete-docker-images-from-Nexus-Repository-3)
 * [Showing Text Box On Hover (In Table)](https://stackoverflow.com/questions/52562345/showing-text-box-on-hover-in-table)
 * [Beautiful Interactive Tables for your Flask Templates](https://blog.miguelgrinberg.com/post/beautiful-interactive-tables-for-your-flask-templates)
 * https://github.com/torfsen/python-systemd-tutorial
 * https://www.digitalocean.com/community/tutorials/how-to-use-templates-in-a-flask-application
 * https://stackoverflow.com/questions/49957034/live-updating-dynamic-variable-on-html-with-flask
 * https://pgjones.gitlab.io/quart/how_to_guides/templating.html
 
 
+### Logging
+
+* https://pgjones.gitlab.io/hypercorn/how_to_guides/logging.html#how-to-log
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

