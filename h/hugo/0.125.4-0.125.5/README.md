# Comparing `tmp/hugo-0.125.4.tar.gz` & `tmp/hugo-0.125.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugo-0.125.4.tar", last modified: Thu Apr 25 14:21:37 2024, max compression
+gzip compressed data, was "hugo-0.125.5.tar", last modified: Wed May  1 17:57:58 2024, max compression
```

## Comparing `hugo-0.125.4.tar` & `hugo-0.125.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-25 14:21:32.000000 hugo-0.125.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-25 14:21:32.000000 hugo-0.125.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-25 14:21:32.000000 hugo-0.125.4/LICENSE-hugo.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-25 14:21:32.000000 hugo-0.125.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21444 2024-04-25 14:21:37.134593 hugo-0.125.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19810 2024-04-25 14:21:32.000000 hugo-0.125.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-25 14:21:32.000000 hugo-0.125.4/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/hugo/
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 14:21:37.134593 hugo-0.125.4/hugo/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/binaries/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-25 14:21:32.000000 hugo-0.125.4/hugo/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-04-25 14:21:32.000000 hugo-0.125.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-25 14:21:37.138593 hugo-0.125.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    18063 2024-04-25 14:21:32.000000 hugo-0.125.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-01 17:57:53.000000 hugo-0.125.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-01 17:57:53.000000 hugo-0.125.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-01 17:57:53.000000 hugo-0.125.5/LICENSE-hugo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 17:57:53.000000 hugo-0.125.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-05-01 17:57:58.416972 hugo-0.125.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19941 2024-05-01 17:57:53.000000 hugo-0.125.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-01 17:57:53.000000 hugo-0.125.5/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/hugo/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:57:58.416972 hugo-0.125.5/hugo/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/binaries/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 17:57:53.000000 hugo-0.125.5/hugo/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2024-05-01 17:57:53.000000 hugo-0.125.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-01 17:57:58.416972 hugo-0.125.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-01 17:57:53.000000 hugo-0.125.5/setup.py
```

### Comparing `hugo-0.125.4/CODE_OF_CONDUCT.md` & `hugo-0.125.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.4/LICENSE` & `hugo-0.125.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hugo-0.125.4/LICENSE-hugo.txt` & `hugo-0.125.5/LICENSE-hugo.txt`

 * *Files identical despite different names*

### Comparing `hugo-0.125.4/PKG-INFO` & `hugo-0.125.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugo
-Version: 0.125.4
+Version: 0.125.5
 Summary: Binaries for the Hugo static site generator, installable with pip
 Author-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 Maintainer-email: Agriya Khetarpal <agriyakhetarpal@outlook.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/agriyakhetarpal/hugo-python-distributions
 Project-URL: Issues, https://github.com/agriyakhetarpal/hugo-python-distributions/issues
 Project-URL: Changelog, https://github.com/agriyakhetarpal/hugo-python-distributions/releases
@@ -74,15 +74,15 @@
 > [!NOTE]
 > This distribution of `Hugo` is currently not affiliated with the official `Hugo` project. Please refer to the [Hugo documentation](https://gohugo.io/documentation/) for more information on Hugo.
 
 ## What version of `hugo` do I install?
 
 This project, `hugo` is versioned alongside the Hugo releases and is aligned with the versioning of Hugo itself, which uses `SemVer` – but is likely versioned according to [0ver](https://0ver.org/) software standards based on their [versioning history](https://github.com/gohugoio/hugo/releases).
 
-Binaries for `hugo` through these wheels are available for Hugo versions **0.121.2** and above, through PyPI or through releases on GitHubr. If you need an older version of `hugo` that is not available through this package, please consider using the [official Hugo binaries](https://github.com/gohugoio/hugo/releases).
+Binaries for `hugo` through these wheels are available for Hugo versions **0.121.2** and above, through PyPI or through releases on GitHub. If you need an older version of `hugo` that is not available through this package, please consider using the [official Hugo binaries](https://github.com/gohugoio/hugo/releases).
 
 Please refer to the section on [Supported platforms](#supported-platforms) for a list of wheels available for supported platforms and architectures. If it does, jump to the [Quickstart](#quickstart) section to get started.
 
 > [!WARNING]
 > Owing to the limitations of overall sizing available on [PyPI](https://pypi.org/project/hugo/#history) for `hugo`, only the most recent versions of Hugo are available for download through `pip`, and older versions of these wheels will be deleted to make space for newer releases. If you need an older version of Hugo, please consider using the wheels that have been uploaded to the [GitHub releases](https://github.com/agriyakhetarpal/hugo-python-distributions/releases) page or the [official Hugo binaries](https://github.com/gohugoio/hugo/releases). The former can be done via `pip` by downloading the `.whl` file, or through `pipx` using the URL directly (recommended). For example, if you need Hugo 0.122.0, you can run `pipx install "https://github.com/agriyakhetarpal/hugo-python-distributions/releases/download/v0.122.0/hugo-0.122.0-cp311-cp311-win_amd64.whl"` to download and install the wheel for Hugo 0.122.0 on Windows for Python 3.11.
 
 ## Documentation
@@ -151,14 +151,16 @@
 
 | Platform | Architecture    | Support                         |
 | -------- | --------------- | ------------------------------- |
 | macOS    | x86_64 (Intel)  | ✅                              |
 | macOS    | arm64 (Silicon) | ✅                              |
 | Linux    | amd64           | ✅                              |
 | Linux    | arm64           | ✅                              |
+| Linux    | s390x           | ✅                              |
+| Linux    | ppc64le         | ✅                              |
 | Windows  | x86_64          | ✅                              |
 | Windows  | arm64           | 💡 Experimental support [^1]    |
 | Windows  | x86             | 💡 Experimental support [^1]    |
 | DragonFlyBSD | amd64       | ❌ Will not receive support[^2] |
 | FreeBSD  | amd64           | ❌ Will not receive support[^2] |
 | OpenBSD  | amd64           | ❌ Will not receive support[^2] |
 | NetBSD   | amd64           | ❌ Will not receive support[^2] |
```

### Comparing `hugo-0.125.4/README.md` & `hugo-0.125.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 > [!NOTE]
 > This distribution of `Hugo` is currently not affiliated with the official `Hugo` project. Please refer to the [Hugo documentation](https://gohugo.io/documentation/) for more information on Hugo.
 
 ## What version of `hugo` do I install?
 
 This project, `hugo` is versioned alongside the Hugo releases and is aligned with the versioning of Hugo itself, which uses `SemVer` – but is likely versioned according to [0ver](https://0ver.org/) software standards based on their [versioning history](https://github.com/gohugoio/hugo/releases).
 
-Binaries for `hugo` through these wheels are available for Hugo versions **0.121.2** and above, through PyPI or through releases on GitHubr. If you need an older version of `hugo` that is not available through this package, please consider using the [official Hugo binaries](https://github.com/gohugoio/hugo/releases).
+Binaries for `hugo` through these wheels are available for Hugo versions **0.121.2** and above, through PyPI or through releases on GitHub. If you need an older version of `hugo` that is not available through this package, please consider using the [official Hugo binaries](https://github.com/gohugoio/hugo/releases).
 
 Please refer to the section on [Supported platforms](#supported-platforms) for a list of wheels available for supported platforms and architectures. If it does, jump to the [Quickstart](#quickstart) section to get started.
 
 > [!WARNING]
 > Owing to the limitations of overall sizing available on [PyPI](https://pypi.org/project/hugo/#history) for `hugo`, only the most recent versions of Hugo are available for download through `pip`, and older versions of these wheels will be deleted to make space for newer releases. If you need an older version of Hugo, please consider using the wheels that have been uploaded to the [GitHub releases](https://github.com/agriyakhetarpal/hugo-python-distributions/releases) page or the [official Hugo binaries](https://github.com/gohugoio/hugo/releases). The former can be done via `pip` by downloading the `.whl` file, or through `pipx` using the URL directly (recommended). For example, if you need Hugo 0.122.0, you can run `pipx install "https://github.com/agriyakhetarpal/hugo-python-distributions/releases/download/v0.122.0/hugo-0.122.0-cp311-cp311-win_amd64.whl"` to download and install the wheel for Hugo 0.122.0 on Windows for Python 3.11.
 
 ## Documentation
@@ -116,14 +116,16 @@
 
 | Platform | Architecture    | Support                         |
 | -------- | --------------- | ------------------------------- |
 | macOS    | x86_64 (Intel)  | ✅                              |
 | macOS    | arm64 (Silicon) | ✅                              |
 | Linux    | amd64           | ✅                              |
 | Linux    | arm64           | ✅                              |
+| Linux    | s390x           | ✅                              |
+| Linux    | ppc64le         | ✅                              |
 | Windows  | x86_64          | ✅                              |
 | Windows  | arm64           | 💡 Experimental support [^1]    |
 | Windows  | x86             | 💡 Experimental support [^1]    |
 | DragonFlyBSD | amd64       | ❌ Will not receive support[^2] |
 | FreeBSD  | amd64           | ❌ Will not receive support[^2] |
 | OpenBSD  | amd64           | ❌ Will not receive support[^2] |
 | NetBSD   | amd64           | ❌ Will not receive support[^2] |
```

### Comparing `hugo-0.125.4/SECURITY.md` & `hugo-0.125.5/SECURITY.md`

 * *Files identical despite different names*

### Comparing `hugo-0.125.4/hugo/cli.py` & `hugo-0.125.5/hugo/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 HUGO_ARCH = {
     "x86_64": "amd64",
     "arm64": "arm64",
     "AMD64": "amd64",
     "aarch64": "arm64",
     "x86": "386",
+    "s390x": "s390x",
+    "ppc64le": "ppc64le",
 }[machine()]
 
 # platform.machine returns AMD64 on Windows because the architecture is
 # 64-bit (even if one is running a 32-bit Python interpreter). Therefore
 # we use sys. maxsize to handle this special case on Windows
 
 if not (maxsize > 2**32) and sysplatform == "win32":
```

### Comparing `hugo-0.125.4/pyproject.toml` & `hugo-0.125.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hugo-0.125.4/setup.py` & `hugo-0.125.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import Command, Extension, setup
 from setuptools.command.build_ext import build_ext
 from setuptools.command.build_py import build_py
 from wheel.bdist_wheel import bdist_wheel
 
 # ------ Hugo build configuration and constants ------------------------------------
 
-HUGO_VERSION = "0.125.4"
+HUGO_VERSION = "0.125.5"
 # The Go toolchain will download the tarball into the hugo_cache/ directory.
 # We will point the build command to that location to build Hugo from source
 HUGO_CACHE_DIR = "hugo_cache"
 FILE_EXT = (
     ".exe" if (sys.platform == "win32" or os.environ.get("GOOS") == "windows") else ""
 )
 # The vendor name is used to set the vendorInfo variable in the Hugo binary
@@ -33,14 +33,17 @@
 # Normalise architecture strings to match the Go toolchain
 HUGO_ARCH = {
     "x86_64": "amd64",
     "arm64": "arm64",
     "AMD64": "amd64",
     "aarch64": "arm64",
     "x86": "386",
+    "s390x": "s390x",
+    "ppc64le": "ppc64le",
+    "armv7l": "arm",
 }[platform.machine()]
 
 # Name of the Hugo binary that will be built
 HUGO_BINARY_NAME = (
     f"hugo-{HUGO_VERSION}-{HUGO_PLATFORM}-{os.environ.get('GOARCH', HUGO_ARCH)}"
     + FILE_EXT
 )
@@ -78,15 +81,15 @@
     def initialize_options(self):
         super().initialize_options()
         self.hugo_version = None
         self.hugo_platform = None
         self.hugo_arch = None
 
     def finalize_options(self):
-        # Platforms and architectures that we will build Hugo for are:
+        # Platforms and architectures that we will build Hugo natively for are:
         # i.e., a subset of "go tool dist list":
         # 1. darwin/amd64
         # 2. darwin/arm64
         # 3. linux/amd64
         # 4. linux/arm64
         # 5. windows/amd64
         # The platform is the first part of the string, the architecture is the second.
@@ -127,14 +130,17 @@
         # caches the build artifacts there for future use.
         os.environ["GOCACHE"] = str(Path(HUGO_CACHE_DIR).resolve())
 
         os.environ["GOOS"] = os.environ.get("GOOS", self.hugo_platform)
         os.environ["GOARCH"] = os.environ.get("GOARCH", self.hugo_arch)
         # i.e., allow override if GOARCH is set!
 
+        if os.environ.get("GOARCH") == "arm" and os.environ.get("GOOS") == "linux":
+            os.environ["GOARM"] = os.environ.get("GOARM", "7")
+
         # Build Hugo from source using the Go toolchain, place it into GOBIN
         # Requires the following dependencies:
         #
         # 1. Go
         # 2. GCC/Clang
         # 3. Git
         #
@@ -184,32 +190,45 @@
             raise OSError(error_message) from err
 
         # These ldflags are passed to the Go linker to set variables at runtime
         ldflags = [
             f"-s -w -X github.com/gohugoio/hugo/common/hugo.vendorInfo={HUGO_VENDOR_NAME}"
         ]
 
+        # Build a static binary on Windows to avoid missing DLLs from MinGW,
+        # i.e., libgcc_s_seh-1.dll, libstdc++-6.dll, etc.
+        BUILDING_FOR_WINDOWS = (
+            os.environ.get("GOOS") == "windows" or sys.platform == "win32"
+        )
+
+        if BUILDING_FOR_WINDOWS:
+            ldflags.append("-extldflags '-static'")
+
         if not (Path(HUGO_CACHE_DIR).resolve() / f"hugo-{HUGO_VERSION}").exists():
             subprocess.check_call(
                 [
                     "git",
                     "clone",
                     "https://github.com/gohugoio/hugo.git",
                     "--depth=1",
                     "--single-branch",
                     "--branch",
                     f"v{HUGO_VERSION}",
                     Path(HUGO_CACHE_DIR) / f"hugo-{HUGO_VERSION}",
+                    # disable warning about detached HEAD
+                    "-c",
+                    "advice.detachedHead=false",
                 ]
             )
 
         subprocess.check_call(
             [
                 "go",
                 "install",
+                "-v",
                 "-ldflags",
                 " ".join(ldflags),
                 "-tags",
                 "extended",
             ],
             cwd=(Path(HUGO_CACHE_DIR) / f"hugo-{HUGO_VERSION}").resolve(),
         )
@@ -358,23 +377,25 @@
         # 6. Cross-compiling from Windows arm64/x86_64/x86 to Linux arm64/x86_64
         #
         # These checks will be activated only when GOOS is set. If GOOS is not set,
         # we will use the platform tag as is based on the above checks.
 
         # Handle cross-compilation on Linux via the Zig compiler
         # ======================================================
-        if (os.environ.get("GOOS") == "linux") or (sys.platform == "linux"):
+        if os.environ.get("GOOS") == "linux":
             if os.environ.get("GOARCH") == "arm64":
                 platform_tag = "linux_aarch64"
             elif os.environ.get("GOARCH") == "amd64":
                 platform_tag = "linux_x86_64"
+            elif os.environ.get("GOARCH") == "ppc64le":
+                platform_tag = "linux_ppc64le"
 
         # Handle cross-compilation on/to Windows via the Zig compiler
         # ===========================================================
-        if os.environ.get("GOOS") == "windows" or (sys.platform == "win32"):
+        elif os.environ.get("GOOS") == "windows":
             if os.environ.get("GOARCH") == "arm64":
                 platform_tag = "win_arm64"
             elif os.environ.get("GOARCH") == "amd64":
                 platform_tag = "win_amd64"
             elif os.environ.get("GOARCH") == "386":
                 platform_tag = "win32"
 
@@ -382,15 +403,15 @@
         # ====================================================================
         # Also, ensure correct platform tags for macOS arm64 and macOS x86_64
         # since macOS 3.12 Python GH Actionsrunners are mislabelling the platform
         # tag to be universal2, see: https://github.com/pypa/wheel/issues/573
         # Also, let cibuildwheel handle the platform tags if it is being used,
         # since that is where we won't cross-compile at all but use the native
         # GitHub Actions runners.
-        if ((os.environ.get("GOOS") == "darwin") or (sys.platform == "darwin")) and (
+        elif (os.environ.get("GOOS") == "darwin") and (
             os.environ.get("CIBUILDWHEEL") != "1"
         ):
             if os.environ.get("GOARCH") == "arm64":
                 platform_tag = "macosx_11_0_arm64"
             elif os.environ.get("GOARCH") == "amd64":
                 platform_tag = "macosx_10_9_x86_64"
```

