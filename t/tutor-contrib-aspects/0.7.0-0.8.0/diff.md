# Comparing `tmp/tutor-contrib-aspects-0.7.0.tar.gz` & `tmp/tutor-contrib-aspects-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-contrib-aspects-0.7.0.tar", last modified: Wed Jul  5 20:42:13 2023, max compression
+gzip compressed data, was "tutor-contrib-aspects-0.8.0.tar", last modified: Thu Jul  6 14:38:35 2023, max compression
```

## Comparing `tutor-contrib-aspects-0.7.0.tar` & `tutor-contrib-aspects-0.8.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11043 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-05 20:42:13.000000 tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/caddyfile
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-deployments
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-jobs
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-services
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-volumes
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/kustomization-configmapgenerator
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-dev-services
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-jobs-services
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-services
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/openedx-cms-common-settings
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/superset-extra-assets
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/patches/superset-jinja-filters
--rw-r--r--   0 runner    (1001) docker     (123)    22371 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.286403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.286403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.290403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.286403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/clickhouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/clickhouse/config/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.286403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/config/env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/docker/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
--rw-r--r--   0 runner    (1001) docker     (123)    41198 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/security/
--rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.294403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/file.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/local.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects-superset/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.286403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/aspects/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 20:42:13.298403 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-05 20:42:06.000000 tutor-contrib-aspects-0.7.0/tutoraspects/templates/base-docker-compose-services
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12239 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 14:38:35.000000 tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/caddyfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-deployments
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-services
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-volumes
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/kustomization-configmapgenerator
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-dev-services
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-services
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/openedx-cms-common-settings
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/superset-extra-assets
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/patches/superset-jinja-filters
+-rw-r--r--   0 runner    (1001) docker     (123)    22371 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/dbt_project.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/packages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.901980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/alembic.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      654 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/clickhouse/config/docker_config.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/ralph_auth/auth.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2113 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/requirements-local.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/
+-rw-r--r--   0 runner    (1001) docker     (123)    45916 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/
+-rw-r--r--   0 runner    (1001) docker     (123)    95955 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/roles.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/file.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/k8s.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/local.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.905980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-pre.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.897980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/aspects/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/aspects/init-aspects.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 14:38:35.909980 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2852 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-07-06 14:38:26.000000 tutor-contrib-aspects-0.8.0/tutoraspects/templates/base-docker-compose-services
```

### Comparing `tutor-contrib-aspects-0.7.0/PKG-INFO` & `tutor-contrib-aspects-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.7.0
+Version: 0.8.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -179,14 +179,33 @@
     ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
+Virtual datasets in Superset
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
+
+To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
+
+.. code-block:: yaml
+
+   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+
+
+However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
+
+.. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
+
+.. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+
+
 Changing Superset Language Settings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Superset localization is a work in progress, but you can change the default language and set alternate languages from the currently supported list by changing the Tutor configuration variables:
 
 Default language: ``tutor config save --set SUPERSET_DEFAULT_LOCALE=en``
```

### Comparing `tutor-contrib-aspects-0.7.0/README.rst` & `tutor-contrib-aspects-0.8.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -158,14 +158,33 @@
     ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
+Virtual datasets in Superset
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
+
+To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
+
+.. code-block:: yaml
+
+   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+
+
+However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
+
+.. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
+
+.. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+
+
 Changing Superset Language Settings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Superset localization is a work in progress, but you can change the default language and set alternate languages from the currently supported list by changing the Tutor configuration variables:
 
 Default language: ``tutor config save --set SUPERSET_DEFAULT_LOCALE=en``
```

### Comparing `tutor-contrib-aspects-0.7.0/setup.py` & `tutor-contrib-aspects-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/PKG-INFO` & `tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-contrib-aspects
-Version: 0.7.0
+Version: 0.8.0
 Summary: Aspects plugin for Tutor
 Home-page: https://github.com/open-craft/tutor-contrib-aspects
 Author: The Open edX Community
 License: AGPLv3
 Project-URL: Code, https://github.com/open-craft/tutor-contrib-aspects
 Project-URL: Issue tracker, https://github.com/open-craft/tutor-contrib-aspects/issues
 Classifier: Development Status :: 3 - Alpha
@@ -179,14 +179,33 @@
     ``clickhousedb+connect://{{CLICKHOUSE_REPORT_URL}}``
 #. Remove any ``metadata.yaml`` files from the export. We generate these as needed during import.
 #. Merge your exported files into the directories and files in the `assets.yaml`_.
 #. Submit a PR with screenshots of your new chart or dashboards, along with an explanation
    of what data question they answer.
 
 
+Virtual datasets in Superset
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+Superset supports creating virtual datasets, which are datasets defined using a SQL query instead of mapping directly to an underlying database object. Aspects leverages virtual datasets, along with `SQL templating <https://superset.apache.org/docs/installation/sql-templating/>`_, to make better use of table indexes.
+
+To make it easier for developers to manage virtual datasets, there is an extra step that can be done on the output of ``tutor aspects serialize``. The ``sql`` section of the dataset yaml can be moved to its own file in the `queries`_ directory and included in the yaml like so:
+
+.. code-block:: yaml
+
+   sql: "{% include 'aspects/apps/superset/pythonpath/queries/query.sql' %}"
+
+
+However, please keep in mind that the assets declaration is itself a jinja template. That means that any jinja used in the dataset definition should be escaped. There are examples of how to handle this in the existing queries, such as `dim_courses.sql`_.
+
+.. _queries: tutoraspects/templates/aspects/apps/superset/pythonpath/queries
+
+.. _dim_courses.sql: tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
+
+
 Changing Superset Language Settings
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Superset localization is a work in progress, but you can change the default language and set alternate languages from the currently supported list by changing the Tutor configuration variables:
 
 Default language: ``tutor config save --set SUPERSET_DEFAULT_LOCALE=en``
```

### Comparing `tutor-contrib-aspects-0.7.0/tutor_contrib_aspects.egg-info/SOURCES.txt` & `tutor-contrib-aspects-0.8.0/tutor_contrib_aspects.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py
 tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql
 tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql
 tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments.sql
+tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql
 tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql
 tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql
 tutoraspects/templates/aspects/apps/superset/security/roles.json
 tutoraspects/templates/aspects/apps/vector/file.toml
 tutoraspects/templates/aspects/apps/vector/k8s.toml
 tutoraspects/templates/aspects/apps/vector/local.toml
 tutoraspects/templates/aspects/apps/vector/partials/common-post.toml
```

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-deployments` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-jobs` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-services` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/k8s-volumes` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/k8s-volumes`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/kustomization-configmapgenerator` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/kustomization-configmapgenerator`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-dev-services` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-dev-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-jobs-services` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-jobs-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/patches/local-docker-compose-services` & `tutor-contrib-aspects-0.8.0/tutoraspects/patches/local-docker-compose-services`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/plugin.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/dbt/profiles.yml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0001_get_org_from_course_url.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0002_raw_xapi_table.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0003_enrollment.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0004_video.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0005_problem.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0006_navigation.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0007_event_sink.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic/versions/0008_vector.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/clickhouse-demo-xapi-data.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/aspects/scripts/dbt.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/ralph/config/env` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/ralph/config/env`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/docker/docker-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/assets.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -784,31 +784,32 @@
   schema: {{ ASPECTS_EVENT_SINK_DATABASE }}
   sql: null
   table_name: {{ ASPECTS_EVENT_SINK_OVERVIEWS_TABLE }}
   template_params: null
   uuid: 46183302-6fa6-41a3-b6a7-79ff6c1c8402
   version: 1.0.0
 
-- _file_name: Instructor_dashboard_5.yaml
+- _file_name: Instructor_dashboard_9.yaml
   css: ''
   dashboard_title: Instructor dashboard
   description: null
   metadata:
     chart_configuration: {}
     color_scheme: ''
     default_filters: '{}'
     expanded_slices: {}
     label_colors: {}
     native_filter_configuration:
     - cascadeParentIds: []
       chartsInScope:
-      - 12
-      - 13
-      - 17
-      - 18
+      - 24
+      - 25
+      - 32
+      - 33
+      - 34
       controlValues:
         defaultToFirstItem: true
         enableEmptyFilter: true
         inverseSelection: false
         multiSelect: true
         searchAllOptions: false
       defaultDataMask:
@@ -829,18 +830,19 @@
       - column:
           name: org
         datasetUuid: 4b274428-d781-41be-b362-ed6917443678
       type: NATIVE_FILTER
     - cascadeParentIds:
       - NATIVE_FILTER-Vx7HxG8_7
       chartsInScope:
-      - 12
-      - 13
-      - 17
-      - 18
+      - 24
+      - 25
+      - 32
+      - 33
+      - 34
       controlValues:
         defaultToFirstItem: false
         enableEmptyFilter: false
         inverseSelection: false
         multiSelect: true
         searchAllOptions: false
       defaultDataMask:
@@ -860,15 +862,20 @@
       - column:
           name: course_name
         datasetUuid: 4b274428-d781-41be-b362-ed6917443678
       type: NATIVE_FILTER
     - cascadeParentIds:
       - NATIVE_FILTER-Vx7HxG8_7
       - NATIVE_FILTER-XPuiTOej4
-      chartsInScope: []
+      chartsInScope:
+      - 24
+      - 25
+      - 32
+      - 33
+      - 34
       controlValues:
         defaultToFirstItem: false
         enableEmptyFilter: false
         inverseSelection: false
         multiSelect: true
         searchAllOptions: false
       defaultDataMask:
@@ -885,79 +892,117 @@
         - ROOT_ID
       tabsInScope: []
       targets:
       - column:
           name: run_name
         datasetUuid: 4b274428-d781-41be-b362-ed6917443678
       type: NATIVE_FILTER
+    - cascadeParentIds: []
+      chartsInScope:
+      - 32
+      - 34
+      controlValues:
+        enableEmptyFilter: false
+      defaultDataMask:
+        extraFormData:
+          time_range: Last month
+        filterState:
+          value: Last month
+      description: ''
+      filterType: filter_time
+      id: NATIVE_FILTER-zxfszG4xH
+      name: Time range
+      scope:
+        excluded: []
+        rootPath:
+        - ROOT_ID
+      tabsInScope: []
+      targets:
+      - {}
+      type: NATIVE_FILTER
     refresh_frequency: 0
     shared_label_colors: {}
     show_native_filters: true
     timed_refresh_immune_slices: []
   position:
     CHART-Jr-gNVms2Q:
       children: []
       id: CHART-Jr-gNVms2Q
       meta:
-        chartId: 18
+        chartId: 34
         height: 50
         sliceName: Enrollment events per day
         uuid: bb1147cc-b7bc-44b7-b06a-79b0db6626aa
         width: 8
       parents:
       - ROOT_ID
       - GRID_ID
       - ROW-je_Wqya3Ga
       type: CHART
     CHART-evjVO-ZSSd:
       children: []
       id: CHART-evjVO-ZSSd
       meta:
-        chartId: 17
+        chartId: 32
         height: 50
         sliceName: Cumulative enrollments by mode
         uuid: 05ed7102-5464-4e2f-86ae-31700b787cc3
         width: 4
       parents:
       - ROOT_ID
       - GRID_ID
       - ROW-je_Wqya3Ga
       type: CHART
     CHART-hCz27s2NEX:
       children: []
       id: CHART-hCz27s2NEX
       meta:
-        chartId: 13
+        chartId: 25
         height: 50
         sliceName: Watches per video
         uuid: 829c1d5b-2844-4115-876a-34ad3b3cad64
         width: 6
       parents:
       - ROOT_ID
       - GRID_ID
       - ROW-7OLwuieb8j
       type: CHART
     CHART-p5SkjOwu0w:
       children: []
       id: CHART-p5SkjOwu0w
       meta:
-        chartId: 12
+        chartId: 24
         height: 50
         sliceName: Transcript/closed captioning usage per video
         uuid: 6b830def-f3ca-4b4c-9455-7a7b7354bce8
         width: 6
       parents:
       - ROOT_ID
       - GRID_ID
       - ROW-7OLwuieb8j
       type: CHART
+    CHART-rnb6PSwCOS:
+      children: []
+      id: CHART-rnb6PSwCOS
+      meta:
+        chartId: 36
+        height: 50
+        sliceName: Enrolled learners per day
+        uuid: ed2fe731-6544-422f-bc55-42f399f48b2c
+        width: 12
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      - ROW-K8s_8uq9IP
+      type: CHART
     DASHBOARD_VERSION_KEY: v2
     GRID_ID:
       children:
       - HEADER-9oReNB0nyf
+      - ROW-K8s_8uq9IP
       - ROW-je_Wqya3Ga
       - HEADER-Jevm46xhwX
       - ROW-7OLwuieb8j
       id: GRID_ID
       parents:
       - ROOT_ID
       type: GRID
@@ -1000,14 +1045,24 @@
       id: ROW-7OLwuieb8j
       meta:
         background: BACKGROUND_TRANSPARENT
       parents:
       - ROOT_ID
       - GRID_ID
       type: ROW
+    ROW-K8s_8uq9IP:
+      children:
+      - CHART-rnb6PSwCOS
+      id: ROW-K8s_8uq9IP
+      meta:
+        background: BACKGROUND_TRANSPARENT
+      parents:
+      - ROOT_ID
+      - GRID_ID
+      type: ROW
     ROW-je_Wqya3Ga:
       children:
       - CHART-evjVO-ZSSd
       - CHART-Jr-gNVms2Q
       id: ROW-je_Wqya3Ga
       meta:
         background: BACKGROUND_TRANSPARENT
@@ -1752,8 +1807,161 @@
   schema: null
   sql: "{% include 'aspects/apps/superset/pythonpath/queries/dim_courses.sql' %}"
   table_name: dim_courses
   template_params: {}
   uuid: 4b274428-d781-41be-b362-ed6917443678
   version: 1.0.0
 
+- _file_name: Enrolled_learners_per_day_36.yaml
+  cache_timeout: null
+  dataset_uuid: 352311fe-12f0-470c-8b8c-d4f6a3936b3d
+  params:
+    adhoc_filters:
+    - clause: WHERE
+      comparator: registered
+      expressionType: SIMPLE
+      filterOptionName: filter_hcnm4t7piq6_hfbtt65nqqs
+      isExtra: false
+      isNew: false
+      operator: ==
+      operatorId: EQUALS
+      sqlExpression: null
+      subject: enrollment_status
+    color_picker:
+      a: 1
+      b: 135
+      g: 122
+      r: 0
+    datasource: 40__table
+    extra_form_data: {}
+    granularity_sqla: enrollment_status_date
+    header_font_size: 0.4
+    metric: count
+    rolling_type: None
+    show_trend_line: true
+    start_y_axis_at_zero: true
+    subheader_font_size: 0.15
+    time_format: smart_date
+    time_grain_sqla: P1D
+    time_range: No filter
+    viz_type: big_number
+    y_axis_format: SMART_NUMBER
+  slice_name: Enrolled learners per day
+  uuid: ed2fe731-6544-422f-bc55-42f399f48b2c
+  version: 1.0.0
+  viz_type: big_number
+
+
+- _file_name: fact_enrollments_by_day.yaml
+  cache_timeout: null
+  columns:
+  - advanced_data_type: null
+    column_name: enrollment_mode
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: LowCardinality(String)
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: enrollment_status_date
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: true
+    python_date_format: null
+    type: Date
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: actor_id
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: course_name
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: enrollment_status
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: run_name
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  - advanced_data_type: null
+    column_name: org
+    description: null
+    expression: null
+    extra: null
+    filterable: true
+    groupby: true
+    is_active: true
+    is_dttm: false
+    python_date_format: null
+    type: String
+    verbose_name: null
+  database_uuid: 21174b6c-4d40-4958-8161-d6c3cf5e77b6
+  default_endpoint: null
+  description: null
+  extra: null
+  fetch_values_predicate: null
+  filter_select_enabled: false
+  main_dttm_col: null
+  metrics:
+  - d3format: null
+    description: null
+    expression: count(*)
+    extra: null
+    metric_name: count
+    metric_type: null
+    verbose_name: null
+    warning_text: null
+  offset: 0
+  params: null
+  schema: null
+  sql: "{% include 'aspects/apps/superset/pythonpath/queries/fact_enrollments_by_day.sql' %}"
+  table_name: fact_enrollments_by_day
+  template_params: {}
+  uuid: 352311fe-12f0-470c-8b8c-d4f6a3936b3d
+  version: 1.0.0
+
+
 {{ patch("superset-extra-assets") }}
```

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_assets.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/create_row_level_security.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_jinja_filters.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/openedx_sso_security_manager.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_course_videos.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/dim_courses.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_transcript_usage.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/queries/fact_video_plays.sql`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/pythonpath/superset_config_docker.py`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/superset/security/roles.json` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/superset/security/roles.json`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/apps/vector/partials/common-post.toml`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/build/aspects-superset/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/clickhouse/init-clickhouse.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-mysql.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-openedx.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/aspects/jobs/init/superset/init-superset.sh`

 * *Files identical despite different names*

### Comparing `tutor-contrib-aspects-0.7.0/tutoraspects/templates/base-docker-compose-services` & `tutor-contrib-aspects-0.8.0/tutoraspects/templates/base-docker-compose-services`

 * *Files identical despite different names*

