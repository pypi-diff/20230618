# Comparing `tmp/universal_test_runner-0.1.0.tar.gz` & `tmp/universal_test_runner-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universal_test_runner-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "universal_test_runner-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `universal_test_runner-0.1.0.tar` & `universal_test_runner-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.1.0/LICENSE
--rw-r--r--   0        0        0     2816 2023-06-07 06:38:05.903262 universal_test_runner-0.1.0/README.md
--rw-r--r--   0        0        0     1108 2023-06-07 06:38:30.977221 universal_test_runner-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.1.0/universal_test_runner/__init__.py
--rw-r--r--   0        0        0      437 2023-06-07 06:34:44.217558 universal_test_runner-0.1.0/universal_test_runner/context.py
--rw-r--r--   0        0        0     1694 2023-06-07 06:34:31.498209 universal_test_runner-0.1.0/universal_test_runner/matchers.py
--rw-r--r--   0        0        0     1235 2023-06-07 06:34:43.526749 universal_test_runner-0.1.0/universal_test_runner/runner.py
--rw-r--r--   0        0        0     3912 1970-01-01 00:00:00.000000 universal_test_runner-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-05 07:04:09.894832 universal_test_runner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3707 2023-06-17 06:38:49.383842 universal_test_runner-0.2.0/README.md
+-rw-r--r--   0        0        0     1198 2023-06-17 06:36:07.561918 universal_test_runner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-05 05:21:33.982200 universal_test_runner-0.2.0/universal_test_runner/__init__.py
+-rw-r--r--   0        0        0     1570 2023-06-18 18:24:18.266813 universal_test_runner-0.2.0/universal_test_runner/context.py
+-rw-r--r--   0        0        0     2481 2023-06-18 18:24:02.933515 universal_test_runner-0.2.0/universal_test_runner/matchers.py
+-rw-r--r--   0        0        0     1080 2023-06-18 18:06:08.532252 universal_test_runner-0.2.0/universal_test_runner/runner.py
+-rw-r--r--   0        0        0     4803 1970-01-01 00:00:00.000000 universal_test_runner-0.2.0/PKG-INFO
```

### Comparing `universal_test_runner-0.1.0/LICENSE` & `universal_test_runner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universal_test_runner-0.1.0/pyproject.toml` & `universal_test_runner-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "universal-test-runner"
-version = "0.1.0"
+version = "0.2.0"
 
 authors = [{ name = "David Brownman", email = "beamneocube@gmail.com" }]
 description = "Universal, language-aware unit test runner."
 readme = "README.md"
 license = { file = "LICENSE" }
 
 requires-python = ">=3.10"
@@ -32,7 +32,13 @@
 
 [project.scripts]
 t = "universal_test_runner.runner:run"
 
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
+
+# needed so the LSP performs typechecking
+[tool.pyright]
+
+[tool.isort]
+profile = "black"
```

### Comparing `universal_test_runner-0.1.0/universal_test_runner/matchers.py` & `universal_test_runner-0.2.0/universal_test_runner/matchers.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional
 
 from universal_test_runner.context import Context
 
 # TODO: add user-enableable debug logs
 
 
-@dataclass(frozen=True)
+@dataclass(frozen=True)  # frozen so I can hash them for tests
 class Matcher:
     name: str
     matches: Callable[[Context], Optional[bool]]
     _command: str
 
     @property
     def command(self) -> list[str]:
@@ -21,32 +21,56 @@
         return f"<Matcher {self.name}>"
 
     @staticmethod
     def basic(name: str, file: str, command: str):
         """
         shorthand for running a command if a single file is in the file list
         """
-        return Matcher(name, lambda c: file in c.files, command)
+        return Matcher(name, lambda c: c.has_files(file), command)
 
 
 # for go modules with nested packages, running `go test` on its own runs no test.
 # so we have to include the ./... to pick up all packages
 go_multi = Matcher(
-    "go_multi", lambda c: "go.mod" in c.files and not c.args, "go test ./..."
+    "go_multi", lambda c: c.has_files("go.mod") and not c.args, "go test ./..."
 )
 # however, if we're in the package root and there's a test file here, then we can just run
 go_single = Matcher(
     "go_single",
-    lambda c: "go.mod" in c.files or any(re.search(r"_test.go$", f) for f in c.files),
+    lambda c: c.has_files("go.mod") or any(re.search(r"_test.go$", f) for f in c.files),
     "go test",
 )
 
+makefile = Matcher(
+    "makefile",
+    lambda c: c.has_files("Makefile")
+    and any(l.startswith("test:") for l in c.read_file("Makefile")),
+    "make test",
+)
+
+has_test_script = lambda d: bool(d.get("scripts", {}).get("test"))
+
+
+def has_test_script_and_lockfile(c: Context, lockfile: str) -> bool:
+    return c.has_files("package.json", lockfile) and has_test_script(
+        c.read_json("package.json")
+    )
+
+
+def build_js_matcher(name: str, lockfile: str):
+    return Matcher(
+        name, lambda c: has_test_script_and_lockfile(c, lockfile), f"{name} test"
+    )
+
+
+npm = build_js_matcher("npm", "package-lock.json")
+yarn = build_js_matcher("yarn", "yarn.lock")
+pnpm = build_js_matcher("pnpm", "pnpm-lock.yaml")
+
 # TODO:
-# - js
-# - makefile?
 # - ruby?
 
 # misc simple cases
 pytest = Matcher.basic("pytest", ".pytest_cache", "pytest")
 py = Matcher.basic("py", "tests.py", "python tests.py")
 elixir = Matcher.basic("elixir", "mix.exs", "mix test")
 rust = Matcher.basic("rust", "Cargo.toml", "cargo test")
@@ -58,8 +82,12 @@
     py,
     # ensure ordering here
     go_multi,
     go_single,
     elixir,
     rust,
     clojure,
+    npm,
+    yarn,
+    pnpm,
+    makefile,
 ]
```

### Comparing `universal_test_runner-0.1.0/universal_test_runner/runner.py` & `universal_test_runner-0.2.0/universal_test_runner/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,48 +2,41 @@
 import subprocess
 import sys
 from pathlib import Path
 
 from universal_test_runner.context import Context
 from universal_test_runner.matchers import ALL_MATCHERS
 
-# TODO: build a context object that has
-# - cwd
-# - filenames
-# - a dict of {name => path object?}
-# - the args the command is run with
-# and pass it to each function
-# i'll be able to put functions in a few file then, I think, since I have all the info I need.
-
 
 def run_test_command(context: Context) -> int:
     for matcher in ALL_MATCHERS:
         if not matcher.matches(context):
             continue
 
         command = [*matcher.command, *context.args]
 
         try:
             return subprocess.run(command).returncode
         except FileNotFoundError:
+            # e.g. if `pytest` is run, but not installed
+            # we capture the error so there's not a Python traceback shown
             print("command not found:", command[0])
             return 1
     else:
         print("no testing method found!")
         return 1
 
 
 def run():
-    # Get the current directory
     current_dir = os.getcwd()
 
     c = Context(
-        # makes the file list deterministic
+        # sorting makes the file list deterministic
         sorted(Path(current_dir).iterdir()),
-        # Pass any arguments to the test runner through to the test command
+        # pass any arguments to the test runner through to the test command
         sys.argv[1:],
     )
 
     sys.exit(run_test_command(c))
 
 
 if __name__ == "__main__":
```

### Comparing `universal_test_runner-0.1.0/PKG-INFO` & `universal_test_runner-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,14 @@
-Metadata-Version: 2.1
-Name: universal-test-runner
-Version: 0.1.0
-Summary: Universal, language-aware unit test runner.
-Keywords: testing
-Author-email: David Brownman <beamneocube@gmail.com>
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Requires-Dist: twine==4.0.2 ; extra == "release"
-Requires-Dist: build==0.10.0 ; extra == "release"
-Requires-Dist: pytest==7.3.1 ; extra == "test"
-Requires-Dist: responses==0.23.1 ; extra == "test"
-Requires-Dist: pyright==1.1.309 ; extra == "test"
-Project-URL: Author, https://xavd.id
-Project-URL: Bug Tracker, https://github.com/xavdid/universal-test-runner/issues
-Project-URL: Changelog, https://github.com/xavdid/universal-test-runner/blob/main/CHANGELOG.md
-Project-URL: Homepage, https://github.com/xavdid/universal-test-runner
-Provides-Extra: release
-Provides-Extra: test
-
 # universal-test-runner
 
 The universal test runner is a zero-configuration, language-aware way to run your unit tests.
 
-<!-- If you're working on a JS project, it runs `[your package manager here] test`. You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo test` coming right up. -->
-
-If you've run `pytest` in this folder before, this tool invokes `pytest`. Rust project? `cargo test` coming right up. Is also clever about running all your `go` module tests (regardless of how they're organized). No matter the command, all args are passed directly into the test runner.
+If you're working on a JS project, it runs `[your package manager here] test`. You've run `pytest` in this folder before? `pytest` it is. Rust project? `cargo test` coming right up. Is also clever about running all your `go` module tests (regardless of how they're organized). No matter the command, all args are passed directly into the test runner.
 
-Currently [supports](#supported-languages) 5 languages, with [more on the way](#upcoming-languages).
+Currently [supports](#supported-languages) 7 languages (and their respective test frameworks). Please open an issue if I'm missing your favorite!
 
 ## Installation
 
 UTR is available on PyPi:
 
 ```bash
 pipx install universal-test-runner
@@ -48,32 +20,28 @@
 2. It should pass all arguments through to the underlying test command
 3. It should have wide language and test runner support; please open an issue if your use case isn't supported!
 
 ## Usage
 
 Once installed, the command `t` will be available. Run that in a folder with tests and it'll do its best to run your unit tests.
 
-```shell
-t
-```
-
 ```
 % t
 ====================== test session starts ======================
 platform darwin -- Python 3.11.0, pytest-7.3.1, pluggy-1.0.0
 rootdir: /Users/david/projects/universal-test-runner
 collected 37 items
 
 tests/test_matchers.py .........................          [ 67%]
 tests/test_runner.py ............                         [100%]
 
 ====================== 37 passed in 0.04s =======================
 ```
 
-If it can't find
+If it can't guess the testing method, it will tell you so. Feel free to open an issue to request wider language support!
 
 ## Supported Languages
 
 1. Python
    - uses `pytest` if you've run `pytest` before
    - looks for a `tests.py` file if not
 2. Rust
@@ -82,22 +50,46 @@
    - if there's a `X_test.go`, then runs a plain `go test`
    - if you pass any args at all, runs `go test your-args-here`
    - otherwise, runs `go test ./...`
 4. Elixir
    - runs `mix test`
 5. Clojure
    - runs `lein test`
-
-### Upcoming Languages
-
-1. JS/TS
+6. Makefile
+   - looks for a line that starts with `test:`
+7. JS/TS
    - if there's a `package.json` and it has a `test` script, runs `[package manager] test`, where `[package manager]` is:
+     - `npm` if there's a `package-lock.json`
      - `yarn` if there's a `yarn.lock`
      - `pnpm` if there's a `pnpm-lock.yaml`
-     - `npm` otherwise
-2. Makefile
-   - looks for a line that starts with `test:`
 
 ## Motivation
 
 I work in a few languages at a time, so I've actually had a [version of this in my dotfiles](https://github.com/xavdid/dotfiles/blob/6bd5f56b1f9ad2dcef9f8b72413d30779b378aef/node/aliases.zsh#L45-L73) for a while. Also, as I've been doing [Exercism's #12in23 program](https://exercism.org/challenges/12in23), I'm _really_ switching languages. It's nice not to have to re-learn any muscle memory. Plus, increasingly complex `bash` was holding me back.
 
+## Development
+
+This section is people making changes to this package.
+
+When in a virtual environment, run the following:
+
+```bash
+pip install -e '.[test]'
+```
+
+This installs the package in `--edit` mode and makes its dependencies available. You can now run `reddit-user-to-sqlite` to invoke the CLI.
+
+### Running Tests
+
+In your virtual environment, a simple `pytest` should run the unit test suite. You can also run `pyright` for type checking.
+
+### Releasing New Versions
+
+> these notes are mostly for myself (or other contributors)
+
+0. ensure tests pass (`pytest`)
+1. install release tooling (`pip install -e '.[release]'`)
+2. build the package (`python -m build`)
+3. upload the release (`python -m twine upload dist/*`)
+   1. give your username as `__token__`
+   2. give your password as your stored API key
+   3. If you're getting invalid password, verify that `~/.pypirc` is empty
```

