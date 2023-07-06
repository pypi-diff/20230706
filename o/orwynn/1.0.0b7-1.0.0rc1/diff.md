# Comparing `tmp/orwynn-1.0.0b7.tar.gz` & `tmp/orwynn-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orwynn-1.0.0b7.tar", max compression
+gzip compressed data, was "orwynn-1.0.0rc1.tar", max compression
```

## Comparing `orwynn-1.0.0b7.tar` & `orwynn-1.0.0rc1.tar`

### file list

```diff
@@ -1,263 +1,263 @@
--rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0b7/LICENSE
--rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0b7/README.md
--rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0b7/orwynn/__init__.py
--rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0b7/orwynn/apiversion/__init__.py
--rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/apiversion/errors.py
--rw-r--r--   0        0        0     4546 2023-06-09 12:16:54.007732 orwynn-1.0.0b7/orwynn/apiversion/test_main.py
--rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0b7/orwynn/app/__init__.py
--rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0b7/orwynn/app/apirouter.py
--rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0b7/orwynn/app/apiwebsocketroute.py
--rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0b7/orwynn/app/app.py
--rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0b7/orwynn/app/config.py
--rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0b7/orwynn/app/core.py
--rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0b7/orwynn/app/mode.py
--rw-r--r--   0        0        0     2206 2023-06-08 13:47:49.295428 orwynn-1.0.0b7/orwynn/app/test_main.py
--rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0b7/orwynn/app/types.py
--rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0b7/orwynn/app/utils.py
--rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0b7/orwynn/apprc/__init__.py
--rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0b7/orwynn/apprc/apprc.py
--rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0b7/orwynn/apprc/constants.py
--rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/apprc/errors.py
--rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0b7/orwynn/apprc/parse.py
--rw-r--r--   0        0        0     2604 2023-06-09 06:20:20.107768 orwynn-1.0.0b7/orwynn/apprc/test_main.py
--rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0b7/orwynn/base/__init__.py
--rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0b7/orwynn/base/config/__init__.py
--rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0b7/orwynn/base/config/config.py
--rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0b7/orwynn/base/config/test_config.py
--rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0b7/orwynn/base/controller/__init__.py
--rw-r--r--   0        0        0     2201 2023-04-07 10:26:00.405258 orwynn-1.0.0b7/orwynn/base/controller/controller.py
--rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0b7/orwynn/base/controller/errors.py
--rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0b7/orwynn/base/database/__init__.py
--rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0b7/orwynn/base/database/database.py
--rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0b7/orwynn/base/database/errors.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0b7/orwynn/base/error/__init__.py
--rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0b7/orwynn/base/error/code.py
--rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0b7/orwynn/base/error/errors.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0b7/orwynn/base/error/test_main.py
--rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0b7/orwynn/base/error/test_utils.py
--rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0b7/orwynn/base/error/utils.py
--rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0b7/orwynn/base/error/valueschema.py
--rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0b7/orwynn/base/errorhandler/__init__.py
--rw-r--r--   0        0        0     2365 2023-06-09 06:03:10.090856 orwynn-1.0.0b7/orwynn/base/errorhandler/errorhandler.py
--rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0b7/orwynn/base/middleware/__init__.py
--rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0b7/orwynn/base/middleware/globalsetup.py
--rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0b7/orwynn/base/middleware/middleware.py
--rw-r--r--   0        0        0     1186 2023-06-09 06:20:20.112767 orwynn-1.0.0b7/orwynn/base/middleware/test_main.py
--rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0b7/orwynn/base/model/__init__.py
--rw-r--r--   0        0        0     1429 2023-06-09 05:54:50.487357 orwynn-1.0.0b7/orwynn/base/model/model.py
--rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0b7/orwynn/base/model/test_model.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0b7/orwynn/base/module/__init__.py
--rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0b7/orwynn/base/module/errors.py
--rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0b7/orwynn/base/module/module.py
--rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0b7/orwynn/base/module/test_module.py
--rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0b7/orwynn/base/service/__init__.py
--rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0b7/orwynn/base/service/framework.py
--rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0b7/orwynn/base/service/service.py
--rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0b7/orwynn/base/worker/__init__.py
--rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0b7/orwynn/base/worker/worker.py
--rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0b7/orwynn/boot/__init__.py
--rw-r--r--   0        0        0    10355 2023-06-09 12:09:03.948090 orwynn-1.0.0b7/orwynn/boot/boot.py
--rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0b7/orwynn/boot/config.py
--rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0b7/orwynn/boot/errors.py
--rw-r--r--   0        0        0     4754 2023-06-09 06:27:59.920644 orwynn-1.0.0b7/orwynn/boot/test_main.py
--rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0b7/orwynn/bootscript/__init__.py
--rw-r--r--   0        0        0      220 2023-06-08 13:59:21.194248 orwynn-1.0.0b7/orwynn/bootscript/bootscript.py
--rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0b7/orwynn/bootscript/callable.py
--rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0b7/orwynn/bootscript/calltime.py
--rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0b7/orwynn/bootscript/errors.py
--rw-r--r--   0        0        0      860 2023-06-09 06:20:20.107768 orwynn-1.0.0b7/orwynn/bootscript/test_main.py
--rw-r--r--   0        0        0     2300 2023-06-09 06:20:20.107768 orwynn-1.0.0b7/orwynn/bootscript/worker.py
--rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0b7/orwynn/context/__init__.py
--rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/context/errors.py
--rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0b7/orwynn/context/manager.py
--rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0b7/orwynn/context/storage.py
--rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0b7/orwynn/di/__init__.py
--rw-r--r--   0        0        0       63 2022-12-11 09:09:39.933971 orwynn-1.0.0b7/orwynn/di/acceptor.py
--rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0b7/orwynn/di/availability.py
--rw-r--r--   0        0        0     1719 2023-06-09 06:20:20.108768 orwynn-1.0.0b7/orwynn/di/collecting/acceptordependencies.py
--rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0b7/orwynn/di/collecting/errors.py
--rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0b7/orwynn/di/collecting/helpers.py
--rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0b7/orwynn/di/collecting/modulecollector.py
--rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/__init__.py
--rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/collect.py
--rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/map.py
--rw-r--r--   0        0        0     1765 2023-06-09 06:20:20.109768 orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/test_main.py
--rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0b7/orwynn/di/collecting/test_modules.py
--rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0b7/orwynn/di/constants.py
--rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0b7/orwynn/di/container.py
--rw-r--r--   0        0        0     4694 2023-06-09 06:20:20.104768 orwynn-1.0.0b7/orwynn/di/di.py
--rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0b7/orwynn/di/errors.py
--rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0b7/orwynn/di/init/acceptors.py
--rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0b7/orwynn/di/init/providers.py
--rw-r--r--   0        0        0     2871 2023-06-09 06:20:20.106768 orwynn-1.0.0b7/orwynn/di/init/test_acceptors.py
--rw-r--r--   0        0        0      615 2023-06-09 06:23:04.561666 orwynn-1.0.0b7/orwynn/di/init/test_providers.py
--rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0b7/orwynn/di/isacceptor.py
--rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0b7/orwynn/di/isprovider.py
--rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0b7/orwynn/di/object.py
--rw-r--r--   0        0        0       39 2022-12-11 09:09:05.931124 orwynn-1.0.0b7/orwynn/di/provider.py
--rw-r--r--   0        0        0      506 2023-06-09 06:20:20.105768 orwynn-1.0.0b7/orwynn/di/testing.py
--rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0b7/orwynn/helpers/constants.py
--rw-r--r--   0        0        0      455 2023-07-04 11:25:22.457577 orwynn-1.0.0b7/orwynn/helpers/errors.py
--rw-r--r--   0        0        0     1140 2023-06-09 06:03:10.090856 orwynn-1.0.0b7/orwynn/helpers/web.py
--rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0b7/orwynn/http/__init__.py
--rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0b7/orwynn/http/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0b7/orwynn/http/context/__init__.py
--rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0b7/orwynn/http/context/id.py
--rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0b7/orwynn/http/context/middleware/builtin.py
--rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0b7/orwynn/http/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0      984 2023-06-09 06:27:59.920644 orwynn-1.0.0b7/orwynn/http/context/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0b7/orwynn/http/controller/__init__.py
--rw-r--r--   0        0        0     5446 2023-06-09 06:03:10.090856 orwynn-1.0.0b7/orwynn/http/controller/controller.py
--rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0b7/orwynn/http/controller/endpoint/__init__.py
--rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0b7/orwynn/http/controller/endpoint/container.py
--rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0b7/orwynn/http/controller/endpoint/endpoint.py
--rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0b7/orwynn/http/controller/endpoint/response.py
--rw-r--r--   0        0        0     2231 2023-06-08 13:56:18.457476 orwynn-1.0.0b7/orwynn/http/controller/endpoint/test_main.py
--rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/http/controller/errors.py
--rw-r--r--   0        0        0     7262 2023-06-09 06:20:20.111767 orwynn-1.0.0b7/orwynn/http/controller/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0b7/orwynn/http/cors/__init__.py
--rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0b7/orwynn/http/cors/cors.py
--rw-r--r--   0        0        0     3491 2023-06-09 12:32:20.369783 orwynn-1.0.0b7/orwynn/http/cors/test_main.py
--rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0b7/orwynn/http/errorhandler/__init__.py
--rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0b7/orwynn/http/errorhandler/default.py
--rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0b7/orwynn/http/errorhandler/middleware.py
--rw-r--r--   0        0        0     6129 2023-06-09 07:32:02.382043 orwynn-1.0.0b7/orwynn/http/errorhandler/test_main.py
--rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0b7/orwynn/http/errors.py
--rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0b7/orwynn/http/log/logger.py
--rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0b7/orwynn/http/log/middleware.py
--rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0b7/orwynn/http/middleware/__init__.py
--rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0b7/orwynn/http/middleware/builtinmiddleware.py
--rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0b7/orwynn/http/middleware/middleware.py
--rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0b7/orwynn/http/middleware/nextcall.py
--rw-r--r--   0        0        0     2150 2023-06-09 06:00:41.008691 orwynn-1.0.0b7/orwynn/http/middleware/test_main.py
--rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0b7/orwynn/http/requests.py
--rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0b7/orwynn/http/responses.py
--rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0b7/orwynn/http/schema/validationvalue.py
--rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0b7/orwynn/http/schema/value.py
--rw-r--r--   0        0        0      873 2023-06-09 05:50:36.425514 orwynn-1.0.0b7/orwynn/http/test_responses.py
--rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0b7/orwynn/http/testing.py
--rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0b7/orwynn/indication/__init__.py
--rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0b7/orwynn/indication/default.py
--rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/indication/errors.py
--rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0b7/orwynn/indication/indicatable.py
--rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0b7/orwynn/indication/indication.py
--rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0b7/orwynn/indication/indicator.py
--rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0b7/orwynn/indication/test_main.py
--rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0b7/orwynn/indication/type.py
--rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0b7/orwynn/log/__init__.py
--rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0b7/orwynn/log/config.py
--rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0b7/orwynn/log/configure.py
--rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0b7/orwynn/log/constants.py
--rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/log/errors.py
--rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0b7/orwynn/log/handler.py
--rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0b7/orwynn/log/helpers.py
--rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0b7/orwynn/log/log.py
--rw-r--r--   0        0        0     1767 2023-06-09 07:50:09.129655 orwynn-1.0.0b7/orwynn/log/test_main.py
--rw-r--r--   0        0        0     3679 2023-06-09 06:00:41.008691 orwynn-1.0.0b7/orwynn/log/test_middleware.py
--rw-r--r--   0        0        0     1443 2023-06-09 06:20:10.150480 orwynn-1.0.0b7/orwynn/log/test_websocketmiddleware.py
--rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0b7/orwynn/log/types.py
--rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0b7/orwynn/mapping/__init__.py
--rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0b7/orwynn/mapping/errors.py
--rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0b7/orwynn/mapping/mapping.py
--rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0b7/orwynn/mapping/test_main.py
--rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0b7/orwynn/mongo/__init__.py
--rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0b7/orwynn/mongo/clientsession.py
--rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0b7/orwynn/mongo/config.py
--rw-r--r--   0        0        0     8705 2023-07-06 07:51:45.996253 orwynn-1.0.0b7/orwynn/mongo/document/__init__.py
--rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0b7/orwynn/mongo/document/errors.py
--rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0b7/orwynn/mongo/document/helpers.py
--rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0b7/orwynn/mongo/document/test_converttoobjectid.py
--rw-r--r--   0        0        0      219 2023-07-06 06:48:26.581243 orwynn-1.0.0b7/orwynn/mongo/document/test_create.py
--rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0b7/orwynn/mongo/document/test_get.py
--rw-r--r--   0        0        0     1128 2023-07-06 07:28:27.150203 orwynn-1.0.0b7/orwynn/mongo/document/test_inc.py
--rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0b7/orwynn/mongo/document/test_refresh.py
--rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0b7/orwynn/mongo/document/test_remove.py
--rw-r--r--   0        0        0     1258 2023-07-06 07:28:27.151203 orwynn-1.0.0b7/orwynn/mongo/document/test_set.py
--rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0b7/orwynn/mongo/document/test_updateoperators.py
--rw-r--r--   0        0        0      708 2023-07-06 07:28:27.148204 orwynn-1.0.0b7/orwynn/mongo/document/testing.py
--rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0b7/orwynn/mongo/entity.py
--rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0b7/orwynn/mongo/errors.py
--rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0b7/orwynn/mongo/mongo.py
--rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0b7/orwynn/mongo/test_main.py
--rw-r--r--   0        0        0      395 2023-07-06 07:28:27.154203 orwynn-1.0.0b7/orwynn/mongo/testing.py
--rw-r--r--   0        0        0     2839 2023-06-09 06:03:10.133848 orwynn-1.0.0b7/orwynn/proxy/boot.py
--rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0b7/orwynn/proxy/indicationonly.py
--rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0b7/orwynn/router/__init__.py
--rw-r--r--   0        0        0     3966 2023-06-09 06:23:57.815708 orwynn-1.0.0b7/orwynn/router/errorhandlermanager.py
--rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/router/errors.py
--rw-r--r--   0        0        0    14259 2023-06-09 06:03:10.133848 orwynn-1.0.0b7/orwynn/router/register/controller.py
--rw-r--r--   0        0        0     9656 2023-06-09 11:05:03.703488 orwynn-1.0.0b7/orwynn/router/register/middleware.py
--rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0b7/orwynn/router/router.py
--rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0b7/orwynn/router/test_globalroute.py
--rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0b7/orwynn/singleton/__init__.py
--rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0b7/orwynn/singleton/singleton.py
--rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0b7/orwynn/sql/__init__.py
--rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0b7/orwynn/sql/config.py
--rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0b7/orwynn/sql/databasekind.py
--rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0b7/orwynn/sql/poolclass.py
--rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0b7/orwynn/sql/sql.py
--rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0b7/orwynn/sql/table.py
--rw-r--r--   0        0        0     5855 2023-06-09 06:20:20.114767 orwynn-1.0.0b7/orwynn/sql/test_main.py
--rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0b7/orwynn/testing/__init__.py
--rw-r--r--   0        0        0    11299 2023-06-09 07:32:18.165326 orwynn-1.0.0b7/orwynn/testing/client.py
--rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0b7/orwynn/testing/embeddedclient.py
--rw-r--r--   0        0        0     2046 2023-06-09 06:20:20.111767 orwynn-1.0.0b7/orwynn/testing/test_main.py
--rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0b7/orwynn/testingtools/__init__.py
--rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0b7/orwynn/utils/basesubclassable.py
--rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0b7/orwynn/utils/crypto/__init__.py
--rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0b7/orwynn/utils/dt/__init__.py
--rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0b7/orwynn/utils/fmt/__init__.py
--rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0b7/orwynn/utils/fmt/test_main.py
--rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0b7/orwynn/utils/klass/__init__.py
--rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0b7/orwynn/utils/klass/errors.py
--rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0b7/orwynn/utils/klass/test_klass.py
--rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0b7/orwynn/utils/mp/__init__.py
--rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0b7/orwynn/utils/mp/dictpp.py
--rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0b7/orwynn/utils/mp/location.py
--rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0b7/orwynn/utils/mp/test_main.py
--rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0b7/orwynn/utils/protocol.py
--rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0b7/orwynn/utils/rnd/__init__.py
--rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0b7/orwynn/utils/rnd/test_main.py
--rw-r--r--   0        0        0      376 2023-07-05 09:14:52.810766 orwynn-1.0.0b7/orwynn/utils/types.py
--rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0b7/orwynn/utils/uio.py
--rw-r--r--   0        0        0      682 2023-06-09 06:02:47.709865 orwynn-1.0.0b7/orwynn/utils/url/__init__.py
--rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0b7/orwynn/utils/url/helpers.py
--rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0b7/orwynn/utils/url/test_utils.py
--rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0b7/orwynn/utils/url/url.py
--rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0b7/orwynn/utils/url/utils.py
--rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0b7/orwynn/utils/url/vars.py
--rw-r--r--   0        0        0     9150 2023-06-09 06:02:55.428511 orwynn-1.0.0b7/orwynn/utils/validation/__init__.py
--rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0b7/orwynn/utils/validation/errors.py
--rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0b7/orwynn/utils/validation/validator.py
--rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0b7/orwynn/utils/yml/__init__.py
--rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0b7/orwynn/utils/yml/errors.py
--rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0b7/orwynn/websocket/__init__.py
--rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0b7/orwynn/websocket/constants.py
--rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0b7/orwynn/websocket/context/__init__.py
--rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0b7/orwynn/websocket/context/id.py
--rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0b7/orwynn/websocket/context/middleware/builtin.py
--rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0b7/orwynn/websocket/context/middleware/contextbuiltin.py
--rw-r--r--   0        0        0     1241 2023-06-09 06:27:59.917644 orwynn-1.0.0b7/orwynn/websocket/context/test_main.py
--rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0b7/orwynn/websocket/controller/controller.py
--rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0b7/orwynn/websocket/controller/eventhandlermethod.py
--rw-r--r--   0        0        0     3806 2023-06-09 07:21:01.679769 orwynn-1.0.0b7/orwynn/websocket/controller/test_controller.py
--rw-r--r--   0        0        0     2888 2023-06-09 06:20:10.147480 orwynn-1.0.0b7/orwynn/websocket/controller/test_globalroute.py
--rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0b7/orwynn/websocket/errorhandler/default.py
--rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0b7/orwynn/websocket/errorhandler/middleware.py
--rw-r--r--   0        0        0     1699 2023-06-09 06:03:10.090856 orwynn-1.0.0b7/orwynn/websocket/errorhandler/test_default.py
--rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0b7/orwynn/websocket/log/logger.py
--rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0b7/orwynn/websocket/log/middleware.py
--rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0b7/orwynn/websocket/middleware/builtin.py
--rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0b7/orwynn/websocket/middleware/connectionbuiltin.py
--rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0b7/orwynn/websocket/middleware/middleware.py
--rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0b7/orwynn/websocket/middleware/nextcall.py
--rw-r--r--   0        0        0     1053 2023-06-09 06:27:59.918644 orwynn-1.0.0b7/orwynn/websocket/middleware/test_main.py
--rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0b7/orwynn/websocket/routing/dispatchfn.py
--rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0b7/orwynn/websocket/routing/genericfn.py
--rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0b7/orwynn/websocket/routing/handlers.py
--rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0b7/orwynn/websocket/routing/helpers.py
--rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0b7/orwynn/websocket/routing/nextcall.py
--rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0b7/orwynn/websocket/routing/stack.py
--rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0b7/orwynn/websocket/websocket.py
--rw-r--r--   0        0        0      823 2023-07-06 08:33:36.519085 orwynn-1.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 orwynn-1.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-12-08 10:08:41.917165 orwynn-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0      307 2023-05-22 08:29:05.173562 orwynn-1.0.0rc1/README.md
+-rw-r--r--   0        0        0       65 2023-03-07 08:24:06.640906 orwynn-1.0.0rc1/orwynn/__init__.py
+-rw-r--r--   0        0        0     1920 2023-06-08 13:46:47.770769 orwynn-1.0.0rc1/orwynn/apiversion/__init__.py
+-rw-r--r--   0        0        0       54 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/apiversion/errors.py
+-rw-r--r--   0        0        0     4546 2023-06-09 12:16:54.007732 orwynn-1.0.0rc1/orwynn/apiversion/test_main.py
+-rw-r--r--   0        0        0       77 2023-06-08 13:47:49.293428 orwynn-1.0.0rc1/orwynn/app/__init__.py
+-rw-r--r--   0        0        0      400 2023-06-08 13:48:58.389784 orwynn-1.0.0rc1/orwynn/app/apirouter.py
+-rw-r--r--   0        0        0     1484 2023-06-08 13:47:28.661538 orwynn-1.0.0rc1/orwynn/app/apiwebsocketroute.py
+-rw-r--r--   0        0        0     2594 2023-06-09 12:20:44.292995 orwynn-1.0.0rc1/orwynn/app/app.py
+-rw-r--r--   0        0        0      188 2023-06-09 10:55:27.417944 orwynn-1.0.0rc1/orwynn/app/config.py
+-rw-r--r--   0        0        0     1560 2023-06-08 13:47:12.703403 orwynn-1.0.0rc1/orwynn/app/core.py
+-rw-r--r--   0        0        0       97 2023-02-27 12:42:05.392452 orwynn-1.0.0rc1/orwynn/app/mode.py
+-rw-r--r--   0        0        0     2206 2023-06-08 13:47:49.295428 orwynn-1.0.0rc1/orwynn/app/test_main.py
+-rw-r--r--   0        0        0       98 2023-06-09 11:05:03.703488 orwynn-1.0.0rc1/orwynn/app/types.py
+-rw-r--r--   0        0        0     2885 2023-03-07 07:26:27.308262 orwynn-1.0.0rc1/orwynn/app/utils.py
+-rw-r--r--   0        0        0       56 2023-06-08 13:49:42.996486 orwynn-1.0.0rc1/orwynn/apprc/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-27 06:15:50.756268 orwynn-1.0.0rc1/orwynn/apprc/apprc.py
+-rw-r--r--   0        0        0      190 2023-02-27 12:42:54.819951 orwynn-1.0.0rc1/orwynn/apprc/constants.py
+-rw-r--r--   0        0        0       47 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/apprc/errors.py
+-rw-r--r--   0        0        0     3493 2023-06-08 13:49:43.002486 orwynn-1.0.0rc1/orwynn/apprc/parse.py
+-rw-r--r--   0        0        0     2604 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/apprc/test_main.py
+-rw-r--r--   0        0        0      374 2023-03-07 08:25:49.974896 orwynn-1.0.0rc1/orwynn/base/__init__.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:49:50.224117 orwynn-1.0.0rc1/orwynn/base/config/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-09 05:54:54.979178 orwynn-1.0.0rc1/orwynn/base/config/config.py
+-rw-r--r--   0        0        0        0 2022-12-18 22:39:38.591866 orwynn-1.0.0rc1/orwynn/base/config/test_config.py
+-rw-r--r--   0        0        0       35 2023-06-08 13:50:00.474596 orwynn-1.0.0rc1/orwynn/base/controller/__init__.py
+-rw-r--r--   0        0        0     2211 2023-07-06 09:35:56.327943 orwynn-1.0.0rc1/orwynn/base/controller/controller.py
+-rw-r--r--   0        0        0      179 2023-03-06 11:23:49.043895 orwynn-1.0.0rc1/orwynn/base/controller/errors.py
+-rw-r--r--   0        0        0       31 2023-06-08 13:50:07.129259 orwynn-1.0.0rc1/orwynn/base/database/__init__.py
+-rw-r--r--   0        0        0      629 2023-06-08 13:55:40.340226 orwynn-1.0.0rc1/orwynn/base/database/database.py
+-rw-r--r--   0        0        0      528 2023-03-06 11:23:49.038895 orwynn-1.0.0rc1/orwynn/base/database/errors.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/base/error/__init__.py
+-rw-r--r--   0        0        0     1009 2023-04-07 09:58:09.846657 orwynn-1.0.0rc1/orwynn/base/error/code.py
+-rw-r--r--   0        0        0      284 2023-06-08 13:54:00.170896 orwynn-1.0.0rc1/orwynn/base/error/errors.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/base/error/test_main.py
+-rw-r--r--   0        0        0      436 2023-06-08 13:50:50.520080 orwynn-1.0.0rc1/orwynn/base/error/test_utils.py
+-rw-r--r--   0        0        0     2006 2023-06-08 13:54:17.686071 orwynn-1.0.0rc1/orwynn/base/error/utils.py
+-rw-r--r--   0        0        0       86 2023-03-06 11:24:23.455706 orwynn-1.0.0rc1/orwynn/base/error/valueschema.py
+-rw-r--r--   0        0        0       39 2023-06-08 13:54:42.338917 orwynn-1.0.0rc1/orwynn/base/errorhandler/__init__.py
+-rw-r--r--   0        0        0     2364 2023-07-06 10:24:26.021973 orwynn-1.0.0rc1/orwynn/base/errorhandler/errorhandler.py
+-rw-r--r--   0        0        0       82 2023-06-08 13:55:03.438934 orwynn-1.0.0rc1/orwynn/base/middleware/__init__.py
+-rw-r--r--   0        0        0       94 2023-06-08 13:55:03.438934 orwynn-1.0.0rc1/orwynn/base/middleware/globalsetup.py
+-rw-r--r--   0        0        0     2919 2023-04-21 09:59:20.018394 orwynn-1.0.0rc1/orwynn/base/middleware/middleware.py
+-rw-r--r--   0        0        0     1186 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/base/middleware/test_main.py
+-rw-r--r--   0        0        0       25 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/base/model/__init__.py
+-rw-r--r--   0        0        0     1423 2023-07-06 09:10:08.307376 orwynn-1.0.0rc1/orwynn/base/model/model.py
+-rw-r--r--   0        0        0      791 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/base/model/test_model.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:21.285106 orwynn-1.0.0rc1/orwynn/base/module/__init__.py
+-rw-r--r--   0        0        0      308 2023-04-03 14:39:07.523996 orwynn-1.0.0rc1/orwynn/base/module/errors.py
+-rw-r--r--   0        0        0     7183 2023-06-08 13:55:37.034379 orwynn-1.0.0rc1/orwynn/base/module/module.py
+-rw-r--r--   0        0        0      950 2023-06-08 13:55:21.291106 orwynn-1.0.0rc1/orwynn/base/module/test_module.py
+-rw-r--r--   0        0        0       69 2023-06-08 13:55:40.340226 orwynn-1.0.0rc1/orwynn/base/service/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-08 13:55:40.342226 orwynn-1.0.0rc1/orwynn/base/service/framework.py
+-rw-r--r--   0        0        0      286 2023-01-10 09:51:48.349126 orwynn-1.0.0rc1/orwynn/base/service/service.py
+-rw-r--r--   0        0        0       27 2023-06-08 13:55:46.418946 orwynn-1.0.0rc1/orwynn/base/worker/__init__.py
+-rw-r--r--   0        0        0      212 2023-06-09 05:57:10.064779 orwynn-1.0.0rc1/orwynn/base/worker/worker.py
+-rw-r--r--   0        0        0       54 2023-06-08 13:56:30.127942 orwynn-1.0.0rc1/orwynn/boot/__init__.py
+-rw-r--r--   0        0        0    10361 2023-07-06 10:25:59.036484 orwynn-1.0.0rc1/orwynn/boot/boot.py
+-rw-r--r--   0        0        0      716 2023-06-09 05:54:54.987177 orwynn-1.0.0rc1/orwynn/boot/config.py
+-rw-r--r--   0        0        0       95 2023-06-08 13:58:33.909354 orwynn-1.0.0rc1/orwynn/boot/errors.py
+-rw-r--r--   0        0        0     4754 2023-06-09 06:27:59.920644 orwynn-1.0.0rc1/orwynn/boot/test_main.py
+-rw-r--r--   0        0        0      154 2023-06-09 06:20:20.102768 orwynn-1.0.0rc1/orwynn/bootscript/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-08 13:59:21.194248 orwynn-1.0.0rc1/orwynn/bootscript/bootscript.py
+-rw-r--r--   0        0        0       70 2023-03-06 14:58:11.412882 orwynn-1.0.0rc1/orwynn/bootscript/callable.py
+-rw-r--r--   0        0        0      240 2023-03-06 13:38:38.458249 orwynn-1.0.0rc1/orwynn/bootscript/calltime.py
+-rw-r--r--   0        0        0      220 2023-03-06 14:11:14.410261 orwynn-1.0.0rc1/orwynn/bootscript/errors.py
+-rw-r--r--   0        0        0      860 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/bootscript/test_main.py
+-rw-r--r--   0        0        0     2300 2023-06-09 06:20:20.107768 orwynn-1.0.0rc1/orwynn/bootscript/worker.py
+-rw-r--r--   0        0        0       73 2023-06-08 13:59:41.390353 orwynn-1.0.0rc1/orwynn/context/__init__.py
+-rw-r--r--   0        0        0      318 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/context/errors.py
+-rw-r--r--   0        0        0      643 2023-06-08 13:59:41.391353 orwynn-1.0.0rc1/orwynn/context/manager.py
+-rw-r--r--   0        0        0     2656 2023-06-08 13:55:46.418946 orwynn-1.0.0rc1/orwynn/context/storage.py
+-rw-r--r--   0        0        0       97 2023-06-08 14:06:22.928960 orwynn-1.0.0rc1/orwynn/di/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-06 09:39:22.689224 orwynn-1.0.0rc1/orwynn/di/acceptor.py
+-rw-r--r--   0        0        0     3780 2023-06-09 06:21:27.250456 orwynn-1.0.0rc1/orwynn/di/availability.py
+-rw-r--r--   0        0        0     1719 2023-06-09 06:20:20.108768 orwynn-1.0.0rc1/orwynn/di/collecting/acceptordependencies.py
+-rw-r--r--   0        0        0     1219 2023-06-08 14:24:49.757165 orwynn-1.0.0rc1/orwynn/di/collecting/errors.py
+-rw-r--r--   0        0        0     3128 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/di/collecting/helpers.py
+-rw-r--r--   0        0        0     3232 2023-04-03 14:59:49.701980 orwynn-1.0.0rc1/orwynn/di/collecting/modulecollector.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:31:34.417910 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/__init__.py
+-rw-r--r--   0        0        0     3229 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/collect.py
+-rw-r--r--   0        0        0     2341 2023-06-09 07:32:02.380043 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/map.py
+-rw-r--r--   0        0        0     1765 2023-06-09 06:20:20.109768 orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/test_main.py
+-rw-r--r--   0        0        0     1084 2023-06-09 06:20:20.103768 orwynn-1.0.0rc1/orwynn/di/collecting/test_modules.py
+-rw-r--r--   0        0        0      840 2023-06-08 14:24:49.775165 orwynn-1.0.0rc1/orwynn/di/constants.py
+-rw-r--r--   0        0        0     5895 2023-06-09 07:32:02.385042 orwynn-1.0.0rc1/orwynn/di/container.py
+-rw-r--r--   0        0        0     4694 2023-06-09 06:20:20.104768 orwynn-1.0.0rc1/orwynn/di/di.py
+-rw-r--r--   0        0        0     1260 2023-06-08 14:25:37.475430 orwynn-1.0.0rc1/orwynn/di/errors.py
+-rw-r--r--   0        0        0     6756 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/di/init/acceptors.py
+-rw-r--r--   0        0        0     4115 2023-06-09 06:22:50.702901 orwynn-1.0.0rc1/orwynn/di/init/providers.py
+-rw-r--r--   0        0        0     2871 2023-06-09 06:20:20.106768 orwynn-1.0.0rc1/orwynn/di/init/test_acceptors.py
+-rw-r--r--   0        0        0      615 2023-06-09 06:23:04.561666 orwynn-1.0.0rc1/orwynn/di/init/test_providers.py
+-rw-r--r--   0        0        0      327 2023-06-08 14:06:45.172014 orwynn-1.0.0rc1/orwynn/di/isacceptor.py
+-rw-r--r--   0        0        0      325 2023-06-08 14:09:24.648261 orwynn-1.0.0rc1/orwynn/di/isprovider.py
+-rw-r--r--   0        0        0      140 2023-02-15 12:49:24.369340 orwynn-1.0.0rc1/orwynn/di/object.py
+-rw-r--r--   0        0        0       45 2023-07-06 09:39:13.705327 orwynn-1.0.0rc1/orwynn/di/provider.py
+-rw-r--r--   0        0        0      506 2023-06-09 06:20:20.105768 orwynn-1.0.0rc1/orwynn/di/testing.py
+-rw-r--r--   0        0        0      877 2023-06-09 06:03:05.647671 orwynn-1.0.0rc1/orwynn/helpers/constants.py
+-rw-r--r--   0        0        0      455 2023-07-04 11:25:22.457577 orwynn-1.0.0rc1/orwynn/helpers/errors.py
+-rw-r--r--   0        0        0     1140 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/helpers/web.py
+-rw-r--r--   0        0        0     1118 2023-06-09 06:20:20.105768 orwynn-1.0.0rc1/orwynn/http/__init__.py
+-rw-r--r--   0        0        0      922 2023-06-09 06:20:20.109768 orwynn-1.0.0rc1/orwynn/http/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:32.323279 orwynn-1.0.0rc1/orwynn/http/context/__init__.py
+-rw-r--r--   0        0        0      959 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/http/context/id.py
+-rw-r--r--   0        0        0      617 2023-06-09 05:50:36.441513 orwynn-1.0.0rc1/orwynn/http/context/middleware/builtin.py
+-rw-r--r--   0        0        0      754 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0      984 2023-06-09 06:27:59.920644 orwynn-1.0.0rc1/orwynn/http/context/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:14.697646 orwynn-1.0.0rc1/orwynn/http/controller/__init__.py
+-rw-r--r--   0        0        0     5446 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/http/controller/controller.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:36:46.319189 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/__init__.py
+-rw-r--r--   0        0        0     1130 2023-06-09 05:49:31.580107 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/container.py
+-rw-r--r--   0        0        0     1231 2023-06-09 05:49:40.023769 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/endpoint.py
+-rw-r--r--   0        0        0      215 2023-06-09 05:51:12.418075 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/response.py
+-rw-r--r--   0        0        0     2231 2023-06-08 13:56:18.457476 orwynn-1.0.0rc1/orwynn/http/controller/endpoint/test_main.py
+-rw-r--r--   0        0        0       64 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/http/controller/errors.py
+-rw-r--r--   0        0        0     7262 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/http/controller/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:19:12.185278 orwynn-1.0.0rc1/orwynn/http/cors/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-09 11:03:10.108801 orwynn-1.0.0rc1/orwynn/http/cors/cors.py
+-rw-r--r--   0        0        0     3491 2023-06-09 12:32:20.369783 orwynn-1.0.0rc1/orwynn/http/cors/test_main.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:37:51.749042 orwynn-1.0.0rc1/orwynn/http/errorhandler/__init__.py
+-rw-r--r--   0        0        0     1204 2023-06-09 06:20:20.110767 orwynn-1.0.0rc1/orwynn/http/errorhandler/default.py
+-rw-r--r--   0        0        0     1094 2023-06-09 05:50:36.426514 orwynn-1.0.0rc1/orwynn/http/errorhandler/middleware.py
+-rw-r--r--   0        0        0     6129 2023-06-09 07:32:02.382043 orwynn-1.0.0rc1/orwynn/http/errorhandler/test_main.py
+-rw-r--r--   0        0        0      220 2023-03-06 11:30:55.550595 orwynn-1.0.0rc1/orwynn/http/errors.py
+-rw-r--r--   0        0        0     4525 2023-06-09 05:47:03.116046 orwynn-1.0.0rc1/orwynn/http/log/logger.py
+-rw-r--r--   0        0        0     1145 2023-06-09 05:50:42.043289 orwynn-1.0.0rc1/orwynn/http/log/middleware.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:38:13.602306 orwynn-1.0.0rc1/orwynn/http/middleware/__init__.py
+-rw-r--r--   0        0        0      274 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/middleware/builtinmiddleware.py
+-rw-r--r--   0        0        0      652 2023-06-09 05:50:36.430513 orwynn-1.0.0rc1/orwynn/http/middleware/middleware.py
+-rw-r--r--   0        0        0      327 2023-06-09 05:47:03.114046 orwynn-1.0.0rc1/orwynn/http/middleware/nextcall.py
+-rw-r--r--   0        0        0     2150 2023-06-09 06:00:41.008691 orwynn-1.0.0rc1/orwynn/http/middleware/test_main.py
+-rw-r--r--   0        0        0       76 2023-02-21 09:41:40.933060 orwynn-1.0.0rc1/orwynn/http/requests.py
+-rw-r--r--   0        0        0      577 2023-05-22 07:24:03.129227 orwynn-1.0.0rc1/orwynn/http/responses.py
+-rw-r--r--   0        0        0      149 2023-03-06 11:39:39.812830 orwynn-1.0.0rc1/orwynn/http/schema/validationvalue.py
+-rw-r--r--   0        0        0      120 2023-03-06 11:39:26.483900 orwynn-1.0.0rc1/orwynn/http/schema/value.py
+-rw-r--r--   0        0        0      873 2023-06-09 05:50:36.425514 orwynn-1.0.0rc1/orwynn/http/test_responses.py
+-rw-r--r--   0        0        0      126 2023-02-27 07:08:40.302249 orwynn-1.0.0rc1/orwynn/http/testing.py
+-rw-r--r--   0        0        0      145 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/indication/__init__.py
+-rw-r--r--   0        0        0      231 2023-06-09 05:51:42.027891 orwynn-1.0.0rc1/orwynn/indication/default.py
+-rw-r--r--   0        0        0      213 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/indication/errors.py
+-rw-r--r--   0        0        0      186 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/indication/indicatable.py
+-rw-r--r--   0        0        0    11518 2023-06-09 07:31:49.349629 orwynn-1.0.0rc1/orwynn/indication/indication.py
+-rw-r--r--   0        0        0      373 2023-02-10 07:31:06.809383 orwynn-1.0.0rc1/orwynn/indication/indicator.py
+-rw-r--r--   0        0        0     3422 2023-06-09 07:31:58.353224 orwynn-1.0.0rc1/orwynn/indication/test_main.py
+-rw-r--r--   0        0        0      491 2023-02-10 07:37:36.270095 orwynn-1.0.0rc1/orwynn/indication/type.py
+-rw-r--r--   0        0        0      120 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/log/__init__.py
+-rw-r--r--   0        0        0      152 2023-06-09 05:51:55.299360 orwynn-1.0.0rc1/orwynn/log/config.py
+-rw-r--r--   0        0        0     1972 2023-06-09 07:45:46.128730 orwynn-1.0.0rc1/orwynn/log/configure.py
+-rw-r--r--   0        0        0      114 2023-02-13 09:24:59.764293 orwynn-1.0.0rc1/orwynn/log/constants.py
+-rw-r--r--   0        0        0       99 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/log/errors.py
+-rw-r--r--   0        0        0      870 2023-06-09 07:50:28.243651 orwynn-1.0.0rc1/orwynn/log/handler.py
+-rw-r--r--   0        0        0      540 2023-06-09 05:52:01.299120 orwynn-1.0.0rc1/orwynn/log/helpers.py
+-rw-r--r--   0        0        0       35 2023-02-14 07:07:42.021607 orwynn-1.0.0rc1/orwynn/log/log.py
+-rw-r--r--   0        0        0     1767 2023-06-09 07:50:09.129655 orwynn-1.0.0rc1/orwynn/log/test_main.py
+-rw-r--r--   0        0        0     3679 2023-06-09 06:00:41.008691 orwynn-1.0.0rc1/orwynn/log/test_middleware.py
+-rw-r--r--   0        0        0     1443 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/log/test_websocketmiddleware.py
+-rw-r--r--   0        0        0       83 2023-06-09 07:50:59.221569 orwynn-1.0.0rc1/orwynn/log/types.py
+-rw-r--r--   0        0        0       29 2023-06-09 05:52:49.668187 orwynn-1.0.0rc1/orwynn/mapping/__init__.py
+-rw-r--r--   0        0        0      667 2023-07-05 09:49:27.438110 orwynn-1.0.0rc1/orwynn/mapping/errors.py
+-rw-r--r--   0        0        0     1808 2023-07-05 09:47:23.970713 orwynn-1.0.0rc1/orwynn/mapping/mapping.py
+-rw-r--r--   0        0        0      504 2023-07-05 09:49:15.096266 orwynn-1.0.0rc1/orwynn/mapping/test_main.py
+-rw-r--r--   0        0        0      216 2023-07-04 11:01:21.049070 orwynn-1.0.0rc1/orwynn/mongo/__init__.py
+-rw-r--r--   0        0        0      111 2022-12-25 22:05:28.493755 orwynn-1.0.0rc1/orwynn/mongo/clientsession.py
+-rw-r--r--   0        0        0      133 2023-02-27 09:58:10.560648 orwynn-1.0.0rc1/orwynn/mongo/config.py
+-rw-r--r--   0        0        0     7634 2023-07-06 08:54:40.455677 orwynn-1.0.0rc1/orwynn/mongo/document/__init__.py
+-rw-r--r--   0        0        0      578 2023-07-06 07:33:03.897136 orwynn-1.0.0rc1/orwynn/mongo/document/errors.py
+-rw-r--r--   0        0        0     1134 2023-07-05 09:33:28.956933 orwynn-1.0.0rc1/orwynn/mongo/document/helpers.py
+-rw-r--r--   0        0        0     1367 2023-07-05 09:33:28.955933 orwynn-1.0.0rc1/orwynn/mongo/document/test_converttoobjectid.py
+-rw-r--r--   0        0        0      219 2023-07-06 06:48:26.581243 orwynn-1.0.0rc1/orwynn/mongo/document/test_create.py
+-rw-r--r--   0        0        0      742 2023-07-06 07:53:44.416182 orwynn-1.0.0rc1/orwynn/mongo/document/test_get.py
+-rw-r--r--   0        0        0      703 2023-07-06 08:55:42.984735 orwynn-1.0.0rc1/orwynn/mongo/document/test_inc.py
+-rw-r--r--   0        0        0      275 2023-07-06 07:46:04.044931 orwynn-1.0.0rc1/orwynn/mongo/document/test_refresh.py
+-rw-r--r--   0        0        0      230 2023-07-06 06:48:10.593442 orwynn-1.0.0rc1/orwynn/mongo/document/test_remove.py
+-rw-r--r--   0        0        0      829 2023-07-06 08:55:42.984735 orwynn-1.0.0rc1/orwynn/mongo/document/test_set.py
+-rw-r--r--   0        0        0     1312 2023-07-06 07:42:00.340990 orwynn-1.0.0rc1/orwynn/mongo/document/test_updateoperators.py
+-rw-r--r--   0        0        0      708 2023-07-06 08:51:37.969595 orwynn-1.0.0rc1/orwynn/mongo/document/testing.py
+-rw-r--r--   0        0        0       19 2022-12-25 11:43:30.248664 orwynn-1.0.0rc1/orwynn/mongo/entity.py
+-rw-r--r--   0        0        0      882 2023-07-05 09:49:15.103266 orwynn-1.0.0rc1/orwynn/mongo/errors.py
+-rw-r--r--   0        0        0     3567 2023-06-09 05:54:25.941338 orwynn-1.0.0rc1/orwynn/mongo/mongo.py
+-rw-r--r--   0        0        0     1354 2023-07-04 11:01:22.010065 orwynn-1.0.0rc1/orwynn/mongo/test_main.py
+-rw-r--r--   0        0        0      395 2023-07-06 07:28:27.154203 orwynn-1.0.0rc1/orwynn/mongo/testing.py
+-rw-r--r--   0        0        0     2839 2023-06-09 06:03:10.133848 orwynn-1.0.0rc1/orwynn/proxy/boot.py
+-rw-r--r--   0        0        0      310 2023-03-07 08:22:29.576929 orwynn-1.0.0rc1/orwynn/proxy/indicationonly.py
+-rw-r--r--   0        0        0       27 2023-06-09 05:56:44.921784 orwynn-1.0.0rc1/orwynn/router/__init__.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:23:57.815708 orwynn-1.0.0rc1/orwynn/router/errorhandlermanager.py
+-rw-r--r--   0        0        0      116 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/router/errors.py
+-rw-r--r--   0        0        0    14259 2023-06-09 06:03:10.133848 orwynn-1.0.0rc1/orwynn/router/register/controller.py
+-rw-r--r--   0        0        0     9656 2023-06-09 11:05:03.703488 orwynn-1.0.0rc1/orwynn/router/register/middleware.py
+-rw-r--r--   0        0        0     2565 2023-06-09 11:05:03.696488 orwynn-1.0.0rc1/orwynn/router/router.py
+-rw-r--r--   0        0        0     2465 2023-02-28 05:48:16.660066 orwynn-1.0.0rc1/orwynn/router/test_globalroute.py
+-rw-r--r--   0        0        0       33 2023-06-09 05:57:10.064779 orwynn-1.0.0rc1/orwynn/singleton/__init__.py
+-rw-r--r--   0        0        0     1318 2023-06-09 06:27:33.730658 orwynn-1.0.0rc1/orwynn/singleton/singleton.py
+-rw-r--r--   0        0        0      203 2023-06-09 06:20:20.112767 orwynn-1.0.0rc1/orwynn/sql/__init__.py
+-rw-r--r--   0        0        0     1964 2023-06-09 06:00:27.751246 orwynn-1.0.0rc1/orwynn/sql/config.py
+-rw-r--r--   0        0        0      105 2023-01-19 15:20:28.442785 orwynn-1.0.0rc1/orwynn/sql/databasekind.py
+-rw-r--r--   0        0        0       65 2023-02-28 06:53:56.326285 orwynn-1.0.0rc1/orwynn/sql/poolclass.py
+-rw-r--r--   0        0        0     3878 2023-06-09 06:00:31.786840 orwynn-1.0.0rc1/orwynn/sql/sql.py
+-rw-r--r--   0        0        0     2636 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/sql/table.py
+-rw-r--r--   0        0        0     5855 2023-06-09 06:20:20.114767 orwynn-1.0.0rc1/orwynn/sql/test_main.py
+-rw-r--r--   0        0        0      721 2023-06-09 06:00:51.915024 orwynn-1.0.0rc1/orwynn/testing/__init__.py
+-rw-r--r--   0        0        0    11299 2023-06-09 07:32:18.165326 orwynn-1.0.0rc1/orwynn/testing/client.py
+-rw-r--r--   0        0        0      101 2022-12-29 09:50:50.883906 orwynn-1.0.0rc1/orwynn/testing/embeddedclient.py
+-rw-r--r--   0        0        0     2046 2023-06-09 06:20:20.111767 orwynn-1.0.0rc1/orwynn/testing/test_main.py
+-rw-r--r--   0        0        0     1106 2023-05-22 08:13:58.515604 orwynn-1.0.0rc1/orwynn/testingtools/__init__.py
+-rw-r--r--   0        0        0       24 2022-12-22 07:52:56.312366 orwynn-1.0.0rc1/orwynn/utils/basesubclassable.py
+-rw-r--r--   0        0        0      866 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/crypto/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-09 07:42:13.220704 orwynn-1.0.0rc1/orwynn/utils/dt/__init__.py
+-rw-r--r--   0        0        0     1746 2023-02-23 07:22:44.852890 orwynn-1.0.0rc1/orwynn/utils/fmt/__init__.py
+-rw-r--r--   0        0        0     1312 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/fmt/test_main.py
+-rw-r--r--   0        0        0     1973 2023-06-09 06:01:29.753531 orwynn-1.0.0rc1/orwynn/utils/klass/__init__.py
+-rw-r--r--   0        0        0       46 2023-03-07 05:33:50.925367 orwynn-1.0.0rc1/orwynn/utils/klass/errors.py
+-rw-r--r--   0        0        0      522 2023-04-07 10:26:52.657368 orwynn-1.0.0rc1/orwynn/utils/klass/test_klass.py
+-rw-r--r--   0        0        0     2544 2023-06-09 06:01:41.912390 orwynn-1.0.0rc1/orwynn/utils/mp/__init__.py
+-rw-r--r--   0        0        0       98 2023-01-11 10:48:59.268124 orwynn-1.0.0rc1/orwynn/utils/mp/dictpp.py
+-rw-r--r--   0        0        0     2448 2023-03-06 11:30:55.553595 orwynn-1.0.0rc1/orwynn/utils/mp/location.py
+-rw-r--r--   0        0        0     1737 2023-06-09 06:01:41.912390 orwynn-1.0.0rc1/orwynn/utils/mp/test_main.py
+-rw-r--r--   0        0        0      133 2023-02-17 07:27:38.315341 orwynn-1.0.0rc1/orwynn/utils/protocol.py
+-rw-r--r--   0        0        0      131 2023-07-05 09:50:46.441135 orwynn-1.0.0rc1/orwynn/utils/rnd/__init__.py
+-rw-r--r--   0        0        0       90 2023-07-05 09:50:46.449134 orwynn-1.0.0rc1/orwynn/utils/rnd/test_main.py
+-rw-r--r--   0        0        0      376 2023-07-05 09:14:52.810766 orwynn-1.0.0rc1/orwynn/utils/types.py
+-rw-r--r--   0        0        0      307 2023-03-07 05:31:01.650091 orwynn-1.0.0rc1/orwynn/utils/uio.py
+-rw-r--r--   0        0        0      682 2023-06-09 06:02:47.709865 orwynn-1.0.0rc1/orwynn/utils/url/__init__.py
+-rw-r--r--   0        0        0     1921 2023-06-09 06:20:20.108768 orwynn-1.0.0rc1/orwynn/utils/url/helpers.py
+-rw-r--r--   0        0        0     1405 2023-06-09 06:02:47.710864 orwynn-1.0.0rc1/orwynn/utils/url/test_utils.py
+-rw-r--r--   0        0        0       79 2023-02-22 12:14:57.519901 orwynn-1.0.0rc1/orwynn/utils/url/url.py
+-rw-r--r--   0        0        0      419 2023-06-09 06:02:30.816698 orwynn-1.0.0rc1/orwynn/utils/url/utils.py
+-rw-r--r--   0        0        0      253 2023-06-09 06:02:47.709865 orwynn-1.0.0rc1/orwynn/utils/url/vars.py
+-rw-r--r--   0        0        0     9150 2023-06-09 06:02:55.428511 orwynn-1.0.0rc1/orwynn/utils/validation/__init__.py
+-rw-r--r--   0        0        0     1796 2023-03-07 05:27:06.425420 orwynn-1.0.0rc1/orwynn/utils/validation/errors.py
+-rw-r--r--   0        0        0      216 2022-12-16 11:42:54.126673 orwynn-1.0.0rc1/orwynn/utils/validation/validator.py
+-rw-r--r--   0        0        0     1743 2023-04-03 14:59:49.716980 orwynn-1.0.0rc1/orwynn/utils/yml/__init__.py
+-rw-r--r--   0        0        0       42 2023-03-06 11:23:49.055894 orwynn-1.0.0rc1/orwynn/utils/yml/errors.py
+-rw-r--r--   0        0        0      638 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/websocket/__init__.py
+-rw-r--r--   0        0        0      995 2023-06-09 06:20:20.113767 orwynn-1.0.0rc1/orwynn/websocket/constants.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:40:48.176846 orwynn-1.0.0rc1/orwynn/websocket/context/__init__.py
+-rw-r--r--   0        0        0     1028 2023-07-05 09:50:46.450135 orwynn-1.0.0rc1/orwynn/websocket/context/id.py
+-rw-r--r--   0        0        0      550 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/context/middleware/builtin.py
+-rw-r--r--   0        0        0      768 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/context/middleware/contextbuiltin.py
+-rw-r--r--   0        0        0     1241 2023-06-09 06:27:59.917644 orwynn-1.0.0rc1/orwynn/websocket/context/test_main.py
+-rw-r--r--   0        0        0     3966 2023-06-09 06:20:10.146480 orwynn-1.0.0rc1/orwynn/websocket/controller/controller.py
+-rw-r--r--   0        0        0      146 2023-06-08 13:55:11.806546 orwynn-1.0.0rc1/orwynn/websocket/controller/eventhandlermethod.py
+-rw-r--r--   0        0        0     3806 2023-06-09 07:21:01.679769 orwynn-1.0.0rc1/orwynn/websocket/controller/test_controller.py
+-rw-r--r--   0        0        0     2888 2023-06-09 06:20:10.147480 orwynn-1.0.0rc1/orwynn/websocket/controller/test_globalroute.py
+-rw-r--r--   0        0        0      410 2023-06-09 06:16:27.158191 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/default.py
+-rw-r--r--   0        0        0     3514 2023-06-09 06:20:20.115767 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/middleware.py
+-rw-r--r--   0        0        0     1699 2023-06-09 06:03:10.090856 orwynn-1.0.0rc1/orwynn/websocket/errorhandler/test_default.py
+-rw-r--r--   0        0        0     1706 2023-06-09 06:16:27.191193 orwynn-1.0.0rc1/orwynn/websocket/log/logger.py
+-rw-r--r--   0        0        0      910 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/log/middleware.py
+-rw-r--r--   0        0        0      303 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/middleware/builtin.py
+-rw-r--r--   0        0        0      856 2023-06-09 06:20:10.150480 orwynn-1.0.0rc1/orwynn/websocket/middleware/connectionbuiltin.py
+-rw-r--r--   0        0        0      737 2023-06-09 06:20:10.149480 orwynn-1.0.0rc1/orwynn/websocket/middleware/middleware.py
+-rw-r--r--   0        0        0      279 2023-06-09 06:16:27.159191 orwynn-1.0.0rc1/orwynn/websocket/middleware/nextcall.py
+-rw-r--r--   0        0        0     1053 2023-06-09 06:27:59.918644 orwynn-1.0.0rc1/orwynn/websocket/middleware/test_main.py
+-rw-r--r--   0        0        0      220 2023-06-09 06:16:27.190193 orwynn-1.0.0rc1/orwynn/websocket/routing/dispatchfn.py
+-rw-r--r--   0        0        0       92 2023-02-15 09:24:37.556326 orwynn-1.0.0rc1/orwynn/websocket/routing/genericfn.py
+-rw-r--r--   0        0        0      427 2023-06-09 06:15:15.485170 orwynn-1.0.0rc1/orwynn/websocket/routing/handlers.py
+-rw-r--r--   0        0        0     5607 2023-06-09 07:32:02.386042 orwynn-1.0.0rc1/orwynn/websocket/routing/helpers.py
+-rw-r--r--   0        0        0     1880 2023-06-09 06:20:20.114767 orwynn-1.0.0rc1/orwynn/websocket/routing/nextcall.py
+-rw-r--r--   0        0        0     6065 2023-06-09 06:16:27.192193 orwynn-1.0.0rc1/orwynn/websocket/routing/stack.py
+-rw-r--r--   0        0        0       82 2022-12-25 23:39:24.206537 orwynn-1.0.0rc1/orwynn/websocket/websocket.py
+-rw-r--r--   0        0        0      928 2023-07-06 10:45:11.657758 orwynn-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1281 1970-01-01 00:00:00.000000 orwynn-1.0.0rc1/PKG-INFO
```

### Comparing `orwynn-1.0.0b7/LICENSE` & `orwynn-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/apiversion/__init__.py` & `orwynn-1.0.0rc1/orwynn/apiversion/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/apiversion/test_main.py` & `orwynn-1.0.0rc1/orwynn/apiversion/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/app/apiwebsocketroute.py` & `orwynn-1.0.0rc1/orwynn/app/apiwebsocketroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/app/app.py` & `orwynn-1.0.0rc1/orwynn/app/app.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/app/core.py` & `orwynn-1.0.0rc1/orwynn/app/core.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/app/test_main.py` & `orwynn-1.0.0rc1/orwynn/app/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/app/utils.py` & `orwynn-1.0.0rc1/orwynn/app/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/apprc/parse.py` & `orwynn-1.0.0rc1/orwynn/apprc/parse.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/apprc/test_main.py` & `orwynn-1.0.0rc1/orwynn/apprc/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/config/config.py` & `orwynn-1.0.0rc1/orwynn/base/config/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/controller/controller.py` & `orwynn-1.0.0rc1/orwynn/base/controller/controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
     MissingControllerClassAttributeError,
 )
 from orwynn.utils import validation
 from orwynn.utils.url import match_routes
 
 
 class Controller:
-    """Entrypoint to some operational service."""
+    """
+    Entrypoint to some operational service.
+    """
     ROUTE: ClassVar[str | None] = None
     VERSION: ClassVar[int | set[int] | Literal["*"] | None] = None
 
     def __init__(self) -> None:
         # Actual route for the controller assigned at boottime
         self._final_routes: set[str] = set()
```

### Comparing `orwynn-1.0.0b7/orwynn/base/database/database.py` & `orwynn-1.0.0rc1/orwynn/base/database/database.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/database/errors.py` & `orwynn-1.0.0rc1/orwynn/base/database/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/error/code.py` & `orwynn-1.0.0rc1/orwynn/base/error/code.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/error/test_main.py` & `orwynn-1.0.0rc1/orwynn/base/error/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/error/utils.py` & `orwynn-1.0.0rc1/orwynn/base/error/utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/errorhandler/errorhandler.py` & `orwynn-1.0.0rc1/orwynn/base/errorhandler/errorhandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from orwynn.log.helpers import catch_error
 from orwynn.proxy.boot import BootProxy
 from orwynn.utils import validation
 from orwynn.utils.protocol import Protocol
 
 
 class ErrorHandler:
-    """Handles outcoming errors from the application.
+    """
+    Handles outcoming errors from the application.
     Method handle(...) should be redefined in subclass in order to work.
 
-    Class-Attributes:
+    Attributes:
         E:
             Exception or a list of handled Exceptions.
         PROTOCOL:
             Protocol the handler works with.
         IS_ERROR_CATCH_LOGGED:
             Whether the handled errors should be automatically logged by
             Log.catch. Defaults to True.
```

### Comparing `orwynn-1.0.0b7/orwynn/base/middleware/middleware.py` & `orwynn-1.0.0rc1/orwynn/base/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/middleware/test_main.py` & `orwynn-1.0.0rc1/orwynn/base/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/model/model.py` & `orwynn-1.0.0rc1/orwynn/base/model/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 RecoverType = TypeVar("RecoverType", bound="Model")
 
 
 class Model(pydantic.BaseModel):
     """Basic way to represent a data in the app.
 
-    Class-Attributes:
+    Attributes:
         INDICATION_TYPE (optional):
             Type to be displayed in final response body. Defaults to OK.
     """
     INDICATION_TYPE: ClassVar[Union["IndicationType", None]] = None
 
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
```

### Comparing `orwynn-1.0.0b7/orwynn/base/model/test_model.py` & `orwynn-1.0.0rc1/orwynn/base/model/test_model.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/module/module.py` & `orwynn-1.0.0rc1/orwynn/base/module/module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/base/module/test_module.py` & `orwynn-1.0.0rc1/orwynn/base/module/test_module.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/boot/boot.py` & `orwynn-1.0.0rc1/orwynn/boot/boot.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,20 +74,20 @@
             Object describes API versioning rules for the project. By default
             only v1 is supported.
         bootscripts (optional):
             List of bootscripts to be launched at different points of boot
             time.
 
     Environs:
-        ORWYNN_MODE:
+        - ORWYNN_MODE:
             Boot mode for application. Defaults to DEV. Alternatively you can
             pass arg "mode".
-        ORWYNN_ROOT_DIR:
+        - ORWYNN_ROOT_DIR:
             Root directory for application. Defaults to os.getcwd()
-        ORWYNN_APPRC_PATH:
+        - ORWYNN_APPRC_PATH:
             Path where app configuration file located. Defaults to
             "./apprc.yml". Alternatively you can pass a dictionary directly in
             "apprc" attribute.
 
     Usage:
     ```py
     # main.py
```

### Comparing `orwynn-1.0.0b7/orwynn/boot/config.py` & `orwynn-1.0.0rc1/orwynn/boot/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/boot/test_main.py` & `orwynn-1.0.0rc1/orwynn/boot/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/bootscript/test_main.py` & `orwynn-1.0.0rc1/orwynn/bootscript/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/bootscript/worker.py` & `orwynn-1.0.0rc1/orwynn/bootscript/worker.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/context/manager.py` & `orwynn-1.0.0rc1/orwynn/context/manager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/context/storage.py` & `orwynn-1.0.0rc1/orwynn/context/storage.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/availability.py` & `orwynn-1.0.0rc1/orwynn/di/availability.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/acceptordependencies.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/acceptordependencies.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/errors.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/helpers.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/modulecollector.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/modulecollector.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/collect.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/collect.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/map.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/map.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/providerdependencies/test_main.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/providerdependencies/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/collecting/test_modules.py` & `orwynn-1.0.0rc1/orwynn/di/collecting/test_modules.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/constants.py` & `orwynn-1.0.0rc1/orwynn/di/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/container.py` & `orwynn-1.0.0rc1/orwynn/di/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/di.py` & `orwynn-1.0.0rc1/orwynn/di/di.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/errors.py` & `orwynn-1.0.0rc1/orwynn/di/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/init/acceptors.py` & `orwynn-1.0.0rc1/orwynn/di/init/acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/init/providers.py` & `orwynn-1.0.0rc1/orwynn/di/init/providers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/init/test_acceptors.py` & `orwynn-1.0.0rc1/orwynn/di/init/test_acceptors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/di/init/test_providers.py` & `orwynn-1.0.0rc1/orwynn/di/init/test_providers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/helpers/constants.py` & `orwynn-1.0.0rc1/orwynn/helpers/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/helpers/web.py` & `orwynn-1.0.0rc1/orwynn/helpers/web.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/__init__.py` & `orwynn-1.0.0rc1/orwynn/http/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/constants.py` & `orwynn-1.0.0rc1/orwynn/http/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/context/id.py` & `orwynn-1.0.0rc1/orwynn/http/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/context/middleware/builtin.py` & `orwynn-1.0.0rc1/orwynn/http/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc1/orwynn/http/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/context/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/context/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/controller/controller.py` & `orwynn-1.0.0rc1/orwynn/http/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/controller/endpoint/container.py` & `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/container.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/controller/endpoint/endpoint.py` & `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/controller/endpoint/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/controller/endpoint/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/controller/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/controller/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/cors/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/cors/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/errorhandler/default.py` & `orwynn-1.0.0rc1/orwynn/http/errorhandler/default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/errorhandler/middleware.py` & `orwynn-1.0.0rc1/orwynn/http/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/errorhandler/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/errorhandler/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/log/logger.py` & `orwynn-1.0.0rc1/orwynn/http/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/log/middleware.py` & `orwynn-1.0.0rc1/orwynn/http/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/middleware/middleware.py` & `orwynn-1.0.0rc1/orwynn/http/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/middleware/test_main.py` & `orwynn-1.0.0rc1/orwynn/http/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/responses.py` & `orwynn-1.0.0rc1/orwynn/http/responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/http/test_responses.py` & `orwynn-1.0.0rc1/orwynn/http/test_responses.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/indication/indication.py` & `orwynn-1.0.0rc1/orwynn/indication/indication.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/indication/test_main.py` & `orwynn-1.0.0rc1/orwynn/indication/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/configure.py` & `orwynn-1.0.0rc1/orwynn/log/configure.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/handler.py` & `orwynn-1.0.0rc1/orwynn/log/handler.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/helpers.py` & `orwynn-1.0.0rc1/orwynn/log/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/test_main.py` & `orwynn-1.0.0rc1/orwynn/log/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/test_middleware.py` & `orwynn-1.0.0rc1/orwynn/log/test_middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/log/test_websocketmiddleware.py` & `orwynn-1.0.0rc1/orwynn/log/test_websocketmiddleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mapping/errors.py` & `orwynn-1.0.0rc1/orwynn/mapping/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mapping/mapping.py` & `orwynn-1.0.0rc1/orwynn/mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/__init__.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -163,18 +163,16 @@
         validation.validate(set, [dict, NoneType])
         validation.validate(inc, [dict, NoneType])
 
         id: str = self.getid()
 
         operation: dict = {}
         if set is not None:
-            self._validate_update_dict(set)
             operation["$set"] = set
         if inc is not None:
-            self._validate_update_dict(inc)
             operation["$inc"] = inc
         if operators is not None:
             if "$set" in operators:
                 raise InvalidOperatorError(
                     operator="$set",
                     explanation="pass it via keyword argument `set=`"
                 )
@@ -242,30 +240,7 @@
     @staticmethod
     def _adjust_id_from_mongo(data: dict) -> dict:
         if "_id" in data:
             if data["_id"] is not None:
                 data["id"] = str(data["_id"])
             del data["_id"]
         return data
-
-    def _validate_update_dict(self, dct: dict) -> None:
-        fields: dict[str, ModelField] = self.__fields__
-
-        for k, v in dct.items():
-            if "." in k:
-                nesting: list[str] = k.split(".")
-
-                # check only outermost key, inner keys can be easily inserted
-                # and updated without additional default checks. In case of
-                # nesting, the value to check should always be dictionary.
-                self._validate_update_dict({nesting[0]: {}})
-            elif k in fields:
-                # Only strict checking should be performed
-                if type(v) != fields[k].type_:
-                    raise DocumentUpdateError(
-                        f"unmatched given type {type(v)} to document type"
-                        f" {fields[k].type_}"
-                    )
-            else:
-                raise DocumentUpdateError(
-                    f"key {k} is not present in document fields"
-                )
```

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/errors.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/helpers.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/test_converttoobjectid.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/test_converttoobjectid.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/test_get.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/test_get.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/test_updateoperators.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/test_updateoperators.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/document/testing.py` & `orwynn-1.0.0rc1/orwynn/mongo/document/testing.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/errors.py` & `orwynn-1.0.0rc1/orwynn/mongo/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/mongo.py` & `orwynn-1.0.0rc1/orwynn/mongo/mongo.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/mongo/test_main.py` & `orwynn-1.0.0rc1/orwynn/mongo/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/proxy/boot.py` & `orwynn-1.0.0rc1/orwynn/proxy/boot.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/router/errorhandlermanager.py` & `orwynn-1.0.0rc1/orwynn/router/errorhandlermanager.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/router/register/controller.py` & `orwynn-1.0.0rc1/orwynn/router/register/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/router/register/middleware.py` & `orwynn-1.0.0rc1/orwynn/router/register/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/router/router.py` & `orwynn-1.0.0rc1/orwynn/router/router.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/router/test_globalroute.py` & `orwynn-1.0.0rc1/orwynn/router/test_globalroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/singleton/singleton.py` & `orwynn-1.0.0rc1/orwynn/singleton/singleton.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/sql/config.py` & `orwynn-1.0.0rc1/orwynn/sql/config.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/sql/sql.py` & `orwynn-1.0.0rc1/orwynn/sql/sql.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/sql/table.py` & `orwynn-1.0.0rc1/orwynn/sql/table.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/sql/test_main.py` & `orwynn-1.0.0rc1/orwynn/sql/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/testing/__init__.py` & `orwynn-1.0.0rc1/orwynn/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/testing/client.py` & `orwynn-1.0.0rc1/orwynn/testing/client.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/testing/test_main.py` & `orwynn-1.0.0rc1/orwynn/testing/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/testingtools/__init__.py` & `orwynn-1.0.0rc1/orwynn/testingtools/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/crypto/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/fmt/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/fmt/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/fmt/test_main.py` & `orwynn-1.0.0rc1/orwynn/utils/fmt/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/klass/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/klass/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/klass/test_klass.py` & `orwynn-1.0.0rc1/orwynn/utils/klass/test_klass.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/mp/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/mp/location.py` & `orwynn-1.0.0rc1/orwynn/utils/mp/location.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/mp/test_main.py` & `orwynn-1.0.0rc1/orwynn/utils/mp/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/url/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/url/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/url/helpers.py` & `orwynn-1.0.0rc1/orwynn/utils/url/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/url/test_utils.py` & `orwynn-1.0.0rc1/orwynn/utils/url/test_utils.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/validation/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/validation/errors.py` & `orwynn-1.0.0rc1/orwynn/utils/validation/errors.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/utils/yml/__init__.py` & `orwynn-1.0.0rc1/orwynn/utils/yml/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/__init__.py` & `orwynn-1.0.0rc1/orwynn/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/constants.py` & `orwynn-1.0.0rc1/orwynn/websocket/constants.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/context/id.py` & `orwynn-1.0.0rc1/orwynn/websocket/context/id.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/context/middleware/builtin.py` & `orwynn-1.0.0rc1/orwynn/websocket/context/middleware/builtin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/context/middleware/contextbuiltin.py` & `orwynn-1.0.0rc1/orwynn/websocket/context/middleware/contextbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/context/test_main.py` & `orwynn-1.0.0rc1/orwynn/websocket/context/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/controller/controller.py` & `orwynn-1.0.0rc1/orwynn/websocket/controller/controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/controller/test_controller.py` & `orwynn-1.0.0rc1/orwynn/websocket/controller/test_controller.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/controller/test_globalroute.py` & `orwynn-1.0.0rc1/orwynn/websocket/controller/test_globalroute.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/errorhandler/middleware.py` & `orwynn-1.0.0rc1/orwynn/websocket/errorhandler/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/errorhandler/test_default.py` & `orwynn-1.0.0rc1/orwynn/websocket/errorhandler/test_default.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/log/logger.py` & `orwynn-1.0.0rc1/orwynn/websocket/log/logger.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/log/middleware.py` & `orwynn-1.0.0rc1/orwynn/websocket/log/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/middleware/connectionbuiltin.py` & `orwynn-1.0.0rc1/orwynn/websocket/middleware/connectionbuiltin.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/middleware/middleware.py` & `orwynn-1.0.0rc1/orwynn/websocket/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/middleware/test_main.py` & `orwynn-1.0.0rc1/orwynn/websocket/middleware/test_main.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/routing/helpers.py` & `orwynn-1.0.0rc1/orwynn/websocket/routing/helpers.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/routing/nextcall.py` & `orwynn-1.0.0rc1/orwynn/websocket/routing/nextcall.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/orwynn/websocket/routing/stack.py` & `orwynn-1.0.0rc1/orwynn/websocket/routing/stack.py`

 * *Files identical despite different names*

### Comparing `orwynn-1.0.0b7/pyproject.toml` & `orwynn-1.0.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orwynn"
-version = "1.0.0b7"
+version = "1.0.0rc1"
 description = "Scalable web-framework with out-of-the-box architecture"
 authors = ["ryzhovalex <thed4rkof@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 fastapi = "^0.88.0"
@@ -26,11 +26,14 @@
 [tool.poetry.group.dev.dependencies]
 lorem = "^0.1.1"
 ruff = "^0.0.215"
 git-changelog = "^1.0.0"
 coverage = "^6.5.0"
 pytest = "^7.2.0"
 pytest-asyncio = "^0.20.3"
+mkdocs = "^1.4.3"
+mkdocstrings = {extras = ["python"], version = "^0.22.0"}
+mkdocs-material = "^9.1.18"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `orwynn-1.0.0b7/PKG-INFO` & `orwynn-1.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orwynn
-Version: 1.0.0b7
+Version: 1.0.0rc1
 Summary: Scalable web-framework with out-of-the-box architecture
 Author: ryzhovalex
 Author-email: thed4rkof@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bcrypt (>=4.0.1,<5.0.0)
```

