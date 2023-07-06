# Comparing `tmp/zhenglin-0.13.6.tar.gz` & `tmp/zhenglin-0.13.7.tar.gz`

## Comparing `zhenglin-0.13.6.tar` & `zhenglin-0.13.7.tar`

### file list

```diff
@@ -1,147 +1,154 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/__init__.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/loss.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/metrics.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/__init__.py
--rw-r--r--   0        0        0     6391 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/cyclegan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/ddpm.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/discriminator.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/edsr.py
--rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/esrgan.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/noise2void.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/pix2pix.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/rcan.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/restormer.py
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/rrdb.py
--rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/srgan.py
--rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/swinir.py
--rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/u2net.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks/unet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/aae/__init__.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/aae/aae.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/acgan/__init__.py
--rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/acgan/acgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/began/__init__.py
--rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/began/began.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bgan/__init__.py
--rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bgan/bgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/__init__.py
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/datasets.py
--rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/__init__.py
--rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/ccgan.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/datasets.py
--rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cgan/__init__.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cgan/cgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cluster_gan/__init__.py
--rw-r--r--   0        0        0    18207 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cluster_gan/clustergan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cogan/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cogan/cogan.py
--rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cogan/mnistm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/__init__.py
--rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/context_encoder.py
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/datasets.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/__init__.py
--rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/cyclegan.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/network.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dcgan/__init__.py
--rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dcgan/dcgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ddpm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/__init__.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/datasets.py
--rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/discogan.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discriminator/__init__.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/discriminator/discriminator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dragan/__init__.py
--rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dragan/dragan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/__init__.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/datasets.py
--rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/dualgan.py
--rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ebgan/__init__.py
--rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/ebgan/ebgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/edsr/__init__.py
--rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/edsr/edsr.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/edsr/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/esrgan/__init__.py
--rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/esrgan/esrgan.py
--rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/esrgan/network.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/gan/__init__.py
--rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/gan/gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/infogan/__init__.py
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/infogan/infogan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/lsgan/__init__.py
--rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/lsgan/lsgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/__init__.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/datasets.py
--rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/models.py
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/munit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/noise2void/__init__.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/noise2void/network.py
--rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/noise2void/noise2void.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pix2pix/__init__.py
--rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pix2pix/network.py
--rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pix2pix/pix2pix.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pixelda/__init__.py
--rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pixelda/mnistm.py
--rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/pixelda/pixelda.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/rcan/__init__.py
--rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/rcan/network.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/rcan/rcan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/relativistic_gan/__init__.py
--rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/__init__.py
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/model.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/restormer.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/rrdb/__init__.py
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/rrdb/rrdb.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/sgan/__init__.py
--rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/sgan/sgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/softmax_gan/__init__.py
--rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/srgan/__init__.py
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/srgan/network.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/srgan/srgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/__init__ copy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/datasets.py
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/models.py
--rw-r--r--   0        0        0    11147 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/stargan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/__init__.py
--rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/network.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/swinir.py
--rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/u2net/__init__.py
--rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/u2net/u2net.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unet/__init__.py
--rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unet/unet.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/__init__.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/datasets.py
--rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/models.py
--rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/unit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan/__init__.py
--rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan/wgan.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_div/__init__.py
--rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_div/wgan_div.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_gp/__init__.py
--rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/__init__.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/dataset.py
--rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/eval.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/network.py
--rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/train.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 zhenglin-0.13.6/src/zhenglin/dl/template/v1/utils.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zhenglin-0.13.6/LICENSE
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 zhenglin-0.13.6/README.md
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 zhenglin-0.13.6/pyproject.toml
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 zhenglin-0.13.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/loss.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/metrics.py
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/__init__.py
+-rw-r--r--   0        0        0     5740 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/cyclegan.py
+-rw-r--r--   0        0        0    14850 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/ddpm.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/discriminator.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/edsr.py
+-rw-r--r--   0        0        0     4948 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/esrgan.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/noise2void.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/pix2pix.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/rcan.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/restormer.py
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/rrdb.py
+-rw-r--r--   0        0        0     3959 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/srgan.py
+-rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/swinir.py
+-rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/u2net.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks/unet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/aae/__init__.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/aae/aae.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/acgan/__init__.py
+-rw-r--r--   0        0        0     8417 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/acgan/acgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/began/__init__.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/began/began.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bgan/__init__.py
+-rw-r--r--   0        0        0     5774 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bgan/bgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/__init__.py
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/datasets.py
+-rw-r--r--   0        0        0     5387 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/__init__.py
+-rw-r--r--   0        0        0     6108 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/ccgan.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/datasets.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cgan/__init__.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cgan/cgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cluster_gan/__init__.py
+-rw-r--r--   0        0        0    18207 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cluster_gan/clustergan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cogan/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cogan/cogan.py
+-rw-r--r--   0        0        0     5022 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cogan/mnistm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/__init__.py
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/context_encoder.py
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/datasets.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/models.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/__init__.py
+-rw-r--r--   0        0        0     8514 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/cyclegan.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/network.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dcgan/__init__.py
+-rw-r--r--   0        0        0     6464 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dcgan/dcgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/__init__.py
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/ddpm.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/ddpm_conditional.py
+-rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/diffusion.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/eval.py
+-rw-r--r--   0        0        0    11474 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/network.py
+-rw-r--r--   0        0        0    16895 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ddpm/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/__init__.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/datasets.py
+-rw-r--r--   0        0        0     8430 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/discogan.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discriminator/__init__.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/discriminator/discriminator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dragan/__init__.py
+-rw-r--r--   0        0        0     7414 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dragan/dragan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/__init__.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/datasets.py
+-rw-r--r--   0        0        0     9093 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/dualgan.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ebgan/__init__.py
+-rw-r--r--   0        0        0     7085 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/ebgan/ebgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/edsr/__init__.py
+-rw-r--r--   0        0        0     4240 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/edsr/edsr.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/edsr/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/esrgan/__init__.py
+-rw-r--r--   0        0        0     9469 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/esrgan/esrgan.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/esrgan/network.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/gan/__init__.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/gan/gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/infogan/__init__.py
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/infogan/infogan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/lsgan/__init__.py
+-rw-r--r--   0        0        0     6415 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/lsgan/lsgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/__init__.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/datasets.py
+-rw-r--r--   0        0        0    10704 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/models.py
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/munit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/noise2void/__init__.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/noise2void/network.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/noise2void/noise2void.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pix2pix/__init__.py
+-rw-r--r--   0        0        0     4301 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pix2pix/network.py
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pix2pix/pix2pix.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pixelda/__init__.py
+-rw-r--r--   0        0        0     5735 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pixelda/mnistm.py
+-rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/pixelda/pixelda.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/rcan/__init__.py
+-rw-r--r--   0        0        0     2384 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/rcan/network.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/rcan/rcan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/relativistic_gan/__init__.py
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/__init__.py
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/model.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/restormer.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/rrdb/__init__.py
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/rrdb/rrdb.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/sgan/__init__.py
+-rw-r--r--   0        0        0     7815 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/sgan/sgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/softmax_gan/__init__.py
+-rw-r--r--   0        0        0     5284 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/srgan/__init__.py
+-rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/srgan/network.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/srgan/srgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/__init__ copy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/datasets.py
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/models.py
+-rw-r--r--   0        0        0    11147 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/stargan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/__init__.py
+-rw-r--r--   0        0        0    37449 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/network.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/swinir.py
+-rw-r--r--   0        0        0     2027 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/u2net/__init__.py
+-rw-r--r--   0        0        0    16069 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/u2net/u2net.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unet/__init__.py
+-rw-r--r--   0        0        0     4121 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unet/unet.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/__init__.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/datasets.py
+-rw-r--r--   0        0        0     4735 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/models.py
+-rw-r--r--   0        0        0    10527 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/unit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan/__init__.py
+-rw-r--r--   0        0        0     5271 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan/wgan.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_div/__init__.py
+-rw-r--r--   0        0        0     6537 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_div/wgan_div.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_gp/__init__.py
+-rw-r--r--   0        0        0     6851 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/__init__.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/dataset.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/eval.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/network.py
+-rw-r--r--   0        0        0     3880 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/train.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 zhenglin-0.13.7/src/zhenglin/dl/template/v1/utils.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zhenglin-0.13.7/LICENSE
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 zhenglin-0.13.7/README.md
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 zhenglin-0.13.7/pyproject.toml
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 zhenglin-0.13.7/PKG-INFO
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/loss.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         super(CharbonnierLoss, self).__init__()
         self.epsilon2=epsilon*epsilon
 
     def forward(self,x):
         value=torch.sqrt(torch.pow(x,2)+self.epsilon2)
         return torch.mean(value)
 
-
 class MeanShift(nn.Conv2d):
     def __init__(
             self, rgb_range,
             rgb_mean=(0.2, 0.2, 0.2), rgb_std=(1, 1, 1), sign=-1):
         super(MeanShift, self).__init__(3, 3, kernel_size=1)
         std = torch.Tensor(rgb_std)
         self.weight.data = torch.eye(3).view(3, 3, 1, 1) / std.view(3, 1, 1, 1)
@@ -24,24 +23,24 @@
         for p in self.parameters():
             p.requires_grad = False
 
 
 class PerceptualLoss_l1(nn.Module):
     def __init__(self, rgb_range=1, device=0):
         super(PerceptualLoss_l1, self).__init__()
-        self.device = device
-        model = models.vgg19(weights='IMAGENET1K_V1').to(self.device)
+        model = models.vgg19(weights='IMAGENET1K_V1').to(device)
         vgg_features = model.features
         modules = [m for m in vgg_features]
 
         self.vgg = nn.Sequential(*modules[:35])
         self.vgg.eval()
         vgg_mean = (0.2, 0.2, 0.2)
         vgg_std = (0.157 * rgb_range, 0.157 * rgb_range, 0.157 * rgb_range)
         self.sub_mean = MeanShift(rgb_range, vgg_mean, vgg_std)
+        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.to(self.device)
 
         for p in self.parameters():
             p.requires_grad = False
 
     def forward(self, hr, sr):
         sr = torch.cat([sr, sr, sr], axis=1).to(self.device)
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/metrics.py` & `zhenglin-0.13.7/src/zhenglin/dl/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import torch
 import torch.nn as nn
 import numpy as np
-from utils.img_utils import denorm_min_max, norm_mean,denorm_mean, norm_min_max, gamma_correction
 from skimage.metrics import structural_similarity
 from skimage.transform import resize
 from torchmetrics.image.lpip import LearnedPerceptualImagePatchSimilarity
 from torchmetrics.image.fid import FrechetInceptionDistance
 from collections import OrderedDict
+from .utils import norm_min_max
 
 def SNR(original:np.ndarray, generated):
     snr = 0
     ch = original.shape[0]
     for c in range(ch):
         noise = original[c] - generated[c]
         snr += 10 * np.log10(np.sum(original**2) / np.sum(noise**2))
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/cyclegan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,146 +1,141 @@
-import random
-
-import torch
 import torch.nn as nn
 import torch.nn.functional as F
+import torch
 from torch.autograd import Variable
+import numpy as np
 
 
-class ReplayBuffer():
-    def __init__(self, pool_size=50):
-        assert (pool_size > 0)
-        self.pool_size = pool_size
-        self.data = []
-
-    def push_and_pop(self, data):
-        to_return = []
-        for element in data.data:   # no grad_fn<>
-            element = torch.unsqueeze(element, 0)   # [N, C, H, W] -> [1, C, H, W]
-            if len(self.data) < self.pool_size:
-                self.data.append(element)
-                to_return.append(element)
-            else:
-                if random.uniform(0,1) > 0.5:
-                    i = random.randint(0, self.pool_size-1)
-                    to_return.append(self.data[i].clone())  # replacement reaction, one sample in batch
-                    self.data[i] = element
-                else:
-                    to_return.append(element)
-        return Variable(torch.cat(to_return))
+def weights_init_normal(m):
+    classname = m.__class__.__name__
+    if classname.find("Conv") != -1:
+        torch.nn.init.normal_(m.weight.data, 0.0, 0.02)
+    elif classname.find("BatchNorm2d") != -1:
+        torch.nn.init.normal_(m.weight.data, 1.0, 0.02)
+        torch.nn.init.constant_(m.bias.data, 0.0)
 
 
 class LambdaLR:
     def __init__(self, n_epochs, offset, decay_start_epoch):
         assert (n_epochs - decay_start_epoch) > 0, "Decay must start before the training session ends!"
         self.n_epochs = n_epochs
         self.offset = offset
         self.decay_start_epoch = decay_start_epoch
 
     def step(self, epoch):
         return 1.0 - max(0, epoch + self.offset - self.decay_start_epoch) / (self.n_epochs - self.decay_start_epoch)
 
 
-
-def weights_init_normal(m):
-    classname = m.__class__.__name__
-    if classname.find("Conv") != -1:
-        torch.nn.init.normal_(m.weight.data, 0.0, 0.02)
-        if hasattr(m, "bias") and m.bias is not None:
-            torch.nn.init.constant_(m.bias.data, 0.0)
-    elif classname.find("BatchNorm2d") != -1:
-        torch.nn.init.normal_(m.weight.data, 1.0, 0.02)
-        torch.nn.init.constant_(m.bias.data, 0.0)
-
-
 ##############################
 #           RESNET
 ##############################
 
 
 class ResidualBlock(nn.Module):
-    def __init__(self, in_features):
+    def __init__(self, features):
         super(ResidualBlock, self).__init__()
 
-        self.block = nn.Sequential(
+        conv_block = [
             nn.ReflectionPad2d(1),
-            nn.Conv2d(in_features, in_features, 3),
-            nn.InstanceNorm2d(in_features),
+            nn.Conv2d(features, features, 3),
+            nn.InstanceNorm2d(features),
             nn.ReLU(inplace=True),
             nn.ReflectionPad2d(1),
-            nn.Conv2d(in_features, in_features, 3),
-            nn.InstanceNorm2d(in_features),
-        )
+            nn.Conv2d(features, features, 3),
+            nn.InstanceNorm2d(features),
+        ]
 
-    def forward(self, x):
-        return x + self.block(x)
+        self.conv_block = nn.Sequential(*conv_block)
 
+    def forward(self, x):
+        return x + self.conv_block(x)
 
-class GeneratorResNet(nn.Module):
-    def __init__(self, input_shape, num_residual_blocks):
-        super(GeneratorResNet, self).__init__()
 
-        channels = input_shape[0]
+class Encoder(nn.Module):
+    def __init__(self, in_channels=3, dim=64, n_downsample=2, shared_block=None):
+        super(Encoder, self).__init__()
 
         # Initial convolution block
-        out_features = 64
-        model = [
-            nn.ReflectionPad2d(channels),
-            nn.Conv2d(channels, out_features, 3),
-            nn.InstanceNorm2d(out_features),
-            nn.ReLU(inplace=True),
+        layers = [
+            nn.ReflectionPad2d(3),
+            nn.Conv2d(in_channels, dim, 7),
+            nn.InstanceNorm2d(64),
+            nn.LeakyReLU(0.2, inplace=True),
         ]
-        in_features = out_features
 
         # Downsampling
-        for _ in range(2):
-            out_features *= 2
-            model += [
-                nn.Conv2d(in_features, out_features, 3, stride=2, padding=1),
-                nn.InstanceNorm2d(out_features),
+        for _ in range(n_downsample):
+            layers += [
+                nn.Conv2d(dim, dim * 2, 4, stride=2, padding=1),
+                nn.InstanceNorm2d(dim * 2),
                 nn.ReLU(inplace=True),
             ]
-            in_features = out_features
+            dim *= 2
 
         # Residual blocks
-        for _ in range(num_residual_blocks):
-            model += [ResidualBlock(out_features)]
+        for _ in range(3):
+            layers += [ResidualBlock(dim)]
+
+        self.model_blocks = nn.Sequential(*layers)
+        self.shared_block = shared_block
+
+    def reparameterization(self, mu):
+        Tensor = torch.cuda.FloatTensor if mu.is_cuda else torch.FloatTensor
+        z = Variable(Tensor(np.random.normal(0, 1, mu.shape)))
+        return z + mu
+
+    def forward(self, x):
+        x = self.model_blocks(x)
+        mu = self.shared_block(x)
+        z = self.reparameterization(mu)
+        return mu, z
+
+
+class Generator(nn.Module):
+    def __init__(self, out_channels=3, dim=64, n_upsample=2, shared_block=None):
+        super(Generator, self).__init__()
+
+        self.shared_block = shared_block
+
+        layers = []
+        dim = dim * 2 ** n_upsample
+        # Residual blocks
+        for _ in range(3):
+            layers += [ResidualBlock(dim)]
 
         # Upsampling
-        for _ in range(2):
-            out_features //= 2
-            model += [
-                nn.Upsample(scale_factor=2),
-                nn.Conv2d(in_features, out_features, 3, stride=1, padding=1),
-                nn.InstanceNorm2d(out_features),
-                nn.ReLU(inplace=True),
+        for _ in range(n_upsample):
+            layers += [
+                nn.ConvTranspose2d(dim, dim // 2, 4, stride=2, padding=1),
+                nn.InstanceNorm2d(dim // 2),
+                nn.LeakyReLU(0.2, inplace=True),
             ]
-            in_features = out_features
+            dim = dim // 2
 
         # Output layer
-        model += [nn.ReflectionPad2d(channels), nn.Conv2d(out_features, channels, 3), nn.Tanh()]
+        layers += [nn.ReflectionPad2d(3), nn.Conv2d(dim, out_channels, 7), nn.Tanh()]
 
-        self.model = nn.Sequential(*model)
+        self.model_blocks = nn.Sequential(*layers)
 
     def forward(self, x):
-        return self.model(x)
+        x = self.shared_block(x)
+        x = self.model_blocks(x)
+        return x
 
 
 ##############################
 #        Discriminator
 ##############################
 
 
 class Discriminator(nn.Module):
     def __init__(self, input_shape):
         super(Discriminator, self).__init__()
-
         channels, height, width = input_shape
-
-        # Calculate output shape of image discriminator (PatchGAN)
+        # Calculate output of image discriminator (PatchGAN)
         self.output_shape = (1, height // 2 ** 4, width // 2 ** 4)
 
         def discriminator_block(in_filters, out_filters, normalize=True):
             """Returns downsampling layers of each discriminator block"""
             layers = [nn.Conv2d(in_filters, out_filters, 4, stride=2, padding=1)]
             if normalize:
                 layers.append(nn.InstanceNorm2d(out_filters))
@@ -148,47 +143,12 @@
             return layers
 
         self.model = nn.Sequential(
             *discriminator_block(channels, 64, normalize=False),
             *discriminator_block(64, 128),
             *discriminator_block(128, 256),
             *discriminator_block(256, 512),
-            nn.ZeroPad2d((1, 0, 1, 0)),
-            nn.Conv2d(512, 1, 4, padding=1)
+            nn.Conv2d(512, 1, 3, padding=1)
         )
 
     def forward(self, img):
         return self.model(img)
-
-
-class ReplayBuffer:
-    def __init__(self, max_size=50):
-        assert max_size > 0, "Empty buffer or trying to create a black hole. Be careful."
-        self.max_size = max_size
-        self.data = []
-
-    def push_and_pop(self, data):
-        to_return = []
-        for element in data.data:
-            element = torch.unsqueeze(element, 0)
-            if len(self.data) < self.max_size:
-                self.data.append(element)
-                to_return.append(element)
-            else:
-                if random.uniform(0, 1) > 0.5:
-                    i = random.randint(0, self.max_size - 1)
-                    to_return.append(self.data[i].clone())
-                    self.data[i] = element
-                else:
-                    to_return.append(element)
-        return Variable(torch.cat(to_return))
-
-
-class LambdaLR:
-    def __init__(self, n_epochs, offset, decay_start_epoch):
-        assert (n_epochs - decay_start_epoch) > 0, "Decay must start before the training session ends!"
-        self.n_epochs = n_epochs
-        self.offset = offset
-        self.decay_start_epoch = decay_start_epoch
-
-    def step(self, epoch):
-        return 1.0 - max(0, epoch + self.offset - self.decay_start_epoch) / (self.n_epochs - self.decay_start_epoch)
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/discriminator.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/discriminator.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/edsr.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/edsr.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/esrgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/esrgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/noise2void.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/noise2void.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/pix2pix.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/pix2pix.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/rcan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/rcan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/restormer.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/restormer.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/rrdb.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/rrdb.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/srgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/srgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/swinir.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/swinir.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/u2net.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/u2net.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks/unet.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks/unet.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/aae/aae.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/aae/aae.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/acgan/acgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/acgan/acgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/began/began.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/began/began.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/bgan/bgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/bgan/bgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/bicyclegan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/bicyclegan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/bicyclegan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/ccgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/ccgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/ccgan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/ccgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cgan/cgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cgan/cgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cluster_gan/clustergan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cluster_gan/clustergan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cogan/cogan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cogan/cogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cogan/mnistm.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cogan/mnistm.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/context_encoder.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/context_encoder.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-"""
-Inpainting using Generative Adversarial Networks.
-The dataset can be downloaded from: https://www.dropbox.com/sh/8oqt9vytwxb3s4r/AADIKlz8PR9zr6Y20qbkunrba/Img/img_align_celeba.zip?dl=0
-(if not available there see if options are listed at http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)
-Instrustion on running the script:
-1. Download the dataset from the provided link
-2. Save the folder 'img_align_celeba' to '../../data/'
-4. Run the sript using command 'python3 context_encoder.py'
-"""
-
-import argparse
-import os
-import numpy as np
-import math
-
-import torchvision.transforms as transforms
-from torchvision.utils import save_image
-from PIL import Image
-
-from torch.utils.data import DataLoader
-from torchvision import datasets
-from torch.autograd import Variable
-
-from datasets import *
-from models import *
-
-import torch.nn as nn
-import torch.nn.functional as F
-import torch
-
-os.makedirs("images", exist_ok=True)
-
-parser = argparse.ArgumentParser()
-parser.add_argument("--n_epochs", type=int, default=200, help="number of epochs of training")
-parser.add_argument("--batch_size", type=int, default=8, help="size of the batches")
-parser.add_argument("--dataset_name", type=str, default="img_align_celeba", help="name of the dataset")
-parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
-parser.add_argument("--b1", type=float, default=0.5, help="adam: decay of first order momentum of gradient")
-parser.add_argument("--b2", type=float, default=0.999, help="adam: decay of first order momentum of gradient")
-parser.add_argument("--n_cpu", type=int, default=4, help="number of cpu threads to use during batch generation")
-parser.add_argument("--latent_dim", type=int, default=100, help="dimensionality of the latent space")
-parser.add_argument("--img_size", type=int, default=128, help="size of each image dimension")
-parser.add_argument("--mask_size", type=int, default=64, help="size of random mask")
-parser.add_argument("--channels", type=int, default=3, help="number of image channels")
-parser.add_argument("--sample_interval", type=int, default=500, help="interval between image sampling")
-opt = parser.parse_args()
-print(opt)
-
-cuda = True if torch.cuda.is_available() else False
-
-# Calculate output of image discriminator (PatchGAN)
-patch_h, patch_w = int(opt.mask_size / 2 ** 3), int(opt.mask_size / 2 ** 3)
-patch = (1, patch_h, patch_w)
-
-
-def weights_init_normal(m):
-    classname = m.__class__.__name__
-    if classname.find("Conv") != -1:
-        torch.nn.init.normal_(m.weight.data, 0.0, 0.02)
-    elif classname.find("BatchNorm2d") != -1:
-        torch.nn.init.normal_(m.weight.data, 1.0, 0.02)
-        torch.nn.init.constant_(m.bias.data, 0.0)
-
-
-# Loss function
-adversarial_loss = torch.nn.MSELoss()
-pixelwise_loss = torch.nn.L1Loss()
-
-# Initialize generator and discriminator
-generator = Generator(channels=opt.channels)
-discriminator = Discriminator(channels=opt.channels)
-
-if cuda:
-    generator.cuda()
-    discriminator.cuda()
-    adversarial_loss.cuda()
-    pixelwise_loss.cuda()
-
-# Initialize weights
-generator.apply(weights_init_normal)
-discriminator.apply(weights_init_normal)
-
-# Dataset loader
-transforms_ = [
-    transforms.Resize((opt.img_size, opt.img_size), Image.BICUBIC),
-    transforms.ToTensor(),
-    transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
-]
-dataloader = DataLoader(
-    ImageDataset("../../data/%s" % opt.dataset_name, transforms_=transforms_),
-    batch_size=opt.batch_size,
-    shuffle=True,
-    num_workers=opt.n_cpu,
-)
-test_dataloader = DataLoader(
-    ImageDataset("../../data/%s" % opt.dataset_name, transforms_=transforms_, mode="val"),
-    batch_size=12,
-    shuffle=True,
-    num_workers=1,
-)
-
-# Optimizers
-optimizer_G = torch.optim.Adam(generator.parameters(), lr=opt.lr, betas=(opt.b1, opt.b2))
-optimizer_D = torch.optim.Adam(discriminator.parameters(), lr=opt.lr, betas=(opt.b1, opt.b2))
-
-Tensor = torch.cuda.FloatTensor if cuda else torch.FloatTensor
-
-
-def save_sample(batches_done):
-    samples, masked_samples, i = next(iter(test_dataloader))
-    samples = Variable(samples.type(Tensor))
-    masked_samples = Variable(masked_samples.type(Tensor))
-    i = i[0].item()  # Upper-left coordinate of mask
-    # Generate inpainted image
-    gen_mask = generator(masked_samples)
-    filled_samples = masked_samples.clone()
-    filled_samples[:, :, i : i + opt.mask_size, i : i + opt.mask_size] = gen_mask
-    # Save sample
-    sample = torch.cat((masked_samples.data, filled_samples.data, samples.data), -2)
-    save_image(sample, "images/%d.png" % batches_done, nrow=6, normalize=True)
-
-
-# ----------
-#  Training
-# ----------
-
-for epoch in range(opt.n_epochs):
-    for i, (imgs, masked_imgs, masked_parts) in enumerate(dataloader):
-
-        # Adversarial ground truths
-        valid = Variable(Tensor(imgs.shape[0], *patch).fill_(1.0), requires_grad=False)
-        fake = Variable(Tensor(imgs.shape[0], *patch).fill_(0.0), requires_grad=False)
-
-        # Configure input
-        imgs = Variable(imgs.type(Tensor))
-        masked_imgs = Variable(masked_imgs.type(Tensor))
-        masked_parts = Variable(masked_parts.type(Tensor))
-
-        # -----------------
-        #  Train Generator
-        # -----------------
-
-        optimizer_G.zero_grad()
-
-        # Generate a batch of images
-        gen_parts = generator(masked_imgs)
-
-        # Adversarial and pixelwise loss
-        g_adv = adversarial_loss(discriminator(gen_parts), valid)
-        g_pixel = pixelwise_loss(gen_parts, masked_parts)
-        # Total loss
-        g_loss = 0.001 * g_adv + 0.999 * g_pixel
-
-        g_loss.backward()
-        optimizer_G.step()
-
-        # ---------------------
-        #  Train Discriminator
-        # ---------------------
-
-        optimizer_D.zero_grad()
-
-        # Measure discriminator's ability to classify real from generated samples
-        real_loss = adversarial_loss(discriminator(masked_parts), valid)
-        fake_loss = adversarial_loss(discriminator(gen_parts.detach()), fake)
-        d_loss = 0.5 * (real_loss + fake_loss)
-
-        d_loss.backward()
-        optimizer_D.step()
-
-        print(
-            "[Epoch %d/%d] [Batch %d/%d] [D loss: %f] [G adv: %f, pixel: %f]"
-            % (epoch, opt.n_epochs, i, len(dataloader), d_loss.item(), g_adv.item(), g_pixel.item())
-        )
-
-        # Generate sample at sample interval
-        batches_done = epoch * len(dataloader) + i
-        if batches_done % opt.sample_interval == 0:
-            save_sample(batches_done)
+"""
+Inpainting using Generative Adversarial Networks.
+The dataset can be downloaded from: https://www.dropbox.com/sh/8oqt9vytwxb3s4r/AADIKlz8PR9zr6Y20qbkunrba/Img/img_align_celeba.zip?dl=0
+(if not available there see if options are listed at http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html)
+Instrustion on running the script:
+1. Download the dataset from the provided link
+2. Save the folder 'img_align_celeba' to '../../data/'
+4. Run the sript using command 'python3 context_encoder.py'
+"""
+
+import argparse
+import os
+import numpy as np
+import math
+
+import torchvision.transforms as transforms
+from torchvision.utils import save_image
+from PIL import Image
+
+from torch.utils.data import DataLoader
+from torchvision import datasets
+from torch.autograd import Variable
+
+from datasets import *
+from models import *
+
+import torch.nn as nn
+import torch.nn.functional as F
+import torch
+
+os.makedirs("images", exist_ok=True)
+
+parser = argparse.ArgumentParser()
+parser.add_argument("--n_epochs", type=int, default=200, help="number of epochs of training")
+parser.add_argument("--batch_size", type=int, default=8, help="size of the batches")
+parser.add_argument("--dataset_name", type=str, default="img_align_celeba", help="name of the dataset")
+parser.add_argument("--lr", type=float, default=0.0002, help="adam: learning rate")
+parser.add_argument("--b1", type=float, default=0.5, help="adam: decay of first order momentum of gradient")
+parser.add_argument("--b2", type=float, default=0.999, help="adam: decay of first order momentum of gradient")
+parser.add_argument("--n_cpu", type=int, default=4, help="number of cpu threads to use during batch generation")
+parser.add_argument("--latent_dim", type=int, default=100, help="dimensionality of the latent space")
+parser.add_argument("--img_size", type=int, default=128, help="size of each image dimension")
+parser.add_argument("--mask_size", type=int, default=64, help="size of random mask")
+parser.add_argument("--channels", type=int, default=3, help="number of image channels")
+parser.add_argument("--sample_interval", type=int, default=500, help="interval between image sampling")
+opt = parser.parse_args()
+print(opt)
+
+cuda = True if torch.cuda.is_available() else False
+
+# Calculate output of image discriminator (PatchGAN)
+patch_h, patch_w = int(opt.mask_size / 2 ** 3), int(opt.mask_size / 2 ** 3)
+patch = (1, patch_h, patch_w)
+
+
+def weights_init_normal(m):
+    classname = m.__class__.__name__
+    if classname.find("Conv") != -1:
+        torch.nn.init.normal_(m.weight.data, 0.0, 0.02)
+    elif classname.find("BatchNorm2d") != -1:
+        torch.nn.init.normal_(m.weight.data, 1.0, 0.02)
+        torch.nn.init.constant_(m.bias.data, 0.0)
+
+
+# Loss function
+adversarial_loss = torch.nn.MSELoss()
+pixelwise_loss = torch.nn.L1Loss()
+
+# Initialize generator and discriminator
+generator = Generator(channels=opt.channels)
+discriminator = Discriminator(channels=opt.channels)
+
+if cuda:
+    generator.cuda()
+    discriminator.cuda()
+    adversarial_loss.cuda()
+    pixelwise_loss.cuda()
+
+# Initialize weights
+generator.apply(weights_init_normal)
+discriminator.apply(weights_init_normal)
+
+# Dataset loader
+transforms_ = [
+    transforms.Resize((opt.img_size, opt.img_size), Image.BICUBIC),
+    transforms.ToTensor(),
+    transforms.Normalize((0.5, 0.5, 0.5), (0.5, 0.5, 0.5)),
+]
+dataloader = DataLoader(
+    ImageDataset("../../data/%s" % opt.dataset_name, transforms_=transforms_),
+    batch_size=opt.batch_size,
+    shuffle=True,
+    num_workers=opt.n_cpu,
+)
+test_dataloader = DataLoader(
+    ImageDataset("../../data/%s" % opt.dataset_name, transforms_=transforms_, mode="val"),
+    batch_size=12,
+    shuffle=True,
+    num_workers=1,
+)
+
+# Optimizers
+optimizer_G = torch.optim.Adam(generator.parameters(), lr=opt.lr, betas=(opt.b1, opt.b2))
+optimizer_D = torch.optim.Adam(discriminator.parameters(), lr=opt.lr, betas=(opt.b1, opt.b2))
+
+Tensor = torch.cuda.FloatTensor if cuda else torch.FloatTensor
+
+
+def save_sample(batches_done):
+    samples, masked_samples, i = next(iter(test_dataloader))
+    samples = Variable(samples.type(Tensor))
+    masked_samples = Variable(masked_samples.type(Tensor))
+    i = i[0].item()  # Upper-left coordinate of mask
+    # Generate inpainted image
+    gen_mask = generator(masked_samples)
+    filled_samples = masked_samples.clone()
+    filled_samples[:, :, i : i + opt.mask_size, i : i + opt.mask_size] = gen_mask
+    # Save sample
+    sample = torch.cat((masked_samples.data, filled_samples.data, samples.data), -2)
+    save_image(sample, "images/%d.png" % batches_done, nrow=6, normalize=True)
+
+
+# ----------
+#  Training
+# ----------
+
+for epoch in range(opt.n_epochs):
+    for i, (imgs, masked_imgs, masked_parts) in enumerate(dataloader):
+
+        # Adversarial ground truths
+        valid = Variable(Tensor(imgs.shape[0], *patch).fill_(1.0), requires_grad=False)
+        fake = Variable(Tensor(imgs.shape[0], *patch).fill_(0.0), requires_grad=False)
+
+        # Configure input
+        imgs = Variable(imgs.type(Tensor))
+        masked_imgs = Variable(masked_imgs.type(Tensor))
+        masked_parts = Variable(masked_parts.type(Tensor))
+
+        # -----------------
+        #  Train Generator
+        # -----------------
+
+        optimizer_G.zero_grad()
+
+        # Generate a batch of images
+        gen_parts = generator(masked_imgs)
+
+        # Adversarial and pixelwise loss
+        g_adv = adversarial_loss(discriminator(gen_parts), valid)
+        g_pixel = pixelwise_loss(gen_parts, masked_parts)
+        # Total loss
+        g_loss = 0.001 * g_adv + 0.999 * g_pixel
+
+        g_loss.backward()
+        optimizer_G.step()
+
+        # ---------------------
+        #  Train Discriminator
+        # ---------------------
+
+        optimizer_D.zero_grad()
+
+        # Measure discriminator's ability to classify real from generated samples
+        real_loss = adversarial_loss(discriminator(masked_parts), valid)
+        fake_loss = adversarial_loss(discriminator(gen_parts.detach()), fake)
+        d_loss = 0.5 * (real_loss + fake_loss)
+
+        d_loss.backward()
+        optimizer_D.step()
+
+        print(
+            "[Epoch %d/%d] [Batch %d/%d] [D loss: %f] [G adv: %f, pixel: %f]"
+            % (epoch, opt.n_epochs, i, len(dataloader), d_loss.item(), g_adv.item(), g_pixel.item())
+        )
+
+        # Generate sample at sample interval
+        batches_done = epoch * len(dataloader) + i
+        if batches_done % opt.sample_interval == 0:
+            save_sample(batches_done)
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/context_encoder/models.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/context_encoder/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/cyclegan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/cyclegan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/cyclegan/utils.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/cyclegan/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/dcgan/dcgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/dcgan/dcgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/discogan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/discogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/discogan/models.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/discogan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/discriminator/discriminator.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/discriminator/discriminator.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/dragan/dragan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/dragan/dragan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/dualgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/dualgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/dualgan/models.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/dualgan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/ebgan/ebgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/ebgan/ebgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/edsr/edsr.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/edsr/edsr.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/edsr/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/edsr/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/esrgan/esrgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/esrgan/esrgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/esrgan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/esrgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/gan/gan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/gan/gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/infogan/infogan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/infogan/infogan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/lsgan/lsgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/lsgan/lsgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/models.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/munit/munit.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/munit/munit.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/noise2void/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/noise2void/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/noise2void/noise2void.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/noise2void/noise2void.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/pix2pix/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/pix2pix/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/pix2pix/pix2pix.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/pix2pix/pix2pix.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/pixelda/mnistm.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/pixelda/mnistm.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/pixelda/pixelda.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/pixelda/pixelda.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/rcan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/rcan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/rcan/rcan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/rcan/rcan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/relativistic_gan/relativistic_gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/model.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/model.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/restormer.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/restormer.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/restormer/utils.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/restormer/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/rrdb/rrdb.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/rrdb/rrdb.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/sgan/sgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/sgan/sgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/softmax_gan/softmax_gan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/srgan/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/srgan/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/srgan/srgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/srgan/srgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/models.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/models.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/stargan/stargan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/stargan/stargan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/network.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/network.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/swinir.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/swinir/swinir.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/swinir/utils.py` & `zhenglin-0.13.7/src/zhenglin/dl/loss.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,39 +8,41 @@
         super(CharbonnierLoss, self).__init__()
         self.epsilon2=epsilon*epsilon
 
     def forward(self,x):
         value=torch.sqrt(torch.pow(x,2)+self.epsilon2)
         return torch.mean(value)
 
+
 class MeanShift(nn.Conv2d):
     def __init__(
             self, rgb_range,
             rgb_mean=(0.2, 0.2, 0.2), rgb_std=(1, 1, 1), sign=-1):
         super(MeanShift, self).__init__(3, 3, kernel_size=1)
         std = torch.Tensor(rgb_std)
         self.weight.data = torch.eye(3).view(3, 3, 1, 1) / std.view(3, 1, 1, 1)
         self.bias.data = sign * rgb_range * torch.Tensor(rgb_mean) / std
         for p in self.parameters():
             p.requires_grad = False
 
 
-class PerceptualLoss_l1(nn.Module):
-    def __init__(self, rgb_range=1, device=0):
-        super(PerceptualLoss_l1, self).__init__()
-        model = models.vgg19(weights='IMAGENET1K_V1').to(device)
+class PerceptualLoss(nn.Module):
+    def __init__(self, criterion='l1', rgb_range=1, device=torch.device(0)):
+        super(PerceptualLoss, self).__init__()
+        self.device = device
+        self.criterion = criterion
+        model = models.vgg19(weights='IMAGENET1K_V1').to(self.device)
         vgg_features = model.features
         modules = [m for m in vgg_features]
 
         self.vgg = nn.Sequential(*modules[:35])
         self.vgg.eval()
         vgg_mean = (0.2, 0.2, 0.2)
         vgg_std = (0.157 * rgb_range, 0.157 * rgb_range, 0.157 * rgb_range)
         self.sub_mean = MeanShift(rgb_range, vgg_mean, vgg_std)
-        self.device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
         self.to(self.device)
 
         for p in self.parameters():
             p.requires_grad = False
 
     def forward(self, hr, sr):
         sr = torch.cat([sr, sr, sr], axis=1).to(self.device)
@@ -50,10 +52,16 @@
             x = self.sub_mean(x)
             x = self.vgg(x)
             return x
 
         vgg_sr = _forward(sr)
         with torch.no_grad():
             vgg_hr = _forward(hr).detach()
-        loss = F.l1_loss(vgg_sr, vgg_hr)
-        # loss = F.mse_loss(vgg_sr, vgg_hr)
+            
+        if self.criterion.lower() == 'l1':
+            loss = F.l1_loss(vgg_sr, vgg_hr)
+        elif self.criterion.lower() == 'l2' or self.criterion.lower() == 'mse':
+            loss = F.mse_loss(vgg_sr, vgg_hr)
+        else:
+            raise NotImplementedError('Loss type {} is not implemented'.format(self.criterion))
+        
         return loss
```

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/u2net/u2net.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/unet/unet.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/unet/unet.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/datasets.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/datasets.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/unit/unit.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/unit/unit.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan/wgan.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan/wgan.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_div/wgan_div.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_div/wgan_div.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py` & `zhenglin-0.13.7/src/zhenglin/dl/networks_/wgan_gp/wgan_gp.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/template/v1/eval.py` & `zhenglin-0.13.7/src/zhenglin/dl/template/v1/eval.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/template/v1/train.py` & `zhenglin-0.13.7/src/zhenglin/dl/template/v1/train.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/src/zhenglin/dl/template/v1/utils.py` & `zhenglin-0.13.7/src/zhenglin/dl/template/v1/utils.py`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/LICENSE` & `zhenglin-0.13.7/LICENSE`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/README.md` & `zhenglin-0.13.7/README.md`

 * *Files identical despite different names*

### Comparing `zhenglin-0.13.6/pyproject.toml` & `zhenglin-0.13.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zhenglin"
-version = "0.13.6"
+version = "0.13.7"
 # version = "TBD.networks_numbers.modification_numbers"
 authors = [
   { name="Zhenglin", email="aidenhpan@gmail.com" },
 ]
 description = "A deep-learning package contains a set of well-organized deep-neural networks&tools."
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `zhenglin-0.13.6/PKG-INFO` & `zhenglin-0.13.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zhenglin
-Version: 0.13.6
+Version: 0.13.7
 Summary: A deep-learning package contains a set of well-organized deep-neural networks&tools.
 Project-URL: Homepage, https://github.com/ZhenglinPan/zhenglin-package
 Project-URL: Bug Tracker, https://github.com/ZhenglinPan/zhenglin-package/issues
 Author-email: Zhenglin <aidenhpan@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

