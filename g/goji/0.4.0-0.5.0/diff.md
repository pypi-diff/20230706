# Comparing `tmp/goji-0.4.0.tar.gz` & `tmp/goji-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goji-0.4.0.tar", max compression
+gzip compressed data, was "goji-0.5.0.tar", max compression
```

## Comparing `goji-0.4.0.tar` & `goji-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1298 2020-08-22 12:48:44.912141 goji-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2020-08-22 12:48:44.912141 goji-0.4.0/goji/__init__.py
--rw-r--r--   0        0        0       37 2020-08-22 12:48:44.912141 goji-0.4.0/goji/__main__.py
--rw-r--r--   0        0        0     1607 2021-03-27 15:02:33.016900 goji-0.4.0/goji/auth.py
--rw-r--r--   0        0        0     7162 2021-03-28 11:37:46.536206 goji-0.4.0/goji/client.py
--rw-r--r--   0        0        0    12411 2021-03-28 11:36:30.699274 goji-0.4.0/goji/commands.py
--rw-r--r--   0        0        0     2060 2021-03-27 19:11:01.238473 goji-0.4.0/goji/config.py
--rw-r--r--   0        0        0     6126 2021-03-27 19:17:31.900193 goji-0.4.0/goji/models.py
--rw-r--r--   0        0        0      711 2021-03-27 14:57:13.469169 goji-0.4.0/goji/utils.py
--rw-r--r--   0        0        0      517 2021-03-28 11:38:03.072930 goji-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      819 2021-03-28 11:38:26.465600 goji-0.4.0/setup.py
--rw-r--r--   0        0        0      686 2021-03-28 11:38:26.465753 goji-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1298 2023-07-06 20:30:02.834858 goji-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-06 20:30:02.834858 goji-0.5.0/goji/__init__.py
+-rw-r--r--   0        0        0       37 2023-07-06 20:30:02.834858 goji-0.5.0/goji/__main__.py
+-rw-r--r--   0        0        0      878 2023-07-06 20:30:02.834858 goji-0.5.0/goji/ansi.py
+-rw-r--r--   0        0        0     1607 2023-07-06 20:30:02.834858 goji-0.5.0/goji/auth.py
+-rw-r--r--   0        0        0     7879 2023-07-06 20:30:02.834858 goji-0.5.0/goji/client.py
+-rw-r--r--   0        0        0    13421 2023-07-06 20:30:02.834858 goji-0.5.0/goji/commands.py
+-rw-r--r--   0        0        0     2135 2023-07-06 20:30:02.834858 goji-0.5.0/goji/config.py
+-rw-r--r--   0        0        0     8978 2023-07-06 20:30:02.834858 goji-0.5.0/goji/models.py
+-rw-r--r--   0        0        0     3143 2023-07-06 20:30:02.838858 goji-0.5.0/goji/text_parser.py
+-rw-r--r--   0        0        0      711 2023-07-06 20:30:02.838858 goji-0.5.0/goji/utils.py
+-rw-r--r--   0        0        0      517 2023-07-06 20:32:35.017890 goji-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      788 1970-01-01 00:00:00.000000 goji-0.5.0/PKG-INFO
```

### Comparing `goji-0.4.0/LICENSE` & `goji-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goji-0.4.0/goji/auth.py` & `goji-0.5.0/goji/auth.py`

 * *Files identical despite different names*

### Comparing `goji-0.4.0/goji/client.py` & `goji-0.5.0/goji/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,24 @@
 from typing import Any, List, Optional
 
 import click
 import requests
 from requests.auth import AuthBase, HTTPBasicAuth
 from requests.compat import urljoin
 
-from goji.models import Attachment, Comment, Issue, Sprint, Transition, User
+from goji.models import (
+    Attachment,
+    Comment,
+    Comments,
+    Issue,
+    SearchResults,
+    Sprint,
+    Transition,
+    UserDetails,
+)
 
 
 class JIRAException(click.ClickException):
     def __init__(self, error_messages: List[str], errors):
         self.error_messages = error_messages
         self.errors = errors
 
@@ -39,15 +48,18 @@
     def __call__(self, request):
         if 'Cookie' in request.headers:
             # Prevent authorization headers when cookies are present as it
             # causes silent authentication errors on the JIRA instance if
             # cookies are used and invalid authorization headers are sent
             # (although request succeeds)
 
-            if 'atlassian.xsrf.token' in request.headers['Cookie'] and len(request.headers['Cookie'].split('=')) == 2:
+            if (
+                'atlassian.xsrf.token' in request.headers['Cookie']
+                and len(request.headers['Cookie'].split('=')) == 2
+            ):
                 # continue if the cookie is ONLY the xsrf token
                 # check is very naive as to not get into cookie parsing
                 # ensure that we check only for key=value (once) being xsrf
                 return super(JIRAAuth, self).__call__(request)
 
             return request
 
@@ -123,26 +135,28 @@
     @property
     def username(self) -> Optional[str]:
         if self.session.auth and isinstance(self.session.auth, JIRAAuth):
             return self.session.auth.username
 
         return None
 
-    def get_user(self) -> Optional[User]:
+    def get_user(self) -> Optional[UserDetails]:
         response = self.get('myself', allow_redirects=False)
         response.raise_for_status()
-        return User.from_json(response.json())
+        return UserDetails.from_json(response.json())
 
     def get_issue(self, issue_key: str) -> Issue:
         response = self.get('issue/%s' % issue_key)
         response.raise_for_status()
         return Issue.from_json(response.json())
 
     def get_issue_transitions(self, issue_key: str) -> List[Transition]:
-        response = self.get('issue/%s/transitions' % issue_key)
+        response = self.get(
+            'issue/%s/transitions' % issue_key, params={'expand': 'transitions.fields'}
+        )
         response.raise_for_status()
         return list(map(Transition.from_json, response.json()['transitions']))
 
     def change_status(self, issue_key: str, transition_id: str) -> None:
         data = {'transition': {'id': transition_id}}
         self.post('issue/%s/transitions' % issue_key, data)
 
@@ -172,18 +186,39 @@
         response = self.put('issue/%s/assignee' % issue_key, {'name': name})
         response.raise_for_status()
 
     def comment(self, issue_key: str, comment: str) -> Comment:
         response = self.post('issue/%s/comment' % issue_key, {'body': comment})
         return Comment.from_json(response.json())
 
-    def search(self, query: str) -> List[Issue]:
-        response = self.post('search', {'jql': query})
+    def comments(self, issue_key: str) -> Comments:
+        response = self.get('issue/%s/comment' % issue_key)
+        return Comments.from_json(response.json())
+
+    def search(
+        self,
+        query: str,
+        fields: Optional[List[str]] = None,
+        max_results: Optional[int] = None,
+        start_at: Optional[int] = None,
+    ) -> SearchResults:
+        body = {'jql': query}
+
+        if start_at:
+            body['startAt'] = start_at
+
+        if max_results is not None:
+            body['maxResults'] = max_results
+
+        if fields:
+            body['fields'] = fields
+
+        response = self.post('search', body)
         response.raise_for_status()
-        return list(map(Issue.from_json, response.json()['issues']))
+        return SearchResults.from_json(response.json())
 
     def create_sprint(
         self,
         board_id: int,
         name: str,
         start_date: Optional[datetime.datetime] = None,
         end_date: Optional[datetime.datetime] = None,
```

### Comparing `goji-0.4.0/goji/commands.py` & `goji-0.5.0/goji/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import sys
+from os import isatty
+from string import Formatter
 from typing import Optional
 
 import click
 import requests
 from requests.compat import urljoin
 
 from goji.auth import get_credentials, set_credentials
@@ -75,20 +77,22 @@
         client.save_cookies()
 
     if response.status_code == 401:
         raise click.ClickException('Incorrect credentials. Try `goji login`.')
 
 
 @click.group()
-@click.option('--profile', default='default')
+@click.option('--profile', envvar='GOJI_PROFILE', default='default')
 @click.option('--base-url', envvar='GOJI_BASE_URL')
 @click.option('--email', envvar='GOJI_EMAIL', default=None)
 @click.option('--password', envvar='GOJI_PASSWORD', default=None)
 @click.pass_context
-def cli(ctx, profile: str, base_url: str, email: Optional[str], password: Optional[str]) -> None:
+def cli(
+    ctx, profile: str, base_url: str, email: Optional[str], password: Optional[str]
+) -> None:
     config = Configuration.load()
     p = config.profiles.get(profile.lower())
 
     if p:
         if not base_url:
             base_url = p.url
 
@@ -223,14 +227,29 @@
             return
 
     transition = transitions[index]
     client.change_status(issue_key, transition.id)
     click.echo('Okay, the status for {} is now "{}".'.format(issue_key, transition))
 
 
+@click.argument('issue_key')
+@cli.command()
+@click.pass_obj
+def comments(client: JIRAClient, issue_key: str) -> None:
+    comments = client.comments(issue_key)
+
+    for index, comment in enumerate(comments.comments):
+        if index != 0:
+            print()
+
+        print('=' * 60)
+        print(comment.author)
+        print(comment)
+
+
 @click.option('--message', '-m', help='Message to comment.')
 @click.argument('issue_key')
 @cli.command()
 @click.pass_obj
 def comment(client: JIRAClient, message: Optional[str], issue_key: str) -> None:
     """Comment on an issue"""
 
@@ -361,33 +380,47 @@
 
     client = JIRAClient(base_url, auth=(email, password))
     check_login(client)
     set_credentials(base_url, email, password)
 
 
 @click.argument('query')
+@click.option('--limit', type=int)
 @click.option('--format', default='{key} {summary}')
+@click.option('--count', is_flag=True, help='Return the count of matched issues')
 @cli.command()
 @click.pass_obj
-def search(client: JIRAClient, format: str, query: str) -> None:
+def search(client: JIRAClient, count: bool, format: str, limit: Optional[int], query: str) -> None:
     """Search issues using JQL"""
 
-    issues = client.search(query)
+    if count:
+        results = client.search(query, fields=['key'], max_results=1)
+        print(results.total)
+        return
+
+    formatter = Formatter()
+    fields = [v[1] for v in formatter.parse(format)]
 
-    for issue in issues:
+    results = client.search(query, fields=fields, max_results=limit)
+
+    for issue in results.issues:
         format_kwargs = dict(
             key=issue.key,
             summary=issue.summary,
             description=issue.description,
             creator=issue.creator,
             assignee=issue.assignee,
             status=issue.status,
             resolution=issue.resolution,
         )
 
+        if isatty(sys.stdout.fileno()):
+            url = urljoin(client.base_url, 'browse/%s' % issue.key)
+            format_kwargs['key'] = f'\033]8;;{url}\a{issue.key}\033]8;;\a'
+
         format_kwargs.update(issue.customfields)
 
         click.echo(format.replace('\\n', '\n').format(**format_kwargs))
 
 
 @cli.group('sprint')
 def sprint() -> None:
```

### Comparing `goji-0.4.0/goji/config.py` & `goji-0.5.0/goji/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,41 +2,38 @@
 from typing import Dict, Optional
 
 import click
 import toml
 from jsonschema import ValidationError, validate
 
 SCHEMA = {
-  'type': 'object',
-  'properties': {
-    'profile': { '$ref': '#/definitions/Profiles' },
-  },
-  'additionalProperties': False,
-  'definitions': {
-    'Profile': {
-      'type': 'object',
-      'properties': {
-        'url': {
-          'type': 'string',
+    'type': 'object',
+    'properties': {
+        'profile': {'$ref': '#/definitions/Profiles'},
+    },
+    'additionalProperties': False,
+    'definitions': {
+        'Profile': {
+            'type': 'object',
+            'properties': {
+                'url': {
+                    'type': 'string',
+                },
+                'email': {
+                    'type': 'string',
+                },
+            },
+            'required': ['url'],
+            'additionalProperties': False,
         },
-        'email': {
-          'type': 'string',
+        'Profiles': {
+            'type': 'object',
+            'additionalProperties': {'$ref': '#/definitions/Profile'},
         },
-      },
-      'required': ['url'],
-      'additionalProperties': False,
-    },
-
-    'Profiles': {
-      'type': 'object',
-      'additionalProperties': {
-        '$ref': '#/definitions/Profile'
-      },
     },
-  },
 }
 
 
 class Profile:
     @classmethod
     def from_dict(cls, data) -> 'Profile':
         return cls(data['url'], data.get('email'))
@@ -60,17 +57,15 @@
         with open(path) as fp:
             data = toml.load(fp)
 
         try:
             validate(instance=data, schema=SCHEMA)
         except ValidationError as exception:
             message = 'Invalid config in {}, at path /{}, {}'.format(
-                path,
-                '/'.join(exception.path),
-                exception.message
+                path, '/'.join(exception.path), exception.message
             )
             raise click.ClickException(message)
 
         profiles: Dict[str, Profile] = {}
         for (profile, data) in data.get('profile', {}).items():
             if profile.lower() in profiles:
                 raise click.ClickException(f'Profile {profile} defined more than once')
```

### Comparing `goji-0.4.0/goji/models.py` & `goji-0.5.0/goji/models.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from typing import Any, Dict, List, Optional
 
 
 class Model(object):
     pass
 
 
-class User(Model):
+class UserDetails(Model):
     @classmethod
-    def from_json(cls, json: Dict[str, Any]) -> Optional['User']:
+    def from_json(cls, json: Dict[str, Any]) -> Optional['UserDetails']:
         if json:
-            return cls(json.get('name') or '', json['displayName'], json.get('emailAddress'))
+            return cls(
+                json.get('name') or '', json['displayName'], json.get('emailAddress')
+            )
 
         return None
 
     def __init__(self, username: Optional[str], name: str, email: Optional[str] = None):
         self.username = username
         self.name = name
         self.email = email
@@ -25,19 +27,20 @@
 class Issue(Model):
     @classmethod
     def from_json(cls, json: Dict[str, Any]) -> 'Issue':
         issue = cls(json['key'])
 
         if 'fields' in json:
             fields = json['fields']
-            issue.summary = fields['summary'].rstrip()
+            issue.summary = fields.get('summary', '').rstrip()
             issue.description = fields.get('description')
-            issue.creator = User.from_json(fields.get('creator'))
-            issue.assignee = User.from_json(fields.get('assignee'))
-            issue.status = Status.from_json(fields['status'])
+            issue.creator = UserDetails.from_json(fields.get('creator'))
+            issue.assignee = UserDetails.from_json(fields.get('assignee'))
+            if 'status' in fields:
+                issue.status = StatusDetails.from_json(fields['status'])
 
             resolution = fields.get('resolution', None)
             if resolution:
                 issue.resolution = Resolution.from_json(resolution)
             else:
                 issue.resolution = None
 
@@ -56,15 +59,15 @@
 
     def __init__(self, key: str):
         self.key = key
         self.summary = None
         self.description = None
         self.creator: Optional[User] = None
         self.assignee: Optional[User] = None
-        self.status: Optional['Status'] = None
+        self.status: Optional['StatusDetails'] = None
         self.resolution: Optional[Resolution] = None
         self.links: List['IssueLink'] = []
         self.customfields: Dict[str, Any] = {}
 
     def __str__(self):
         return self.key
 
@@ -115,44 +118,87 @@
             raise Exception('IssueLink is missing outward or inward issue')
 
         return '{direction}: {issue.key} ({issue.status})'.format(
             direction=direction, issue=issue
         )
 
 
+class TransitionField(Model):
+    @classmethod
+    def from_json(cls, json: Dict[str, Any]) -> 'Transition':
+        return cls(
+            id=json['fieldId'], name=json.get('name'), is_required=json.get('required')
+        )
+
+    def __init__(self, id: str, name: str, is_required: bool):
+        self.id = id
+        self.name = name
+        self.is_required = is_required
+
+    def __str__(self) -> str:
+        return self.name
+
+
 class Transition(Model):
     @classmethod
     def from_json(cls, json: Dict[str, Any]) -> 'Transition':
-        return cls(json['id'], json['name'])
+        fields = list(map(TransitionField.from_json, json.get('fields', {}).values()))
+        return cls(json['id'], json['name'], fields)
 
-    def __init__(self, identifier: str, name: str):
+    def __init__(
+        self, identifier: str, name: str, fields: Optional[List[TransitionField]] = None
+    ):
         self.id = identifier
         self.name = name
+        self.fields = fields
 
     def __str__(self) -> str:
         return self.name
 
 
 class Comment(Model):
     @classmethod
     def from_json(cls, json: Dict[str, Any]) -> 'Comment':
         comment = cls(json['id'], json['body'])
 
         if 'author' in json:
-            comment.author = User.from_json(json['author'])
+            comment.author = UserDetails.from_json(json['author'])
 
         return comment
 
-    def __init__(self, identifier: str, message: str):
+    def __init__(self, identifier: str, body: str):
         self.id = identifier
-        self.message = message
-        self.author: Optional[User] = None
+        self.body = body
+        self.author: Optional[UserDetails] = None
 
     def __str__(self) -> str:
-        return self.message
+        return self.body
+
+
+class Comments(Model):
+    @classmethod
+    def from_json(cls, json: Dict[str, Any]) -> 'Comments':
+        return cls(
+            comments=list(map(Comment.from_json, json['comments'])),
+            start_at=json['startAt'],
+            max_results=json['maxResults'],
+            total=json['total'],
+        )
+
+    def __init__(
+        self,
+        comments: List[Comment],
+        start_at: int,
+        max_results: int,
+        total: int,
+    ):
+        self.comments = comments
+        self.start_at = start_at
+        self.max_results = max_results
+        self.total = total
 
 
 class Sprint(Model):
     @classmethod
     def from_json(cls, json: Dict[str, Any]) -> 'Sprint':
         return cls(json['id'], json['name'], json['state'])
 
@@ -161,23 +207,35 @@
         self.name = name
         self.state = state
 
     def __str__(self) -> str:
         return self.name
 
 
-class Status(Model):
+class StatusDetails(Model):
     @classmethod
-    def from_json(cls, json: Dict[str, Any]) -> 'Status':
-        return cls(json['id'], json['name'], json.get('description', None))
+    def from_json(cls, json: Dict[str, Any]) -> 'StatusDetails':
+        return cls(
+            json['id'],
+            json['name'],
+            json.get('description', None),
+            StatusCategory.from_json(json['statusCategory']),
+        )
 
-    def __init__(self, identifier: str, name: str, description: Optional[str] = None):
+    def __init__(
+        self,
+        identifier: str,
+        name: str,
+        description: Optional[str],
+        status_category: 'StatusCategory',
+    ):
         self.id = identifier
         self.name = name
         self.description = description
+        self.status_category = status_category
 
     def __str__(self) -> str:
         return self.name
 
 
 class Resolution(Model):
     @classmethod
@@ -192,19 +250,52 @@
     def __str__(self) -> str:
         return self.name
 
 
 class Attachment(Model):
     @classmethod
     def from_json(cls, json: Dict[str, Any]) -> 'Attachment':
-        return cls(json.get('filename'), int(json['size']))
+        return cls(
+            json.get('filename'),
+            int(json['size']),
+            UserDetails.from_json(json['author']),
+        )
 
-    def __init__(self, filename: Optional[str], size: int):
+    def __init__(self, filename: Optional[str], size: int, author: UserDetails):
         self.filename = filename
         self.size = size
+        self.author = author
+
+
+class SearchResults(Model):
+    # https://docs.atlassian.com/software/jira/docs/api/REST/8.22.6/#search-search
+
+    @classmethod
+    def from_json(cls, json: Dict[str, Any]) -> 'SearchResults':
+        return cls(
+            issues=list(map(Issue.from_json, json['issues'])),
+            expand=json['expand'].split(','),
+            start_at=json['startAt'],
+            max_results=json['maxResults'],
+            total=json['total'],
+        )
+
+    def __init__(
+        self,
+        issues: List[Issue],
+        expand: List[str],
+        start_at: int,
+        max_results: int,
+        total: int,
+    ):
+        self.issues = issues
+        self.expand = expand
+        self.start_at = start_at
+        self.max_results = max_results
+        self.total = total
 
 
 """
 class IssueType(object):
     id
     description
     name
@@ -213,7 +304,21 @@
     issue type
     creator
     assignee
     url
     summary
     description
 """
+
+
+class StatusCategory(Model):
+    @classmethod
+    def from_json(cls, json: Dict[str, Any]) -> 'StatusCategory':
+        return cls(json['id'], json['key'], json['name'])
+
+    def __init__(self, identifier: str, key: str, name: str):
+        self.id = identifier
+        self.key = key
+        self.name = name
+
+    def __str__(self) -> str:
+        return self.name
```

### Comparing `goji-0.4.0/goji/utils.py` & `goji-0.5.0/goji/utils.py`

 * *Files identical despite different names*

### Comparing `goji-0.4.0/pyproject.toml` & `goji-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "goji"
-version = "0.4.0"
+version = "0.5.0"
 description = "Command line JIRA client"
 authors = ["Kyle Fuller <kyle@fuller.li>"]
 license = "BSD"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 click = "^7.1.2"
```

### Comparing `goji-0.4.0/PKG-INFO` & `goji-0.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: goji
-Version: 0.4.0
+Version: 0.5.0
 Summary: Command line JIRA client
 License: BSD
 Author: Kyle Fuller
 Author-email: kyle@fuller.li
 Requires-Python: >=3.6,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
 Requires-Dist: requests-html (>=0.10.0,<0.11.0)
 Requires-Dist: requests[socks] (>=2.25.1,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
```

