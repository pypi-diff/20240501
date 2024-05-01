# Comparing `tmp/gitblog2-2.2.0.tar.gz` & `tmp/gitblog2-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitblog2-2.2.0.tar", max compression
+gzip compressed data, was "gitblog2-2.2.1.tar", max compression
```

## Comparing `gitblog2-2.2.0.tar` & `gitblog2-2.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.2.0/LICENSE
--rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.2.0/build.py
--rw-r--r--   0        0        0     5724 2024-04-30 20:29:05.248299 gitblog2-2.2.0/docs/index.md
--rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.2.0/gitblog2/__init__.py
--rw-r--r--   0        0        0     3120 2024-05-01 07:13:51.643163 gitblog2-2.2.0/gitblog2/blog_posts.py
--rwxr-xr-x   0        0        0     2122 2024-05-01 07:45:59.555677 gitblog2-2.2.0/gitblog2/cli.py
--rw-r--r--   0        0        0    16173 2024-05-01 07:43:59.187765 gitblog2-2.2.0/gitblog2/lib.py
--rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.2.0/gitblog2/media/favicon.svg
--rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.2.0/gitblog2/media/icons.svg
--rw-r--r--   0        0        0      576 2024-04-30 22:21:55.113810 gitblog2-2.2.0/gitblog2/repo_utils.py
--rw-r--r--   0        0        0     6749 2024-04-30 21:08:14.949907 gitblog2-2.2.0/gitblog2/style.css
--rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/article.html.j2
--rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/footer.html.j2
--rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/head_common.html.j2
--rw-r--r--   0        0        0      868 2024-05-01 07:49:50.931184 gitblog2-2.2.0/gitblog2/templates/index.html.j2
--rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/templates/navbar.html.j2
--rw-r--r--   0        0        0     1183 2024-05-01 07:57:13.613841 gitblog2-2.2.0/gitblog2/tests/example_output/index.html
--rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/media/favicon.svg
--rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/media/icons.svg
--rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/style.css
--rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/tech/example.html
--rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.2.0/gitblog2/tests/example_output/tech/index.html
--rw-r--r--   0        0        0     1000 2024-05-01 07:48:06.899524 gitblog2-2.2.0/gitblog2/tests/test_e2e.py
--rw-r--r--   0        0        0      145 2024-05-01 01:12:36.414254 gitblog2-2.2.0/gitblog2/utils.py
--rw-r--r--   0        0        0      885 2024-05-01 07:58:34.245659 gitblog2-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6655 1970-01-01 00:00:00.000000 gitblog2-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-02-18 16:19:17.029548 gitblog2-2.2.1/LICENSE
+-rw-r--r--   0        0        0      261 2023-04-08 12:33:53.131324 gitblog2-2.2.1/build.py
+-rw-r--r--   0        0        0     5724 2024-04-30 20:29:05.248299 gitblog2-2.2.1/docs/index.md
+-rw-r--r--   0        0        0       25 2023-02-18 16:19:17.029548 gitblog2-2.2.1/gitblog2/__init__.py
+-rw-r--r--   0        0        0     3126 2024-05-01 08:08:38.396500 gitblog2-2.2.1/gitblog2/blog_posts.py
+-rwxr-xr-x   0        0        0     2122 2024-05-01 07:45:59.555677 gitblog2-2.2.1/gitblog2/cli.py
+-rw-r--r--   0        0        0    16179 2024-05-01 08:10:39.776299 gitblog2-2.2.1/gitblog2/lib.py
+-rw-r--r--   0        0        0      362 2023-04-22 16:58:21.192330 gitblog2-2.2.1/gitblog2/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2023-09-27 15:11:44.319193 gitblog2-2.2.1/gitblog2/media/icons.svg
+-rw-r--r--   0        0        0      576 2024-04-30 22:21:55.113810 gitblog2-2.2.1/gitblog2/repo_utils.py
+-rw-r--r--   0        0        0     6749 2024-05-01 08:00:01.993470 gitblog2-2.2.1/gitblog2/style.css
+-rw-r--r--   0        0        0     1004 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/templates/article.html.j2
+-rw-r--r--   0        0        0      650 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/templates/footer.html.j2
+-rw-r--r--   0        0        0      327 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/templates/head_common.html.j2
+-rw-r--r--   0        0        0      868 2024-05-01 07:49:50.931184 gitblog2-2.2.1/gitblog2/templates/index.html.j2
+-rw-r--r--   0        0        0      360 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/templates/navbar.html.j2
+-rw-r--r--   0        0        0     1183 2024-05-01 07:57:13.613841 gitblog2-2.2.1/gitblog2/tests/example_output/index.html
+-rw-r--r--   0        0        0      362 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/tests/example_output/media/favicon.svg
+-rw-r--r--   0        0        0     7951 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/tests/example_output/media/icons.svg
+-rw-r--r--   0        0        0     6749 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/tests/example_output/style.css
+-rw-r--r--   0        0        0     3398 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/tests/example_output/tech/example.html
+-rw-r--r--   0        0        0     1184 2024-01-21 12:38:57.005522 gitblog2-2.2.1/gitblog2/tests/example_output/tech/index.html
+-rw-r--r--   0        0        0     1000 2024-05-01 07:48:06.899524 gitblog2-2.2.1/gitblog2/tests/test_e2e.py
+-rw-r--r--   0        0        0      145 2024-05-01 01:12:36.414254 gitblog2-2.2.1/gitblog2/utils.py
+-rw-r--r--   0        0        0      885 2024-05-01 08:11:21.788228 gitblog2-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6655 1970-01-01 00:00:00.000000 gitblog2-2.2.1/PKG-INFO
```

### Comparing `gitblog2-2.2.0/LICENSE` & `gitblog2-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/docs/index.md` & `gitblog2-2.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/blog_posts.py` & `gitblog2-2.2.1/gitblog2/blog_posts.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
         for path, file_hash in self._gen_path_and_hashes(latest_commit.tree, repo_subdir):
             path_to_hash[path] = file_hash
             self.path_to_blog_post[path] = BlogPost(
                 datetime.min,
                 datetime.min,
                 str(latest_commit.author),
-                path.relative_to(repo_subdir).with_suffix(''),
+                path.relative_to(repo_subdir or "").with_suffix(''),
             )
         parent_commit = latest_commit
         # Traverse commit history to find posts creation dates
         for commit in commits:
             changed_paths, new_path_to_hash = fast_diff(path_to_hash, commit.tree)
             for path in changed_paths:
                 blog_post = self.path_to_blog_post[path]
```

### Comparing `gitblog2-2.2.0/gitblog2/cli.py` & `gitblog2-2.2.1/gitblog2/cli.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/lib.py` & `gitblog2-2.2.1/gitblog2/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
         Return content in html format based on the jinja2 template"""
         if template is None:
             template = self.j2env.get_template("article.html.j2")
         title, description, md_content = self.parse_md(content)
         # TODO fix indexes not beeing rendered when render_article not previously called
         self.blog_posts[path].title = title
         self.blog_posts[path].description = description
-        section = path.relative_to(self.repo_subdir).parts[0]
+        section = path.relative_to(self.repo_subdir or "").parts[0]
         self.section_to_paths[section].add(path)
         html_content = markdown(
             md_content,
             extensions=MD_LIB_EXTENSIONS,
             extension_configs=MD_LIB_EXTENSION_CONFIGS,
         )
         try:
```

### Comparing `gitblog2-2.2.0/gitblog2/media/icons.svg` & `gitblog2-2.2.1/gitblog2/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/repo_utils.py` & `gitblog2-2.2.1/gitblog2/repo_utils.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/style.css` & `gitblog2-2.2.1/gitblog2/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/templates/article.html.j2` & `gitblog2-2.2.1/gitblog2/templates/article.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/templates/footer.html.j2` & `gitblog2-2.2.1/gitblog2/templates/footer.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/templates/index.html.j2` & `gitblog2-2.2.1/gitblog2/templates/index.html.j2`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/example_output/index.html` & `gitblog2-2.2.1/gitblog2/tests/example_output/index.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/example_output/media/icons.svg` & `gitblog2-2.2.1/gitblog2/tests/example_output/media/icons.svg`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/example_output/style.css` & `gitblog2-2.2.1/gitblog2/tests/example_output/style.css`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/example_output/tech/example.html` & `gitblog2-2.2.1/gitblog2/tests/example_output/tech/example.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/example_output/tech/index.html` & `gitblog2-2.2.1/gitblog2/tests/example_output/tech/index.html`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/gitblog2/tests/test_e2e.py` & `gitblog2-2.2.1/gitblog2/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `gitblog2-2.2.0/pyproject.toml` & `gitblog2-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitblog2"
-version = "2.2.0"
+version = "2.2.1"
 description = "Git + Markdown = blog"
 authors = ["Henri Hannetel <henri.hannetel@pm.me>"]
 license = "MIT"
 readme = "docs/index.md"
 documentation = "https://henritel.github.io/gitblog2"
 repository = "https://github.com/HenriTEL/gitblog2"
 packages = [{ include = "gitblog2" }]
```

### Comparing `gitblog2-2.2.0/PKG-INFO` & `gitblog2-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitblog2
-Version: 2.2.0
+Version: 2.2.1
 Summary: Git + Markdown = blog
 Home-page: https://github.com/HenriTEL/gitblog2
 License: MIT
 Author: Henri Hannetel
 Author-email: henri.hannetel@pm.me
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

