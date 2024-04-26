# Comparing `tmp/mergify_cli-2024.4.8.14.47.tar.gz` & `tmp/mergify_cli-2024.4.9.11.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mergify_cli-2024.4.8.14.47.tar", max compression
+gzip compressed data, was "mergify_cli-2024.4.9.11.31.tar", max compression
```

## Comparing `mergify_cli-2024.4.8.14.47.tar` & `mergify_cli-2024.4.9.11.31.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    10143 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/LICENSE
--rw-r--r--   0        0        0     1127 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/README.md
--rwxr-xr-x   0        0        0    25540 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/__init__.py
--rw-r--r--   0        0        0     1797 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/hooks/commit-msg
--rw-r--r--   0        0        0        0 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/__init__.py
--rw-r--r--   0        0        0    16887 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/test_mergify_cli.py
--rw-r--r--   0        0        0     2093 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/mergify_cli/tests/utils.py
--rw-r--r--   0        0        0     2598 2024-04-08 14:47:18.564366 mergify_cli-2024.4.8.14.47/pyproject.toml
--rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 mergify_cli-2024.4.8.14.47/PKG-INFO
+-rw-r--r--   0        0        0    10143 2024-04-09 11:31:53.528693 mergify_cli-2024.4.9.11.31/LICENSE
+-rw-r--r--   0        0        0     1127 2024-04-09 11:31:53.528693 mergify_cli-2024.4.9.11.31/README.md
+-rwxr-xr-x   0        0        0    25342 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/hooks/commit-msg
+-rw-r--r--   0        0        0        0 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/__init__.py
+-rw-r--r--   0        0        0    16292 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/test_mergify_cli.py
+-rw-r--r--   0        0        0     2339 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/mergify_cli/tests/utils.py
+-rw-r--r--   0        0        0     2598 2024-04-09 11:31:53.532693 mergify_cli-2024.4.9.11.31/pyproject.toml
+-rw-r--r--   0        0        0     1803 1970-01-01 00:00:00.000000 mergify_cli-2024.4.9.11.31/PKG-INFO
```

### Comparing `mergify_cli-2024.4.8.14.47/LICENSE` & `mergify_cli-2024.4.9.11.31/LICENSE`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.8.14.47/README.md` & `mergify_cli-2024.4.9.11.31/README.md`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.8.14.47/mergify_cli/__init__.py` & `mergify_cli-2024.4.9.11.31/mergify_cli/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 
 import argparse
 import asyncio
+import contextlib
 import dataclasses
 import importlib.metadata
 import os
 import pathlib
 import re
 import shutil
 import subprocess
@@ -37,14 +38,15 @@
 
 CHANGEID_RE = re.compile(r"Change-Id: (I[0-9a-z]{40})")
 READY_FOR_REVIEW_TEMPLATE = 'mutation { markPullRequestReadyForReview(input: { pullRequestId: "%s" }) { clientMutationId } }'
 DRAFT_TEMPLATE = 'mutation { convertPullRequestToDraft(input: { pullRequestId: "%s" }) { clientMutationId } }'
 console = rich.console.Console(log_path=False, log_time=False)
 
 DEBUG = False
+TMP_STACK_BRANCH = "mergify-cli-tmp"
 
 
 def check_for_graphql_errors(response: httpx.Response) -> None:
     data = response.json()
     if "errors" in data:
         console.print(f"url: {response.request.url}", style="red")
         console.print(f"data: {response.request.content.decode()}", style="red")
@@ -59,15 +61,16 @@
 def check_for_status(response: httpx.Response) -> None:
     if response.status_code < 400:
         return
 
     if response.status_code < 500:
         data = response.json()
         console.print(f"url: {response.request.url}", style="red")
-        console.print(f"data: {response.request.content.decode()}", style="red")
+        with contextlib.suppress(httpx.RequestNotRead):
+            console.print(f"data: {response.request.content.decode()}", style="red")
         console.print(
             f"HTTPError {response.status_code}: {data['message']}",
             style="red",
         )
         if "errors" in data:
             console.print(
                 "\n".join(f"* {e.get('message') or e}" for e in data["errors"]),
@@ -306,43 +309,39 @@
     @staticmethod
     def is_stack_comment(comment: Comment) -> bool:
         return comment["body"].startswith(StackComment.STACK_COMMENT_FIRST_LINE)
 
 
 async def create_or_update_stack(  # noqa: PLR0913,PLR0917
     client: httpx.AsyncClient,
+    remote: str,
     stacked_base_branch: str,
     stacked_dest_branch: str,
     changeid: ChangeId,
     commit: str,
     title: str,
     message: str,
     known_changeids: KnownChangeIDs,
     create_as_draft: bool,
     keep_pull_request_title_and_body: bool,
 ) -> tuple[PullRequest, str]:
     if changeid in known_changeids:
         pull = known_changeids.get(changeid)
-        with console.status(
-            f"* updating stacked branch `{stacked_dest_branch}` ({commit[-7:]}) - {pull['html_url'] if pull else '<stack branch without associated pull>'})",
-        ):
-            r = await client.patch(
-                f"git/refs/heads/{stacked_dest_branch}",
-                json={"sha": commit, "force": True},
-            )
+        status_message = f"* updating stacked branch `{stacked_dest_branch}` ({commit[-7:]}) - {pull['html_url'] if pull else '<stack branch without associated pull>'})"
     else:
-        with console.status(
-            f"* creating stacked branch `{stacked_dest_branch}` ({commit[-7:]})",
-        ):
-            r = await client.post(
-                "git/refs",
-                json={"ref": f"refs/heads/{stacked_dest_branch}", "sha": commit},
-            )
+        status_message = (
+            f"* creating stacked branch `{stacked_dest_branch}` ({commit[-7:]})"
+        )
 
-    check_for_status(r)
+    with console.status(status_message):
+        await git(f"branch {TMP_STACK_BRANCH} {commit}")
+        try:
+            await git(f"push -f {remote} {TMP_STACK_BRANCH}:{stacked_dest_branch}")
+        finally:
+            await git(f"branch -D {TMP_STACK_BRANCH}")
 
     pull = known_changeids.get(changeid)
     if pull and pull["head"]["sha"] == commit:
         action = "nothing"
     elif pull:
         action = "updated"
         with console.status(
@@ -532,20 +531,14 @@
         else:
             with console.status(
                 f"Rebasing branch `{dest_branch}` on `{remote}/{base_branch}`...",
             ):
                 await git(f"pull --rebase {remote} {base_branch}")
             console.log(f"branch `{dest_branch}` rebased on `{remote}/{base_branch}`")
 
-        with console.status(
-            f"Pushing branch `{dest_branch}` to `{remote}/{stack_prefix}/aio`...",
-        ):
-            await git(f"push -f {remote} {dest_branch}:{stack_prefix}/aio")
-        console.log(f"branch `{dest_branch}` pushed to `{remote}/{stack_prefix}/aio` ")
-
     base_commit_sha = await git(f"merge-base --fork-point {remote}/{base_branch}")
     if not base_commit_sha:
         console.log(
             f"Common commit between `{remote}/{base_branch}` and `{dest_branch}` branches not found",
             style="red",
         )
         sys.exit(1)
@@ -583,14 +576,15 @@
             refs = typing.cast(list[GitRef], r.json())
 
             tasks = [
                 asyncio.create_task(
                     get_changeid_and_pull(client, user, stack_prefix, ref),
                 )
                 for ref in refs
+                # For backward compat
                 if not ref["ref"].endswith("/aio")
             ]
             if tasks:
                 done, _ = await asyncio.wait(tasks)
                 for task in done:
                     known_changeids.update(dict([await task]))
 
@@ -617,14 +611,15 @@
         continue_create_or_update = True
         for changeid, commit, title, message in changes:
             depends_on = pulls[-1] if pulls else None
             stacked_dest_branch = f"{stack_prefix}/{changeid}"
             if continue_create_or_update:
                 pull, action = await create_or_update_stack(
                     client,
+                    remote,
                     stacked_base_branch,
                     stacked_dest_branch,
                     changeid,
                     commit,
                     title,
                     format_pull_description(message, depends_on),
                     known_changeids,
```

### Comparing `mergify_cli-2024.4.8.14.47/mergify_cli/hooks/commit-msg` & `mergify_cli-2024.4.9.11.31/mergify_cli/hooks/commit-msg`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.8.14.47/mergify_cli/tests/test_mergify_cli.py` & `mergify_cli-2024.4.9.11.31/mergify_cli/tests/test_mergify_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,14 @@
     )
 
     # Mock HTTP calls
     respx_mock.get("/repos/user/repo/git/matching-refs/heads//current-branch/").respond(
         200,
         json=[],
     )
-    respx_mock.post("/repos/user/repo/git/refs").respond(200, json={})
     post_pull1_mock = respx_mock.post(
         "/repos/user/repo/pulls",
         json__title="Title commit 1",
     ).respond(
         200,
         json={
             "html_url": "https://github.com/repo/user/pull/1",
@@ -228,15 +227,14 @@
     )
 
     # Mock HTTP calls
     respx_mock.get("/repos/user/repo/git/matching-refs/heads//current-branch/").respond(
         200,
         json=[],
     )
-    respx_mock.post("/repos/user/repo/git/refs").respond(200, json={})
     post_pull_mock = respx_mock.post(
         "/repos/user/repo/pulls",
         json__title="Title commit 1",
     ).respond(
         200,
         json={
             "html_url": "https://github.com/repo/user/pull/1",
@@ -307,17 +305,14 @@
                 "head": {"sha": "previous_commit_sha"},
                 "state": "open",
                 "draft": False,
                 "node_id": "",
             },
         ],
     )
-    respx_mock.patch(
-        "/repos/user/repo/git/refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
-    ).respond(200, json={})
     patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
         200,
         json={},
     )
     respx_mock.get("/repos/user/repo/issues/123/comments").respond(
         200,
         json=[
@@ -386,17 +381,14 @@
                 "head": {"sha": "previous_commit_sha"},
                 "state": "open",
                 "draft": False,
                 "node_id": "",
             },
         ],
     )
-    respx_mock.patch(
-        "/repos/user/repo/git/refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
-    ).respond(200, json={})
     patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
         200,
         json={},
     )
     respx_mock.get("/repos/user/repo/issues/123/comments").respond(
         200,
         json=[
@@ -465,17 +457,14 @@
                 "head": {"sha": "previous_commit_sha"},
                 "state": "open",
                 "draft": False,
                 "node_id": "",
             },
         ],
     )
-    respx_mock.patch(
-        "/repos/user/repo/git/refs/heads//current-branch/I29617d37762fd69809c255d7e7073cb11f8fbf50",
-    ).respond(200, json={})
     patch_pull_mock = respx_mock.patch("/repos/user/repo/pulls/123").respond(
         200,
         json={},
     )
     respx_mock.get("/repos/user/repo/issues/123/comments").respond(
         200,
         json=[
```

### Comparing `mergify_cli-2024.4.8.14.47/mergify_cli/tests/utils.py` & `mergify_cli-2024.4.9.11.31/mergify_cli/tests/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,7 +56,13 @@
         # Commit title
         self.mock(f"log -1 --format='%s' {commit['sha']}", commit["title"])
         # List of commit SHAs
         self.mock(
             "log --format='%H' base_commit_sha..current-branch",
             "\n".join(c["sha"] for c in reversed(self._commits)),
         )
+        self.mock(f"branch mergify-cli-tmp {commit['sha']}", "")
+        self.mock("branch -D mergify-cli-tmp", "")
+        self.mock(
+            f"push -f origin mergify-cli-tmp:/current-branch/{commit['change_id']}",
+            "",
+        )
```

### Comparing `mergify_cli-2024.4.8.14.47/pyproject.toml` & `mergify_cli-2024.4.9.11.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mergify_cli-2024.4.8.14.47/PKG-INFO` & `mergify_cli-2024.4.9.11.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mergify_cli
-Version: 2024.4.8.14.47
+Version: 2024.4.9.11.31
 Summary: Mergify CLI is a tool that automates the creation and management of stacked pull requests on GitHub
 License: Apache License
 Author: Mehdi Abaakouk
 Author-email: sileht@mergify.com
 Requires-Python: >=3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

