# Comparing `tmp/gitlabx-0.3.0-py3-none-any.whl.zip` & `tmp/gitlabx-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 12446 bytes, number of entries: 22
+Zip file size: 12520 bytes, number of entries: 22
 -rwxrwxrwx  2.0 unx        0 b- defN 23-Jun-28 23:28 gitlabx/__init__.py
 -rwxrwxrwx  2.0 unx      380 b- defN 23-Jun-29 10:14 gitlabx/abstract.py
 -rwxrwxrwx  2.0 unx      950 b- defN 23-Jun-29 23:39 gitlabx/branches.py
--rwxrwxrwx  2.0 unx     1241 b- defN 23-Jul-02 23:24 gitlabx/commits.py
+-rwxrwxrwx  2.0 unx     2105 b- defN 23-Jul-06 19:28 gitlabx/commits.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/deployments.py
 -rwxrwxrwx  2.0 unx      902 b- defN 23-Jun-29 11:24 gitlabx/events.py
 -rwxrwxrwx  2.0 unx     2795 b- defN 23-Jul-02 23:47 gitlabx/factories.py
 -rwxrwxrwx  2.0 unx      944 b- defN 23-Jun-29 11:24 gitlabx/issues.py
 -rwxrwxrwx  2.0 unx      984 b- defN 23-Jul-02 23:37 gitlabx/jobs.py
 -rwxrwxrwx  2.0 unx      974 b- defN 23-Jul-02 22:40 gitlabx/member.py
 -rwxrwxrwx  2.0 unx     1204 b- defN 23-Jul-02 23:01 gitlabx/merge_request.py
 -rwxrwxrwx  2.0 unx     1233 b- defN 23-Jul-02 23:49 gitlabx/pipelines.py
 -rwxrwxrwx  2.0 unx     1121 b- defN 23-Jul-02 23:38 gitlabx/pipelines_schedules.py
 -rwxrwxrwx  2.0 unx      785 b- defN 23-Jun-29 11:24 gitlabx/project.py
 -rwxrwxrwx  2.0 unx      979 b- defN 23-Jun-29 11:24 gitlabx/projectLanguages.py
 -rwxrwxrwx  2.0 unx     1026 b- defN 23-Jun-29 11:24 gitlabx/repositories.py
 -rwxrwxrwx  2.0 unx     1376 b- defN 23-Jul-02 22:55 gitlabx/repositoryTree.py
 -rwxrwxrwx  2.0 unx     1062 b- defN 23-Jul-02 23:34 gitlabx/trriggers.py
--rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1682 b- defN 23-Jul-03 00:08 gitlabx-0.3.0.dist-info/RECORD
-22 files, 22439 bytes uncompressed, 9756 bytes compressed:  56.5%
+-rwxrwxrwx  2.0 unx     1675 b- defN 23-Jul-06 19:55 gitlabx-0.4.0.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-06 19:55 gitlabx-0.4.0.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-Jul-06 19:55 gitlabx-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1682 b- defN 23-Jul-06 19:55 gitlabx-0.4.0.dist-info/RECORD
+22 files, 23303 bytes uncompressed, 9830 bytes compressed:  57.8%
```

## zipnote {}

```diff
@@ -48,20 +48,20 @@
 
 Filename: gitlabx/repositoryTree.py
 Comment: 
 
 Filename: gitlabx/trriggers.py
 Comment: 
 
-Filename: gitlabx-0.3.0.dist-info/METADATA
+Filename: gitlabx-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: gitlabx-0.3.0.dist-info/WHEEL
+Filename: gitlabx-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: gitlabx-0.3.0.dist-info/top_level.txt
+Filename: gitlabx-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: gitlabx-0.3.0.dist-info/RECORD
+Filename: gitlabx-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gitlabx/commits.py

```diff
@@ -5,26 +5,56 @@
 
 # Represents a software Project
 class Commits(AbstractGitLab):
 
 	def __init__(self,personal_access_token, gitlab_url = None):
 		super(Commits,self).__init__(personal_access_token=personal_access_token,gitlab_url=gitlab_url)
 	
+	def get_by_project(self, project_id):
+		
+		commit_list = []
+
+		try:
+			logging.info("Start function: get_commit_projeto")
+			project = self.gl.projects.get(project_id)
+
+			logging.info("Start function: get_Commits:"+project.name )
+			commits = project.commits.list(iterator=True,get_all=True)
+			project = project.asdict()
+			for	commit in commits:
+				commitX = commit.asdict()
+				commitX['project_id'] = project['id']
+				commitX['merge_requests'] = commit.merge_requests()
+				commitX['refs'] = commit.refs() 
+				commitX['comments'] = commit.comments.list()
+				commitX['statuses '] = commit.statuses.list()
+
+				commit_list.append(commitX)
+			
+		except Exception as e: 
+			logging.error("OS error: {0}".format(e))
+			logging.error(e.__dict__) 
+
+		logging.info("Retrieve All Project``s Commits")
+		
+		return commit_list
+	
+	
 	def get_all(self, today=False): 
 		
 		result = []
 		commit_list = []
 
 		try:
 			logging.info("Start function: get_Commits")
 			result = self.gl.projects.list(owned=True, iterator=True)
 
 			for project in result:
 				logging.info("Start function: get_Commits:"+project.name )
-				commits = project.commits.list(iterator=True,all=True)
+				commits = project.commits.list(iterator=True,get_all=True)
 				project = project.asdict()
 				for	commit in commits:
 					commitX = commit.asdict()
 					commitX['project_id'] = project['id']
 					commitX['merge_requests'] = commit.merge_requests()
 					commitX['refs'] = commit.refs() 
 					commitX['comments'] = commit.comments.list()
```

## Comparing `gitlabx-0.3.0.dist-info/METADATA` & `gitlabx-0.4.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabx
-Version: 0.3.0
+Version: 0.4.0
 Summary: Uma Lib para buscar dados do Gitlab
 Home-page: https://gitlab.com/immigrant-data-driven-development/libs/application/gitlab
 Author: Carlos Henrique Maulaz de Freitas
 Author-email: carlosmaulaz@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `gitlabx-0.3.0.dist-info/RECORD` & `gitlabx-0.4.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 gitlabx/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gitlabx/abstract.py,sha256=mc5cmcD-klDfmHwo0HSl8itgsAiHx9nla1d5FQFjmcQ,380
 gitlabx/branches.py,sha256=HRgOYKxRQbjYDo50ZbwqbgvC5qxyLKEzsKC4nF8Zyw8,950
-gitlabx/commits.py,sha256=mXk5ixBVtbtjxxKDTH09yT9ey5EAvYrIVlb5AjRRTJ8,1241
+gitlabx/commits.py,sha256=1tUycSBA8_g036Dngq0bxOvVa6h4NgnLQHCuQ-xY7fs,2105
 gitlabx/deployments.py,sha256=sa8S9wmox-8ihRLwZq1mvpxKU5N8iKK0S7W8R1L11Q8,1026
 gitlabx/events.py,sha256=Nl6q0E3mc_x_XFlyGDNLj1m8Z5iieLiKfMs1HEvZTIY,902
 gitlabx/factories.py,sha256=KCiNkYpxBdOiZek2Xc99TZBt4ZuAYZnhQ1C9YL44w00,2795
 gitlabx/issues.py,sha256=WRiKt2Oz23quLD_8RoFCZfZwfxiYgRBs7N19DxFtDSw,944
 gitlabx/jobs.py,sha256=306PTUqAn9YjxRjy5Y7NOVcs75r79_JhMvJiqWvZMXE,984
 gitlabx/member.py,sha256=dUFBKal2MYaLoWHEqqZ6KME3p6-7cDDD1NS6fTPsEBU,974
 gitlabx/merge_request.py,sha256=CEM_mVTxh-mP7rwocPSpfcngZJAbGbnbTGAWGjgmw20,1204
 gitlabx/pipelines.py,sha256=P8QnCKI0E2T5__MJ-7rqXbpRm9Z4SBkJd-mKgytJOG0,1233
 gitlabx/pipelines_schedules.py,sha256=OYcWI7fn64WtHOZG7e5liQ8Vuv1osKiCq0eeDXAoaqo,1121
 gitlabx/project.py,sha256=28QdSWWM0swGkFC9LeCZW5mAXobXp02UKNZYEIhky50,785
 gitlabx/projectLanguages.py,sha256=qhRf543cotBVMdAlkaZ_CW9KU1y9e2Pxyw6Vsj4zkls,979
 gitlabx/repositories.py,sha256=o5p06Cf_x1hXmltKiecFvWO1MyQyX5L6jLy-He0_sgs,1026
 gitlabx/repositoryTree.py,sha256=QHMvOaXoW4LijmVysHI7a6tUZ2bEVBi04hqEymS4bUo,1376
 gitlabx/trriggers.py,sha256=KanV0r_eERuTMhsK6d2ZRxzhzkQFwnyHE-_gfLbUNks,1062
-gitlabx-0.3.0.dist-info/METADATA,sha256=BTzdxhLoJIzn34qAP8AdSBZuZISjCmZG-hNJIa5TpGA,1675
-gitlabx-0.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gitlabx-0.3.0.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
-gitlabx-0.3.0.dist-info/RECORD,,
+gitlabx-0.4.0.dist-info/METADATA,sha256=u2wy9jqztmHlOaTJ3KJGhUSvPne7NwiMcpLJmLQ8400,1675
+gitlabx-0.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gitlabx-0.4.0.dist-info/top_level.txt,sha256=EkmcO7CZ14bNE_fgl8kFTFfgu1K7yvMO481rj0zu6ns,8
+gitlabx-0.4.0.dist-info/RECORD,,
```

