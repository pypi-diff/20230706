# Comparing `tmp/rq-exporter-2.0.0.tar.gz` & `tmp/rq-exporter-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rq-exporter-2.0.0.tar", last modified: Fri Jul 15 09:25:34 2022, max compression
+gzip compressed data, was "rq-exporter-2.1.0.tar", last modified: Thu Jul  6 17:29:04 2023, max compression
```

## Comparing `rq-exporter-2.0.0.tar` & `rq-exporter-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:25:34.339329 rq-exporter-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14480 2022-07-15 09:25:34.339329 rq-exporter-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13653 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:25:34.339329 rq-exporter-2.0.0/rq_exporter/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7277 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1841 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1873 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/rq_exporter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-15 09:25:34.339329 rq-exporter-2.0.0/rq_exporter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14480 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-15 09:25:34.000000 rq-exporter-2.0.0/rq_exporter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-15 09:25:34.339329 rq-exporter-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1507 2022-07-15 09:25:26.000000 rq-exporter-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:29:04.244000 rq-exporter-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-06 17:29:04.244000 rq-exporter-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13895 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:29:04.244000 rq-exporter-2.1.0/rq_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/rq_exporter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 17:29:04.244000 rq-exporter-2.1.0/rq_exporter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 17:29:04.000000 rq-exporter-2.1.0/rq_exporter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 17:29:04.244000 rq-exporter-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-07-06 17:28:55.000000 rq-exporter-2.1.0/setup.py
```

### Comparing `rq-exporter-2.0.0/LICENSE` & `rq-exporter-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rq-exporter-2.0.0/PKG-INFO` & `rq-exporter-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rq-exporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: Prometheus exporter for Python RQ (Redis Queue)
 Home-page: https://github.com/mdawar/rq-exporter
 Author: Pierre Mdawar
 Author-email: pierre@mdawar.dev
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -32,37 +31,37 @@
 
 [![Grafana dashboard](https://grafana.com/api/dashboards/12196/images/8017/image)](https://grafana.com/grafana/dashboards/12196)
 
 ## Installation
 
 Install the Python package:
 
-```console
+```sh
 $ # Install the latest version
 $ pip install rq-exporter
-$ # Or you can install a specific version
-$ pip install rq-exporter==1.0.0
+$ # Or install a specific version
+$ pip install rq-exporter==2.1.0
 ```
 
 Or download the [Docker image](https://hub.docker.com/r/mdawar/rq-exporter):
 
-```console
+```sh
 $ # Pull the latest image
 $ docker pull mdawar/rq-exporter
-$ # Or you can pull a specific version
-$ docker pull mdawar/rq-exporter:v1.0.0
+$ # Or pull a specific version
+$ docker pull mdawar/rq-exporter:v2.1.0
 ```
 
 The releases are available as [Docker image tags](https://hub.docker.com/r/mdawar/rq-exporter/tags).
 
 ## Usage
 
 **Python package**:
 
-```console
+```sh
 $ # Start the exporter on port 9726
 $ rq-exporter
 $ # Start the exporter on a specific port and host (Default: 0.0.0.0:9726)
 $ rq-exporter --host localhost --port 8080
 $ # By default the exporter will connect to Redis on `localhost` port `6379`
 $ # You can specify a Redis URL
 $ rq-exporter --redis-url redis://:123456@redis_host:6379/0
@@ -70,15 +69,15 @@
 $ rq-exporter --redis-host 192.168.1.10 --redis-port 6380 --redis-pass 123456 --redis-db 1
 $ # You can also specify a password file path (eg: mounted Docker secret)
 $ rq-exporter --redis-pass-file /run/secrets/redis_pass
 ```
 
 **Docker image**:
 
-```console
+```sh
 $ # Run the exporter and publish the port 9726 on the host
 $ docker run -it -p 9726:9726 rq-exporter
 $ # Use the -d option to run the container in the background (detached)
 $ docker run -d -p 9726:9726 rq-exporter
 $ # All the command line arguments will be passed to rq-exporter
 $ docker run -it -p 9726:9726 rq-exporter --redis-host redis --redis-pass 123456
 $ # You can also configure the exporter using environment variables
@@ -115,15 +114,15 @@
 | --------------------------------------- | ------- | -------------------------------------------- |
 | `rq_request_processing_seconds_count`   | Summary | Number of times the RQ data were collected   |
 | `rq_request_processing_seconds_sum`     | Summary | Total sum of time spent collecting RQ data   |
 | `rq_request_processing_seconds_created` | Gauge   | Time created at (`time.time()` return value) |
 
 Example:
 
-```bash
+```sh
 # HELP rq_request_processing_seconds Time spent collecting RQ data
 # TYPE rq_request_processing_seconds summary
 rq_request_processing_seconds_count 1.0
 rq_request_processing_seconds_sum 0.029244607000009637
 # TYPE rq_request_processing_seconds_created gauge
 rq_request_processing_seconds_created 1.5878023726039658e+09
 # HELP rq_workers RQ workers
@@ -140,43 +139,44 @@
 rq_jobs{queue="default", status="scheduled"} 2.0
 ```
 
 ## Configuration
 
 You can configure the exporter using command line arguments or environment variables:
 
-| CLI Argument        | Env Variable              | Default Value                                           | Description                                                     |
-| ------------------- | ------------------------- | ------------------------------------------------------- | --------------------------------------------------------------- |
-| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                 |
-| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                 |
-| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`  |
-| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                 |
-| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                               |
-| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                           |
-| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel host                                             |
-| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port                                             |
-| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                      |
-| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                  |
-| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret) |
-| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                 |
-| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                  |
-| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                   |
-| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                   |
-| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                 |
+| CLI Argument        | Env Variable              | Default Value                                           | Description                                                              |
+| ------------------- | ------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------------ |
+| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                          |
+| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                          |
+| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`           |
+| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                          |
+| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                                        |
+| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                                    |
+| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel hosts separated by commas e.g `sentinel1,sentinel2:26380` |
+| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port, default port used when not set with the host        |
+| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                               |
+| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                           |
+| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret)          |
+| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                          |
+| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                           |
+| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                            |
+| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                            |
+| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                          |
 
-**Note**:
+**Notes**:
 
 - When Redis URL is set using `--redis-url` or `RQ_REDIS_URL` the other Redis options will be ignored
 - When the Redis password is set using `--redis-pass-file` or `RQ_REDIS_PASS_FILE`, then `--redis-pass` and `RQ_REDIS_PASS` will be ignored
+- The Sentinel port will default to the value of `--sentinel-port` if not set for each host with `--sentinel-host` or `RQ_SENTINEL_HOST`
 
 ## Serving with Gunicorn
 
 The WSGI application can be created using the `rq_exporter.create_app()` function:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --log-level info
 ```
 
 Example [`Dockerfile`](https://github.com/mdawar/rq-exporter/blob/master/Dockerfile.gunicorn) to create a **Docker** image to serve the application with **Gunicorn**
 
 ```dockerfile
 FROM mdawar/rq-exporter:latest
@@ -200,96 +200,98 @@
 - `rq_request_processing_seconds_sum`
 - `rq_request_processing_seconds_created`
 
 This is fine if you don't care about these metrics, these are only for measuring the count and time processing the RQ data, so the other RQ metrics are not going to be affected.
 
 But you can still use multiple threads with 1 worker process to handle multiple concurrent requests:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --threads 2
 ```
 
 ## Building the Docker Image
 
-```console
+```sh
 $ # Build the docker image and tag it rq-exporter:latest
 $ docker build -t rq-exporter .
+$ # Or
+$ make build
 
-$ # M1 MacOs Build the docker image and tag it rq-exporter:latest
+$ # M1 MacOS Build the docker image and tag it rq-exporter:latest
 $ docker buildx build --platform linux/amd64 -t rq-exporter .
 ```
 
-The image can also be built using `docker-compose`:
+The image can also be built using `docker compose`:
 
-```console
-$ docker-compose build
+```sh
+$ docker compose build
 ```
 
-Check out the `docker-compose.yml` file for usage example.
+Check the `docker-compose.yml` file for usage example.
 
 ## Development
 
 To start a full development environment with **RQ** workers, **Prometheus** and **Grafana**:
 
-```console
-$ docker-compose up
+```sh
+$ docker compose up
 $ # If you want to start multiple workers use the --compatibility flag
-$ # which will make docker-compose read the `deploy` section and start multiple replicas
-$ docker-compose --compatibility up
+$ # which will make docker compose read the `deploy` section and start multiple replicas
+$ docker compose --compatibility up
 ```
 
 You can access the services on these ports on your local machine:
 
 - **RQ exporter**: [`9726`](http://localhost:9726)
 - **Redis**: [`6379`](http://localhost:6379)
 - **RQ Dashboard**: [`9181`](http://localhost:9181)
 - **Prometheus**: [`9090`](http://localhost:9090)
 - **Grafana**: [`3000`](http://localhost:3000) (Login using `admin:admin`)
 
 You can specify the services that you want to start by their name in the `docker-compose.yml` file:
 
-```console
+```sh
 $ # Example starting only the `rq_exporter` and `redis` services
-$ docker-compose up rq_exporter redis
+$ docker compose up rq_exporter redis
 ```
 
 To run more workers and enqueue more jobs you can scale the `worker` and `enqueue` services:
 
-```console
+```sh
 $ # Run 5 workers
-$ docker-compose up -d --scale worker=5
+$ docker compose up -d --scale worker=5
 $ # Enqueue more jobs
 $ # Scale the enqueue service and the workers
-$ docker-compose up -d --scale worker=5 --scale enqueue=2
+$ docker compose up -d --scale worker=5 --scale enqueue=2
 ```
 
 To cleanup after development:
 
-```console
+```sh
 $ # Use -v to remove volumes
-$ docker-compose down -v
+$ docker compose down -v
 ```
 
 You can also start another `rq-exporter` instance that collects stats from a project using custom **RQ** `Worker` and `Queue` classes:
 
-```console
+```sh
 $ # Using -f to pass multiple docker-compose files
 $ # docker-compose.custom.yml defines services using custom RQ classes
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml up
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml up
 $ # To cleanup you need to also pass the same files
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml down
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml down
 ```
 
 A new **RQ exporter** instance will be exposed on port `9727` on your local machine.
 
-**Note**: If you don't have `docker-compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
+**Note**: If you don't have `docker compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
 
 If you want to use the package manually:
 
-```console
+```sh
 $ # Clone the repository
 $ git clone <REPO_URL>
 $ # Change to the project directory
 $ cd rq-exporter
 $ # Create a new virtualenv
 $ python -m venv /path/to/env
 $ # Activate the environment
@@ -300,21 +302,21 @@
 $ python -m rq_exporter
 $ # You can configure the exporter using command line arguments
 $ python -m rq_exporter --port 8080
 ```
 
 ## Running the Tests
 
-```console
+```sh
+$ make test
+$ # Or
 $ python -m unittest
 ```
 
 ## Contributing
 
 1. Fork the [repository](https://github.com/mdawar/rq-exporter)
 2. Clone the forked repository `git clone <URL>`
 3. Create a new feature branch `git checkout -b <BRANCH_NAME>`
 4. Make changes and add tests if needed and commit your changes `git commit -am "Your commit message"`
 5. Push the new branch to Github `git push origin <BRANCH_NAME>`
 6. Create a pull request
-
-
```

### Comparing `rq-exporter-2.0.0/README.md` & `rq-exporter-2.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 [![Grafana dashboard](https://grafana.com/api/dashboards/12196/images/8017/image)](https://grafana.com/grafana/dashboards/12196)
 
 ## Installation
 
 Install the Python package:
 
-```console
+```sh
 $ # Install the latest version
 $ pip install rq-exporter
-$ # Or you can install a specific version
-$ pip install rq-exporter==1.0.0
+$ # Or install a specific version
+$ pip install rq-exporter==2.1.0
 ```
 
 Or download the [Docker image](https://hub.docker.com/r/mdawar/rq-exporter):
 
-```console
+```sh
 $ # Pull the latest image
 $ docker pull mdawar/rq-exporter
-$ # Or you can pull a specific version
-$ docker pull mdawar/rq-exporter:v1.0.0
+$ # Or pull a specific version
+$ docker pull mdawar/rq-exporter:v2.1.0
 ```
 
 The releases are available as [Docker image tags](https://hub.docker.com/r/mdawar/rq-exporter/tags).
 
 ## Usage
 
 **Python package**:
 
-```console
+```sh
 $ # Start the exporter on port 9726
 $ rq-exporter
 $ # Start the exporter on a specific port and host (Default: 0.0.0.0:9726)
 $ rq-exporter --host localhost --port 8080
 $ # By default the exporter will connect to Redis on `localhost` port `6379`
 $ # You can specify a Redis URL
 $ rq-exporter --redis-url redis://:123456@redis_host:6379/0
@@ -47,15 +47,15 @@
 $ rq-exporter --redis-host 192.168.1.10 --redis-port 6380 --redis-pass 123456 --redis-db 1
 $ # You can also specify a password file path (eg: mounted Docker secret)
 $ rq-exporter --redis-pass-file /run/secrets/redis_pass
 ```
 
 **Docker image**:
 
-```console
+```sh
 $ # Run the exporter and publish the port 9726 on the host
 $ docker run -it -p 9726:9726 rq-exporter
 $ # Use the -d option to run the container in the background (detached)
 $ docker run -d -p 9726:9726 rq-exporter
 $ # All the command line arguments will be passed to rq-exporter
 $ docker run -it -p 9726:9726 rq-exporter --redis-host redis --redis-pass 123456
 $ # You can also configure the exporter using environment variables
@@ -92,15 +92,15 @@
 | --------------------------------------- | ------- | -------------------------------------------- |
 | `rq_request_processing_seconds_count`   | Summary | Number of times the RQ data were collected   |
 | `rq_request_processing_seconds_sum`     | Summary | Total sum of time spent collecting RQ data   |
 | `rq_request_processing_seconds_created` | Gauge   | Time created at (`time.time()` return value) |
 
 Example:
 
-```bash
+```sh
 # HELP rq_request_processing_seconds Time spent collecting RQ data
 # TYPE rq_request_processing_seconds summary
 rq_request_processing_seconds_count 1.0
 rq_request_processing_seconds_sum 0.029244607000009637
 # TYPE rq_request_processing_seconds_created gauge
 rq_request_processing_seconds_created 1.5878023726039658e+09
 # HELP rq_workers RQ workers
@@ -117,43 +117,44 @@
 rq_jobs{queue="default", status="scheduled"} 2.0
 ```
 
 ## Configuration
 
 You can configure the exporter using command line arguments or environment variables:
 
-| CLI Argument        | Env Variable              | Default Value                                           | Description                                                     |
-| ------------------- | ------------------------- | ------------------------------------------------------- | --------------------------------------------------------------- |
-| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                 |
-| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                 |
-| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`  |
-| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                 |
-| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                               |
-| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                           |
-| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel host                                             |
-| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port                                             |
-| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                      |
-| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                  |
-| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret) |
-| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                 |
-| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                  |
-| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                   |
-| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                   |
-| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                 |
+| CLI Argument        | Env Variable              | Default Value                                           | Description                                                              |
+| ------------------- | ------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------------ |
+| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                          |
+| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                          |
+| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`           |
+| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                          |
+| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                                        |
+| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                                    |
+| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel hosts separated by commas e.g `sentinel1,sentinel2:26380` |
+| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port, default port used when not set with the host        |
+| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                               |
+| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                           |
+| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret)          |
+| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                          |
+| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                           |
+| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                            |
+| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                            |
+| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                          |
 
-**Note**:
+**Notes**:
 
 - When Redis URL is set using `--redis-url` or `RQ_REDIS_URL` the other Redis options will be ignored
 - When the Redis password is set using `--redis-pass-file` or `RQ_REDIS_PASS_FILE`, then `--redis-pass` and `RQ_REDIS_PASS` will be ignored
+- The Sentinel port will default to the value of `--sentinel-port` if not set for each host with `--sentinel-host` or `RQ_SENTINEL_HOST`
 
 ## Serving with Gunicorn
 
 The WSGI application can be created using the `rq_exporter.create_app()` function:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --log-level info
 ```
 
 Example [`Dockerfile`](https://github.com/mdawar/rq-exporter/blob/master/Dockerfile.gunicorn) to create a **Docker** image to serve the application with **Gunicorn**
 
 ```dockerfile
 FROM mdawar/rq-exporter:latest
@@ -177,96 +178,98 @@
 - `rq_request_processing_seconds_sum`
 - `rq_request_processing_seconds_created`
 
 This is fine if you don't care about these metrics, these are only for measuring the count and time processing the RQ data, so the other RQ metrics are not going to be affected.
 
 But you can still use multiple threads with 1 worker process to handle multiple concurrent requests:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --threads 2
 ```
 
 ## Building the Docker Image
 
-```console
+```sh
 $ # Build the docker image and tag it rq-exporter:latest
 $ docker build -t rq-exporter .
+$ # Or
+$ make build
 
-$ # M1 MacOs Build the docker image and tag it rq-exporter:latest
+$ # M1 MacOS Build the docker image and tag it rq-exporter:latest
 $ docker buildx build --platform linux/amd64 -t rq-exporter .
 ```
 
-The image can also be built using `docker-compose`:
+The image can also be built using `docker compose`:
 
-```console
-$ docker-compose build
+```sh
+$ docker compose build
 ```
 
-Check out the `docker-compose.yml` file for usage example.
+Check the `docker-compose.yml` file for usage example.
 
 ## Development
 
 To start a full development environment with **RQ** workers, **Prometheus** and **Grafana**:
 
-```console
-$ docker-compose up
+```sh
+$ docker compose up
 $ # If you want to start multiple workers use the --compatibility flag
-$ # which will make docker-compose read the `deploy` section and start multiple replicas
-$ docker-compose --compatibility up
+$ # which will make docker compose read the `deploy` section and start multiple replicas
+$ docker compose --compatibility up
 ```
 
 You can access the services on these ports on your local machine:
 
 - **RQ exporter**: [`9726`](http://localhost:9726)
 - **Redis**: [`6379`](http://localhost:6379)
 - **RQ Dashboard**: [`9181`](http://localhost:9181)
 - **Prometheus**: [`9090`](http://localhost:9090)
 - **Grafana**: [`3000`](http://localhost:3000) (Login using `admin:admin`)
 
 You can specify the services that you want to start by their name in the `docker-compose.yml` file:
 
-```console
+```sh
 $ # Example starting only the `rq_exporter` and `redis` services
-$ docker-compose up rq_exporter redis
+$ docker compose up rq_exporter redis
 ```
 
 To run more workers and enqueue more jobs you can scale the `worker` and `enqueue` services:
 
-```console
+```sh
 $ # Run 5 workers
-$ docker-compose up -d --scale worker=5
+$ docker compose up -d --scale worker=5
 $ # Enqueue more jobs
 $ # Scale the enqueue service and the workers
-$ docker-compose up -d --scale worker=5 --scale enqueue=2
+$ docker compose up -d --scale worker=5 --scale enqueue=2
 ```
 
 To cleanup after development:
 
-```console
+```sh
 $ # Use -v to remove volumes
-$ docker-compose down -v
+$ docker compose down -v
 ```
 
 You can also start another `rq-exporter` instance that collects stats from a project using custom **RQ** `Worker` and `Queue` classes:
 
-```console
+```sh
 $ # Using -f to pass multiple docker-compose files
 $ # docker-compose.custom.yml defines services using custom RQ classes
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml up
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml up
 $ # To cleanup you need to also pass the same files
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml down
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml down
 ```
 
 A new **RQ exporter** instance will be exposed on port `9727` on your local machine.
 
-**Note**: If you don't have `docker-compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
+**Note**: If you don't have `docker compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
 
 If you want to use the package manually:
 
-```console
+```sh
 $ # Clone the repository
 $ git clone <REPO_URL>
 $ # Change to the project directory
 $ cd rq-exporter
 $ # Create a new virtualenv
 $ python -m venv /path/to/env
 $ # Activate the environment
@@ -277,15 +280,17 @@
 $ python -m rq_exporter
 $ # You can configure the exporter using command line arguments
 $ python -m rq_exporter --port 8080
 ```
 
 ## Running the Tests
 
-```console
+```sh
+$ make test
+$ # Or
 $ python -m unittest
 ```
 
 ## Contributing
 
 1. Fork the [repository](https://github.com/mdawar/rq-exporter)
 2. Clone the forked repository `git clone <URL>`
```

### Comparing `rq-exporter-2.0.0/rq_exporter/__main__.py` & `rq-exporter-2.1.0/rq_exporter/__main__.py`

 * *Files identical despite different names*

### Comparing `rq-exporter-2.0.0/rq_exporter/collector.py` & `rq-exporter-2.1.0/rq_exporter/collector.py`

 * *Files identical despite different names*

### Comparing `rq-exporter-2.0.0/rq_exporter/config.py` & `rq-exporter-2.1.0/rq_exporter/config.py`

 * *Files identical despite different names*

### Comparing `rq-exporter-2.0.0/rq_exporter/exporter.py` & `rq-exporter-2.1.0/rq_exporter/exporter.py`

 * *Files identical despite different names*

### Comparing `rq-exporter-2.0.0/rq_exporter/utils.py` & `rq-exporter-2.1.0/rq_exporter/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,22 @@
 
     # Use password file if provided
     if password_file:
         with open(password_file, 'r') as f:
             password = f.read().strip()
 
     if sentinel:
-        addr_list = [(url, sentinel_port) for url in sentinel.split(",")]
+        addr_list = [
+            (
+                url.split(':')[0],
+                url.split(':')[1] if ':' in url else sentinel_port
+            )
+            for url in sentinel.split(",")
+        ]
+
         sentinel = Sentinel(addr_list, socket_timeout=1)
         return sentinel.master_for(sentinel_master, socket_timeout=1, db=db)
 
     return Redis(host=host, port=port, db=db, password=password)
 
 
 def get_workers_stats(worker_class=None):
```

### Comparing `rq-exporter-2.0.0/rq_exporter.egg-info/PKG-INFO` & `rq-exporter-2.1.0/rq_exporter.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: rq-exporter
-Version: 2.0.0
+Version: 2.1.0
 Summary: Prometheus exporter for Python RQ (Redis Queue)
 Home-page: https://github.com/mdawar/rq-exporter
 Author: Pierre Mdawar
 Author-email: pierre@mdawar.dev
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
@@ -32,37 +31,37 @@
 
 [![Grafana dashboard](https://grafana.com/api/dashboards/12196/images/8017/image)](https://grafana.com/grafana/dashboards/12196)
 
 ## Installation
 
 Install the Python package:
 
-```console
+```sh
 $ # Install the latest version
 $ pip install rq-exporter
-$ # Or you can install a specific version
-$ pip install rq-exporter==1.0.0
+$ # Or install a specific version
+$ pip install rq-exporter==2.1.0
 ```
 
 Or download the [Docker image](https://hub.docker.com/r/mdawar/rq-exporter):
 
-```console
+```sh
 $ # Pull the latest image
 $ docker pull mdawar/rq-exporter
-$ # Or you can pull a specific version
-$ docker pull mdawar/rq-exporter:v1.0.0
+$ # Or pull a specific version
+$ docker pull mdawar/rq-exporter:v2.1.0
 ```
 
 The releases are available as [Docker image tags](https://hub.docker.com/r/mdawar/rq-exporter/tags).
 
 ## Usage
 
 **Python package**:
 
-```console
+```sh
 $ # Start the exporter on port 9726
 $ rq-exporter
 $ # Start the exporter on a specific port and host (Default: 0.0.0.0:9726)
 $ rq-exporter --host localhost --port 8080
 $ # By default the exporter will connect to Redis on `localhost` port `6379`
 $ # You can specify a Redis URL
 $ rq-exporter --redis-url redis://:123456@redis_host:6379/0
@@ -70,15 +69,15 @@
 $ rq-exporter --redis-host 192.168.1.10 --redis-port 6380 --redis-pass 123456 --redis-db 1
 $ # You can also specify a password file path (eg: mounted Docker secret)
 $ rq-exporter --redis-pass-file /run/secrets/redis_pass
 ```
 
 **Docker image**:
 
-```console
+```sh
 $ # Run the exporter and publish the port 9726 on the host
 $ docker run -it -p 9726:9726 rq-exporter
 $ # Use the -d option to run the container in the background (detached)
 $ docker run -d -p 9726:9726 rq-exporter
 $ # All the command line arguments will be passed to rq-exporter
 $ docker run -it -p 9726:9726 rq-exporter --redis-host redis --redis-pass 123456
 $ # You can also configure the exporter using environment variables
@@ -115,15 +114,15 @@
 | --------------------------------------- | ------- | -------------------------------------------- |
 | `rq_request_processing_seconds_count`   | Summary | Number of times the RQ data were collected   |
 | `rq_request_processing_seconds_sum`     | Summary | Total sum of time spent collecting RQ data   |
 | `rq_request_processing_seconds_created` | Gauge   | Time created at (`time.time()` return value) |
 
 Example:
 
-```bash
+```sh
 # HELP rq_request_processing_seconds Time spent collecting RQ data
 # TYPE rq_request_processing_seconds summary
 rq_request_processing_seconds_count 1.0
 rq_request_processing_seconds_sum 0.029244607000009637
 # TYPE rq_request_processing_seconds_created gauge
 rq_request_processing_seconds_created 1.5878023726039658e+09
 # HELP rq_workers RQ workers
@@ -140,43 +139,44 @@
 rq_jobs{queue="default", status="scheduled"} 2.0
 ```
 
 ## Configuration
 
 You can configure the exporter using command line arguments or environment variables:
 
-| CLI Argument        | Env Variable              | Default Value                                           | Description                                                     |
-| ------------------- | ------------------------- | ------------------------------------------------------- | --------------------------------------------------------------- |
-| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                 |
-| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                 |
-| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`  |
-| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                 |
-| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                               |
-| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                           |
-| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel host                                             |
-| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port                                             |
-| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                      |
-| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                  |
-| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret) |
-| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                 |
-| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                  |
-| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                   |
-| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                   |
-| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                 |
+| CLI Argument        | Env Variable              | Default Value                                           | Description                                                              |
+| ------------------- | ------------------------- | ------------------------------------------------------- | ------------------------------------------------------------------------ |
+| `--host`            | `RQ_EXPORTER_HOST`        | `0.0.0.0`                                               | Serve the exporter on this host                                          |
+| `-p`, `--port`      | `RQ_EXPORTER_PORT`        | `9726`                                                  | Serve the exporter on this port                                          |
+| `--redis-url`       | `RQ_REDIS_URL`            | `None`                                                  | Redis URL in the form `redis://:[password]@[host]:[port]/[db]`           |
+| `--redis-host`      | `RQ_REDIS_HOST`           | `localhost`                                             | Redis host name                                                          |
+| `--redis-port`      | `RQ_REDIS_PORT`           | `6379`                                                  | Redis port number                                                        |
+| `--redis-db`        | `RQ_REDIS_DB`             | `0`                                                     | Redis database number                                                    |
+| `--sentinel-host`   | `RQ_SENTINEL_HOST`        | `None`                                                  | Redis Sentinel hosts separated by commas e.g `sentinel1,sentinel2:26380` |
+| `--sentinel-port`   | `RQ_SENTINEL_PORT`        | `26379`                                                 | Redis Sentinel port, default port used when not set with the host        |
+| `--sentinel-master` | `RQ_SENTINEL_MASTER`      | `master`                                                | Redis Sentinel master name                                               |
+| `--redis-pass`      | `RQ_REDIS_PASS`           | `None`                                                  | Redis password                                                           |
+| `--redis-pass-file` | `RQ_REDIS_PASS_FILE`      | `None`                                                  | Redis password file path (e.g. Path of a mounted Docker secret)          |
+| `--worker-class`    | `RQ_WORKER_CLASS`         | `rq.Worker`                                             | RQ worker class                                                          |
+| `--queue-class`     | `RQ_QUEUE_CLASS`          | `rq.Queue`                                              | RQ queue class                                                           |
+| `--log-level`       | `RQ_EXPORTER_LOG_LEVEL`   | `INFO`                                                  | Logging level                                                            |
+| `--log-format`      | `RQ_EXPORTER_LOG_FORMAT`  | `[%(asctime)s] [%(name)s] [%(levelname)s]: %(message)s` | Logging handler format string                                            |
+| `--log-datefmt`     | `RQ_EXPORTER_LOG_DATEFMT` | `%Y-%m-%d %H:%M:%S`                                     | Logging date/time format string                                          |
 
-**Note**:
+**Notes**:
 
 - When Redis URL is set using `--redis-url` or `RQ_REDIS_URL` the other Redis options will be ignored
 - When the Redis password is set using `--redis-pass-file` or `RQ_REDIS_PASS_FILE`, then `--redis-pass` and `RQ_REDIS_PASS` will be ignored
+- The Sentinel port will default to the value of `--sentinel-port` if not set for each host with `--sentinel-host` or `RQ_SENTINEL_HOST`
 
 ## Serving with Gunicorn
 
 The WSGI application can be created using the `rq_exporter.create_app()` function:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --log-level info
 ```
 
 Example [`Dockerfile`](https://github.com/mdawar/rq-exporter/blob/master/Dockerfile.gunicorn) to create a **Docker** image to serve the application with **Gunicorn**
 
 ```dockerfile
 FROM mdawar/rq-exporter:latest
@@ -200,96 +200,98 @@
 - `rq_request_processing_seconds_sum`
 - `rq_request_processing_seconds_created`
 
 This is fine if you don't care about these metrics, these are only for measuring the count and time processing the RQ data, so the other RQ metrics are not going to be affected.
 
 But you can still use multiple threads with 1 worker process to handle multiple concurrent requests:
 
-```console
+```sh
 $ gunicorn "rq_exporter:create_app()" -b 0.0.0.0:9726 --threads 2
 ```
 
 ## Building the Docker Image
 
-```console
+```sh
 $ # Build the docker image and tag it rq-exporter:latest
 $ docker build -t rq-exporter .
+$ # Or
+$ make build
 
-$ # M1 MacOs Build the docker image and tag it rq-exporter:latest
+$ # M1 MacOS Build the docker image and tag it rq-exporter:latest
 $ docker buildx build --platform linux/amd64 -t rq-exporter .
 ```
 
-The image can also be built using `docker-compose`:
+The image can also be built using `docker compose`:
 
-```console
-$ docker-compose build
+```sh
+$ docker compose build
 ```
 
-Check out the `docker-compose.yml` file for usage example.
+Check the `docker-compose.yml` file for usage example.
 
 ## Development
 
 To start a full development environment with **RQ** workers, **Prometheus** and **Grafana**:
 
-```console
-$ docker-compose up
+```sh
+$ docker compose up
 $ # If you want to start multiple workers use the --compatibility flag
-$ # which will make docker-compose read the `deploy` section and start multiple replicas
-$ docker-compose --compatibility up
+$ # which will make docker compose read the `deploy` section and start multiple replicas
+$ docker compose --compatibility up
 ```
 
 You can access the services on these ports on your local machine:
 
 - **RQ exporter**: [`9726`](http://localhost:9726)
 - **Redis**: [`6379`](http://localhost:6379)
 - **RQ Dashboard**: [`9181`](http://localhost:9181)
 - **Prometheus**: [`9090`](http://localhost:9090)
 - **Grafana**: [`3000`](http://localhost:3000) (Login using `admin:admin`)
 
 You can specify the services that you want to start by their name in the `docker-compose.yml` file:
 
-```console
+```sh
 $ # Example starting only the `rq_exporter` and `redis` services
-$ docker-compose up rq_exporter redis
+$ docker compose up rq_exporter redis
 ```
 
 To run more workers and enqueue more jobs you can scale the `worker` and `enqueue` services:
 
-```console
+```sh
 $ # Run 5 workers
-$ docker-compose up -d --scale worker=5
+$ docker compose up -d --scale worker=5
 $ # Enqueue more jobs
 $ # Scale the enqueue service and the workers
-$ docker-compose up -d --scale worker=5 --scale enqueue=2
+$ docker compose up -d --scale worker=5 --scale enqueue=2
 ```
 
 To cleanup after development:
 
-```console
+```sh
 $ # Use -v to remove volumes
-$ docker-compose down -v
+$ docker compose down -v
 ```
 
 You can also start another `rq-exporter` instance that collects stats from a project using custom **RQ** `Worker` and `Queue` classes:
 
-```console
+```sh
 $ # Using -f to pass multiple docker-compose files
 $ # docker-compose.custom.yml defines services using custom RQ classes
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml up
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml up
 $ # To cleanup you need to also pass the same files
-$ docker-compose -f docker-compose.yml -f docker-compose.custom.yml down
+$ docker compose -f docker-compose.yml -f docker-compose.custom.yml down
 ```
 
 A new **RQ exporter** instance will be exposed on port `9727` on your local machine.
 
-**Note**: If you don't have `docker-compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
+**Note**: If you don't have `docker compose` installed follow the [installation](https://docs.docker.com/compose/install/) instructions on the official website.
 
 If you want to use the package manually:
 
-```console
+```sh
 $ # Clone the repository
 $ git clone <REPO_URL>
 $ # Change to the project directory
 $ cd rq-exporter
 $ # Create a new virtualenv
 $ python -m venv /path/to/env
 $ # Activate the environment
@@ -300,21 +302,21 @@
 $ python -m rq_exporter
 $ # You can configure the exporter using command line arguments
 $ python -m rq_exporter --port 8080
 ```
 
 ## Running the Tests
 
-```console
+```sh
+$ make test
+$ # Or
 $ python -m unittest
 ```
 
 ## Contributing
 
 1. Fork the [repository](https://github.com/mdawar/rq-exporter)
 2. Clone the forked repository `git clone <URL>`
 3. Create a new feature branch `git checkout -b <BRANCH_NAME>`
 4. Make changes and add tests if needed and commit your changes `git commit -am "Your commit message"`
 5. Push the new branch to Github `git push origin <BRANCH_NAME>`
 6. Create a pull request
-
-
```

### Comparing `rq-exporter-2.0.0/setup.py` & `rq-exporter-2.1.0/setup.py`

 * *Files identical despite different names*

