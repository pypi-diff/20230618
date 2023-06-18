# Comparing `tmp/gitmopy-0.3.1.tar.gz` & `tmp/gitmopy-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitmopy-0.3.1.tar", max compression
+gzip compressed data, was "gitmopy-0.3.2.tar", max compression
```

## Comparing `gitmopy-0.3.1.tar` & `gitmopy-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.1/LICENSE
--rw-r--r--   0        0        0     6463 2023-06-16 20:29:37.545684 gitmopy-0.3.1/README.md
--rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.1/gitmopy/__init__.py
--rw-r--r--   0        0        0    12141 2023-06-16 23:33:09.831575 gitmopy-0.3.1/gitmopy/cli.py
--rw-r--r--   0        0        0     4961 2023-06-16 23:35:02.460050 gitmopy-0.3.1/gitmopy/git.py
--rw-r--r--   0        0        0     2989 2023-06-16 22:57:56.570034 gitmopy-0.3.1/gitmopy/history.py
--rw-r--r--   0        0        0     8085 2023-06-16 23:05:04.031161 gitmopy-0.3.1/gitmopy/prompt.py
--rw-r--r--   0        0        0    20219 2023-06-16 23:13:01.706550 gitmopy-0.3.1/gitmopy/utils.py
--rw-r--r--   0        0        0      578 2023-06-16 23:06:27.602301 gitmopy-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     7429 1970-01-01 00:00:00.000000 gitmopy-0.3.1/setup.py
--rw-r--r--   0        0        0     7091 1970-01-01 00:00:00.000000 gitmopy-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-16 22:59:50.534602 gitmopy-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7683 2023-06-18 20:40:56.282671 gitmopy-0.3.2/README.md
+-rw-r--r--   0        0        0      112 2023-06-16 19:39:04.304895 gitmopy-0.3.2/gitmopy/__init__.py
+-rw-r--r--   0        0        0    14362 2023-06-18 20:57:59.788436 gitmopy-0.3.2/gitmopy/cli.py
+-rw-r--r--   0        0        0     5913 2023-06-18 20:32:40.124115 gitmopy-0.3.2/gitmopy/git.py
+-rw-r--r--   0        0        0     2989 2023-06-16 22:57:56.570034 gitmopy-0.3.2/gitmopy/history.py
+-rw-r--r--   0        0        0     8085 2023-06-18 20:57:59.722229 gitmopy-0.3.2/gitmopy/prompt.py
+-rw-r--r--   0        0        0    20342 2023-06-18 20:17:35.746117 gitmopy-0.3.2/gitmopy/utils.py
+-rw-r--r--   0        0        0      578 2023-06-18 20:56:57.856741 gitmopy-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     8664 1970-01-01 00:00:00.000000 gitmopy-0.3.2/setup.py
+-rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 gitmopy-0.3.2/PKG-INFO
```

### Comparing `gitmopy-0.3.1/LICENSE` & `gitmopy-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.1/README.md` & `gitmopy-0.3.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gitmopy
+# `gitmopy`
 
 An interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/
 
 ```text
 pip install gitmopy
 ```
 
@@ -74,14 +74,16 @@
 $ gitmopy info
 
 # print helps
 $ gitmopy --help
 $ gitmopy commit --help
 ```
 
+⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.
+
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
   version : 0.1.0
@@ -134,23 +136,34 @@
 
  Usage: gitmopy commit [OPTIONS]
 
  Commit staged files. Use --add to interactively select files to stage if none is
  already staged
 
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
-│ --repo                 TEXT  Path to the git repository [default: .]                │
-│ --add     --no-add           Whether or not to interactively select files to stage  │
-│                              if none is already staged                              │
-│                              [default: no-add]                                      │
-│ --push    --no-push          Whether to `git push` after commit. Disabled by        │
-│                              default.                                               │
-│                              [default: no-push]                                     │
-│ --dry     --no-dry           Whether or not to actually commit. [default: no-dry]   │
-│ --help                       Show this message and exit.                            │
+│ --repo                             TEXT  Path to the git repository [default: .]    │
+│ --add           --no-add                 Whether or not to interactively select     │
+│                                          files to stage if none is already staged   │
+│                                          [default: no-add]                          │
+│ --push          --no-push                Whether to `git push` after commit. If     │
+│                                          multiple remotes exist, you will be asked  │
+│                                          to interactively choose the ones to push   │
+│                                          to. Use --remote to skip interactive       │
+│                                          selection. Disabled by default.            │
+│                                          [default: no-push]                         │
+│ --dry           --no-dry                 Whether or not to actually commit.         │
+│                                          [default: no-dry]                          │
+│ --remote                           TEXT  Remote to push to after commit. Use to     │
+│                                          skip interactive remote selection when     │
+│                                          several exist. Use several '--remote       │
+│                                          {remote name}' to push to multiple remotes │
+│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │
+│                                          commit, to be ready for another one.       │
+│                                          [default: no-keep-alive]                   │
+│ --help                                   Show this message and exit.                │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## To Do
 
 * Features
   * *If requested:*
@@ -161,14 +174,14 @@
   * https://typer.tiangolo.com/tutorial/testing/
   * 👋 **Help wanted**
 * Docs
   * Not critical
 
 ## Resources
 
-`gitmopy` is inspired by [`gitmoji-cli](https://github.com/carloscuesta/gitmoji-cli).
+`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).
 
 It is built thanks to:
 
 * [`typer`](https://github.com/tiangolo/typer)
 * [`InquirePy`](https://github.com/kazhala/InquirerPy)
-* [`GitPython](https://github.com/gitpython-developers/GitPython)
+* [`GitPython`](https://github.com/gitpython-developers/GitPython)
```

### Comparing `gitmopy-0.3.1/gitmopy/cli.py` & `gitmopy-0.3.2/gitmopy/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,41 @@
 """
 Command line interface for gitmopy.
 """
 from typing import List, Optional
 
 import git
-from git import Repo
 import typer
+from git import Repo
 from rich import print
 from typing_extensions import Annotated
 
-from gitmopy.git import CatchRemoteException, get_files_status, format_remotes_diff
+from gitmopy.git import CatchRemoteException, format_remotes_diff, get_files_status
 from gitmopy.history import gitmojis_setup, save_to_history
 from gitmopy.prompt import (
     choose_remote_prompt,
     commit_prompt,
     config_prompt,
     git_add_prompt,
     set_upstream_prompt,
 )
 from gitmopy.utils import (
     APP_PATH,
     CONFIG_PATH,
     HISTORY_PATH,
+    _sentinels,
     load_config,
     message_from_commit_dict,
     print_staged_files,
     resolve_path,
 )
 
 app = typer.Typer()
 gitmojis_setup()
 
-_stop = object()
-_restart = object()
-_cancelled = object()
-
 
 def catch_keyboard_interrupt(func, *args, **kwargs):
     """
     Function to wrap another function in a try/finally block and catch Aborts.
 
     Executes its first argument with the following arguments and keyword arguments.
     When the function is done (or has been aborted by ctrl+c), it will prompt the
@@ -54,25 +51,25 @@
     """
 
     def _func(*_args, **_kwargs):
         """
         Function wrapper that catches typer.Abort exceptions.
 
         Returns:
-            Any: The wrapped function's return value or the ``_cancelled``
+            Any: The wrapped function's return value or the ``_sentinels["cancelled"]``
                 sentinel if the function was aborted.
         """
-        return_value = _cancelled
+        return_value = _sentinels["cancelled"]
         try:
             return_value = func(*_args, **_kwargs)
         finally:
             return return_value
 
     return_value = _func(*args, **kwargs)
-    if return_value is not _cancelled:
+    if return_value is not _sentinels["cancelled"]:
         # function was not aborted
         return return_value
 
     print(
         "\n[yellow]Press [b green]enter[/b green] to restart commit process"
         + " or [b red]ctrl+c[/b red] again to quit (or [b red]q[/b red]).",
         end="",
@@ -81,19 +78,19 @@
         "", prompt_suffix="", default="enter", show_default=False
     )
 
     # at this point if the user presses ctrl+c again, the program will exit
 
     # user asked to quit
     if should_stop == "q":
-        return _stop
+        return _sentinels["stop"]
 
     # user wants to restart the commit process
     print()
-    return _restart
+    return _sentinels["restart"]
 
 
 def should_commit_again(repo: Repo, remote: List[str]) -> bool:
     """
     Prompt the user to continue or stop the current commit loop.
 
     Args:
@@ -104,26 +101,35 @@
     """
     gitmojis_setup()
     prompt_txt = (
         "\n🔄 [u]Ready to commit again[/u]. Press [b green]enter[/b green] "
         + "to commit again"
     )
 
+    print()
     remotes_diff = format_remotes_diff(repo)
     if remotes_diff:
-        print("\n\n" + remotes_diff)
+        print(remotes_diff)
         prompt_txt += ", [b dodger_blue2]p[/b dodger_blue2] to push and commit again,"
+        if "does not have a branch" not in remotes_diff:
+            prompt_txt += (
+                " [b dodger_blue2]s[/b dodger_blue2] to sync (pull then pull) "
+                + " and commit again,"
+            )
 
     print(prompt_txt + " or [b red]q[/b red] to quit.", end="")
 
     commit_again = typer.prompt(
         "", default="enter", show_default=False, prompt_suffix=""
     )
-    if remotes_diff and commit_again == "p":
-        push_cli(repo, remote)
+    if remotes_diff:
+        if commit_again == "s":
+            pull_cli(repo, remote)
+        if commit_again in {"p", "s"}:
+            push_cli(repo, remote)
         return should_commit_again(repo, remote)
 
     commit_again = commit_again != "q"
 
     if commit_again:
         print()
 
@@ -172,14 +178,50 @@
                             repo.git.push(
                                 "--set-upstream",
                                 remote.name,
                                 repo.active_branch.name,
                             )
 
 
+def pull_cli(repo, remote):
+    # pull from remotes. If several remotes, use either the values from --remote
+    # or prompt the user to choose them.
+    # If no remote, ignore push.
+    if len(repo.remotes) == 0:
+        print("[yellow]No remote found. Ignoring pull.[/yellow]")
+    else:
+        selected_remotes = set([repo.remotes[0].name])
+        if len(repo.remotes) > 1:
+            if remote:
+                # use --remote values
+                selected_remotes = set(remote)
+            else:
+                # PROMPT: choose remote
+                selected_remotes = choose_remote_prompt(repo.remotes)
+            if not selected_remotes:
+                # stop if no remote selected
+                print("[yellow]No remote selected. Aborting.[/yellow]")
+                raise typer.Exit(1)
+            selected_remotes = set(selected_remotes)
+        print()
+        color = "dodger_blue3"
+
+        # there is at least one remote to push to at this point
+        for remote in repo.remotes:
+            if remote.name in selected_remotes:
+                print(
+                    f"[{color}]Pulling from remote {remote.name}[/{color}]",
+                )
+                # push to remote, catch exception if it fails to be able to
+                # 1. continue pushing to other remotes
+                # 2. potentially set the upstream branch
+                with CatchRemoteException(remote.name):
+                    repo.git.pull(remote.name, repo.active_branch.name)
+
+
 @app.command(
     help="Commit staged files. Use --add to interactively select files to"
     + " stage if none is already staged",
 )
 def commit(
     repo: Annotated[str, typer.Option(help="Path to the git repository")] = ".",
     add: Annotated[
@@ -281,18 +323,25 @@
                 print(
                     "\n[yellow]Ignoring --remote flag because --push is not set[/yellow]\n"
                 )
             # no staged files fbut user wants to add: start prompt
             if not status["staged"] and add:
                 # PROMPT: list files to user and add their selection
                 to_add = catch_keyboard_interrupt(git_add_prompt, status)
-                if to_add is _stop:
+                if to_add is _sentinels["stop"]:
                     break
-                elif to_add is _restart:
+                elif to_add is _sentinels["restart"]:
                     continue
+                elif not to_add:
+                    print("[yellow]No file selected, nothing to commit.[/yellow]")
+                    if should_commit_again(repo, remote):
+                        # user wants to commit again: start over
+                        continue
+                    # user wants to stop: break loop
+                    break
             else:
                 # there are staged files: list them to user
                 if add:
                     print(
                         "[yellow]Ignoring --add flag because the stage is"
                         + " not empty[/yellow]\n"
                     )
@@ -303,17 +352,17 @@
         # not dry run print files about to be committed
         if not dry:
             print_staged_files(to_add or status["staged"])
 
         # PROMPT: get user's commit details
         print("\n[u green3]Commit details:[/u green3]")
         commit_dict = catch_keyboard_interrupt(commit_prompt, config)
-        if commit_dict is _stop:
+        if commit_dict is _sentinels["stop"]:
             break
-        elif commit_dict is _restart:
+        elif commit_dict is _sentinels["restart"]:
             continue
 
         # make commit messsage
         commit_message = message_from_commit_dict(commit_dict)
 
         if dry:
             # Don't do anything, just print the commit message
```

### Comparing `gitmopy-0.3.1/gitmopy/git.py` & `gitmopy-0.3.2/gitmopy/git.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 `gitmopy`'s Git-related utility functions.
 """
 from typing import Dict, List
 
 from git import Repo
 from git.exc import GitCommandError
+from rich import print
+
+from gitmopy.utils import _sentinels
 
 
 class CatchRemoteException:
     def __init__(self, remote: str):
         """
         Context manager to catch GitCommandError when pushing to a remote.
 
@@ -135,33 +138,43 @@
     Args:
         repo (Repo): GitPython repository object.
 
     Returns:
         int: Number of commits the local current branch is behind for each remote.
     """
     b = repo.active_branch.name
-    return {
-        r.name: len(list(repo.iter_commits(f"{b}..{r.name}/{b}"))) for r in repo.remotes
-    }
+    behinds = {}
+    for r in repo.remotes:
+        try:
+            behinds[r.name] = len(list(repo.iter_commits(f"{b}..{r.name}/{b}")))
+        except GitCommandError as e:
+            if "fatal: bad revision" in str(e):
+                behinds[r.name] = _sentinels["no-branch"]
+    return behinds
 
 
 def commits_ahead(repo: Repo) -> int:
     """
     Get the number of commits the local current branch is behind for each remote.
 
     Args:
         repo (Repo): GitPython repository object.
 
     Returns:
         int: Number of commits the local current branch is behind for each remote.
     """
     b = repo.active_branch.name
-    return {
-        r.name: len(list(repo.iter_commits(f"{r.name}/{b}..{b}"))) for r in repo.remotes
-    }
+    aheads = {}
+    for r in repo.remotes:
+        try:
+            aheads[r.name] = len(list(repo.iter_commits(f"{r.name}/{b}..{b}")))
+        except GitCommandError as e:
+            # already caught and printed in commits_behind
+            pass
+    return aheads
 
 
 def format_remotes_diff(repo: Repo) -> str:
     """
     Format the remotes diff.
 
     Args:
@@ -169,18 +182,36 @@
 
     Returns:
         str: Formatted remotes diff.
     """
     behind = commits_behind(repo)
     ahead = commits_ahead(repo)
 
-    if not (sum(behind.values()) + sum(ahead.values())):
+    no_branch = [k for k, v in behind.items() if v is _sentinels["no-branch"]]
+
+    if (
+        not (
+            sum([b for b in behind.values() if b is not _sentinels["no-branch"]])
+            + sum(ahead.values())
+        )
+        and not no_branch
+    ):
         return ""
 
     s = "[u green]Remotes diff:[/u green]\n"
     for r in repo.remotes:
         if behind[r.name]:
-            s += f"[orange3]behind {r.name} by {behind[r.name]} commit(s)[/orange3]\n"
+            if behind[r.name] is _sentinels["no-branch"]:
+                b = repo.active_branch
+                s += f"[yellow]remote {r.name} does not have a branch {b}[/yellow]\n"
+                continue
+            s += (
+                f"[orange3]local is behind {r.name} by {behind[r.name]} "
+                + "commit(s)[/orange3]\n"
+            )
         if ahead[r.name]:
-            s += f"[plum3]ahead {r.name} by {ahead[r.name]} commit(s)[/plum3]\n"
+            s += (
+                f"[plum3]local is ahead of {r.name} by {ahead[r.name]}"
+                + " commit(s)[/plum3]\n"
+            )
 
     return s
```

### Comparing `gitmopy-0.3.1/gitmopy/history.py` & `gitmopy-0.3.2/gitmopy/history.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.1/gitmopy/prompt.py` & `gitmopy-0.3.2/gitmopy/prompt.py`

 * *Files identical despite different names*

### Comparing `gitmopy-0.3.1/gitmopy/utils.py` & `gitmopy-0.3.2/gitmopy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,21 @@
 """
 
 HISTORY_PATH = APP_PATH / "history.json"
 """
 Path to the history file.
 """
 
+_sentinels = {
+    k: object() for k in ["stop", "restart", "cancelled", "sync", "no-branch"]
+}
+"""
+Private constants
+"""
+
 DEFAULT_CHOICES = [
     {
         "value": "skip_scope",
         "name": "Skip commit scope",
         "default": False,
     },
     {
```

### Comparing `gitmopy-0.3.1/pyproject.toml` & `gitmopy-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitmopy"
-version = "0.3.1"
+version = "0.3.2"
 description = "A python command-line for gitmoji"
 authors = ["vict0rsch <vsch@pm.me>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gitmopy-0.3.1/setup.py` & `gitmopy-0.3.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'typer[all]>=0.8.0']
 
 entry_points = \
 {'console_scripts': ['gitmopy = gitmopy.cli:app']}
 
 setup_kwargs = {
     'name': 'gitmopy',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'A python command-line for gitmoji',
-    'long_description': '# gitmopy\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* Select option with **`space`**\n* Validate selection with **`enter`**\n* Press **`tab`** to auto-complete\n  * Press `tab` on an empty line to see history\n* Restart commit with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.1.0\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                 TEXT  Path to the git repository [default: .]                │\n│ --add     --no-add           Whether or not to interactively select files to stage  │\n│                              if none is already staged                              │\n│                              [default: no-add]                                      │\n│ --push    --no-push          Whether to `git push` after commit. Disabled by        │\n│                              default.                                               │\n│                              [default: no-push]                                     │\n│ --dry     --no-dry           Whether or not to actually commit. [default: no-dry]   │\n│ --help                       Show this message and exit.                            │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython](https://github.com/gitpython-developers/GitPython)\n',
+    'long_description': '# `gitmopy`\n\nAn interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/\n\n```text\npip install gitmopy\n```\n\n![demo-gitmopy](./assets/demo-gitmopy.gif)\n\n## How to use\n\n* I typically use `$ gitmopy commit --add --keep-alive`\n* Navigate through options with ⬆️ and ⬇️\n* Select option with **`space`**\n* Validate selection with **`enter`**\n* Press **`tab`** to auto-complete\n  * Press `tab` on an empty line to see history\n* Restart commit with **`crtl+c`**\n  * The keyboard interruption will be caught once, then press `enter` to restart\n\n## Suggested shortcuts\n\n```bash\nalias gpy="gitmopy"\nalias gpyc="gitmopy commit"\nalias gpya="gitmopy commit --add"\nalias gpyk="gitmopy commit --add --keep-alive"\n```\n\n![gpyk depo](assets/gpyk.png)\n\n## Examples\n\n```bash\n# Typical daily use-case\n# ----------------------\n\n# continuously commit, interactively select files to stage\n$ gitmopy commit --add --keep-alive\n\n# same using an alias, + push after every commit (could be dangerous)\n$ gpyk --push\n\n\n# Specific usage\n# --------------\n\n# commit currently staged files. Will fail if no file is staged.\n$ gitmopy commit\n\n# Enable interactive file selection if no file is currently staged. Ignored if\n# there are staged files.\n$ gitmopy commit --add\n\n# Commit continuously: don\'t leave the CLI after the first commit but restart\n# the commit procedure.\n$ gitmopy commit --keep-alive\n\n# Push to remote repositories after commit.\n# Interactively select remotes to push to if there are more than 1.\n$ gitmopy commit --push\n\n# Push to specific remotes\n$ gitmopy commit --push --remote origin --remote upstream\n\n# Make and display a commit message without staging/committing/pushing\n$ gitmopy commit --dry\n\n# configure gitmopy\n$ gitmopy config\n\n# print version, data paths and current configuration\n$ gitmopy info\n\n# print helps\n$ gitmopy --help\n$ gitmopy commit --help\n```\n\n⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.\n\n## User guide\n\n```text\n$ gitmopy info\n\ngitmopy info:\n  version : 0.1.0\n  app path: /Users/victor/.gitmopy\n  history : /Users/victor/.gitmopy/history.json\n  config  : /Users/victor/.gitmopy/config.yaml\n\nCurrent configuration:\n  skip_scope      : False\n  skip_message    : False\n  capitalize_title: True\n  enable_history  : True\n```\n\nUpdate configuration with\n\n```text\n$ gitmopy config\n$ gitmopy config\n❓ Configure gitmopy locally. Use \'space\' to (de-)select, \'enter\' to validate.\n❯ ○ Skip commit scope\n  ○ Skip commit message\n  ◉ Capitalize commit title\n  ◉ Remember commit history for auto-complete and emoji sorting\n\nConfig will be saved in /Users/victor/.gitmopy/config.yaml.\n```\n\nGet help with\n\n```text\n$ gitmopy --help\n\n Usage: gitmopy [OPTIONS] COMMAND [ARGS]...\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --install-completion          Install completion for the current shell.             │\n│ --show-completion             Show completion for the current shell, to copy it or  │\n│                               customize the installation.                           │\n│ --help                        Show this message and exit.                           │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n╭─ Commands ──────────────────────────────────────────────────────────────────────────╮\n│ commit  Commit staged files. Use --add to interactively select files to stage if    │\n│         none is already staged                                                      │\n│ config  Configure gitmopy                                                           │\n│ info    Print gitmopy info                                                          │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n\n$ gitmopy commit --help\n\n Usage: gitmopy commit [OPTIONS]\n\n Commit staged files. Use --add to interactively select files to stage if none is\n already staged\n\n╭─ Options ───────────────────────────────────────────────────────────────────────────╮\n│ --repo                             TEXT  Path to the git repository [default: .]    │\n│ --add           --no-add                 Whether or not to interactively select     │\n│                                          files to stage if none is already staged   │\n│                                          [default: no-add]                          │\n│ --push          --no-push                Whether to `git push` after commit. If     │\n│                                          multiple remotes exist, you will be asked  │\n│                                          to interactively choose the ones to push   │\n│                                          to. Use --remote to skip interactive       │\n│                                          selection. Disabled by default.            │\n│                                          [default: no-push]                         │\n│ --dry           --no-dry                 Whether or not to actually commit.         │\n│                                          [default: no-dry]                          │\n│ --remote                           TEXT  Remote to push to after commit. Use to     │\n│                                          skip interactive remote selection when     │\n│                                          several exist. Use several \'--remote       │\n│                                          {remote name}\' to push to multiple remotes │\n│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │\n│                                          commit, to be ready for another one.       │\n│                                          [default: no-keep-alive]                   │\n│ --help                                   Show this message and exit.                │\n╰─────────────────────────────────────────────────────────────────────────────────────╯\n```\n\n## To Do\n\n* Features\n  * *If requested:*\n    * Install hook\n    * `git commit` flags (like `-S`)\n    * max history length (if loading the json becomes slow)\n* Tests\n  * https://typer.tiangolo.com/tutorial/testing/\n  * 👋 **Help wanted**\n* Docs\n  * Not critical\n\n## Resources\n\n`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).\n\nIt is built thanks to:\n\n* [`typer`](https://github.com/tiangolo/typer)\n* [`InquirePy`](https://github.com/kazhala/InquirerPy)\n* [`GitPython`](https://github.com/gitpython-developers/GitPython)\n',
     'author': 'vict0rsch',
     'author_email': 'vsch@pm.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `gitmopy-0.3.1/PKG-INFO` & `gitmopy-0.3.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitmopy
-Version: 0.3.1
+Version: 0.3.2
 Summary: A python command-line for gitmoji
 License: MIT
 Author: vict0rsch
 Author-email: vsch@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: GitPython (>=3.1.31,<4.0.0)
 Requires-Dist: inquirerpy (>=0.3.4,<0.4.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: typer[all] (>=0.8.0)
 Description-Content-Type: text/markdown
 
-# gitmopy
+# `gitmopy`
 
 An interactive Python implementation of the Gitmoji standard: https://gitmoji.dev/
 
 ```text
 pip install gitmopy
 ```
 
@@ -93,14 +93,16 @@
 $ gitmopy info
 
 # print helps
 $ gitmopy --help
 $ gitmopy commit --help
 ```
 
+⚠️ The sync feature is still experimental. It will `pull` then `push` but in the case of several remotes and the branch not existing on one of them, I recommend you deal with it with `git` manually.
+
 ## User guide
 
 ```text
 $ gitmopy info
 
 gitmopy info:
   version : 0.1.0
@@ -153,23 +155,34 @@
 
  Usage: gitmopy commit [OPTIONS]
 
  Commit staged files. Use --add to interactively select files to stage if none is
  already staged
 
 ╭─ Options ───────────────────────────────────────────────────────────────────────────╮
-│ --repo                 TEXT  Path to the git repository [default: .]                │
-│ --add     --no-add           Whether or not to interactively select files to stage  │
-│                              if none is already staged                              │
-│                              [default: no-add]                                      │
-│ --push    --no-push          Whether to `git push` after commit. Disabled by        │
-│                              default.                                               │
-│                              [default: no-push]                                     │
-│ --dry     --no-dry           Whether or not to actually commit. [default: no-dry]   │
-│ --help                       Show this message and exit.                            │
+│ --repo                             TEXT  Path to the git repository [default: .]    │
+│ --add           --no-add                 Whether or not to interactively select     │
+│                                          files to stage if none is already staged   │
+│                                          [default: no-add]                          │
+│ --push          --no-push                Whether to `git push` after commit. If     │
+│                                          multiple remotes exist, you will be asked  │
+│                                          to interactively choose the ones to push   │
+│                                          to. Use --remote to skip interactive       │
+│                                          selection. Disabled by default.            │
+│                                          [default: no-push]                         │
+│ --dry           --no-dry                 Whether or not to actually commit.         │
+│                                          [default: no-dry]                          │
+│ --remote                           TEXT  Remote to push to after commit. Use to     │
+│                                          skip interactive remote selection when     │
+│                                          several exist. Use several '--remote       │
+│                                          {remote name}' to push to multiple remotes │
+│ --keep-alive    --no-keep-alive          Whether or not to keep the app alive after │
+│                                          commit, to be ready for another one.       │
+│                                          [default: no-keep-alive]                   │
+│ --help                                   Show this message and exit.                │
 ╰─────────────────────────────────────────────────────────────────────────────────────╯
 ```
 
 ## To Do
 
 * Features
   * *If requested:*
@@ -180,15 +193,15 @@
   * https://typer.tiangolo.com/tutorial/testing/
   * 👋 **Help wanted**
 * Docs
   * Not critical
 
 ## Resources
 
-`gitmopy` is inspired by [`gitmoji-cli](https://github.com/carloscuesta/gitmoji-cli).
+`gitmopy` is inspired by [`gitmoji-cli`](https://github.com/carloscuesta/gitmoji-cli).
 
 It is built thanks to:
 
 * [`typer`](https://github.com/tiangolo/typer)
 * [`InquirePy`](https://github.com/kazhala/InquirerPy)
-* [`GitPython](https://github.com/gitpython-developers/GitPython)
+* [`GitPython`](https://github.com/gitpython-developers/GitPython)
```

