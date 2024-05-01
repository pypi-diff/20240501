# Comparing `tmp/gitblog2-2.1.5.tar.gz` & `tmp/gitblog2-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitblog2-2.1.5.tar", max compression
+gzip compressed data, was "gitblog2-2.2.0.tar", max compression
```

## Comparing `gitblog2-2.1.5.tar` & `gitblog2-2.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.1.5/LICENSE
--rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.1.5/build.py
--rw-r--r--   0        0        0     5724 2024-04-30 20:29:05.248299 gitblog2-2.1.5/docs/index.md
--rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.1.5/gitblog2/__init__.py
--rw-r--r--   0        0        0     2766 2024-01-21 12:53:51.615585 gitblog2-2.1.5/gitblog2/blog_posts.py
--rwxr-xr-x   0        0        0     1918 2024-04-30 20:42:27.991108 gitblog2-2.1.5/gitblog2/cli.py
--rw-r--r--   0        0        0    15850 2024-01-21 13:01:17.531760 gitblog2-2.1.5/gitblog2/lib.py
--rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.1.5/gitblog2/media/favicon.svg
--rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.1.5/gitblog2/media/icons.svg
--rw-r--r--   0        0        0      541 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/repo_utils.py
--rw-r--r--   0        0        0     6749 2024-04-30 20:59:18.502341 gitblog2-2.1.5/gitblog2/style.css
--rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/templates/article.html.j2
--rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/templates/footer.html.j2
--rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/templates/head_common.html.j2
--rw-r--r--   0        0        0      867 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/templates/index.html.j2
--rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/templates/navbar.html.j2
--rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/index.html
--rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/media/favicon.svg
--rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/media/icons.svg
--rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/style.css
--rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/tech/example.html
--rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.1.5/gitblog2/tests/example_output/tech/index.html
--rw-r--r--   0        0        0      951 2024-04-30 20:54:51.750226 gitblog2-2.1.5/gitblog2/tests/test_e2e.py
--rw-r--r--   0        0        0      779 2024-04-30 21:07:54.549953 gitblog2-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     6481 1970-01-01 00:00:00.000000 gitblog2-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.2.0/LICENSE
+-rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.2.0/build.py
+-rw-r--r--   0        0        0     5724 2024-04-30 20:29:05.248299 gitblog2-2.2.0/docs/index.md
+-rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.2.0/gitblog2/__init__.py
+-rw-r--r--   0        0        0     3120 2024-05-01 07:13:51.643163 gitblog2-2.2.0/gitblog2/blog_posts.py
+-rwxr-xr-x   0        0        0     2122 2024-05-01 07:45:59.555677 gitblog2-2.2.0/gitblog2/cli.py
+-rw-r--r--   0        0        0    16173 2024-05-01 07:43:59.187765 gitblog2-2.2.0/gitblog2/lib.py
+-rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.2.0/gitblog2/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.2.0/gitblog2/media/icons.svg
+-rw-r--r--   0        0        0      576 2024-04-30 22:21:55.113810 gitblog2-2.2.0/gitblog2/repo_utils.py
+-rw-r--r--   0        0        0     6749 2024-04-30 21:08:14.949907 gitblog2-2.2.0/gitblog2/style.css
+-rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/article.html.j2
+-rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/footer.html.j2
+-rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/head_common.html.j2
+-rw-r--r--   0        0        0      868 2024-05-01 07:49:50.931184 gitblog2-2.2.0/gitblog2/templates/index.html.j2
+-rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/navbar.html.j2
+-rw-r--r--   0        0        0     1183 2024-05-01 07:57:13.613841 gitblog2-2.2.0/gitblog2/tests/example_output/index.html
+-rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/media/icons.svg
+-rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/style.css
+-rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/tech/example.html
+-rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/tech/index.html
+-rw-r--r--   0        0        0     1000 2024-05-01 07:48:06.899524 gitblog2-2.2.0/gitblog2/tests/test_e2e.py
+-rw-r--r--   0        0        0      145 2024-05-01 01:12:36.414254 gitblog2-2.2.0/gitblog2/utils.py
+-rw-r--r--   0        0        0      885 2024-05-01 07:58:34.245659 gitblog2-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6655 1970-01-01 00:00:00.000000 gitblog2-2.2.0/PKG-INFO
```

### Comparing `gitblog2-2.1.5/LICENSE` & `gitblog2-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/docs/index.md` & `gitblog2-2.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/blog_posts.py` & `gitblog2-2.2.0/gitblog2/blog_posts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 from dataclasses import dataclass
 from datetime import datetime
 import logging
+from pathlib import Path
 from typing import Generator, Iterator
 from git import Commit, Tree
 
 from gitblog2.repo_utils import fast_diff
+from gitblog2.utils import NONE_PATH, NonePath
 
 
 @dataclass
 class BlogPost:
     creation_dt: datetime
     last_update_dt: datetime
     author: str
-    relative_path: str
+    relative_path: Path
     title: str = ""
     description: str = ""
 
     @property
     def human_time(self):
         return self.last_update_dt.strftime("%b %d, %Y")
 
 
 class BlogPosts:
     def __init__(
         self,
         commits: Iterator[Commit],
-        repo_subdir: str = "",
+        repo_subdir: Path = NonePath(),
         ignore_dirs: tuple[str, ...] = (),
         ignore_files: tuple[str, ...] = (),
     ):
         self.ignore_dirs = ignore_dirs
         self.ignore_files = ignore_files
         self._init_path_to_blog_post(commits, repo_subdir)
 
-    def _init_path_to_blog_post(self, commits: Iterator[Commit], repo_subdir: str):
-        self.path_to_blog_post: dict[str, BlogPost] = {}
-        path_to_hash: dict[str, str] = {}
+    def _init_path_to_blog_post(self, commits: Iterator[Commit], repo_subdir: Path):
+        self.path_to_blog_post: dict[Path, BlogPost] = {}
+        path_to_hash: dict[Path, str] = {}
         latest_commit = next(commits)
 
-        for path, file_hash in self._gen_path_and_hashes(latest_commit.tree):
+        for path, file_hash in self._gen_path_and_hashes(latest_commit.tree, repo_subdir):
             path_to_hash[path] = file_hash
             self.path_to_blog_post[path] = BlogPost(
                 datetime.min,
                 datetime.min,
                 str(latest_commit.author),
-                path[:-3].removeprefix(repo_subdir),
+                path.relative_to(repo_subdir).with_suffix(''),
             )
         parent_commit = latest_commit
         # Traverse commit history to find posts creation dates
         for commit in commits:
             changed_paths, new_path_to_hash = fast_diff(path_to_hash, commit.tree)
             for path in changed_paths:
                 blog_post = self.path_to_blog_post[path]
@@ -58,23 +60,27 @@
                     blog_post.creation_dt = parent_commit.committed_datetime
             if not new_path_to_hash:
                 break
             parent_commit = commit
             path_to_hash = new_path_to_hash
 
     def _gen_path_and_hashes(
-        self, tree: Tree
-    ) -> Generator[tuple[str, str], None, None]:
+        self, tree: Tree, repo_subdir: Path
+    ) -> Generator[tuple[Path, str], None, None]:
         for obj in tree:
             if obj.type == "tree" and obj.name not in self.ignore_dirs:
-                yield from self._gen_path_and_hashes(obj)
+                yield from self._gen_path_and_hashes(obj, repo_subdir)
             elif obj.type == "blob" and obj.name.endswith(".md"):
+                path = Path(obj.path)
+                if repo_subdir is not NONE_PATH and not path.is_relative_to(repo_subdir):
+                    logging.debug("Skipped `%s`", path)
+                    continue
                 if obj.name in self.ignore_files:
-                    logging.debug("Skipped %s", obj.path)
+                    logging.debug("Skipped `%s`", path)
                     continue
-                yield str(obj.path), obj.hexsha
+                yield Path(obj.path), obj.hexsha
 
-    def __getitem__(self, path: str) -> BlogPost:
+    def __getitem__(self, path: Path) -> BlogPost:
         return self.path_to_blog_post[path]
 
     def values(self):
         return self.path_to_blog_post.values()
```

### Comparing `gitblog2-2.1.5/gitblog2/cli.py` & `gitblog2-2.2.0/gitblog2/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,65 @@
 #!/usr/bin/env python3
 from enum import Enum
 import logging
 import os
+from pathlib import Path
+from typing import Optional
 from urllib.parse import urlparse
 
 import typer
 from typing_extensions import Annotated
 
-from .lib import GitBlog
+from gitblog2.lib import GitBlog
+from gitblog2.utils import NONE_PATH, NonePath
 
 
 class LogLevel(str, Enum):
     DEBUG = "debug"
     INFO = "info"
     WARNING = "warning"
     ERROR = "error"
 
 
-def main():
-    typer.run(cli)
-
-
-def cli(
+def main(
+    clone_dir: Annotated[Optional[Path], typer.Option()] = None,
+    repo_subdir: Annotated[Optional[Path], typer.Option()] = None,
     source_repo: Annotated[
         str,
         typer.Argument(
             envvar="SOURCE_REPO",
         ),
     ] = "./",
-    output_dir: Annotated[str, typer.Argument(envvar="OUTPUT_DIR")] = "./public",
-    clone_dir: Annotated[str, typer.Option(envvar="CLONE_DIR")] = "",
-    repo_subdir: Annotated[str, typer.Option(envvar="REPO_SUBDIR")] = "",
+    output_dir: Annotated[Path, typer.Argument()] = Path("./public"),
     loglevel: Annotated[
-        LogLevel, typer.Option("--loglevel", "-l", envvar="LOG_LEVEL")
+        LogLevel, typer.Option("--loglevel", "-l", show_default="info")
     ] = LogLevel.INFO,
-    force: Annotated[bool, typer.Option("-f")] = False,
-    no_social: Annotated[bool, typer.Option(envvar="NO_SOCIAL")] = False,
-    no_fetch: Annotated[bool, typer.Option(envvar="NO_FETCH")] = False,
-    base_url: Annotated[str, typer.Option(envvar="BASE_URL")] = "",
+    force: Annotated[bool, typer.Option("--force", "-f")] = False,
+    no_social: Annotated[bool, typer.Option("--no-social")] = False,
+    no_fetch: Annotated[bool, typer.Option("--no-fetch")] = False,
+    base_url: Annotated[str, typer.Option()] = "",
 ):  # TODO add arguments descriptions
     logging.basicConfig(level=loglevel.upper(), format="%(levelname)s: %(message)s")
-    if os.path.exists(output_dir):
-        with os.scandir(output_dir) as it:
-            if any(it):
-                if not force:
-                    raise FileExistsError(
-                        f"The output directory '{output_dir}' is not empty, use --force to overwrite."
-                    )
-                logging.warning("The output directory is not empty.")
-
-    print(f"Generating blog into '{output_dir}'...")
+    if output_dir.exists():
+        if not output_dir.is_dir():
+            raise FileNotFoundError(f"`{output_dir}` is not a valid directory")
+        if any(output_dir.iterdir()):
+            if not force:
+                raise FileExistsError(
+                    f"The output directory `{output_dir}` is not empty, use --force to overwrite."
+                )
+            logging.warning(f"The output directory `{output_dir}` is not empty.")
+
+    print(f"Generating blog into `{output_dir}`...")
+    clone_dir = clone_dir or NONE_PATH
+    repo_subdir = repo_subdir or NONE_PATH
     with GitBlog(source_repo, clone_dir, repo_subdir, fetch=(not no_fetch)) as git_blog:
         git_blog.write_blog(
             output_dir,
             with_social=(not no_social),
             base_url=urlparse(base_url),
         )
     print("Done.")
 
 
 if __name__ == "__main__":
-    main()
+    typer.run(main)
```

### Comparing `gitblog2-2.1.5/gitblog2/lib.py` & `gitblog2-2.2.0/gitblog2/lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from base64 import b64encode
 from collections import defaultdict
 import logging
 import os
+from pathlib import Path
 import re
-import shutil
+import subprocess
 from tempfile import TemporaryDirectory
 from types import TracebackType
 from typing import Type, cast, Generator, Optional
 from urllib import request
 from urllib.parse import ParseResult, urlparse
 from functools import cached_property
 
 from feedgen.feed import FeedGenerator
 from feedgen.entry import FeedEntry
 import jinja2
 from markdown import markdown
 import requests
 from git.repo import Repo
 from git import Commit, Tree
-from git.types import PathLike
 
 from gitblog2.blog_posts import BlogPosts
+from gitblog2.utils import NONE_PATH
 
 
 MD_LIB_EXTENSIONS = ["extra", "toc"]
 MD_LIB_EXTENSION_CONFIGS = {"toc": {"title": " Table of contents"}}
 GITHUB_API_HEADERS = {
     "Accept": "application/vnd.github+json",
     "Authorization": f"Bearer {os.getenv('GITHUB_TOKEN')}",
@@ -32,51 +33,49 @@
 }
 
 
 class GitBlog:
     def __init__(
         self,
         source_repo: str,
-        clone_dir: str = "",
-        repo_subdir: str = "",
+        clone_path: Path = NONE_PATH,
+        repo_subdir: Path = NONE_PATH,
         ignore_dirs: tuple[str, ...] = ("draft", "media", "templates", ".github"),
         ignore_files: tuple[str, ...] = ("README.md", "LICENSE.md"),
         fetch: bool = True,
     ):
         self.source_repo = source_repo
-        self.repo_subdir = repo_subdir.strip("/")
+        self.repo_subdir = repo_subdir
         self.ignore_dirs = ignore_dirs
         self.ignore_files = ignore_files
 
         self.workdir = TemporaryDirectory()
         if _is_uri(self.source_repo):
-            self.clone_dir = clone_dir.rstrip("/") if clone_dir else self.workdir.name
+            self.clone_path = clone_path or Path(self.workdir.name)
         else:
-            self.clone_dir = source_repo.rstrip("/")
-        self.blog_path = (
-            self.clone_dir + "/" + self.repo_subdir
-            if self.repo_subdir
-            else self.clone_dir
-        ).rstrip("/")
+            self.clone_path = Path(source_repo)
+        logging.debug("Using clone_path `%s`", self.clone_path)
+        self.blog_path = self.clone_path / (self.repo_subdir or "")
+        logging.debug("Using blog_path `%s`", self.blog_path)
 
-        self.pkgdir = os.path.dirname(__file__)
+        self.pkgdir = Path(__file__).parent
+        logging.debug("pkgdir is`%s`", self.pkgdir)
         self.repo = self._init_repo(fetch)
         self.j2env = self._init_templating()
         commits = self.repo.iter_commits(self.last_commit, paths=self.repo_subdir)
         self.blog_posts = BlogPosts(
             commits, self.repo_subdir, self.ignore_dirs, self.ignore_files
         )
 
-        self.section_to_paths: defaultdict[str, set[str]] = defaultdict(set)
+        self.section_to_paths: defaultdict[str, set[Path]] = defaultdict(set)
         self.old_to_new_path: dict[str, str] = {}
 
     @cached_property
     def sections(self) -> list[str]:
         _sections = list(self.gen_sections())
-        logging.debug("Built sections.")
         return _sections
 
     @property
     def last_commit(self) -> Commit:
         return self.repo.head.commit
 
     @cached_property
@@ -101,15 +100,15 @@
             )
             for account in gh_social_accounts:
                 _social_accounts[account["provider"]] = account["url"]
         return _social_accounts
 
     def write_blog(
         self,
-        output_dir: str,
+        output_dir: Path,
         with_social: bool = True,
         base_url: ParseResult = urlparse(""),
     ):
         if with_social and not base_url.geturl():
             raise ValueError(
                 "You need to provide your website base URL in order to generate social feeds."
             )
@@ -118,37 +117,41 @@
 
         self.write_articles(output_dir, with_social)
         self.write_indexes(output_dir, with_social)
         if with_social:
             self.write_syndication_feeds(output_dir, base_url=base_url)
         self.add_static_assets(output_dir)
 
-    def write_articles(self, output_dir: str, with_social: bool = True):
+    def write_articles(self, output_dir: Path, with_social: bool = True):
         template = self.j2env.get_template("article.html.j2")
         for path, content in self.gen_articles_content():
-            rel_path = self.blog_posts[str(path)].relative_path
-            full_page = self.render_article(content, str(path), template, with_social)
-            target_path = output_dir + rel_path + ".html"
-            print(target_path)
-            _write_file(full_page, target_path)
+            rel_path = self.blog_posts[path].relative_path
+            full_page = self.render_article(content, path, template, with_social)
+            target_path = (output_dir / rel_path).with_suffix(".html")
+            target_path.parent.mkdir(parents=True, exist_ok=True)
+            target_path.write_text(full_page)
+            logging.debug("Added `%s`", target_path)
 
-    def write_indexes(self, output_dir: str, with_social: bool = True):
+    def write_indexes(self, output_dir: Path, with_social: bool = True):
         for section in self.sections:
-            target_path = f"{output_dir}/{section}/index.html"
+            target_path = output_dir / section / "index.html"
             try:
                 full_page = self.render_index(section, with_social)
             except Exception as ex:
                 logging.error("Failed to render index for section %s", section)
                 raise ex
-            _write_file(full_page, target_path)
+            target_path.write_text(full_page)
+            logging.debug("Added `%s`", target_path)
 
         home_page = self.render_index(with_social=with_social)
-        _write_file(home_page, f"{output_dir}/index.html")
+        home_path = output_dir / "index.html"
+        home_path.write_text(home_page)
+        logging.debug("Added `%s`", home_path)
 
-    def write_syndication_feeds(self, output_dir: str, base_url: ParseResult):
+    def write_syndication_feeds(self, output_dir: Path, base_url: ParseResult):
         url_hash = b64encode(base_url.geturl().encode()).decode()
         feed_id = f"ni://{base_url.hostname}/base64;{url_hash}"
         last_commit_dt = self.last_commit.committed_datetime
         author = str(self.last_commit.author)
         description = f"The latest news from {author}"
         feed = FeedGenerator()
         feed.id(feed_id)
@@ -157,45 +160,45 @@
         feed.author(name=author)
         feed.link(href=base_url.geturl())
         feed.logo(base_url.geturl() + "/media/favicon.svg")
         feed.updated(last_commit_dt)
         for _, paths in self.section_to_paths.items():
             for path in paths:
                 blog_post = self.blog_posts[path]
-                article_url = base_url.geturl() + "/" + blog_post.relative_path
+                article_url = base_url.geturl() + f"/{blog_post.relative_path}"
                 url_hash = b64encode(article_url.encode()).decode()
                 entry_id = f"ni://{base_url.hostname}/base64;{url_hash}"
 
                 feed_entry = FeedEntry()
                 feed_entry.id(entry_id)
                 feed_entry.title(blog_post.title)
                 feed_entry.summary(blog_post.description)
                 feed_entry.link(href=article_url, rel="alternate")
                 feed_entry.updated(blog_post.last_update_dt)
                 feed.add_entry(feed_entry)
-        feed.atom_file(output_dir + "/atom.xml")
-        feed.rss_file(output_dir + "/rss.xml")
+        feed.atom_file(str(output_dir / "atom.xml"))
+        feed.rss_file(str(output_dir / "rss.xml"))
         logging.debug("Wrote syndication feeds.")
 
     def render_article(
         self,
         content: str,
-        path: str,
+        path: Path,
         template: Optional[jinja2.Template] = None,
         with_social: bool = True,
     ) -> str:
         """content: Markdown content
         Return content in html format based on the jinja2 template"""
         if template is None:
             template = self.j2env.get_template("article.html.j2")
         title, description, md_content = self.parse_md(content)
         # TODO fix indexes not beeing rendered when render_article not previously called
         self.blog_posts[path].title = title
         self.blog_posts[path].description = description
-        section = path.removeprefix(self.repo_subdir).lstrip("/").split("/")[0]
+        section = path.relative_to(self.repo_subdir).parts[0]
         self.section_to_paths[section].add(path)
         html_content = markdown(
             md_content,
             extensions=MD_LIB_EXTENSIONS,
             extension_configs=MD_LIB_EXTENSION_CONFIGS,
         )
         try:
@@ -203,26 +206,26 @@
                 blog_post=self.blog_posts[path],
                 main_content=html_content,
                 sections=self.sections,
                 avatar_url="/media/avatar" if with_social else None,
                 social_accounts=self.social_accounts if with_social else None,
             )
         except Exception as e:
-            logging.error("Failed to render %s", path)
+            logging.error("Failed to render `%s`", path)
             raise e
         return final_html
 
     def render_index(
         self,
         section: str = "Home",
         with_social: bool = True,
     ) -> str:
         template = self.j2env.get_template("index.html.j2")
         if section == "Home":
-            section_paths = [p for ps in self.section_to_paths.values() for p in ps]
+            section_paths = {p for ps in self.section_to_paths.values() for p in ps}
         else:
             section_paths = self.section_to_paths[section]
         section_posts = [self.blog_posts[p] for p in section_paths]
         if section == "Home" and with_social:
             feeds = {"atom": "/atom.xml", "rss": "/rss.xml"}
         else:
             feeds = {}
@@ -231,73 +234,71 @@
             blog_posts=section_posts,
             sections=self.sections,
             feeds=feeds,
             avatar_url="/media/avatar" if with_social else None,
             social_accounts=self.social_accounts if with_social else None,
         )
 
-    def add_static_assets(self, output_dir: str):
+    def add_static_assets(self, output_dir: Path):
         """Copy static assets from the repo into the outupt dir.
         Use files from the package if not found"""
-        media_dst = output_dir + "/media"
-        custom_media = self.blog_path + "/media"
-        if os.path.exists(custom_media):
+        media_dst = output_dir / "media"
+        custom_media = self.blog_path / "media"
+        if custom_media.exists():
             sync_dir(custom_media, media_dst)
-        default_media = self.pkgdir + "/media"
+        default_media = self.pkgdir / "media"
         sync_dir(default_media, media_dst)
 
-        css_dst = output_dir + "/style.css"
-        default_css = self.pkgdir + "/style.css"
-        custom_css = self.blog_path + "/style.css"
-        if os.path.exists(custom_css):
-            shutil.copyfile(custom_css, css_dst)
-        else:
-            shutil.copyfile(default_css, css_dst)
+        css_dst = output_dir / "style.css"
+        default_css = self.pkgdir / "style.css"
+        custom_css = self.blog_path / "style.css"
+        css_content = custom_css.read_bytes() if custom_css.is_file() else default_css.read_bytes()
+        css_dst.write_bytes(css_content)
         logging.debug("Added static assets.")
 
-    def download_avatar(self, output_dir: str) -> None:
-        avatar_dst = output_dir + "/media/avatar"
-        if os.path.exists(avatar_dst):
+    def download_avatar(self, output_dir: Path) -> None:
+        avatar_dst = output_dir / "media/avatar"
+        if avatar_dst.exists():
             logging.warning("Avatar already downloaded.")
             return
         avatar_url = ""
         if self.repo_uri.hostname == "github.com":
             avatar_url = self._github_api_get("/user")["avatar_url"]
 
         if avatar_url:
-            os.makedirs(os.path.dirname(avatar_dst), exist_ok=True)
+            avatar_dst.parent.mkdir(parents=True, exist_ok=True)
             _, response = request.urlretrieve(avatar_url, avatar_dst)
             if response.get("content-type", "").startswith("image/"):
                 print("Avatar downloaded.")
             else:
                 logging.error("Avatar download response headers:\n%s", response)
 
     def gen_articles_content(
         self, tree: Optional[Tree] = None
-    ) -> Generator[tuple[PathLike, str], None, None]:
+    ) -> Generator[tuple[Path, str], None, None]:
         """Traverse repo files an return any (path, content) tuple corresponding to non blacklisted Markdown files.
         The path parameter is recursively constructed as we traverse the tree."""
         if tree is None:
             tree = self.last_commit.tree
             if self.repo_subdir:
-                tree = cast(Tree, tree[self.repo_subdir])
+                tree = cast(Tree, tree[str(self.repo_subdir)])
         for obj in tree:
             if obj.type == "tree" and obj.name not in self.ignore_dirs:
                 yield from self.gen_articles_content(obj)
             elif obj.type == "blob" and obj.name.endswith(".md"):
                 if obj.name in self.ignore_files:
-                    logging.debug("Skipped %s", obj.path)
+                    logging.debug("Skipped `%s`", obj.path)
                     continue
-                yield obj.path, cast(bytes, obj.data_stream.read()).decode("utf-8")
+                yield Path(obj.path), cast(bytes, obj.data_stream.read()).decode("utf-8")
 
     def gen_sections(self) -> Generator[str, None, None]:
         """Yield all sections found for this blog"""
         blog_root = self.last_commit.tree
         if self.repo_subdir:
-            blog_root = cast(Tree, blog_root[self.repo_subdir])
+            blog_root = cast(Tree, blog_root[str(self.repo_subdir)])
         # Enumerate all valid toplevel dirs
         for tree in blog_root.trees:
             if tree.name not in self.ignore_dirs:
                 yield tree.name
 
     def parse_md(self, md_content: str) -> tuple[str, str, str]:
         """Return title, description and main_content of the article
@@ -322,80 +323,79 @@
         response.raise_for_status()
         return response.json()
 
     def _init_repo(self, fetch: bool = True) -> Repo:
         """Check if there is an existing repo at self.clone_dir and clone the repo there otherwise.
         Optionally fetch changes after that."""
 
-        cloned_already = os.path.exists(self.clone_dir + "/.git/")
+        cloned_already = (self.clone_path / ".git").exists()
         if cloned_already:
-            repo = Repo(self.clone_dir)
+            repo = Repo(self.clone_path)
         else:
             repo = Repo.clone_from(
                 self.source_repo,
-                self.clone_dir,
+                self.clone_path,
                 multi_options=["--depth 1", "--no-checkout"],
             )
-            logging.debug("Cloned repo with depth 1 into %s", self.clone_dir)
+            logging.debug("Cloned repo with depth 1 into `%s`", self.clone_path)
         if fetch:
             # TODO check shallow
+            cmd = "git rev-parse --is-shallow-repository"
+            is_shallow = subprocess.check_output(cmd, shell=True).decode().startswith("true")
             repo.remotes.origin.fetch(
                 refspec=None,
                 progress=None,
                 verbose=True,
                 kill_after_timeout=None,
                 allow_unsafe_protocols=False,
                 allow_unsafe_options=False,
                 filter="blob:none",
                 no_tags=True,
-                unshallow=True,
+                unshallow=is_shallow,
             )
         return repo
 
     def _init_templating(self) -> jinja2.Environment:
         """Copy missing templates into the template dir if necessary
         and return a Jinja2Environment"""
-        templates_dst = self.workdir.name + "/templates"
-        custom_templates = self.blog_path + "/templates"
-        if os.path.exists(custom_templates):
+        templates_dst = Path(self.workdir.name) / "templates"
+        custom_templates = self.blog_path / "templates"
+        if custom_templates.exists():
             sync_dir(custom_templates, templates_dst, symlink=True)
-        default_templates = self.pkgdir + "/templates"
+        default_templates = self.pkgdir / "templates"
         sync_dir(default_templates, templates_dst, symlink=True)
         return jinja2.Environment(loader=jinja2.FileSystemLoader(templates_dst))
 
     def __enter__(self):
         return self
 
     def __exit__(
         self,
         exception_type: Optional[Type[BaseException]],
         exception: Optional[BaseException],
         traceback: Optional[TracebackType],
     ):
-        self.workdir.cleanup()
+        # self.workdir.cleanup()
+        pass
 
 
-def sync_dir(src: str, dst: str, symlink: bool = False):
+def sync_dir(src: Path, dst: Path, symlink: bool = False):
     """Add files that are missing from src into dst, optionally using symlinks"""
-    os.makedirs(dst, exist_ok=True)
-    for file in os.listdir(src):
-        dst_file = f"{dst}/{file}"
-        if not os.path.exists(dst_file):
+    dst.mkdir(parents=True, exist_ok=True)
+    for file in src.iterdir():
+        src_file = src / file.name
+        dst_file = dst / file.name
+        if dst_file.is_dir():
+            raise FileExistsError(f"Cannot create file `{dst_file}` as it is an existing directory.")
+        if not dst_file.exists():
             if symlink:
-                os.symlink(f"{src}/{file}", dst_file)
+                dst_file.symlink_to(src_file)
             else:
-                shutil.copyfile(f"{src}/{file}", dst_file)
-            logging.debug("Added %s", dst_file)
-
-
-def _write_file(content: str, target_path: str):
-    os.makedirs(os.path.dirname(target_path), exist_ok=True)
-    with open(target_path, "w+", encoding="utf-8") as file_descriptor:
-        file_descriptor.write(content)
-    logging.debug("Wrote %s", target_path)
+                dst_file.write_bytes(src_file.read_bytes())
+            logging.debug("Added `%s` to `%s`", src_file, dst)
 
 
 def _is_uri(repo_link: str):
     return repo_link.startswith(("http", "git@"))
 
 
 def _parse_uri(repo_link: str) -> ParseResult:
```

### Comparing `gitblog2-2.1.5/gitblog2/media/icons.svg` & `gitblog2-2.2.0/gitblog2/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/style.css` & `gitblog2-2.2.0/gitblog2/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/templates/article.html.j2` & `gitblog2-2.2.0/gitblog2/templates/article.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/templates/footer.html.j2` & `gitblog2-2.2.0/gitblog2/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/templates/index.html.j2` & `gitblog2-2.2.0/gitblog2/templates/index.html.j2`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     {% include "navbar.html.j2" %}
     {% endwith %}
   </header>
 
   <main>
     {%- for blog_post in blog_posts|sort(attribute='creation_dt', reverse=True) %}
     <article>
-      <strong><a href="{{ blog_post.relative_path }}">{{ blog_post.title }}</a></strong>
+      <strong><a href="/{{ blog_post.relative_path }}">{{ blog_post.title }}</a></strong>
       <p>
       {{ blog_post.description }}
       </p>
       <small>
         Last updated on {{ blog_post.human_time }}
       </small>
     </article>
```

### Comparing `gitblog2-2.1.5/gitblog2/tests/example_output/index.html` & `gitblog2-2.2.0/gitblog2/tests/example_output/tech/index.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html lang="en">
 
 <head>
   <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 
-<title>Home</title>
+<title>Tech</title>
 <link rel="icon" href="/media/favicon.svg">
 <link rel="stylesheet" href="/style.css" />
 <style>
   svg {
     width: 1em;
     height: 1em;
     fill: currentcolor;
```

### Comparing `gitblog2-2.1.5/gitblog2/tests/example_output/media/icons.svg` & `gitblog2-2.2.0/gitblog2/tests/example_output/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/tests/example_output/style.css` & `gitblog2-2.2.0/gitblog2/tests/example_output/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/tests/example_output/tech/example.html` & `gitblog2-2.2.0/gitblog2/tests/example_output/tech/example.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.1.5/gitblog2/tests/example_output/tech/index.html` & `gitblog2-2.2.0/gitblog2/tests/example_output/index.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html lang="en">
 
 <head>
   <meta charset="utf-8">
 <meta name="viewport" content="width=device-width, initial-scale=1">
 
-<title>Tech</title>
+<title>Home</title>
 <link rel="icon" href="/media/favicon.svg">
 <link rel="stylesheet" href="/style.css" />
 <style>
   svg {
     width: 1em;
     height: 1em;
     fill: currentcolor;
@@ -32,15 +32,15 @@
   <main>
     <article>
       <strong><a href="/tech/example">This article was made for GitBlog2</a></strong>
       <p>
       It aims at testing all content features as broadly as possible.
       </p>
       <small>
-        Last updated on Apr 22, 2023
+        Last updated on May 1, 2024
       </small>
     </article>
   </main>
   
   <footer>
   <p>
     <b title="Creative Commons Attribution 4.0 International license">
```

#### html2text {}

```diff
@@ -1,5 +1,5 @@
     * _TT_ee_cc_hh
 _TT_hh_ii_ss_ _aa_rr_tt_ii_cc_ll_ee_ _ww_aa_ss_ _mm_aa_dd_ee_ _ff_oo_rr_ _GG_ii_tt_BB_ll_oo_gg_22
 It aims at testing all content features as broadly as possible.
-Last updated on Apr 22, 2023
+Last updated on May 1, 2024
 HHeennrrii HHaannnneetteell | made with _G_i_t_B_l_o_g_2
```

### Comparing `gitblog2-2.1.5/gitblog2/tests/test_e2e.py` & `gitblog2-2.2.0/gitblog2/tests/test_e2e.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     subprocess.run(cmd, check=True)
 
     expected_content_dir = Path(__file__).resolve().parent / "example_output"
     files = ["index.html", "tech/example.html", "tech/index.html"]
     (match, mismatch, errors) = filecmp.cmpfiles(
         tmp_path, expected_content_dir, files
     )
+    print((tmp_path / "index.html").read_text())
 
     assert len(match) == len(files), f"mismatch: {mismatch}, errors: {errors}"
 
 
 def test_has_static_assets(tmp_path: Path):
     cmd = GITBLOG_CMD + [str(tmp_path)]
     subprocess.run(cmd, check=True)
```

### Comparing `gitblog2-2.1.5/pyproject.toml` & `gitblog2-2.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "gitblog2"
-version = "2.1.5"
+version = "2.2.0"
 description = "Git + Markdown = blog"
 authors = ["Henri Hannetel <henri.hannetel@pm.me>"]
 license = "MIT"
 readme = "docs/index.md"
+documentation = "https://henritel.github.io/gitblog2"
+repository = "https://github.com/HenriTEL/gitblog2"
 packages = [{ include = "gitblog2" }]
 include = ["gitblog2/*", "docs/index.md"]
 exclude = ["gitblog2/tests"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 Jinja2 = "^3.1.2"
```

### Comparing `gitblog2-2.1.5/PKG-INFO` & `gitblog2-2.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: gitblog2
-Version: 2.1.5
+Version: 2.2.0
 Summary: Git + Markdown = blog
+Home-page: https://github.com/HenriTEL/gitblog2
 License: MIT
 Author: Henri Hannetel
 Author-email: henri.hannetel@pm.me
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: Markdown (>=3.4.1,<4.0.0)
 Requires-Dist: feedgen (>=0.9.0,<0.10.0)
 Requires-Dist: gitpython (>=3.1.36,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: typer (>=0.7.0)
+Project-URL: Documentation, https://henritel.github.io/gitblog2
+Project-URL: Repository, https://github.com/HenriTEL/gitblog2
 Description-Content-Type: text/markdown
 
 # ![Gitblog2 Logo](https://blog.henritel.com/media/favicon.svg "title") Gitblog2
 
 > Git + Markdown = Blog
 
 [![PyPI Version][pypi-v-image]][pypi-v-link]
```

