# Comparing `tmp/ancv-1.3.1.tar.gz` & `tmp/ancv-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ancv-1.3.1.tar", max compression
+gzip compressed data, was "ancv-1.4.0.tar", max compression
```

## Comparing `ancv-1.3.1.tar` & `ancv-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1067 2023-04-21 20:08:22.234434 ancv-1.3.1/LICENSE
--rw-r--r--   0        0        0    10301 2023-04-21 20:08:22.234434 ancv-1.3.1/README.md
--rw-r--r--   0        0        0      308 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/__init__.py
--rw-r--r--   0        0        0     8719 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/__main__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/__init__.py
--rw-r--r--   0        0        0     3102 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/github.py
--rw-r--r--   0        0        0    13506 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/models/resume.py
--rw-r--r--   0        0        0     7803 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/showcase.resume.json
--rw-r--r--   0        0        0      932 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/data/validation.py
--rw-r--r--   0        0        0      250 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/py.typed
--rw-r--r--   0        0        0     3115 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/reflection.py
--rw-r--r--   0        0        0     1639 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/timing.py
--rw-r--r--   0        0        0      172 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/__init__.py
--rw-r--r--   0        0        0    30290 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/templates.py
--rw-r--r--   0        0        0     4199 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/themes.py
--rw-r--r--   0        0        0     2778 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/visualization/translations.py
--rw-r--r--   0        0        0        0 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/__init__.py
--rw-r--r--   0        0        0     4004 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/client.py
--rw-r--r--   0        0        0     8835 2023-04-21 20:08:22.234434 ancv-1.3.1/ancv/web/server.py
--rw-r--r--   0        0        0     2732 2023-04-21 20:08:22.246434 ancv-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    12351 1970-01-01 00:00:00.000000 ancv-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-01 14:29:59.445387 ancv-1.4.0/LICENSE
+-rw-r--r--   0        0        0    10748 2024-05-01 14:29:59.445387 ancv-1.4.0/README.md
+-rw-r--r--   0        0        0      308 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/__init__.py
+-rw-r--r--   0        0        0     8727 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/models/__init__.py
+-rw-r--r--   0        0        0     3343 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/models/github.py
+-rw-r--r--   0        0        0    15593 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/models/resume.py
+-rw-r--r--   0        0        0     7803 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/showcase.resume.json
+-rw-r--r--   0        0        0      932 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/data/validation.py
+-rw-r--r--   0        0        0      250 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/py.typed
+-rw-r--r--   0        0        0     3830 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/reflection.py
+-rw-r--r--   0        0        0     1639 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/timing.py
+-rw-r--r--   0        0        0      172 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/visualization/__init__.py
+-rw-r--r--   0        0        0    30589 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/visualization/templates.py
+-rw-r--r--   0        0        0     4139 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/visualization/themes.py
+-rw-r--r--   0        0        0     2778 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/visualization/translations.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/web/__init__.py
+-rw-r--r--   0        0        0     4004 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/web/client.py
+-rw-r--r--   0        0        0     8827 2024-05-01 14:29:59.445387 ancv-1.4.0/ancv/web/server.py
+-rw-r--r--   0        0        0     2959 2024-05-01 14:29:59.453387 ancv-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12748 1970-01-01 00:00:00.000000 ancv-1.4.0/PKG-INFO
```

### Comparing `ancv-1.3.1/LICENSE` & `ancv-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/README.md` & `ancv-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,25 @@
    <img src="docs/images/users-venn.svg" alt="users venn diagram">
 </p>
 
 ## Getting started
 
 1. Create your resume according to the [JSON Resume Schema](https://jsonresume.org/schema/) (see also the [schema specification](https://github.com/jsonresume/resume-schema/blob/master/schema.json)) either:
 
+   - use ChatGPT (or another LLM) with the following prompt (you need to fill in the spaces for `[resume]` and `[json_schema]`):
+      ```
+      Resume:[resume]
+
+      JSON Resume Schema:[json_schema]
+
+      Provide JSON data structure of the resume, formatted according to the JSON Resume Schema
+      
+      Output json, no yapping
+      ```
+      Note: for `json_schema` you can just use the example [from here](https://jsonresume.org/schema/)
    - manually (see [the `heyho` sample](./ancv/data/showcase.resume.json) for a possible starting point),
    - exporting from [LinkedIn](https://www.linkedin.com/) using [Joshua Tzucker's LinkedIn exporter](https://joshuatz.com/projects/web-stuff/linkedin-profile-to-json-resume-exporter/) ([repo](https://github.com/joshuatz/linkedin-to-jsonresume))[^1], or
    - exporting from one of the platforms advertised as offering [JSON resume integration](https://jsonresume.org/schema/).
 2. [Create a **public** gist](https://gist.github.com/) named `resume.json` with your resume contents.
 3. You're now the proud owner of an ancv.
    Time to try it out.
```

### Comparing `ancv-1.3.1/ancv/__main__.py` & `ancv-1.4.0/ancv/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     api = APIHandler(
         # https://docs.github.com/en/rest/overview/resources-in-the-rest-api#user-agent-required :
         requester=os.environ.get("GH_REQUESTER", METADATA.name),
         # Not specifying a token works just as well, but has a much lower request
         # ceiling:
         token=os.environ.get("GH_TOKEN"),
         terminal_landing_page=os.environ.get(
-            "HOMEPAGE", METADATA.home_page or "NO HOMEPAGE SET"
+            "HOMEPAGE", str(METADATA.home_page) or "NO HOMEPAGE SET"
         ),
         # When visiting this endpoint in a browser, we want to redirect to the homepage.
         # That page cannot be this same path under the same hostname again, else we get
         # a loop.
         browser_landing_page=os.environ.get(
             "LANDING_PAGE",
             METADATA.project_url[0] if METADATA.project_url else "https://github.com/",
@@ -69,15 +69,15 @@
 
 
 @app.command()
 def render(
     path: Path = typer.Argument(
         Path("resume.json"),
         help="File path to the JSON resume file.",
-    )
+    ),
 ) -> None:
     """Locally renders the JSON resume at the given file path."""
 
     from ancv.visualization.templates import Template
 
     template = Template.from_file(path)
     output = template.render()
@@ -86,15 +86,15 @@
 
 
 @app.command()
 def validate(
     path: Path = typer.Argument(
         Path("resume.json"),
         help="File path to the JSON resume file.",
-    )
+    ),
 ) -> None:
     """Checks the validity of the given JSON resume without rendering."""
 
     from pydantic import ValidationError
 
     from ancv.exceptions import ResumeConfigError
     from ancv.visualization.templates import Template
@@ -221,15 +221,15 @@
     print(json.dumps(schema, indent=4))
 
 
 @app.callback()
 def main(
     verbose: bool = typer.Option(
         False, "--verbose", "-v", help="Turn on verbose logging output."
-    )
+    ),
 ) -> None:
     """CLI-wide, global options.
 
     https://typer.tiangolo.com/tutorial/commands/callback/
     """
 
     import logging
```

### Comparing `ancv-1.3.1/ancv/data/models/github.py` & `ancv-1.4.0/ancv/data/models/github.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,82 @@
 """This module contains models for the relevant parts of GitHub's API."""
 
+import typing as t
 from datetime import datetime
-from typing import Mapping, Optional
 
 from pydantic import BaseModel, Field, HttpUrl
 
 
 class File(BaseModel):
     """Modelling a GitHub gist's file.
 
-    See: https://docs.github.com/en/rest/gists/gists?apiVersion=2022-11-28#list-gists-for-the-authenticated-user, under the "files" key."""
+    See: https://docs.github.com/en/rest/gists/gists?apiVersion=2022-11-28#list-gists-for-the-authenticated-user, under the "files" key.
+    """
 
-    filename: Optional[str]
-    type: Optional[str]
-    language: Optional[str]
-    raw_url: Optional[HttpUrl]
-    size: Optional[int]
+    filename: t.Optional[str] = None
+    type: t.Optional[str] = None
+    language: t.Optional[str] = None
+    raw_url: t.Optional[HttpUrl] = None
+    size: t.Optional[int] = None
 
 
 class GistUser(BaseModel):
     """Modelling a GitHub gist's owner/user.
 
-    See: https://docs.github.com/en/rest/gists/gists?apiVersion=2022-11-28#list-gists-for-the-authenticated-user"""
+    See: https://docs.github.com/en/rest/gists/gists?apiVersion=2022-11-28#list-gists-for-the-authenticated-user
+    """
 
-    name: Optional[str] = None
-    email: Optional[str] = None
-    login: str = Field(..., examples=["octocat"])
-    id: int = Field(..., examples=[1])
-    node_id: str = Field(..., examples=["MDQ6VXNlcjE="])
-    avatar_url: HttpUrl = Field(
-        ..., examples=["https://github.com/images/error/octocat_happy.gif"]
-    )
-    gravatar_id: Optional[str] = Field(
-        ..., examples=["41d064eb2195891e12d0413f63227ea7"]
-    )
-    url: HttpUrl = Field(..., examples=["https://api.github.com/users/octocat"])
-    html_url: HttpUrl = Field(..., examples=["https://github.com/octocat"])
-    followers_url: HttpUrl = Field(
-        ..., examples=["https://api.github.com/users/octocat/followers"]
-    )
-    following_url: str = Field(
-        ..., examples=["https://api.github.com/users/octocat/following{/other_user}"]
-    )
-    gists_url: str = Field(
-        ..., examples=["https://api.github.com/users/octocat/gists{/gist_id}"]
-    )
-    starred_url: str = Field(
-        ..., examples=["https://api.github.com/users/octocat/starred{/owner}{/repo}"]
-    )
-    subscriptions_url: HttpUrl = Field(
-        ..., examples=["https://api.github.com/users/octocat/subscriptions"]
-    )
-    organizations_url: HttpUrl = Field(
-        ..., examples=["https://api.github.com/users/octocat/orgs"]
-    )
-    repos_url: HttpUrl = Field(
-        ..., examples=["https://api.github.com/users/octocat/repos"]
-    )
-    events_url: str = Field(
-        ..., examples=["https://api.github.com/users/octocat/events{/privacy}"]
-    )
-    received_events_url: HttpUrl = Field(
-        ..., examples=["https://api.github.com/users/octocat/received_events"]
-    )
-    type: str = Field(..., examples=["User"])
+    name: t.Optional[str] = None
+    email: t.Optional[str] = None
+    login: t.Annotated[str, Field(examples=["octocat"])]
+    id: t.Annotated[int, Field(examples=[1])]
+    node_id: t.Annotated[str, Field(examples=["MDQ6VXNlcjE="])]
+    avatar_url: t.Annotated[
+        HttpUrl, Field(examples=["https://github.com/images/error/octocat_happy.gif"])
+    ]
+    gravatar_id: t.Annotated[
+        t.Optional[str], Field(examples=["41d064eb2195891e12d0413f63227ea7"])
+    ]
+    url: t.Annotated[HttpUrl, Field(examples=["https://api.github.com/users/octocat"])]
+    html_url: t.Annotated[HttpUrl, Field(examples=["https://github.com/octocat"])]
+    followers_url: t.Annotated[
+        HttpUrl, Field(examples=["https://api.github.com/users/octocat/followers"])
+    ]
+    following_url: t.Annotated[
+        str,
+        Field(examples=["https://api.github.com/users/octocat/following{/other_user}"]),
+    ]
+    gists_url: t.Annotated[
+        str, Field(examples=["https://api.github.com/users/octocat/gists{/gist_id}"])
+    ]
+    starred_url: t.Annotated[
+        str,
+        Field(examples=["https://api.github.com/users/octocat/starred{/owner}{/repo}"]),
+    ]
+    subscriptions_url: t.Annotated[
+        HttpUrl, Field(examples=["https://api.github.com/users/octocat/subscriptions"])
+    ]
+    organizations_url: t.Annotated[
+        HttpUrl, Field(examples=["https://api.github.com/users/octocat/orgs"])
+    ]
+    repos_url: t.Annotated[
+        HttpUrl, Field(examples=["https://api.github.com/users/octocat/repos"])
+    ]
+    events_url: t.Annotated[
+        str, Field(examples=["https://api.github.com/users/octocat/events{/privacy}"])
+    ]
+    received_events_url: t.Annotated[
+        HttpUrl,
+        Field(examples=["https://api.github.com/users/octocat/received_events"]),
+    ]
+    type: t.Annotated[str, Field(examples=["User"])]
     site_admin: bool
-    starred_at: Optional[datetime] = Field(None, examples=['"2020-07-09T00:17:55Z"'])
+    starred_at: t.Annotated[
+        t.Optional[datetime], Field(None, examples=['"2020-07-09T00:17:55Z"'])
+    ]
 
 
 class Gist(BaseModel):
     """Modelling a GitHub gist.
 
     See: https://docs.github.com/en/rest/gists/gists?apiVersion=2022-11-28"""
 
@@ -77,17 +84,17 @@
     forks_url: HttpUrl
     commits_url: HttpUrl
     id: str
     node_id: str
     git_pull_url: HttpUrl
     git_push_url: HttpUrl
     html_url: HttpUrl
-    files: Mapping[str, File]
+    files: t.Mapping[str, File]
     public: bool
     created_at: datetime
     updated_at: datetime
-    description: Optional[str]
+    description: t.Optional[str] = None
     comments: int
-    user: Optional[GistUser]
+    user: t.Optional[GistUser] = None
     comments_url: HttpUrl
-    owner: Optional[GistUser] = None
-    truncated: Optional[bool] = None
+    owner: t.Optional[GistUser] = None
+    truncated: t.Optional[bool] = None
```

### Comparing `ancv-1.3.1/ancv/data/models/resume.py` & `ancv-1.4.0/ancv/data/models/resume.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,388 +1,477 @@
 """This module contains models for the JSON Resume standard.
 
 See: https://jsonresume.org/schema/.
 """
 
-from __future__ import annotations
+import datetime
+import typing as t
 
-from datetime import date, datetime
-from typing import Optional, Union
-
-from pydantic import AnyUrl, BaseModel, EmailStr, Extra, Field
+from pydantic import AnyUrl, BaseModel, ConfigDict, EmailStr, Field
 
 
 class Location(BaseModel):
     """Modelling a JSON resume location item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L50-L73"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L50-L73
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    address: Optional[str] = Field(
-        None,
-        description="To add multiple address lines, use \n. For example, 1234 Glücklichkeit Straße\nHinterhaus 5. Etage li.",
-    )
-    postalCode: Optional[str] = None
-    city: Optional[str] = None
-    countryCode: Optional[str] = Field(
-        None, description="code as per ISO-3166-1 ALPHA-2, e.g. US, AU, IN"
-    )
-    region: Optional[str] = Field(
-        None,
-        description="The general region where you live. Can be a US state, or a province, for instance.",
-    )
+    address: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="To add multiple address lines, use \n. For example, 1234 Glücklichkeit Straße\nHinterhaus 5. Etage li.",
+        ),
+    ] = None
+    postalCode: t.Optional[str] = None
+    city: t.Optional[str] = None
+    countryCode: t.Annotated[
+        t.Optional[str],
+        Field(description="code as per ISO-3166-1 ALPHA-2, e.g. US, AU, IN"),
+    ] = None
+    region: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="The general region where you live. Can be a US state, or a province, for instance.",
+        ),
+    ] = None
 
 
 class Profile(BaseModel):
     """Modelling a JSON resume profile item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L74-L99"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L74-L99
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    network: Optional[str] = Field(None, description="e.g. Facebook or Twitter")
-    username: Optional[str] = Field(None, description="e.g. neutralthoughts")
-    url: Optional[AnyUrl] = Field(
-        None, description="e.g. http://twitter.example.com/neutralthoughts"
-    )
+    network: t.Annotated[
+        t.Optional[str], Field(description="e.g. Facebook or Twitter")
+    ] = None
+    username: t.Annotated[
+        t.Optional[str], Field(description="e.g. neutralthoughts")
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(description="e.g. http://twitter.example.com/neutralthoughts"),
+    ] = None
 
 
 class Basics(BaseModel):
     """Modelling a JSON resume basics item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L17-L49"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L17-L49
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = None
-    label: Optional[str] = Field(None, description="e.g. Web Developer")
-    image: Optional[str] = Field(
-        None, description="URL (as per RFC 3986) to a image in JPEG or PNG format"
-    )
-    email: Optional[EmailStr] = Field(None, description="e.g. thomas@gmail.com")
-    phone: Optional[str] = Field(
-        None,
-        description="Phone numbers are stored as strings so use any format you like, e.g. 712-117-2923",
-    )
-    url: Optional[AnyUrl] = Field(
-        None,
-        description="URL (as per RFC 3986) to your website, e.g. personal homepage",
-    )
-    summary: Optional[str] = Field(
-        None, description="Write a short 2-3 sentence biography about yourself"
-    )
-    location: Optional[Location] = None
-    profiles: Optional[list[Profile]] = Field(
-        None,
-        description="Specify any number of social networks that you participate in",
-    )
+    name: t.Optional[str] = None
+    label: t.Annotated[t.Optional[str], Field(description="e.g. Web Developer")] = None
+    image: t.Annotated[
+        t.Optional[str],
+        Field(description="URL (as per RFC 3986) to a image in JPEG or PNG format"),
+    ] = None
+    email: t.Annotated[
+        t.Optional[EmailStr], Field(description="e.g. thomas@gmail.com")
+    ] = None
+    phone: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="Phone numbers are stored as strings so use any format you like, e.g. 712-117-2923",
+        ),
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(
+            description="URL (as per RFC 3986) to your website, e.g. personal homepage",
+        ),
+    ] = None
+    summary: t.Annotated[
+        t.Optional[str],
+        Field(description="Write a short 2-3 sentence biography about yourself"),
+    ] = None
+    location: t.Optional[Location] = None
+    profiles: t.Annotated[
+        t.Optional[list[Profile]],
+        Field(
+            description="Specify any number of social networks that you participate in",
+        ),
+    ] = None
 
 
 class Certificate(BaseModel):
     """Modelling a JSON resume certificate item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L264-L292"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L264-L292
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(
-        None, description="e.g. Certified Kubernetes Administrator"
-    )
-    date: Optional[date] = Field(None, description="e.g. 1989-06-12")
-    url: Optional[AnyUrl] = Field(None, description="e.g. http://example.com")
-    issuer: Optional[str] = Field(None, description="e.g. CNCF")
+    name: t.Annotated[
+        t.Optional[str], Field(description="e.g. Certified Kubernetes Administrator")
+    ] = None
+    date: t.Annotated[
+        t.Optional[datetime.date], Field(description="e.g. 1989-06-12")
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl], Field(description="e.g. http://example.com")
+    ] = None
+    issuer: t.Annotated[t.Optional[str], Field(description="e.g. CNCF")] = None
 
 
 class Skill(BaseModel):
     """Modelling a JSON resume skill item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L324-L351"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L324-L351
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. Web Development")
-    level: Optional[str] = Field(None, description="e.g. Master")
-    keywords: Optional[list[str]] = Field(
-        None, description="List some keywords pertaining to this skill"
-    )
+    name: t.Annotated[t.Optional[str], Field(description="e.g. Web Development")] = None
+    level: t.Annotated[t.Optional[str], Field(description="e.g. Master")] = None
+    keywords: t.Annotated[
+        t.Optional[list[str]],
+        Field(description="List some keywords pertaining to this skill"),
+    ] = None
 
 
 class Language(BaseModel):
     """Modelling a JSON resume language item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L352-L370"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L352-L370
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    language: Optional[str] = Field(None, description="e.g. English, Spanish")
-    fluency: Optional[str] = Field(None, description="e.g. Fluent, Beginner")
+    language: t.Annotated[
+        t.Optional[str], Field(description="e.g. English, Spanish")
+    ] = None
+    fluency: t.Annotated[
+        t.Optional[str], Field(description="e.g. Fluent, Beginner")
+    ] = None
 
 
 class Interest(BaseModel):
     """Modelling a JSON resume interest item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L371-L392"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L371-L392
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. Philosophy")
-    keywords: Optional[list[str]] = None
+    name: t.Annotated[t.Optional[str], Field(description="e.g. Philosophy")] = None
+    keywords: t.Optional[list[str]] = None
 
 
 class Reference(BaseModel):
     """Modelling a JSON resume reference item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L393-L411"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L393-L411
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. Timothy Cook")
-    reference: Optional[str] = Field(
-        None,
-        description="e.g. Joe blogs was a great employee, who turned up to work at least once a week. He exceeded my expectations when it came to doing nothing.",
-    )
+    name: t.Annotated[t.Optional[str], Field(description="e.g. Timothy Cook")] = None
+    reference: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="e.g. Joe blogs was a great employee, who turned up to work at least once a week. He exceeded my expectations when it came to doing nothing.",
+        ),
+    ] = None
 
 
 class TemplateConfig(BaseModel):
     """Modelling ancv-specific template configuration.
 
     This controls ancv-specific settings such as the template and theme to use.
     It occurs as an additional, but optional field in the JSON resume.
     """
 
-    template: Optional[str]
-    theme: Optional[str]
-    language: Optional[str]
-    ascii_only: Optional[bool]
-    dec31_as_year: Optional[bool]
+    template: t.Optional[str] = None
+    theme: t.Optional[str] = None
+    language: t.Optional[str] = None
+    ascii_only: t.Optional[bool] = None
+    dec31_as_year: t.Optional[bool] = None
 
 
 class Meta(BaseModel):
     """Modelling a JSON resume meta item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L477-L497"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L477-L497
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    canonical: Optional[AnyUrl] = Field(
-        None, description="URL (as per RFC 3986) to latest version of this document"
-    )
-    version: Optional[str] = Field(
-        None, description="A version field which follows semver - e.g. v1.0.0"
-    )
-    lastModified: Optional[datetime] = Field(
-        None, description="Using ISO 8601 with YYYY-MM-DDThh:mm:ss"
-    )
-    config: Optional[TemplateConfig] = Field(
-        None,
-        alias="ancv",
-        description="Template configuration to control display",
-    )
+    canonical: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(description="URL (as per RFC 3986) to latest version of this document"),
+    ] = None
+    version: t.Annotated[
+        t.Optional[str],
+        Field(description="A version field which follows semver - e.g. v1.0.0"),
+    ] = None
+    lastModified: t.Annotated[
+        t.Optional[datetime.datetime],
+        Field(description="Using ISO 8601 with YYYY-MM-DDThh:mm:ss"),
+    ] = None
+    config: t.Annotated[
+        t.Optional[TemplateConfig],
+        Field(
+            alias="ancv",
+            description="Template configuration to control display",
+        ),
+    ] = None
 
 
 class WorkItem(BaseModel):
     """Modelling a JSON resume work item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L100-L149"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L100-L149
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. Facebook")
-    location: Optional[str] = Field(None, description="e.g. Menlo Park, CA")
-    description: Optional[str] = Field(None, description="e.g. Social Media Company")
-    position: Optional[str] = Field(None, description="e.g. Software Engineer")
-    url: Optional[AnyUrl] = Field(None, description="e.g. http://facebook.example.com")
-    startDate: Optional[date] = None
-    endDate: Optional[date] = None
-    summary: Optional[str] = Field(
-        None, description="Give an overview of your responsibilities at the company"
-    )
-    highlights: Optional[list[str]] = Field(
-        None, description="Specify multiple accomplishments"
-    )
+    name: t.Annotated[t.Optional[str], Field(description="e.g. Facebook")] = None
+    location: t.Annotated[t.Optional[str], Field(description="e.g. Menlo Park, CA")] = (
+        None
+    )
+    description: t.Annotated[
+        t.Optional[str], Field(description="e.g. Social Media Company")
+    ] = None
+    position: t.Annotated[
+        t.Optional[str], Field(description="e.g. Software Engineer")
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl], Field(description="e.g. http://facebook.example.com")
+    ] = None
+    startDate: t.Optional[datetime.date] = None
+    endDate: t.Optional[datetime.date] = None
+    summary: t.Annotated[
+        t.Optional[str],
+        Field(description="Give an overview of your responsibilities at the company"),
+    ] = None
+    highlights: t.Annotated[
+        t.Optional[list[str]], Field(description="Specify multiple accomplishments")
+    ] = None
 
 
 class VolunteerItem(BaseModel):
     """Modelling a JSON resume volunteer item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L150-L191"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L150-L191
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    organization: Optional[str] = Field(None, description="e.g. Facebook")
-    position: Optional[str] = Field(None, description="e.g. Software Engineer")
-    url: Optional[AnyUrl] = Field(None, description="e.g. http://facebook.example.com")
-    startDate: Optional[date] = None
-    endDate: Optional[date] = None
-    summary: Optional[str] = Field(
-        None, description="Give an overview of your responsibilities at the company"
-    )
-    highlights: Optional[list[str]] = Field(
-        None, description="Specify accomplishments and achievements"
+    organization: t.Annotated[t.Optional[str], Field(description="e.g. Facebook")] = (
+        None
     )
+    position: t.Annotated[
+        t.Optional[str], Field(description="e.g. Software Engineer")
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl], Field(description="e.g. http://facebook.example.com")
+    ] = None
+    startDate: t.Optional[datetime.date] = None
+    endDate: t.Optional[datetime.date] = None
+    summary: t.Annotated[
+        t.Optional[str],
+        Field(description="Give an overview of your responsibilities at the company"),
+    ] = None
+    highlights: t.Annotated[
+        t.Optional[list[str]],
+        Field(description="Specify accomplishments and achievements"),
+    ] = None
 
 
 class EducationItem(BaseModel):
     """Modelling a JSON resume education item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L192-L237"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L192-L237
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    institution: Optional[str] = Field(
-        None, description="e.g. Massachusetts Institute of Technology"
-    )
-    url: Optional[AnyUrl] = Field(None, description="e.g. http://facebook.example.com")
-    area: Optional[str] = Field(None, description="e.g. Arts")
-    studyType: Optional[str] = Field(None, description="e.g. Bachelor")
-    startDate: Optional[date] = None
-    endDate: Optional[date] = None
-    score: Optional[str] = Field(None, description="grade point average, e.g. 3.67/4.0")
-    courses: Optional[list[str]] = Field(
-        None, description="List notable courses/subjects"
-    )
+    institution: t.Annotated[
+        t.Optional[str], Field(description="e.g. Massachusetts Institute of Technology")
+    ] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl], Field(description="e.g. http://facebook.example.com")
+    ] = None
+    area: t.Annotated[t.Optional[str], Field(description="e.g. Arts")] = None
+    studyType: t.Annotated[t.Optional[str], Field(description="e.g. Bachelor")] = None
+    startDate: t.Optional[datetime.date] = None
+    endDate: t.Optional[datetime.date] = None
+    score: t.Annotated[
+        t.Optional[str], Field(description="grade point average, e.g. 3.67/4.0")
+    ] = None
+    courses: t.Annotated[
+        t.Optional[list[str]], Field(description="List notable courses/subjects")
+    ] = None
 
 
 class Award(BaseModel):
     """Modelling a JSON resume award item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L238-L263"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L238-L263
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    title: Optional[str] = Field(
-        None, description="e.g. One of the 100 greatest minds of the century"
-    )
-    date: Optional[date] = None
-    awarder: Optional[str] = Field(None, description="e.g. Time Magazine")
-    summary: Optional[str] = Field(
-        None, description="e.g. Received for my work with Quantum Physics"
-    )
+    title: t.Annotated[
+        t.Optional[str],
+        Field(description="e.g. One of the 100 greatest minds of the century"),
+    ] = None
+    date: datetime.date | None = None
+    awarder: t.Annotated[t.Optional[str], Field(description="e.g. Time Magazine")] = (
+        None
+    )
+    summary: t.Annotated[
+        t.Optional[str],
+        Field(description="e.g. Received for my work with Quantum Physics"),
+    ] = None
 
 
 class Publication(BaseModel):
     """Modelling a JSON resume publication item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L293-L323"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L293-L323
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. The World Wide Web")
-    publisher: Optional[str] = Field(None, description="e.g. IEEE, Computer Magazine")
-    releaseDate: Optional[date] = None
-    url: Optional[AnyUrl] = Field(
-        None,
-        description="e.g. http://www.computer.org.example.com/csdl/mags/co/1996/10/rx069-abs.html",
-    )
-    summary: Optional[str] = Field(
-        None,
-        description="Short summary of publication. e.g. Discussion of the World Wide Web, HTTP, HTML.",
+    name: t.Annotated[t.Optional[str], Field(description="e.g. The World Wide Web")] = (
+        None
     )
+    publisher: t.Annotated[
+        t.Optional[str], Field(description="e.g. IEEE, Computer Magazine")
+    ] = None
+    releaseDate: t.Optional[datetime.date] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(
+            description="e.g. http://www.computer.org.example.com/csdl/mags/co/1996/10/rx069-abs.html",
+        ),
+    ] = None
+    summary: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="Short summary of publication. e.g. Discussion of the World Wide Web, HTTP, HTML.",
+        ),
+    ] = None
 
 
 class Project(BaseModel):
     """Modelling a JSON resume project item.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L412-L476"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json#L412-L476
+    """
 
-    class Config:
-        extra = Extra.allow
+    model_config = ConfigDict(extra="allow")
 
-    name: Optional[str] = Field(None, description="e.g. The World Wide Web")
-    description: Optional[str] = Field(
-        None, description="Short summary of project. e.g. Collated works of 2017."
-    )
-    highlights: Optional[list[str]] = Field(
-        None, description="Specify multiple features"
-    )
-    keywords: Optional[list[str]] = Field(
-        None, description="Specify special elements involved"
-    )
-    startDate: Optional[date] = None
-    endDate: Optional[date] = None
-    url: Optional[AnyUrl] = Field(
-        None,
-        description="e.g. http://www.computer.org/csdl/mags/co/1996/10/rx069-abs.html",
-    )
-    roles: Optional[list[str]] = Field(
-        None, description="Specify your role on this project or in company"
-    )
-    entity: Optional[str] = Field(
-        None,
-        description="Specify the relevant company/entity affiliations e.g. 'greenpeace', 'corporationXYZ'",
-    )
-    type: Optional[str] = Field(
-        None,
-        description=" e.g. 'volunteering', 'presentation', 'talk', 'application', 'conference'",
+    name: t.Annotated[t.Optional[str], Field(description="e.g. The World Wide Web")] = (
+        None
     )
+    description: t.Annotated[
+        t.Optional[str],
+        Field(description="Short summary of project. e.g. Collated works of 2017."),
+    ] = None
+    highlights: t.Annotated[
+        t.Optional[list[str]], Field(description="Specify multiple features")
+    ] = None
+    keywords: t.Annotated[
+        t.Optional[list[str]], Field(description="Specify special elements involved")
+    ] = None
+    startDate: t.Optional[datetime.date] = None
+    endDate: t.Optional[datetime.date] = None
+    url: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(
+            description="e.g. http://www.computer.org/csdl/mags/co/1996/10/rx069-abs.html",
+        ),
+    ] = None
+    roles: t.Annotated[
+        t.Optional[list[str]],
+        Field(description="Specify your role on this project or in company"),
+    ] = None
+    entity: t.Annotated[
+        t.Optional[str],
+        Field(
+            description="Specify the relevant company/entity affiliations e.g. 'greenpeace', 'corporationXYZ'",
+        ),
+    ] = None
+    type: t.Annotated[
+        t.Optional[str],
+        Field(
+            description=" e.g. 'volunteering', 'presentation', 'talk', 'application', 'conference'",
+        ),
+    ] = None
 
 
 class ResumeSchema(BaseModel):
     """Modelling a complete JSON resume schema.
 
-    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json"""
+    See: https://github.com/alexpovel/resume-schema/blob/6e3244639cebfa89e66ee60d47c665a96e01a811/schema.json
+    """
 
-    class Config:
-        extra = Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
-    schema_: Optional[AnyUrl] = Field(
-        None,
-        alias="$schema",
-        description="link to the version of the schema that can validate the resume",
-    )
-    basics: Optional[Basics] = None
-    work: Optional[list[WorkItem]] = None
-    volunteer: Optional[list[VolunteerItem]] = None
-    education: Optional[list[EducationItem]] = None
-    awards: Optional[list[Award]] = Field(
-        None,
-        description="Specify any awards you have received throughout your professional career",
-    )
-    certificates: Optional[list[Certificate]] = Field(
-        None,
-        description="Specify any certificates you have received throughout your professional career",
-    )
-    publications: Optional[list[Publication]] = Field(
-        None, description="Specify your publications through your career"
-    )
-    skills: Optional[list[Skill]] = Field(
-        None, description="List out your professional skill-set"
-    )
-    languages: Optional[list[Language]] = Field(
-        None, description="List any other languages you speak"
-    )
-    interests: Optional[list[Interest]] = None
-    references: Optional[list[Reference]] = Field(
-        None, description="List references you have received"
-    )
-    projects: Optional[list[Project]] = Field(
-        None, description="Specify career projects"
-    )
-    meta: Meta = Field(
-        Meta(),
-        description="The schema version and any other tooling configuration lives here",
-    )
+    schema_: t.Annotated[
+        t.Optional[AnyUrl],
+        Field(
+            alias="$schema",
+            description="link to the version of the schema that can validate the resume",
+        ),
+    ] = None
+    basics: t.Optional[Basics] = None
+    work: t.Optional[list[WorkItem]] = None
+    volunteer: t.Optional[list[VolunteerItem]] = None
+    education: t.Optional[list[EducationItem]] = None
+    awards: t.Annotated[
+        t.Optional[list[Award]],
+        Field(
+            description="Specify any awards you have received throughout your professional career",
+        ),
+    ] = None
+    certificates: t.Annotated[
+        t.Optional[list[Certificate]],
+        Field(
+            description="Specify any certificates you have received throughout your professional career",
+        ),
+    ] = None
+    publications: t.Annotated[
+        t.Optional[list[Publication]],
+        Field(description="Specify your publications through your career"),
+    ] = None
+    skills: t.Annotated[
+        t.Optional[list[Skill]],
+        Field(description="List out your professional skill-set"),
+    ] = None
+    languages: t.Annotated[
+        t.Optional[list[Language]],
+        Field(description="List any other languages you speak"),
+    ] = None
+    interests: t.Optional[list[Interest]] = None
+    references: t.Annotated[
+        t.Optional[list[Reference]],
+        Field(description="List references you have received"),
+    ] = None
+    projects: t.Annotated[
+        t.Optional[list[Project]], Field(description="Specify career projects")
+    ] = None
+    meta: t.Annotated[
+        Meta,
+        Field(
+            description="The schema version and any other tooling configuration lives here",
+        ),
+    ] = Meta()
 
 
-ResumeItem = Union[
+ResumeItem = t.Union[
     Award,
     Basics,
     Certificate,
     EducationItem,
     Interest,
     Language,
     Location,
```

### Comparing `ancv-1.3.1/ancv/data/showcase.resume.json` & `ancv-1.4.0/ancv/data/showcase.resume.json`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/ancv/data/validation.py` & `ancv-1.4.0/ancv/data/validation.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/ancv/timing.py` & `ancv-1.4.0/ancv/timing.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/ancv/visualization/templates.py` & `ancv-1.4.0/ancv/visualization/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,21 @@
             model: The pydantic resume model to create the template from.
 
         Returns:
             A template instance.
         """
 
         if (config := model.meta.config) is None:
-            config = TemplateConfig()
+            config = TemplateConfig(
+                template=None,
+                theme=None,
+                language=None,
+                ascii_only=None,
+                dec31_as_year=None,
+            )
 
         if (theme_name := config.theme) is None:
             theme_name = "lollipop"
         try:
             theme = THEMES[theme_name]
         except KeyError as e:
             raise ResumeConfigError(f"Unknown theme: {theme_name}") from e
@@ -450,15 +456,17 @@
         if name := item.name:
             yield from self._section(name)
 
         if label := item.label:
             yield Align.center(Text(label, style=self.theme.emphasis.strong))
             yield NewLine()
 
-        contact_items = [item for item in (item.email, item.phone, item.url) if item]
+        contact_items = [
+            str(item) for item in (item.email, item.phone, item.url) if item
+        ]
         if contact_items:
             yield Align.center(
                 Text(
                     f" {self.theme.sep} ".join(contact_items),
                     style=self.theme.emphasis.weak,
                 )
             )
@@ -539,15 +547,15 @@
             yield indent(
                 Text.assemble(
                     (location or "", self.theme.emphasis.weak),
                     (
                         f" {self.theme.sep} " if (location and url) else "",
                         self.theme.emphasis.weak,
                     ),
-                    (url or "", self.theme.emphasis.weak),
+                    ("" if url is None else str(url), self.theme.emphasis.weak),
                 )
             )
 
     @format.register
     def _(self, item: Skill) -> RenderableGenerator:
         """Formats aka renders a `Skill` item."""
 
@@ -596,15 +604,15 @@
                             style=self.theme.emphasis.medium,
                         )
                     )
                 )
 
         if url := item.url:
             yield NewLine()
-            yield indent(Text(url, self.theme.emphasis.weak))
+            yield indent(Text(str(url), self.theme.emphasis.weak))
 
     @format.register
     def _(self, item: EducationItem) -> RenderableGenerator:
         """Formats aka renders a `EducationItem` item."""
 
         yield from horizontal_fill(
             Text.assemble(
@@ -643,15 +651,15 @@
                             style=self.theme.emphasis.weak,
                         )
                     )
                 )
 
         if url := item.url:
             yield NewLine()
-            yield indent(Text(url, style=self.theme.emphasis.weak))
+            yield indent(Text(str(url), style=self.theme.emphasis.weak))
 
     @format.register
     def _(self, item: Award) -> RenderableGenerator:
         """Formats aka renders a `Award` item."""
 
         yield from horizontal_fill(
             Text.assemble(
@@ -683,15 +691,15 @@
                 self._format_date(item.date) if item.date else "",
                 style=self.theme.emphasis.weak,
             ),
         )
 
         if url := item.url:
             yield NewLine()
-            yield indent(Text(url, style=self.theme.emphasis.weak))
+            yield indent(Text(str(url), style=self.theme.emphasis.weak))
 
     @format.register
     def _(self, item: Publication) -> RenderableGenerator:
         """Formats aka renders a `Publication` item."""
 
         yield from horizontal_fill(
             Text.assemble(
@@ -710,15 +718,15 @@
 
         if summary := item.summary:
             yield NewLine()
             yield indent(Text(summary, style=self.theme.emphasis.medium))
 
         if url := item.url:
             yield NewLine()
-            yield indent(Text(url, style=self.theme.emphasis.weak))
+            yield indent(Text(str(url), style=self.theme.emphasis.weak))
 
     @format.register
     def _(self, item: Language) -> RenderableGenerator:
         """Formats aka renders a `Language` item."""
 
         if language := item.language:
             yield NewLine()
@@ -806,15 +814,17 @@
             yield NewLine()
 
         if keywords := item.keywords:
             yield indent(Text(", ".join(keywords), style=self.theme.emphasis.medium))
             yield NewLine()
 
         footer = join(
-            (item.url, Style()), (item.entity, Style()), separator=self.theme.sep
+            ("" if item.url is None else str(item.url), Style()),
+            (item.entity, Style()),
+            separator=self.theme.sep,
         )
         if footer:
             footer.style = self.theme.emphasis.weak
             yield indent(footer)
             yield NewLine()
 
     def __rich_console__(
```

### Comparing `ancv-1.3.1/ancv/visualization/themes.py` & `ancv-1.4.0/ancv/visualization/themes.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from babel.dates import DateTimePattern, parse_pattern
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 from rich.style import Style
 
 
 class Emphasis(BaseModel):
     """Emphasis styles for different levels of importance.
 
     Using `rich.Style`, each can be styled arbitrarily.
     """
 
     maximum: Style
     strong: Style
     medium: Style
     weak: Style
-
-    class Config:
-        arbitrary_types_allowed = True  # No validator for `Style` available
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class DateFormat(BaseModel):
     """Date formats for different levels of detail.
 
     The `full` format is as detailed as possible, while `year_only` should only contain
     the year. Formats may otherwise be in whatever format you desire (ISO8601,
@@ -30,17 +28,15 @@
     considerably better type safety (`str` is the worst offender in terms of typing) and
     fast failure: at application startup, when a theme is loaded but `parse_pattern` (or
     similar) fails, the program won't launch altogether, instead of failing at runtime.
     """
 
     full: DateTimePattern
     year_only: DateTimePattern
-
-    class Config:
-        arbitrary_types_allowed = True  # No validator for `DateTimePattern`
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class Theme(BaseModel):
     """A theme, containing styles and other formatting options."""
 
     emphasis: Emphasis  # styles for different levels of importance
     bullet: str  # bullet character to use in (unordered) lists
```

### Comparing `ancv-1.3.1/ancv/visualization/translations.py` & `ancv-1.4.0/ancv/visualization/translations.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/ancv/web/client.py` & `ancv-1.4.0/ancv/web/client.py`

 * *Files identical despite different names*

### Comparing `ancv-1.3.1/ancv/web/server.py` & `ancv-1.4.0/ancv/web/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,16 +50,15 @@
     path: Optional[str]
 
 
 class Runnable(ABC):
     """A server object that can be `run`, enabling different server implementations."""
 
     @abstractmethod
-    def run(self, context: ServerContext) -> None:
-        ...
+    def run(self, context: ServerContext) -> None: ...
 
 
 class APIHandler(Runnable):
     """A runnable server for handling dynamic API requests.
 
     This is the core application server powering the API. It is responsible for handling
     requests for the resume of a given user, and returning the appropriate response. It
```

### Comparing `ancv-1.3.1/pyproject.toml` & `ancv-1.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ancv"
-version = "1.3.1"
+version = "1.4.0"
 description = "Renders your (JSON) resume/CV for online & pretty terminal display"
 authors = ["Alex Povel <python@alexpovel.de>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://ancv.io"
 repository = "https://github.com/alexpovel/ancv/"
 classifiers = [
@@ -36,48 +36,48 @@
 "Changelog" = "https://github.com/alexpovel/ancv/blob/main/CHANGELOG.md"
 "Pull Requests" = "https://github.com/alexpovel/ancv/pulls"
 
 [tool.poetry.dependencies]
 # https://stackoverflow.com/a/69608708/11477374:
 python = "^3.10"
 gidgethub = "^5.1.0"
-aiohttp = {extras = ["speedups"], version = "^3.8.1"}
-pydantic = {extras = ["email"], version = "^1.9.1"}
-structlog = ">=21.5,<23.0"
+aiohttp = { extras = ["speedups"], version = "^3.8.1" }
+pydantic = { extras = ["email"], version = "^2.5.3" }
+structlog = ">=21.5,<25.0"
 cachetools = "^5.2.0"
 humanize = "^4.1.0"
 rich = ">=12.4.4,<14.0.0"
-typer = ">=0.6.1,<0.8.0"
+typer = ">=0.6.1,<0.10.0"
 Babel = "^2.10.3"
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-pytest = "^7.1.2"
-datamodel-code-generator = {extras = ["http"], version = "^0.13.0"}
-mypy = "^0.960"
+pytest = ">=7.1.2,<9.0.0"
+datamodel-code-generator = { extras = ["http"], version = ">=0.13,<0.26" }
+mypy = ">=0.960,<1.11"
 types-cachetools = "^5.0.1"
 pydeps = "^1.10.18"
-pytest-cov = "^4.0.0"
+pytest-cov = ">=4,<6"
 pytest-aiohttp = "^1.0.4"
-pytest-rerunfailures = "^10.2"
+pytest-rerunfailures = ">=10.2,<13.0"
 requests = "^2.28.1"
 types-babel = "^2.10.0"
-ruff = ">=0.0.224,<0.0.261"
+ruff = ">=0.3.2,<0.5.0"
+ipython = "^8.14.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ancv = "ancv.__main__:app"
 
 [tool.coverage.run]
 branch = true
 
-[tool.ruff]
+[tool.ruff.lint]
 # `E501` is line length violation
 ignore = ["E501"]
 
 [tool.coverage.report]
 fail_under = 80.0
 
 [tool.datamodel-codegen]
@@ -85,15 +85,18 @@
 
 [tool.mypy]
 mypy_path = "stubs/"
 show_error_codes = true
 strict = true
 namespace_packages = true
 disallow_any_unimported = true
-disallow_any_explicit = true
+# Disable until https://github.com/python/mypy/issues/16454 fixed (inheriting from
+# `Basemodel` gives ancv/visualization/translations.py:4: error: Explicit "Any" is not
+# allowed  [misc])
+disallow_any_explicit = false
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_defs = true
 no_implicit_optional = true
 check_untyped_defs = true
 warn_return_any = true
 warn_unused_ignores = true
```

### Comparing `ancv-1.3.1/PKG-INFO` & `ancv-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancv
-Version: 1.3.1
+Version: 1.4.0
 Summary: Renders your (JSON) resume/CV for online & pretty terminal display
 Home-page: https://ancv.io
 License: MIT
 Author: Alex Povel
 Author-email: python@alexpovel.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,33 +18,32 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: German
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Office/Business
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: Terminals
 Classifier: Topic :: Terminals :: Terminal Emulators/X Terminals
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Typing :: Typed
 Requires-Dist: Babel (>=2.10.3,<3.0.0)
 Requires-Dist: aiohttp[speedups] (>=3.8.1,<4.0.0)
 Requires-Dist: cachetools (>=5.2.0,<6.0.0)
 Requires-Dist: gidgethub (>=5.1.0,<6.0.0)
 Requires-Dist: humanize (>=4.1.0,<5.0.0)
-Requires-Dist: pydantic[email] (>=1.9.1,<2.0.0)
+Requires-Dist: pydantic[email] (>=2.5.3,<3.0.0)
 Requires-Dist: rich (>=12.4.4,<14.0.0)
-Requires-Dist: structlog (>=21.5,<23.0)
-Requires-Dist: typer (>=0.6.1,<0.8.0)
+Requires-Dist: structlog (>=21.5,<25.0)
+Requires-Dist: typer (>=0.6.1,<0.10.0)
 Project-URL: Bug Tracker, https://github.com/alexpovel/ancv/issues/
 Project-URL: Changelog, https://github.com/alexpovel/ancv/blob/main/CHANGELOG.md
 Project-URL: Pull Requests, https://github.com/alexpovel/ancv/pulls
 Project-URL: Repository, https://github.com/alexpovel/ancv/
 Description-Content-Type: text/markdown
 
 # [ancv](https://github.com/alexpovel/ancv)
@@ -61,14 +60,25 @@
    <img src="docs/images/users-venn.svg" alt="users venn diagram">
 </p>
 
 ## Getting started
 
 1. Create your resume according to the [JSON Resume Schema](https://jsonresume.org/schema/) (see also the [schema specification](https://github.com/jsonresume/resume-schema/blob/master/schema.json)) either:
 
+   - use ChatGPT (or another LLM) with the following prompt (you need to fill in the spaces for `[resume]` and `[json_schema]`):
+      ```
+      Resume:[resume]
+
+      JSON Resume Schema:[json_schema]
+
+      Provide JSON data structure of the resume, formatted according to the JSON Resume Schema
+      
+      Output json, no yapping
+      ```
+      Note: for `json_schema` you can just use the example [from here](https://jsonresume.org/schema/)
    - manually (see [the `heyho` sample](./ancv/data/showcase.resume.json) for a possible starting point),
    - exporting from [LinkedIn](https://www.linkedin.com/) using [Joshua Tzucker's LinkedIn exporter](https://joshuatz.com/projects/web-stuff/linkedin-profile-to-json-resume-exporter/) ([repo](https://github.com/joshuatz/linkedin-to-jsonresume))[^1], or
    - exporting from one of the platforms advertised as offering [JSON resume integration](https://jsonresume.org/schema/).
 2. [Create a **public** gist](https://gist.github.com/) named `resume.json` with your resume contents.
 3. You're now the proud owner of an ancv.
    Time to try it out.
```

