# Comparing `tmp/tweeterpy-0.0.8.tar.gz` & `tmp/tweeterpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweeterpy-0.0.8.tar", last modified: Wed Jul  5 14:53:56 2023, max compression
+gzip compressed data, was "tweeterpy-0.0.9.tar", last modified: Thu Jul  6 15:09:45 2023, max compression
```

## Comparing `tweeterpy-0.0.8.tar` & `tweeterpy-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 14:53:56.277643 tweeterpy-0.0.8/
--rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3389 2023-07-05 14:53:56.277643 tweeterpy-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-05 14:53:56.277643 tweeterpy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1499 2023-07-05 14:30:35.000000 tweeterpy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:53:56.262005 tweeterpy-0.0.8/tweeterpy/
--rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.8/tweeterpy/__init__.py
--rw-rw-rw-   0        0        0     4037 2023-06-28 13:39:17.000000 tweeterpy-0.0.8/tweeterpy/api_util.py
--rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.8/tweeterpy/config.py
--rw-rw-rw-   0        0        0     2784 2023-07-05 06:41:31.000000 tweeterpy-0.0.8/tweeterpy/constants.py
--rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.8/tweeterpy/login_util.py
--rw-rw-rw-   0        0        0     1653 2023-06-20 07:35:05.000000 tweeterpy-0.0.8/tweeterpy/request_util.py
--rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.8/tweeterpy/session_util.py
--rw-rw-rw-   0        0        0    24985 2023-07-05 06:58:56.000000 tweeterpy-0.0.8/tweeterpy/tweeterpy.py
--rw-rw-rw-   0        0        0     3593 2023-06-28 07:54:04.000000 tweeterpy-0.0.8/tweeterpy/util.py
-drwxrwxrwx   0        0        0        0 2023-07-05 14:53:56.262005 tweeterpy-0.0.8/tweeterpy.egg-info/
--rw-rw-rw-   0        0        0     3389 2023-07-05 14:53:56.000000 tweeterpy-0.0.8/tweeterpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2023-07-05 14:53:56.000000 tweeterpy-0.0.8/tweeterpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 14:53:56.000000 tweeterpy-0.0.8/tweeterpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      235 2023-07-05 14:53:56.000000 tweeterpy-0.0.8/tweeterpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-05 14:53:56.000000 tweeterpy-0.0.8/tweeterpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 15:09:45.237949 tweeterpy-0.0.9/
+-rw-rw-rw-   0        0        0     1093 2023-05-19 18:11:22.000000 tweeterpy-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       22 2023-06-20 15:06:14.000000 tweeterpy-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3389 2023-07-06 15:09:45.237949 tweeterpy-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-06-22 07:42:40.000000 tweeterpy-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:09:45.253601 tweeterpy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1499 2023-07-06 15:07:58.000000 tweeterpy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:09:45.237949 tweeterpy-0.0.9/tweeterpy/
+-rw-rw-rw-   0        0        0       34 2023-06-20 15:09:15.000000 tweeterpy-0.0.9/tweeterpy/__init__.py
+-rw-rw-rw-   0        0        0     4037 2023-07-06 15:09:28.000000 tweeterpy-0.0.9/tweeterpy/api_util.py
+-rw-rw-rw-   0        0        0      671 2023-06-25 06:51:11.000000 tweeterpy-0.0.9/tweeterpy/config.py
+-rw-rw-rw-   0        0        0     2784 2023-07-05 06:41:31.000000 tweeterpy-0.0.9/tweeterpy/constants.py
+-rw-rw-rw-   0        0        0     6654 2023-06-24 14:06:58.000000 tweeterpy-0.0.9/tweeterpy/login_util.py
+-rw-rw-rw-   0        0        0     1631 2023-07-06 09:25:11.000000 tweeterpy-0.0.9/tweeterpy/request_util.py
+-rw-rw-rw-   0        0        0     2278 2023-06-25 06:51:11.000000 tweeterpy-0.0.9/tweeterpy/session_util.py
+-rw-rw-rw-   0        0        0    25592 2023-07-06 14:59:08.000000 tweeterpy-0.0.9/tweeterpy/tweeterpy.py
+-rw-rw-rw-   0        0        0     4900 2023-07-06 08:19:59.000000 tweeterpy-0.0.9/tweeterpy/util.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:09:45.237949 tweeterpy-0.0.9/tweeterpy.egg-info/
+-rw-rw-rw-   0        0        0     3389 2023-07-06 15:09:45.000000 tweeterpy-0.0.9/tweeterpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2023-07-06 15:09:45.000000 tweeterpy-0.0.9/tweeterpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:09:45.000000 tweeterpy-0.0.9/tweeterpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      235 2023-07-06 15:09:45.000000 tweeterpy-0.0.9/tweeterpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-06 15:09:45.000000 tweeterpy-0.0.9/tweeterpy.egg-info/top_level.txt
```

### Comparing `tweeterpy-0.0.8/LICENSE` & `tweeterpy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/PKG-INFO` & `tweeterpy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.8 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.9 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `tweeterpy-0.0.8/README.md` & `tweeterpy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/setup.py` & `tweeterpy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 SHORT_DESCRIPTION = "TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc."
 
 with open("requirements.txt") as file:
     dependencies = file.read().splitlines()
 with open("README.md", "r") as file:
     DESCRIPTION = file.read()
```

### Comparing `tweeterpy-0.0.8/tweeterpy/api_util.py` & `tweeterpy-0.0.9/tweeterpy/api_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/tweeterpy/config.py` & `tweeterpy-0.0.9/tweeterpy/config.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/tweeterpy/constants.py` & `tweeterpy-0.0.9/tweeterpy/constants.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/tweeterpy/login_util.py` & `tweeterpy-0.0.9/tweeterpy/login_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/tweeterpy/request_util.py` & `tweeterpy-0.0.9/tweeterpy/request_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,31 +13,30 @@
         session = config._DEFAULT_SESSION or requests.Session()
     if timeout is None:
         timeout = config.TIMEOUT or 30
     for retry_count, _ in enumerate(range(max_retries), start=1):
         try:
             response_text = ""
             response = session.request(method, url, timeout=timeout, **kwargs)
+            api_limit_stats = util.check_api_rate_limits(response)
             soup = bs4.BeautifulSoup(response.content, "lxml")
             if "json" in response.headers["Content-Type"]:
                 return util.check_for_errors(response.json())
             response_text = "\n".join(
                 [line.strip() for line in soup.text.split("\n") if line.strip()])
             response.raise_for_status()
             return soup
         except KeyboardInterrupt:
             print("Keyboard Interruption...")
             return
-        except requests.exceptions.RequestException as error:
-            print(f"Retry No. ==> {retry_count}", end="\r")
-            if retry_count >= max_retries:
-                print(f"{error}\n{response_text}")
-                raise Exception(error)
         except Exception as error:
             print(f"Retry No. ==> {retry_count}", end="\r")
             if retry_count >= max_retries:
-                print(f"{error}\n{response_text}")
-                raise Exception(error)
+                print(f"{error}\n\n{response_text}\n")
+                if api_limit_stats.get('rate_limit_exhausted'):
+                    print(
+                        f"\033[91m Rate Limit Exceeded:\033[0m {api_limit_stats}")
+                raise error
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `tweeterpy-0.0.8/tweeterpy/session_util.py` & `tweeterpy-0.0.9/tweeterpy/session_util.py`

 * *Files identical despite different names*

### Comparing `tweeterpy-0.0.8/tweeterpy/tweeterpy.py` & `tweeterpy-0.0.9/tweeterpy/tweeterpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,21 @@
         url = util.generate_url(url_path=Path.VIEWER_ENDPOINT)
         query = {"variables": json.dumps({"withCommunitiesMemberships": True,
                                           "withSubscribedTab": True, "withCommunitiesCreation": True}),
                  "features": json.dumps(util.generate_features())}
         response = self.session.get(url, params=query).json()
         return response
 
+    def login_decorator(original_function):
+        def wrapper(self, *args, **kwargs):
+            if not self.logged_in():
+                self.login()
+            return original_function(self, *args, **kwargs)
+        return wrapper
+
     def generate_session(self, auth_token=None):
         """Generate a twitter session. With/Without Login.
 
         Args:
             auth_token (str, optional): Generate session with an auth-token. If auth_token is None (Default Behaviour), generates a guest session without login. Defaults to None.
 
         Returns:
@@ -178,14 +185,15 @@
         if username is None:
             username = str(input("Enter Your Username or Email : ")).strip()
         if password is None:
             password = getpass.getpass()
         TaskHandler().login(username, password)
         util.generate_headers(session=self.session)
 
+    @login_decorator
     def get_user_id(self, username):
         """Get user ID of a twitter user.
 
         Args:
             username (str): Twitter username.
 
         Returns:
@@ -194,14 +202,15 @@
         if isinstance(username, int) or username.isnumeric():
             return username
         url, query_params = self._generate_request_data(
             Path.USER_ID_ENDPOINT, {"screen_name": username})
         response = make_request(url, params=query_params)
         return response['data']['user_result_by_screen_name']['result']['rest_id']
 
+    @login_decorator
     def get_user_info(self, user_id):
         """Extracts user details like username, userid, bio, website, follower/following count etc.
 
         Args:
             user_id (str/int): User ID.
 
         Returns:
@@ -210,14 +219,15 @@
         user_id = self.get_user_id(user_id)
         variables = {"userId": user_id, "withSafetyModeUserFields": True}
         url, query_params = self._generate_request_data(
             Path.USER_INFO_ENDPOINT, variables, user_data_features=True)
         response = make_request(url, params=query_params)
         return response['data']['user']['result']
 
+    @login_decorator
     def get_user_data(self, username):
         """Extracts user details as same as get_user_info method. Except this one returns info about blue tick verification badge as well.
 
         Args:
             username (str): Twitter username.
 
         Returns:
@@ -225,14 +235,15 @@
         """
         variables = {"screen_name": username, "withSafetyModeUserFields": True}
         url, query_params = self._generate_request_data(
             Path.USER_DATA_ENDPOINT, variables, user_info_feautres=True)
         response = make_request(url, params=query_params)
         return response['data']['user']['result']
 
+    @login_decorator
     def get_multiple_users_data(self, user_ids):
         """Get user information of multiple twitter users.
 
         Args:
             user_ids (list): List of twitter users' IDs.
 
         Returns:
@@ -240,14 +251,15 @@
         """
         variables = {"userIds": user_ids}
         url, query_params = self._generate_request_data(
             Path.MULTIPLE_USERS_DATA_ENDPOINT, variables, default_features=True)
         response = make_request(url, params=query_params)
         return response['data']['users']
 
+    @login_decorator
     def get_user_tweets(self, user_id, with_replies=False, end_cursor=None, total=None):
         """Get Tweets from a user's profile.
 
         Args:
             user_id (int): User ID.
             with_replies (bool, optional): Set to True if want to get the tweets user replied to, from user's profile page. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
@@ -268,14 +280,15 @@
 
         url, query_params = self._generate_request_data(
             query_endpoint, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_user_media(self, user_id, end_cursor=None, total=None):
         """Get media from a user's profile.
 
         Args:
             user_id (int): User ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
@@ -288,14 +301,15 @@
                      "withClientEventToken": False, "withBirdwatchNotes": False, "withVoice": True, "withV2Timeline": True}
         url, query_params = self._generate_request_data(
             Path.USER_MEDIA_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_tweet(self, tweet_id, with_tweet_replies=False, end_cursor=None, total=None):
         """Get Tweets from a user's profile.
 
         Args:
             tweet_id (int): Tweet ID.
             with_tweet_replies (bool, optional): Set to True if want to get the tweets replies as well. Defaults to False.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Only applicable if with with_tweet_replies is True. Defaults to None.
@@ -316,14 +330,15 @@
             Path.TWEET_DETAILS_ENDPOINT, variables, additional_features=True)
         data_path = (
             'data', 'threaded_conversation_with_injections_v2', 'instructions')
         if with_tweet_replies:
             return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
         return make_request(url, params=query_params)
 
+    @login_decorator
     def get_liked_tweets(self, user_id, end_cursor=None, total=None):
         """Get Tweets liked by a user.
 
         Args:
             user_id (int): User ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
@@ -338,14 +353,15 @@
                      "withClientEventToken": False, "withBirdwatchNotes": False, "withVoice": True, "withV2Timeline": True}
         url, query_params = self._generate_request_data(
             Path.LIKED_TWEETS_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline_v2',
                      'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_user_timeline(self, end_cursor=None, total=None):
         """Get tweets from home timeline (Home Page).
 
         Args:
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
 
@@ -357,14 +373,15 @@
         variables = {"count": 40, "includePromotedContent": True,
                      "latestControlAvailable": True, "withCommunity": True}
         url, query_params = self._generate_request_data(
             Path.HOME_TIMELINE_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'home', 'home_timeline_urt', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_list_tweets(self, list_id, end_cursor=None, total=None):
         """Get tweets from a Tweets List.
 
         Args:
             list_id (str/int): Tweets List ID. (Can be extracted from twitter mobile app.)
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
@@ -375,14 +392,15 @@
         variables = {"listId": list_id, "count": 100}
         url, query_params = self._generate_request_data(
             Path.TWEETS_LIST_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'list', 'tweets_timeline',
                      'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_topic_tweets(self, topic_id, end_cursor=None, total=None):
         """Get tweets from a Topic.
 
         Args:
             topic_id (str/int): Topic ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
@@ -393,14 +411,15 @@
         variables = {"rest_id": topic_id, "count": 100}
         url, query_params = self._generate_request_data(
             Path.TOPIC_TWEETS_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'topic_by_rest_id', 'topic_page',
                      'body', 'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def search(self, search_query, end_cursor=None, total=None, search_filter=None):
         """Get search results.
 
         Args:
             search_query (str): Search term.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) Number of results you want to get. If None, extracts all results. Defaults to None.
@@ -415,14 +434,15 @@
                      "querySource": "hashtag_click", "product": search_filter}
         url, query_params = self._generate_request_data(
             Path.SEARCH_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'search_by_raw_query',
                      'search_timeline', 'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_friends(self, user_id, follower=False, following=False, mutual_follower=False, end_cursor=None, total=None):
         """Get User's follower, followings or mutual followers.
 
         Args:
             user_id (int): User ID.
             follower (bool, optional): Set to True if want to extract User's follower. Defaults to False.
             following (bool, optional): Set to True if want to extract User's following. Defaults to False.
@@ -444,14 +464,15 @@
                      "includePromotedContent": False}
         url, query_params = self._generate_request_data(
             query_path, variables, additional_features=True)
         data_path = ('data', 'user', 'result', 'timeline',
                      'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_profile_business_category(self, user_id):
         """Extracts profile category of a Professional/Business twitter profile. Can also be extracted from get_user_info and get_user_data methods.
 
         Args:
             user_id (int): User ID.
 
         Returns:
@@ -460,48 +481,50 @@
         user_id = self.get_user_id(user_id)
         variables = {"rest_id": user_id}
         url, query_params = self._generate_request_data(
             Path.PROFILE_CATEGORY_ENDPOINT, variables)
         response = make_request(url, params=query_params)
         return response
 
+    @login_decorator
     def get_tweet_likes(self, tweet_id, end_cursor=None, total=None):
         """Returns data about the users who liked the given tweet post.
 
         Args:
             tweet_id (int): Tweet ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         if not self.logged_in():
             self.login()
-        variables = {"tweetId": tweet_id, "count": 100,
+        variables = {"tweetId": str(tweet_id), "count": 100,
                      "includePromotedContent": True}
         url, query_params = self._generate_request_data(
             Path.TWEET_LIKES_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'favoriters_timeline', 'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
 
+    @login_decorator
     def get_retweeters(self, tweet_id, end_cursor=None, total=None):
         """Returs data about the users who retweeted the given tweet post.
 
         Args:
             tweet_id (int): Tweet ID.
             end_cursor (str, optional): Last endcursor point. (To start from where you left off last time). Defaults to None.
             total (int, optional): Total(Max) number of results you want to get. If None, extracts all results. Defaults to None.
 
         Returns:
             dict: Returns data, cursor_endpoint, has_next_page
         """
         if not self.logged_in():
             self.login()
-        variables = {"tweetId": tweet_id, "count": 100,
+        variables = {"tweetId": str(tweet_id), "count": 100,
                      "includePromotedContent": True}
         url, query_params = self._generate_request_data(
             Path.RETWEETED_BY_ENDPOINT, variables, additional_features=True)
         data_path = ('data', 'retweeters_timeline', 'timeline', 'instructions')
         return self._handle_pagination(url, query_params, end_cursor=end_cursor, data_path=data_path, total=total)
```

### Comparing `tweeterpy-0.0.8/tweeterpy.egg-info/PKG-INFO` & `tweeterpy-0.0.9/tweeterpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweeterpy
-Version: 0.0.8
+Version: 0.0.9
 Summary: TweeterPy is a python library to extract data from Twitter. TweeterPy API lets you scrape data from a user's profile like username, userid, bio, followers/followings list, profile media, tweets, etc.
 Home-page: https://github.com/iSarabjitDhiman/TweeterPy
 Author: Sarabjit Dhiman
 Author-email: hello@sarabjitdhiman.com
 License: MIT
 Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data extraction,twitter api,twitter python,tweet api,tweetpy
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.8 Summary: TweeterPy is a
+Metadata-Version: 2.1 Name: tweeterpy Version: 0.0.9 Summary: TweeterPy is a
 python library to extract data from Twitter. TweeterPy API lets you scrape data
 from a user's profile like username, userid, bio, followers/followings list,
 profile media, tweets, etc. Home-page: https://github.com/iSarabjitDhiman/
 TweeterPy Author: Sarabjit Dhiman Author-email: hello@sarabjitdhiman.com
 License: MIT Keywords: tweeterpy,twitter scraper,tweet scraper,twitter data
 extraction,twitter api,twitter python,tweet api,tweetpy Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: End Users/Desktop
```

