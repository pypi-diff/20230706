# Comparing `tmp/moesifwsgi-1.8.1.tar.gz` & `tmp/moesifwsgi-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/moesifwsgi-1.8.1.tar", last modified: Thu Jun 29 23:52:20 2023, max compression
+gzip compressed data, was "/Users/praveen/workspace/git/moesif/sdks/moesifwsgi/dist/.tmp-n0j4h22e/moesifwsgi-1.8.2.tar", last modified: Thu Jul  6 07:01:42 2023, max compression
```

## Comparing `moesifwsgi-1.8.1.tar` & `moesifwsgi-1.8.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.336958 moesifwsgi-1.8.1/
--rwxr-xr-x   0 keyur      (501) staff       (20)    11911 2020-06-25 11:08:31.000000 moesifwsgi-1.8.1/LICENSE
--rw-r--r--   0 keyur      (501) staff       (20)       61 2020-04-19 17:20:34.000000 moesifwsgi-1.8.1/MANIFEST.in
--rw-r--r--   0 keyur      (501) staff       (20)    22428 2023-06-29 23:52:20.337592 moesifwsgi-1.8.1/PKG-INFO
--rwxr-xr-x   0 keyur      (501) staff       (20)    17486 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/README.md
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.334104 moesifwsgi-1.8.1/moesifwsgi/
--rw-r--r--   0 keyur      (501) staff       (20)       26 2020-04-19 17:20:34.000000 moesifwsgi-1.8.1/moesifwsgi/__init__.py
--rw-r--r--   0 keyur      (501) staff       (20)     4634 2020-12-29 19:45:45.000000 moesifwsgi-1.8.1/moesifwsgi/client_ip.py
--rw-r--r--   0 keyur      (501) staff       (20)     4570 2023-06-15 14:36:10.000000 moesifwsgi-1.8.1/moesifwsgi/config_manager.py
--rw-r--r--   0 keyur      (501) staff       (20)     3526 2023-05-12 21:29:24.000000 moesifwsgi-1.8.1/moesifwsgi/event_mapper.py
--rw-r--r--   0 keyur      (501) staff       (20)     1067 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/http_response_catcher.py
--rw-r--r--   0 keyur      (501) staff       (20)    10558 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/moesifwsgi/logger_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     9910 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/moesifwsgi/middleware.py
--rw-r--r--   0 keyur      (501) staff       (20)     3071 2023-05-12 21:29:36.000000 moesifwsgi-1.8.1/moesifwsgi/moesif_data_holder.py
--rw-r--r--   0 keyur      (501) staff       (20)     2344 2020-12-29 19:47:50.000000 moesifwsgi-1.8.1/moesifwsgi/parse_body.py
--rw-r--r--   0 keyur      (501) staff       (20)     4018 2022-01-13 23:06:22.000000 moesifwsgi-1.8.1/moesifwsgi/regex_config_helper.py
--rw-r--r--   0 keyur      (501) staff       (20)     8531 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/update_companies.py
--rw-r--r--   0 keyur      (501) staff       (20)     8100 2023-04-20 01:32:27.000000 moesifwsgi-1.8.1/moesifwsgi/update_users.py
--rw-r--r--   0 keyur      (501) staff       (20)     6887 2023-06-15 14:36:10.000000 moesifwsgi-1.8.1/moesifwsgi/workers.py
-drwxr-xr-x   0 keyur      (501) staff       (20)        0 2023-06-29 23:52:20.336746 moesifwsgi-1.8.1/moesifwsgi.egg-info/
--rw-r--r--   0 keyur      (501) staff       (20)    22428 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/PKG-INFO
--rw-r--r--   0 keyur      (501) staff       (20)      581 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/SOURCES.txt
--rw-r--r--   0 keyur      (501) staff       (20)        1 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/dependency_links.txt
--rw-r--r--   0 keyur      (501) staff       (20)      130 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/requires.txt
--rw-r--r--   0 keyur      (501) staff       (20)       11 2023-06-29 23:52:20.000000 moesifwsgi-1.8.1/moesifwsgi.egg-info/top_level.txt
--rw-r--r--   0 keyur      (501) staff       (20)       67 2023-06-29 23:52:20.339119 moesifwsgi-1.8.1/setup.cfg
--rw-r--r--   0 keyur      (501) staff       (20)     3693 2023-06-29 23:50:56.000000 moesifwsgi-1.8.1/setup.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/
+-rwxr-xr-x   0 praveen    (501) staff       (20)    11911 2021-12-24 00:24:54.000000 moesifwsgi-1.8.2/LICENSE
+-rw-r--r--   0 praveen    (501) staff       (20)       61 2021-12-24 00:24:54.000000 moesifwsgi-1.8.2/MANIFEST.in
+-rw-r--r--   0 praveen    (501) staff       (20)    18915 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/PKG-INFO
+-rwxr-xr-x   0 praveen    (501) staff       (20)    17486 2023-07-06 06:25:41.000000 moesifwsgi-1.8.2/README.md
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi/
+-rw-r--r--   0 praveen    (501) staff       (20)       26 2021-12-24 00:24:54.000000 moesifwsgi-1.8.2/moesifwsgi/__init__.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4634 2021-12-24 00:24:54.000000 moesifwsgi-1.8.2/moesifwsgi/client_ip.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4570 2023-06-15 03:06:35.000000 moesifwsgi-1.8.2/moesifwsgi/config_manager.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3526 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/event_mapper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     1067 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/http_response_catcher.py
+-rw-r--r--   0 praveen    (501) staff       (20)    10558 2023-07-06 06:25:41.000000 moesifwsgi-1.8.2/moesifwsgi/logger_helper.py
+-rw-r--r--   0 praveen    (501) staff       (20)    10201 2023-07-06 06:25:41.000000 moesifwsgi-1.8.2/moesifwsgi/middleware.py
+-rw-r--r--   0 praveen    (501) staff       (20)     3071 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/moesif_data_holder.py
+-rw-r--r--   0 praveen    (501) staff       (20)     2344 2021-12-24 00:24:54.000000 moesifwsgi-1.8.2/moesifwsgi/parse_body.py
+-rw-r--r--   0 praveen    (501) staff       (20)     4018 2022-09-21 22:56:45.000000 moesifwsgi-1.8.2/moesifwsgi/regex_config_helper.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8531 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/update_companies.py
+-rw-r--r--   0 praveen    (501) staff       (20)     8100 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/update_users.py
+-rw-r--r--   0 praveen    (501) staff       (20)     6887 2023-05-16 00:12:53.000000 moesifwsgi-1.8.2/moesifwsgi/workers.py
+drwxr-xr-x   0 praveen    (501) staff       (20)        0 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/
+-rw-r--r--   0 praveen    (501) staff       (20)    18915 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/PKG-INFO
+-rw-r--r--   0 praveen    (501) staff       (20)      581 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/SOURCES.txt
+-rw-r--r--   0 praveen    (501) staff       (20)        1 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/dependency_links.txt
+-rw-r--r--   0 praveen    (501) staff       (20)      130 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/requires.txt
+-rw-r--r--   0 praveen    (501) staff       (20)       11 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/moesifwsgi.egg-info/top_level.txt
+-rw-r--r--   0 praveen    (501) staff       (20)       67 2023-07-06 07:01:42.000000 moesifwsgi-1.8.2/setup.cfg
+-rw-r--r--   0 praveen    (501) staff       (20)     3693 2023-07-06 06:25:41.000000 moesifwsgi-1.8.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `moesifwsgi-1.8.1/LICENSE` & `moesifwsgi-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/PKG-INFO` & `moesifwsgi-1.8.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,456 +1,16 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.8.1
+Version: 1.8.2
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
-Description: # Moesif Middleware for Python WSGI based Frameworks
-        
-        [![Built For][ico-built-for]][link-built-for]
-        [![Latest Version][ico-version]][link-package]
-        [![Language Versions][ico-language]][link-language]
-        [![Software License][ico-license]][link-license]
-        [![Source Code][ico-source]][link-source]
-        
-        WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
-        Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
-        
-        [Source Code on GitHub](https://github.com/moesif/moesifwsgi)
-        
-        [WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
-        is a standard (PEP 3333) that describes
-        how a web server communicates with web applications. Many Python Frameworks
-        are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
-        [Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
-        Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
-        easily integrate with [Moesif](https://www.moesif.com).
-        
-        ## How to install
-        
-        ```shell
-        pip install moesifwsgi
-        ```
-        
-        ## How to use
-        
-        ### Flask
-        
-        Wrap your wsgi_app with the Moesif middleware.
-        
-        ```python
-        from moesifwsgi import MoesifMiddleware
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-        
-        You can always find your Moesif Application Id at any time by logging 
-        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
-        and then clicking _API Keys_.
-        
-        For an example with Flask, see example in the `/examples/flask` folder of this repo.
-        
-        ### Bottle
-        Wrap your bottle app with the Moesif middleware.
-        
-        ```python
-        
-        from moesifwsgi import MoesifMiddleware
-        
-        app = bottle.Bottle()
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        bottle.run(app=MoesifMiddleware(app, moesif_settings))
-        
-        ```
-        
-        For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
-        
-        ### Pyramid
-        
-        
-        ```python
-        from pyramid.config import Configurator
-        from moesifwsgi import MoesifMiddleware
-        
-        if __name__ == '__main__':
-            config = Configurator()
-            config.add_route('hello', '/')
-            config.scan()
-            app = config.make_wsgi_app()
-        
-            # configure your moesif settings
-            moesif_settings = {
-                'APPLICATION_ID': 'Your Moesif Application Id',
-                'LOG_BODY': True,
-                # ... For other options see below.
-            }
-            # Put middleware
-            app = MoesifMiddleware(app, moesif_settings)
-        
-            server = make_server('0.0.0.0', 8080, app)
-            server.serve_forever()
-        
-        ```
-        ### Other WSGI frameworks
-        
-        If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
-        Please read the documentation for your specific framework on how to add middleware.
-        
-        ## Configuration options
-        
-        The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
-        Also, Moesif adds the following to the environ variable
-        ```
-        environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
-        environ["moesif.response_body_chunks"] - A response body chunks
-        environ["moesif.response_headers"] - A dict representing the response headers
-        ```
-        
-        #### __`APPLICATION_ID`__
-        (__required__), _string_, is obtained via your Moesif Account, this is required.
-        
-        #### __`SKIP`__
-        (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event.
-        
-        #### __`IDENTIFY_USER`__
-        (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        #### __`IDENTIFY_COMPANY`__
-        (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
-        
-        #### __`GET_METADATA`__
-        (optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
-        returns a dictionary (must be able to be encoded into JSON). This allows your
-        to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
-        
-        #### __`GET_SESSION_TOKEN`__
-        (optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        #### __`MASK_EVENT_MODEL`__
-        (optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
-        
-        #### __`DEBUG`__
-        (optional) _boolean_, a flag to see debugging messages.
-        
-        #### __`LOG_BODY`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        #### __`EVENT_QUEUE_SIZE`__
-        (optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
-        
-        ### __`EVENT_WORKER_COUNT`__
-        (optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
-        
-        #### __`BATCH_SIZE`__
-        (optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
-        
-        #### __`EVENT_BATCH_TIMEOUT`__
-        (optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
-        
-        #### __`AUTHORIZATION_HEADER_NAME`__
-        (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
-        
-        #### __`AUTHORIZATION_USER_ID_FIELD`__
-        (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
-        
-        #### __`BASE_URI`__
-        (optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
-        
-        ### Options specific to outgoing API calls 
-        
-        The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
-        
-        For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
-        
-        If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
-        
-        #### __`CAPTURE_OUTGOING_REQUESTS`__
-        _boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
-        
-        ##### __`GET_METADATA_OUTGOING`__
-        (optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
-        Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
-        returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
-        
-        ##### __`SKIP_OUTGOING`__
-        (optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
-        and returns true if you want to skip this particular event.
-        
-        ##### __`IDENTIFY_USER_OUTGOING`__
-        (optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        ##### __`IDENTIFY_COMPANY_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
-        
-        ##### __`GET_SESSION_TOKEN_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        ##### __`LOG_BODY_OUTGOING`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        ### Example:
-        
-        ```python
-        def identify_user(app, environ, response_headers=dict()):
-            # Your custom code that returns a user id string
-            return "12345"
-        
-        def identify_company(app, environ, response_headers=dict()):
-            # Your custom code that returns a company id string
-            return "67890"
-        
-        def should_skip(app, environ):
-            # Your custom code that returns true to skip logging
-            return "health/probe" in environ.get('PATH_INFO', '')
-        
-        def get_token(app, environ):
-            # If you don't want to use the standard WSGI session token,
-            # add your custom code that returns a string for session/API token
-            return "XXXXXXXXXXXXXX"
-        
-        def mask_event(eventmodel):
-            # Your custom code to change or remove any sensitive fields
-            if 'password' in eventmodel.response.body:
-                eventmodel.response.body['password'] = None
-            return eventmodel
-        
-        def get_metadata(app, environ):
-            return {
-                'datacenter': 'westus',
-                'deployment_version': 'v1.2.3',
-            }
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'DEBUG': False,
-            'LOG_BODY': True,
-            'IDENTIFY_USER': identify_user,
-            'IDENTIFY_COMPANY': identify_company,
-            'GET_SESSION_TOKEN': get_token,
-            'SKIP': should_skip,
-            'MASK_EVENT_MODEL': mask_event,
-            'GET_METADATA': get_metadata,
-            'CAPTURE_OUTGOING_REQUESTS': False
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        ## Update User
-        
-        ### Update A Single User
-        Create or update a user profile in Moesif.
-        The metadata field can be any customer demographic or other info you want to store.
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only user_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#users for campaign schema
-        # metadata can be any custom object
-        user = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        update_user = api_client.update_user(user)
-        ```
-        
-        ### Update Users in Batch
-        Similar to update_user, but used to update a list of users in one batch. 
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        userA = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        userB = {
-          'user_id': '54321',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'mary@acmeinc.com',
-            'first_name': 'Mary',
-            'last_name': 'Jane',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 48000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        update_users = api_client.update_users_batch([userA, userB])
-        ```
-        
-        ## Update Company
-        
-        ### Update A Single Company
-        Create or update a company profile in Moesif.
-        The metadata field can be any company demographic or other info you want to store.
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only company_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
-        # metadata can be any custom object
-        company = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        update_company = api_client.update_company(company)
-        ```
-        
-        ### Update Companies in Batch
-        Similar to update_company, but used to update a list of companies in one batch. 
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        companyA = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        companyB = {
-          'company_id': '09876',
-          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Contoso, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 48000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 53
-            },
-          }
-        }
-        
-        update_companies = api_client.update_companies_batch([companyA, companyB])
-        ```
-        ## Troubleshooting
-        
-        When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
-        In order to resolve that, add the following line to your Dockerfile
-        ```
-        ENV TZ=UTC
-        ```
-        or you could add `RUN apt-get install tzdata` in the Dockerfile.
-        
-        ## Other integrations
-        
-        To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
-        
-        [ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
-        [ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
-        [ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
-        [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-        [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
-        
-        [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
-        [link-package]: https://pypi.python.org/pypi/moesifwsgi
-        [link-language]: https://pypi.python.org/pypi/moesifwsgi
-        [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
-        [link-source]: https://github.com/Moesif/moesifwsgi
-        
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
@@ -465,7 +25,447 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Moesif Middleware for Python WSGI based Frameworks
+
+[![Built For][ico-built-for]][link-built-for]
+[![Latest Version][ico-version]][link-package]
+[![Language Versions][ico-language]][link-language]
+[![Software License][ico-license]][link-license]
+[![Source Code][ico-source]][link-source]
+
+WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
+Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
+
+[Source Code on GitHub](https://github.com/moesif/moesifwsgi)
+
+[WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
+is a standard (PEP 3333) that describes
+how a web server communicates with web applications. Many Python Frameworks
+are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
+[Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
+Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
+easily integrate with [Moesif](https://www.moesif.com).
+
+## How to install
+
+```shell
+pip install moesifwsgi
+```
+
+## How to use
+
+### Flask
+
+Wrap your wsgi_app with the Moesif middleware.
+
+```python
+from moesifwsgi import MoesifMiddleware
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+
+You can always find your Moesif Application Id at any time by logging 
+into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+and then clicking _API Keys_.
+
+For an example with Flask, see example in the `/examples/flask` folder of this repo.
+
+### Bottle
+Wrap your bottle app with the Moesif middleware.
+
+```python
+
+from moesifwsgi import MoesifMiddleware
+
+app = bottle.Bottle()
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+bottle.run(app=MoesifMiddleware(app, moesif_settings))
+
+```
+
+For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
+
+### Pyramid
+
+
+```python
+from pyramid.config import Configurator
+from moesifwsgi import MoesifMiddleware
+
+if __name__ == '__main__':
+    config = Configurator()
+    config.add_route('hello', '/')
+    config.scan()
+    app = config.make_wsgi_app()
+
+    # configure your moesif settings
+    moesif_settings = {
+        'APPLICATION_ID': 'Your Moesif Application Id',
+        'LOG_BODY': True,
+        # ... For other options see below.
+    }
+    # Put middleware
+    app = MoesifMiddleware(app, moesif_settings)
+
+    server = make_server('0.0.0.0', 8080, app)
+    server.serve_forever()
+
+```
+### Other WSGI frameworks
+
+If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
+Please read the documentation for your specific framework on how to add middleware.
+
+## Configuration options
+
+The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+Also, Moesif adds the following to the environ variable
+```
+environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
+environ["moesif.response_body_chunks"] - A response body chunks
+environ["moesif.response_headers"] - A dict representing the response headers
+```
+
+#### __`APPLICATION_ID`__
+(__required__), _string_, is obtained via your Moesif Account, this is required.
+
+#### __`SKIP`__
+(optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
+and returns true if you want to skip this particular event.
+
+#### __`IDENTIFY_USER`__
+(optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+#### __`IDENTIFY_COMPANY`__
+(optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
+
+#### __`GET_METADATA`__
+(optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
+returns a dictionary (must be able to be encoded into JSON). This allows your
+to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
+
+#### __`GET_SESSION_TOKEN`__
+(optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+#### __`MASK_EVENT_MODEL`__
+(optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
+
+#### __`DEBUG`__
+(optional) _boolean_, a flag to see debugging messages.
+
+#### __`LOG_BODY`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+#### __`EVENT_QUEUE_SIZE`__
+(optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
+
+### __`EVENT_WORKER_COUNT`__
+(optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
+
+#### __`BATCH_SIZE`__
+(optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
+
+#### __`EVENT_BATCH_TIMEOUT`__
+(optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
+
+#### __`AUTHORIZATION_HEADER_NAME`__
+(optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
+
+#### __`AUTHORIZATION_USER_ID_FIELD`__
+(optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
+
+#### __`BASE_URI`__
+(optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
+
+### Options specific to outgoing API calls 
+
+The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
+
+For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
+
+If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
+
+#### __`CAPTURE_OUTGOING_REQUESTS`__
+_boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
+
+##### __`GET_METADATA_OUTGOING`__
+(optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
+Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
+returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
+
+##### __`SKIP_OUTGOING`__
+(optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
+and returns true if you want to skip this particular event.
+
+##### __`IDENTIFY_USER_OUTGOING`__
+(optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+##### __`IDENTIFY_COMPANY_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
+
+##### __`GET_SESSION_TOKEN_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+##### __`LOG_BODY_OUTGOING`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+### Example:
+
+```python
+def identify_user(app, environ, response_headers=dict()):
+    # Your custom code that returns a user id string
+    return "12345"
+
+def identify_company(app, environ, response_headers=dict()):
+    # Your custom code that returns a company id string
+    return "67890"
+
+def should_skip(app, environ):
+    # Your custom code that returns true to skip logging
+    return "health/probe" in environ.get('PATH_INFO', '')
+
+def get_token(app, environ):
+    # If you don't want to use the standard WSGI session token,
+    # add your custom code that returns a string for session/API token
+    return "XXXXXXXXXXXXXX"
+
+def mask_event(eventmodel):
+    # Your custom code to change or remove any sensitive fields
+    if 'password' in eventmodel.response.body:
+        eventmodel.response.body['password'] = None
+    return eventmodel
+
+def get_metadata(app, environ):
+    return {
+        'datacenter': 'westus',
+        'deployment_version': 'v1.2.3',
+    }
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'DEBUG': False,
+    'LOG_BODY': True,
+    'IDENTIFY_USER': identify_user,
+    'IDENTIFY_COMPANY': identify_company,
+    'GET_SESSION_TOKEN': get_token,
+    'SKIP': should_skip,
+    'MASK_EVENT_MODEL': mask_event,
+    'GET_METADATA': get_metadata,
+    'CAPTURE_OUTGOING_REQUESTS': False
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+## Update User
+
+### Update A Single User
+Create or update a user profile in Moesif.
+The metadata field can be any customer demographic or other info you want to store.
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only user_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#users for campaign schema
+# metadata can be any custom object
+user = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+update_user = api_client.update_user(user)
+```
+
+### Update Users in Batch
+Similar to update_user, but used to update a list of users in one batch. 
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+userA = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+userB = {
+  'user_id': '54321',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'mary@acmeinc.com',
+    'first_name': 'Mary',
+    'last_name': 'Jane',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 48000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+update_users = api_client.update_users_batch([userA, userB])
+```
+
+## Update Company
+
+### Update A Single Company
+Create or update a company profile in Moesif.
+The metadata field can be any company demographic or other info you want to store.
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only company_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#update-a-company for campaign schema
+# metadata can be any custom object
+company = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+update_company = api_client.update_company(company)
+```
+
+### Update Companies in Batch
+Similar to update_company, but used to update a list of companies in one batch. 
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+companyA = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+companyB = {
+  'company_id': '09876',
+  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Contoso, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 48000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 53
+    },
+  }
+}
+
+update_companies = api_client.update_companies_batch([companyA, companyB])
+```
+## Troubleshooting
+
+When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
+In order to resolve that, add the following line to your Dockerfile
+```
+ENV TZ=UTC
+```
+or you could add `RUN apt-get install tzdata` in the Dockerfile.
+
+## Other integrations
+
+To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
+
+[ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
+[ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
+[ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
+[ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+[ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
+
+[link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
+[link-package]: https://pypi.python.org/pypi/moesifwsgi
+[link-language]: https://pypi.python.org/pypi/moesifwsgi
+[link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
+[link-source]: https://github.com/Moesif/moesifwsgi
```

### Comparing `moesifwsgi-1.8.1/README.md` & `moesifwsgi-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/client_ip.py` & `moesifwsgi-1.8.2/moesifwsgi/client_ip.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/config_manager.py` & `moesifwsgi-1.8.2/moesifwsgi/config_manager.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/event_mapper.py` & `moesifwsgi-1.8.2/moesifwsgi/event_mapper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/http_response_catcher.py` & `moesifwsgi-1.8.2/moesifwsgi/http_response_catcher.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/logger_helper.py` & `moesifwsgi-1.8.2/moesifwsgi/logger_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/middleware.py` & `moesifwsgi-1.8.2/moesifwsgi/middleware.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import atexit
 import logging
 
 from moesifapi.moesif_api_client import *
 from moesifpythonrequest.app_config.app_config import AppConfig
 from moesifpythonrequest.start_capture.start_capture import StartCapture
-
+from moesifapi.api_helper import *
 from .client_ip import ClientIp
 from .event_mapper import EventMapper
 from .http_response_catcher import HttpResponseCatcher
 from .logger_helper import LoggerHelper
 from .moesif_data_holder import DataHolder
 from .parse_body import ParseBody
 from .update_companies import Company
@@ -182,17 +182,21 @@
 
         # Add proportionate weight to the event for sampling percentage lower than 100
         event_data.weight = 1 if event_sampling_percentage == 0 else math.floor(100 / event_sampling_percentage)
         try:
             # Add Event to the queue if able and count the dropped event if at capacity
             if self.worker_pool.add_event(event_data):
                 logger.debug("Add Event to the queue")
+                if self.DEBUG:
+                    logger.debug("Event added to the queue - " + APIHelper.json_serialize(event_data))
             else:
                 self.dropped_events += 1
                 logger.info("Dropped Event due to queue capacity drop_count=" + str(self.dropped_events))
+                if self.DEBUG:
+                    logger.debug("Event dropped - " + APIHelper.json_serialize(event_data))
         # add_event does not throw exceptions so this is unexepected
         except Exception as ex:
             logger.exception("Error while adding event to the queue for", ex)
 
 
     def process_data(self, data):
         # Prepare Event Request Model
```

### Comparing `moesifwsgi-1.8.1/moesifwsgi/moesif_data_holder.py` & `moesifwsgi-1.8.2/moesifwsgi/moesif_data_holder.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/parse_body.py` & `moesifwsgi-1.8.2/moesifwsgi/parse_body.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/regex_config_helper.py` & `moesifwsgi-1.8.2/moesifwsgi/regex_config_helper.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/update_companies.py` & `moesifwsgi-1.8.2/moesifwsgi/update_companies.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/update_users.py` & `moesifwsgi-1.8.2/moesifwsgi/update_users.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi/workers.py` & `moesifwsgi-1.8.2/moesifwsgi/workers.py`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/moesifwsgi.egg-info/PKG-INFO` & `moesifwsgi-1.8.2/moesifwsgi.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,456 +1,16 @@
 Metadata-Version: 2.1
 Name: moesifwsgi
-Version: 1.8.1
+Version: 1.8.2
 Summary: Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)
 Home-page: https://www.moesif.com/docs/server-integration/python-wsgi/
 Author: Moesif, Inc
 Author-email: xing@moesif.com
 License: Apache Software License
-Description: # Moesif Middleware for Python WSGI based Frameworks
-        
-        [![Built For][ico-built-for]][link-built-for]
-        [![Latest Version][ico-version]][link-package]
-        [![Language Versions][ico-language]][link-language]
-        [![Software License][ico-license]][link-license]
-        [![Source Code][ico-source]][link-source]
-        
-        WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
-        Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
-        
-        [Source Code on GitHub](https://github.com/moesif/moesifwsgi)
-        
-        [WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
-        is a standard (PEP 3333) that describes
-        how a web server communicates with web applications. Many Python Frameworks
-        are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
-        [Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
-        Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
-        easily integrate with [Moesif](https://www.moesif.com).
-        
-        ## How to install
-        
-        ```shell
-        pip install moesifwsgi
-        ```
-        
-        ## How to use
-        
-        ### Flask
-        
-        Wrap your wsgi_app with the Moesif middleware.
-        
-        ```python
-        from moesifwsgi import MoesifMiddleware
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
-        After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
-        
-        You can always find your Moesif Application Id at any time by logging 
-        into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
-        and then clicking _API Keys_.
-        
-        For an example with Flask, see example in the `/examples/flask` folder of this repo.
-        
-        ### Bottle
-        Wrap your bottle app with the Moesif middleware.
-        
-        ```python
-        
-        from moesifwsgi import MoesifMiddleware
-        
-        app = bottle.Bottle()
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'LOG_BODY': True,
-            # ... For other options see below.
-        }
-        
-        bottle.run(app=MoesifMiddleware(app, moesif_settings))
-        
-        ```
-        
-        For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
-        
-        ### Pyramid
-        
-        
-        ```python
-        from pyramid.config import Configurator
-        from moesifwsgi import MoesifMiddleware
-        
-        if __name__ == '__main__':
-            config = Configurator()
-            config.add_route('hello', '/')
-            config.scan()
-            app = config.make_wsgi_app()
-        
-            # configure your moesif settings
-            moesif_settings = {
-                'APPLICATION_ID': 'Your Moesif Application Id',
-                'LOG_BODY': True,
-                # ... For other options see below.
-            }
-            # Put middleware
-            app = MoesifMiddleware(app, moesif_settings)
-        
-            server = make_server('0.0.0.0', 8080, app)
-            server.serve_forever()
-        
-        ```
-        ### Other WSGI frameworks
-        
-        If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
-        Please read the documentation for your specific framework on how to add middleware.
-        
-        ## Configuration options
-        
-        The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
-        Also, Moesif adds the following to the environ variable
-        ```
-        environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
-        environ["moesif.response_body_chunks"] - A response body chunks
-        environ["moesif.response_headers"] - A dict representing the response headers
-        ```
-        
-        #### __`APPLICATION_ID`__
-        (__required__), _string_, is obtained via your Moesif Account, this is required.
-        
-        #### __`SKIP`__
-        (optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
-        and returns true if you want to skip this particular event.
-        
-        #### __`IDENTIFY_USER`__
-        (optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        #### __`IDENTIFY_COMPANY`__
-        (optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
-        
-        #### __`GET_METADATA`__
-        (optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
-        returns a dictionary (must be able to be encoded into JSON). This allows your
-        to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
-        
-        #### __`GET_SESSION_TOKEN`__
-        (optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        #### __`MASK_EVENT_MODEL`__
-        (optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
-        
-        #### __`DEBUG`__
-        (optional) _boolean_, a flag to see debugging messages.
-        
-        #### __`LOG_BODY`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        #### __`EVENT_QUEUE_SIZE`__
-        (optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
-        
-        ### __`EVENT_WORKER_COUNT`__
-        (optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
-        
-        #### __`BATCH_SIZE`__
-        (optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
-        
-        #### __`EVENT_BATCH_TIMEOUT`__
-        (optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
-        
-        #### __`AUTHORIZATION_HEADER_NAME`__
-        (optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
-        
-        #### __`AUTHORIZATION_USER_ID_FIELD`__
-        (optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
-        
-        #### __`BASE_URI`__
-        (optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
-        
-        ### Options specific to outgoing API calls 
-        
-        The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
-        
-        For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
-        
-        If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
-        
-        #### __`CAPTURE_OUTGOING_REQUESTS`__
-        _boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
-        
-        ##### __`GET_METADATA_OUTGOING`__
-        (optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
-        Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
-        returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
-        
-        ##### __`SKIP_OUTGOING`__
-        (optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
-        and returns true if you want to skip this particular event.
-        
-        ##### __`IDENTIFY_USER_OUTGOING`__
-        (optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
-        but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
-        
-        ##### __`IDENTIFY_COMPANY_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
-        
-        ##### __`GET_SESSION_TOKEN_OUTGOING`__
-        (optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
-        
-        ##### __`LOG_BODY_OUTGOING`__
-        (optional) _boolean_, default True, Set to False to remove logging request and response body.
-        
-        ### Example:
-        
-        ```python
-        def identify_user(app, environ, response_headers=dict()):
-            # Your custom code that returns a user id string
-            return "12345"
-        
-        def identify_company(app, environ, response_headers=dict()):
-            # Your custom code that returns a company id string
-            return "67890"
-        
-        def should_skip(app, environ):
-            # Your custom code that returns true to skip logging
-            return "health/probe" in environ.get('PATH_INFO', '')
-        
-        def get_token(app, environ):
-            # If you don't want to use the standard WSGI session token,
-            # add your custom code that returns a string for session/API token
-            return "XXXXXXXXXXXXXX"
-        
-        def mask_event(eventmodel):
-            # Your custom code to change or remove any sensitive fields
-            if 'password' in eventmodel.response.body:
-                eventmodel.response.body['password'] = None
-            return eventmodel
-        
-        def get_metadata(app, environ):
-            return {
-                'datacenter': 'westus',
-                'deployment_version': 'v1.2.3',
-            }
-        
-        moesif_settings = {
-            'APPLICATION_ID': 'Your Moesif Application Id',
-            'DEBUG': False,
-            'LOG_BODY': True,
-            'IDENTIFY_USER': identify_user,
-            'IDENTIFY_COMPANY': identify_company,
-            'GET_SESSION_TOKEN': get_token,
-            'SKIP': should_skip,
-            'MASK_EVENT_MODEL': mask_event,
-            'GET_METADATA': get_metadata,
-            'CAPTURE_OUTGOING_REQUESTS': False
-        }
-        
-        app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
-        
-        ```
-        
-        ## Update User
-        
-        ### Update A Single User
-        Create or update a user profile in Moesif.
-        The metadata field can be any customer demographic or other info you want to store.
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only user_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#users for campaign schema
-        # metadata can be any custom object
-        user = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        update_user = api_client.update_user(user)
-        ```
-        
-        ### Update Users in Batch
-        Similar to update_user, but used to update a list of users in one batch. 
-        Only the `user_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        userA = {
-          'user_id': '12345',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'john@acmeinc.com',
-            'first_name': 'John',
-            'last_name': 'Doe',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 24000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        
-        userB = {
-          'user_id': '54321',
-          'company_id': '67890', # If set, associate user with a company object
-          'metadata': {
-            'email': 'mary@acmeinc.com',
-            'first_name': 'Mary',
-            'last_name': 'Jane',
-            'title': 'Software Engineer',
-            'sales_info': {
-                'stage': 'Customer',
-                'lifetime_value': 48000,
-                'account_owner': 'mary@contoso.com'
-            },
-          }
-        }
-        update_users = api_client.update_users_batch([userA, userB])
-        ```
-        
-        ## Update Company
-        
-        ### Update A Single Company
-        Create or update a company profile in Moesif.
-        The metadata field can be any company demographic or other info you want to store.
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        # Only company_id is required.
-        # Campaign object is optional, but useful if you want to track ROI of acquisition channels
-        # See https://www.moesif.com/docs/api#update-a-company for campaign schema
-        # metadata can be any custom object
-        company = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'campaign': {
-            'utm_source': 'google',
-            'utm_medium': 'cpc', 
-            'utm_campaign': 'adwords',
-            'utm_term': 'api+tooling',
-            'utm_content': 'landing'
-          },
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        update_company = api_client.update_company(company)
-        ```
-        
-        ### Update Companies in Batch
-        Similar to update_company, but used to update a list of companies in one batch. 
-        Only the `company_id` field is required.
-        For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
-        
-        ```python
-        api_client = MoesifAPIClient("Your Moesif Application Id").api
-        
-        companyA = {
-          'company_id': '67890',
-          'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Acme, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 24000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 47
-            },
-          }
-        }
-        
-        companyB = {
-          'company_id': '09876',
-          'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
-          'metadata': {
-            'org_name': 'Contoso, Inc',
-            'plan_name': 'Free',
-            'deal_stage': 'Lead',
-            'mrr': 48000,
-            'demographics': {
-                'alexa_ranking': 500000,
-                'employee_count': 53
-            },
-          }
-        }
-        
-        update_companies = api_client.update_companies_batch([companyA, companyB])
-        ```
-        ## Troubleshooting
-        
-        When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
-        In order to resolve that, add the following line to your Dockerfile
-        ```
-        ENV TZ=UTC
-        ```
-        or you could add `RUN apt-get install tzdata` in the Dockerfile.
-        
-        ## Other integrations
-        
-        To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
-        
-        [ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
-        [ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
-        [ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
-        [ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
-        [ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
-        
-        [link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
-        [link-package]: https://pypi.python.org/pypi/moesifwsgi
-        [link-language]: https://pypi.python.org/pypi/moesifwsgi
-        [link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
-        [link-source]: https://github.com/Moesif/moesifwsgi
-        
 Keywords: log analysis restful api development debug wsgi flask bottle http middleware
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Internet :: Log Analysis
 Classifier: Topic :: Software Development :: Debuggers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: License :: OSI Approved :: Apache Software License
@@ -465,7 +25,447 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
+License-File: LICENSE
+
+# Moesif Middleware for Python WSGI based Frameworks
+
+[![Built For][ico-built-for]][link-built-for]
+[![Latest Version][ico-version]][link-package]
+[![Language Versions][ico-language]][link-language]
+[![Software License][ico-license]][link-license]
+[![Source Code][ico-source]][link-source]
+
+WSGI middleware that automatically logs _incoming_ or _outgoing_ API calls and sends to [Moesif](https://www.moesif.com) for API analytics and monitoring.
+Supports Python Frameworks built on WSGI such as Flask, Bottle, and Pyramid.
+
+[Source Code on GitHub](https://github.com/moesif/moesifwsgi)
+
+[WSGI (Web Server Gateway Interface)](https://wsgi.readthedocs.io/en/latest/)
+is a standard (PEP 3333) that describes
+how a web server communicates with web applications. Many Python Frameworks
+are build on top of WSGI, such as [Flask](http://flask.pocoo.org/),
+[Bottle](https://bottlepy.org/docs/dev/), [Pyramid](https://trypyramid.com/) etc.
+Moesif WSGI Middleware help APIs that are build on top of these Frameworks to
+easily integrate with [Moesif](https://www.moesif.com).
+
+## How to install
+
+```shell
+pip install moesifwsgi
+```
+
+## How to use
+
+### Flask
+
+Wrap your wsgi_app with the Moesif middleware.
+
+```python
+from moesifwsgi import MoesifMiddleware
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+Your Moesif Application Id can be found in the [_Moesif Portal_](https://www.moesif.com/).
+After signing up for a Moesif account, your Moesif Application Id will be displayed during the onboarding steps. 
+
+You can always find your Moesif Application Id at any time by logging 
+into the [_Moesif Portal_](https://www.moesif.com/), click on the top right menu,
+and then clicking _API Keys_.
+
+For an example with Flask, see example in the `/examples/flask` folder of this repo.
+
+### Bottle
+Wrap your bottle app with the Moesif middleware.
+
+```python
+
+from moesifwsgi import MoesifMiddleware
+
+app = bottle.Bottle()
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'LOG_BODY': True,
+    # ... For other options see below.
+}
+
+bottle.run(app=MoesifMiddleware(app, moesif_settings))
+
+```
+
+For an example with Bottle, see example in the `/examples/bottle` folder of this repo.
+
+### Pyramid
+
+
+```python
+from pyramid.config import Configurator
+from moesifwsgi import MoesifMiddleware
+
+if __name__ == '__main__':
+    config = Configurator()
+    config.add_route('hello', '/')
+    config.scan()
+    app = config.make_wsgi_app()
+
+    # configure your moesif settings
+    moesif_settings = {
+        'APPLICATION_ID': 'Your Moesif Application Id',
+        'LOG_BODY': True,
+        # ... For other options see below.
+    }
+    # Put middleware
+    app = MoesifMiddleware(app, moesif_settings)
+
+    server = make_server('0.0.0.0', 8080, app)
+    server.serve_forever()
+
+```
+### Other WSGI frameworks
+
+If you are using a framework that is built on top of WSGI, it should work just by adding the Moesif middleware.
+Please read the documentation for your specific framework on how to add middleware.
+
+## Configuration options
+
+The app is the original WSGI app instance, and the environ is a [WSGI environ](http://wsgi.readthedocs.io/en/latest/definitions.html).
+Also, Moesif adds the following to the environ variable
+```
+environ['moesif.request_body'] - A json object or base64 encoded string if couldn't parse the request body as json 
+environ["moesif.response_body_chunks"] - A response body chunks
+environ["moesif.response_headers"] - A dict representing the response headers
+```
+
+#### __`APPLICATION_ID`__
+(__required__), _string_, is obtained via your Moesif Account, this is required.
+
+#### __`SKIP`__
+(optional) _(app, environ) => boolean_, a function that takes a WSGI app and an environ,
+and returns true if you want to skip this particular event.
+
+#### __`IDENTIFY_USER`__
+(optional, but highly recommended) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+#### __`IDENTIFY_COMPANY`__
+(optional) _(app, environ, response_headers) => string_, a function that takes an app, an environ and an optional parameter response headers, and returns a string that is the company id for this event.
+
+#### __`GET_METADATA`__
+(optional) _(app, environ) => dictionary_, a function that takes an app and an environ, and
+returns a dictionary (must be able to be encoded into JSON). This allows your
+to associate this event with custom metadata. For example, you may want to save a VM instance_id, a trace_id, or a tenant_id with the request.
+
+#### __`GET_SESSION_TOKEN`__
+(optional) _(app, environ) => string_, a function that takes an app and an environ, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+#### __`MASK_EVENT_MODEL`__
+(optional) _(EventModel) => EventModel_, a function that takes an EventModel and returns an EventModel with desired data removed. The return value must be a valid EventModel required by Moesif data ingestion API. For details regarding EventModel please see the [Moesif Python API Documentation](https://www.moesif.com/docs/api?python).
+
+#### __`DEBUG`__
+(optional) _boolean_, a flag to see debugging messages.
+
+#### __`LOG_BODY`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+#### __`EVENT_QUEUE_SIZE`__
+(optional) __int__, default 10000, the maximum number of event objects queued in memory pending upload to Moesif.  If the queue is full additional calls to `MoesifMiddleware` will return immediately without logging the event, so this number should be set based on the expected event size and memory capacity
+
+### __`EVENT_WORKER_COUNT`__
+(optional) __int__, default 2, the number of worker threads to use for uploading events to Moesif.  If you have a large number of events being logged, increasing this number can improve upload performance.
+
+#### __`BATCH_SIZE`__
+(optional) __int__, default 100, Maximum batch size when sending events to Moesif when reading from the queue
+
+#### __`EVENT_BATCH_TIMEOUT`__
+(optional) __int__, default 2, Maximum time in seconds to wait before sending a batch of events to Moesif when reading from the queue
+
+#### __`AUTHORIZATION_HEADER_NAME`__
+(optional) _string_, A request header field name used to identify the User in Moesif. Default value is `authorization`. Also, supports a comma separated string. We will check headers in order like `"X-Api-Key,Authorization"`.
+
+#### __`AUTHORIZATION_USER_ID_FIELD`__
+(optional) _string_, A field name used to parse the User from authorization header in Moesif. Default value is `sub`.
+
+#### __`BASE_URI`__
+(optional) _string_, A local proxy hostname when sending traffic via secure proxy. Please set this field when using secure proxy. For more details, refer [secure proxy documentation.](https://www.moesif.com/docs/platform/secure-proxy/#2-configure-moesif-sdk)
+
+### Options specific to outgoing API calls 
+
+The options below are applicable to outgoing API calls (calls you initiate using the Python [Requests](http://docs.python-requests.org/en/master/) lib to third parties like Stripe or to your own services.
+
+For options that use the request and response as input arguments, these use the [Requests](http://docs.python-requests.org/en/master/api/) lib's request or response objects.
+
+If you are not using WSGI, you can import the [moesifpythonrequest](https://github.com/Moesif/moesifpythonrequest) directly.
+
+#### __`CAPTURE_OUTGOING_REQUESTS`__
+_boolean_, Default False. Set to True to capture all outgoing API calls. False will disable this functionality. 
+
+##### __`GET_METADATA_OUTGOING`__
+(optional) _(req, res) => dictionary_, a function that enables you to return custom metadata associated with the logged API calls. 
+Takes in the [Requests](http://docs.python-requests.org/en/master/api/) request and response object as arguments. You should implement a function that 
+returns a dictionary containing your custom metadata. (must be able to be encoded into JSON). For example, you may want to save a VM instance_id, a trace_id, or a resource_id with the request.
+
+##### __`SKIP_OUTGOING`__
+(optional) _(req, res) => boolean_, a function that takes a [Requests](http://docs.python-requests.org/en/master/api/) request and response,
+and returns true if you want to skip this particular event.
+
+##### __`IDENTIFY_USER_OUTGOING`__
+(optional, but highly recommended) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the user id used by your system. While Moesif tries to identify users automatically,
+but different frameworks and your implementation might be very different, it would be helpful and much more accurate to provide this function.
+
+##### __`IDENTIFY_COMPANY_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the company id for this event.
+
+##### __`GET_SESSION_TOKEN_OUTGOING`__
+(optional) _(req, res) => string_, a function that takes [Requests](http://docs.python-requests.org/en/master/api/) request and response, and returns a string that is the session token for this event. Again, Moesif tries to get the session token automatically, but if you setup is very different from standard, this function will be very help for tying events together, and help you replay the events.
+
+##### __`LOG_BODY_OUTGOING`__
+(optional) _boolean_, default True, Set to False to remove logging request and response body.
+
+### Example:
+
+```python
+def identify_user(app, environ, response_headers=dict()):
+    # Your custom code that returns a user id string
+    return "12345"
+
+def identify_company(app, environ, response_headers=dict()):
+    # Your custom code that returns a company id string
+    return "67890"
+
+def should_skip(app, environ):
+    # Your custom code that returns true to skip logging
+    return "health/probe" in environ.get('PATH_INFO', '')
+
+def get_token(app, environ):
+    # If you don't want to use the standard WSGI session token,
+    # add your custom code that returns a string for session/API token
+    return "XXXXXXXXXXXXXX"
+
+def mask_event(eventmodel):
+    # Your custom code to change or remove any sensitive fields
+    if 'password' in eventmodel.response.body:
+        eventmodel.response.body['password'] = None
+    return eventmodel
+
+def get_metadata(app, environ):
+    return {
+        'datacenter': 'westus',
+        'deployment_version': 'v1.2.3',
+    }
+
+moesif_settings = {
+    'APPLICATION_ID': 'Your Moesif Application Id',
+    'DEBUG': False,
+    'LOG_BODY': True,
+    'IDENTIFY_USER': identify_user,
+    'IDENTIFY_COMPANY': identify_company,
+    'GET_SESSION_TOKEN': get_token,
+    'SKIP': should_skip,
+    'MASK_EVENT_MODEL': mask_event,
+    'GET_METADATA': get_metadata,
+    'CAPTURE_OUTGOING_REQUESTS': False
+}
+
+app.wsgi_app = MoesifMiddleware(app.wsgi_app, moesif_settings)
+
+```
+
+## Update User
+
+### Update A Single User
+Create or update a user profile in Moesif.
+The metadata field can be any customer demographic or other info you want to store.
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-user).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only user_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#users for campaign schema
+# metadata can be any custom object
+user = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+update_user = api_client.update_user(user)
+```
+
+### Update Users in Batch
+Similar to update_user, but used to update a list of users in one batch. 
+Only the `user_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-users-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+userA = {
+  'user_id': '12345',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'john@acmeinc.com',
+    'first_name': 'John',
+    'last_name': 'Doe',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 24000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+
+userB = {
+  'user_id': '54321',
+  'company_id': '67890', # If set, associate user with a company object
+  'metadata': {
+    'email': 'mary@acmeinc.com',
+    'first_name': 'Mary',
+    'last_name': 'Jane',
+    'title': 'Software Engineer',
+    'sales_info': {
+        'stage': 'Customer',
+        'lifetime_value': 48000,
+        'account_owner': 'mary@contoso.com'
+    },
+  }
+}
+update_users = api_client.update_users_batch([userA, userB])
+```
+
+## Update Company
+
+### Update A Single Company
+Create or update a company profile in Moesif.
+The metadata field can be any company demographic or other info you want to store.
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-a-company).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+# Only company_id is required.
+# Campaign object is optional, but useful if you want to track ROI of acquisition channels
+# See https://www.moesif.com/docs/api#update-a-company for campaign schema
+# metadata can be any custom object
+company = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'campaign': {
+    'utm_source': 'google',
+    'utm_medium': 'cpc', 
+    'utm_campaign': 'adwords',
+    'utm_term': 'api+tooling',
+    'utm_content': 'landing'
+  },
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+update_company = api_client.update_company(company)
+```
+
+### Update Companies in Batch
+Similar to update_company, but used to update a list of companies in one batch. 
+Only the `company_id` field is required.
+For details, visit the [Python API Reference](https://www.moesif.com/docs/api?python#update-companies-in-batch).
+
+```python
+api_client = MoesifAPIClient("Your Moesif Application Id").api
+
+companyA = {
+  'company_id': '67890',
+  'company_domain': 'acmeinc.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Acme, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 24000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 47
+    },
+  }
+}
+
+companyB = {
+  'company_id': '09876',
+  'company_domain': 'contoso.com', # If domain is set, Moesif will enrich your profiles with publicly available info 
+  'metadata': {
+    'org_name': 'Contoso, Inc',
+    'plan_name': 'Free',
+    'deal_stage': 'Lead',
+    'mrr': 48000,
+    'demographics': {
+        'alexa_ranking': 500000,
+        'employee_count': 53
+    },
+  }
+}
+
+update_companies = api_client.update_companies_batch([companyA, companyB])
+```
+## Troubleshooting
+
+When using Docker with Ubuntu based image, if events are not being captured, it could be possible as the image can't find any timezone configuration. 
+In order to resolve that, add the following line to your Dockerfile
+```
+ENV TZ=UTC
+```
+or you could add `RUN apt-get install tzdata` in the Dockerfile.
+
+## Other integrations
+
+To view more documentation on integration options, please visit __[the Integration Options Documentation](https://www.moesif.com/docs/getting-started/integration-options/).__
+
+[ico-built-for]: https://img.shields.io/badge/built%20for-python%20wsgi-blue.svg
+[ico-version]: https://img.shields.io/pypi/v/moesifwsgi.svg
+[ico-language]: https://img.shields.io/pypi/pyversions/moesifwsgi.svg
+[ico-license]: https://img.shields.io/badge/License-Apache%202.0-green.svg
+[ico-source]: https://img.shields.io/github/last-commit/moesif/moesifwsgi.svg?style=social
+
+[link-built-for]: https://en.wikipedia.org/wiki/Web_Server_Gateway_Interface
+[link-package]: https://pypi.python.org/pypi/moesifwsgi
+[link-language]: https://pypi.python.org/pypi/moesifwsgi
+[link-license]: https://raw.githubusercontent.com/Moesif/moesifwsgi/master/LICENSE
+[link-source]: https://github.com/Moesif/moesifwsgi
```

### Comparing `moesifwsgi-1.8.1/moesifwsgi.egg-info/SOURCES.txt` & `moesifwsgi-1.8.2/moesifwsgi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moesifwsgi-1.8.1/setup.py` & `moesifwsgi-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 setup(
     name='moesifwsgi',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.8.1',
+    version='1.8.2',
 
     description='Moesif Middleware for Python WSGI based platforms (Flask, Bottle & Others)',
     long_description=long_description,
     long_description_content_type="text/markdown",
 
     # The project's main homepage.
     url='https://www.moesif.com/docs/server-integration/python-wsgi/',
```

