# Comparing `tmp/donpapi-1.0.0.tar.gz` & `tmp/donpapi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donpapi-1.0.0.tar", max compression
+gzip compressed data, was "donpapi-1.0.1.tar", max compression
```

## Comparing `donpapi-1.0.0.tar` & `donpapi-1.0.1.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/__init__.py
--rw-r--r--   0        0        0      283 2023-06-27 13:00:10.510761 donpapi-1.0.0/donpapi/config/donpapi_config.json
--rw-r--r--   0        0        0    97440 2023-07-01 14:08:43.974722 donpapi-1.0.0/donpapi/database.py
--rw-r--r--   0        0        0    14936 2023-06-27 12:20:07.502667 donpapi-1.0.0/donpapi/entry.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/__init__.py
--rw-r--r--   0        0        0        2 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/__init__.py
--rw-r--r--   0        0        0     5275 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/blob.py
--rw-r--r--   0        0        0     3706 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/credfile.py
--rw-r--r--   0        0        0     4260 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/credhist.py
--rw-r--r--   0        0        0    15313 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/crypto.py
--rw-r--r--   0        0        0     4466 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/eater.py
--rw-r--r--   0        0        0    18015 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/masterkey.py
--rw-r--r--   0        0        0      957 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/system.py
--rw-r--r--   0        0        0    17204 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/DPAPI/vault.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/__init__.py
--rw-r--r--   0        0        0     6449 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/change_privileges.py
--rw-r--r--   0        0        0     2044 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/constant.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/__init__.py
--rw-r--r--   0        0        0    32239 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/pyDes.py
--rw-r--r--   0        0        0     2087 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/__init__.py
--rw-r--r--   0        0        0    60310 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/aes.py
--rw-r--r--   0        0        0     8123 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py
--rw-r--r--   0        0        0     2060 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/util.py
--rw-r--r--   0        0        0     1545 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/crypto/rc4.py
--rw-r--r--   0        0        0     9631 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/dico.py
--rw-r--r--   0        0        0     6595 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/dpapi_structure.py
--rw-r--r--   0        0        0     3630 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/execute_cmd.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/__init__.py
--rw-r--r--   0        0        0     3463 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/Address.py
--rw-r--r--   0        0        0     1798 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/BaseProcess.py
--rw-r--r--   0        0        0    11069 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/LinProcess.py
--rw-r--r--   0        0        0      427 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/LinStructures.py
--rw-r--r--   0        0        0     3156 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/Locator.py
--rw-r--r--   0        0        0     8318 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/MemWorker.py
--rw-r--r--   0        0        0     5948 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/OSXProcess.py
--rw-r--r--   0        0        0      375 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/Process.py
--rw-r--r--   0        0        0     5069 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/SunProcess.py
--rw-r--r--   0        0        0    11967 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/WinProcess.py
--rw-r--r--   0        0        0     6155 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/WinStructures.py
--rw-r--r--   0        0        0     1081 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/__init__.py
--rw-r--r--   0        0        0      155 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/structures.py
--rw-r--r--   0        0        0     3336 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/utils.py
--rw-r--r--   0        0        0       92 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/version.py
--rw-r--r--   0        0        0     1227 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/wintools.py
--rw-r--r--   0        0        0     6004 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/manage_modules.py
--rw-r--r--   0        0        0     1407 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/module_info.py
--rw-r--r--   0        0        0    10076 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/run.py
--rw-r--r--   0        0        0     2939 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/users.py
--rw-r--r--   0        0        0    20971 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/winstructure.py
--rw-r--r--   0        0        0    14449 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/config/write_output.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/browsers/__init__.py
--rw-r--r--   0        0        0    10511 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/browsers/chromium_based.py
--rw-r--r--   0        0        0     6989 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/browsers/ie.py
--rw-r--r--   0        0        0    23438 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/browsers/mozilla.py
--rw-r--r--   0        0        0      880 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/browsers/ucbrowser.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/chats/__init__.py
--rw-r--r--   0        0        0      917 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/chats/pidgin.py
--rw-r--r--   0        0        0     1993 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/chats/psi.py
--rw-r--r--   0        0        0     5133 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/chats/skype.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/__init__.py
--rw-r--r--   0        0        0     2792 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/dbvis.py
--rw-r--r--   0        0        0     1019 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/postgresql.py
--rw-r--r--   0        0        0     3919 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/robomongo.py
--rw-r--r--   0        0        0     4374 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/sqldeveloper.py
--rw-r--r--   0        0        0      945 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/databases/squirrel.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/games/__init__.py
--rw-r--r--   0        0        0     1828 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/games/galconfusion.py
--rw-r--r--   0        0        0     1336 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/games/kalypsomedia.py
--rw-r--r--   0        0        0     1378 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/games/roguestale.py
--rw-r--r--   0        0        0     1776 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/games/turba.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/git/__init__.py
--rw-r--r--   0        0        0     2263 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/git/gitforwindows.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/mails/__init__.py
--rw-r--r--   0        0        0     3662 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/mails/outlook.py
--rw-r--r--   0        0        0      280 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/mails/thunderbird.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/maven/__init__.py
--rw-r--r--   0        0        0     5712 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/maven/mavenrepositories.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/__init__.py
--rw-r--r--   0        0        0     1171 2023-06-27 12:17:45.106662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/keepass.py
--rw-r--r--   0        0        0   361825 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/keethief.py
--rw-r--r--   0        0        0     2159 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/__init__.py
--rw-r--r--   0        0        0     9068 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/common.py
--rw-r--r--   0        0        0     1638 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/crypto.py
--rw-r--r--   0        0        0     4214 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/hbio.py
--rw-r--r--   0        0        0    15332 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py
--rw-r--r--   0        0        0    13773 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py
--rw-r--r--   0        0        0     6259 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/memory/memorydump.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/multimedia/__init__.py
--rw-r--r--   0        0        0     4144 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/multimedia/eyecon.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/php/__init__.py
--rw-r--r--   0        0        0     2199 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/php/composer.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/svn/__init__.py
--rw-r--r--   0        0        0     2448 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/svn/tortoise.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/__init__.py
--rw-r--r--   0        0        0     2409 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py
--rw-r--r--   0        0        0     1950 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/coreftp.py
--rw-r--r--   0        0        0     2107 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/cyberduck.py
--rw-r--r--   0        0        0    13660 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/d3des.py
--rw-r--r--   0        0        0     2049 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/filezilla.py
--rw-r--r--   0        0        0     1493 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/filezillaserver.py
--rw-r--r--   0        0        0     1640 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py
--rw-r--r--   0        0        0     2454 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/iisapppool.py
--rw-r--r--   0        0        0     5312 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py
--rw-r--r--   0        0        0     5427 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/keepassconfig.py
--rw-r--r--   0        0        0     4016 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py
--rw-r--r--   0        0        0     2109 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/openvpn.py
--rw-r--r--   0        0        0     1628 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/puttycm.py
--rw-r--r--   0        0        0     3610 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/rdpmanager.py
--rw-r--r--   0        0        0     3184 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/unattended.py
--rw-r--r--   0        0        0     6857 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/vnc.py
--rw-r--r--   0        0        0     4078 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/winscp.py
--rw-r--r--   0        0        0     1543 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/wsl.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/wifi/__init__.py
--rw-r--r--   0        0        0     4629 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/wifi/wifi.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/__init__.py
--rw-r--r--   0        0        0     1614 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/autologon.py
--rw-r--r--   0        0        0      699 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/cachedump.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/__init__.py
--rw-r--r--   0        0        0     4434 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/addrspace.py
--rw-r--r--   0        0        0    10218 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/newobj.py
--rw-r--r--   0        0        0     4990 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/object.py
--rw-r--r--   0        0        0     2542 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/types.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/__init__.py
--rw-r--r--   0        0        0     4411 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py
--rw-r--r--   0        0        0    10430 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py
--rw-r--r--   0        0        0     5138 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py
--rw-r--r--   0        0        0     2297 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py
--rw-r--r--   0        0        0      899 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/credfiles.py
--rw-r--r--   0        0        0     1455 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/credman.py
--rw-r--r--   0        0        0      528 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/hashdump.py
--rw-r--r--   0        0        0     1227 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/lsa_secrets.py
--rw-r--r--   0        0        0     2717 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/ppypykatz.py
--rw-r--r--   0        0        0     2942 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/vault.py
--rw-r--r--   0        0        0      920 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/vaultfiles.py
--rw-r--r--   0        0        0     3275 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lazagne/softwares/windows/windows.py
--rw-r--r--   0        0        0     4974 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/RecentFiles.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/__init__.py
--rw-r--r--   0        0        0    16870 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/adconnect.py
--rw-r--r--   0        0        0    42137 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/certificates.py
--rw-r--r--   0        0        0     4605 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/compliance_security.py
--rw-r--r--   0        0        0     2141 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/defines.py
--rw-r--r--   0        0        0    30141 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/dpapi.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/dpapi_pick/__init__.py
--rw-r--r--   0        0        0    11994 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/dpapi_pick/credhist.py
--rw-r--r--   0        0        0    14585 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/dpapi_pick/crypto.py
--rw-r--r--   0        0        0     4466 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/dpapi_pick/eater.py
--rw-r--r--   0        0        0     4466 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/eater.py
--rw-r--r--   0        0        0    10656 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/fileops.py
--rw-r--r--   0        0        0     3938 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/neo4jconnection.py
--rw-r--r--   0        0        0     3006 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/new_module.py
--rw-r--r--   0        0        0    19699 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/reg.py
--rw-r--r--   0        0        0   116877 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/secretsdump.py
--rw-r--r--   0        0        0     3542 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/toolbox.py
--rw-r--r--   0        0        0     3484 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/lib/wmi.py
--rw-r--r--   0        0        0   103749 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/myseatbelt.py
--rw-r--r--   0        0        0     5699 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/myusers.py
--rw-r--r--   0        0        0    52548 2023-06-27 13:00:16.858761 donpapi-1.0.0/donpapi/res/Logo_LOGIN.PNG
--rw-r--r--   0        0        0     3429 2023-06-27 13:00:02.574761 donpapi-1.0.0/donpapi/res/style.css
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/browser/__init__.py
--rw-r--r--   0        0        0    10104 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/browser/chrome_decrypt.py
--rw-r--r--   0        0        0     7015 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/browser/firefox_decrypt.py
--rw-r--r--   0        0        0    17891 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/browser/mozilla.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/manager/__init__.py
--rw-r--r--   0        0        0    23725 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/manager/keepass.py
--rw-r--r--   0        0        0     4486 2023-06-27 12:17:45.110662 donpapi-1.0.0/donpapi/software/manager/lastpass.py
--rw-r--r--   0        0        0     5902 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/manager/mRemoteNG-local.py
--rw-r--r--   0        0        0    12420 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/manager/mRemoteNG.py
--rw-r--r--   0        0        0        0 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/__init__.py
--rw-r--r--   0        0        0    13660 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/d3des.py
--rw-r--r--   0        0        0     6545 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/mobaxterm.py
--rw-r--r--   0        0        0     2186 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/putty.py
--rw-r--r--   0        0        0      210 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/teamviewer.py
--rw-r--r--   0        0        0     2653 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/vnc-local.py
--rw-r--r--   0        0        0     9808 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/vnc.py
--rw-r--r--   0        0        0     6545 2023-06-27 12:17:45.114662 donpapi-1.0.0/donpapi/software/sysadmin/winscp.py
--rw-r--r--   0        0        0     1015 2023-06-27 12:17:45.114662 donpapi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    11514 2023-07-01 14:52:31.862553 donpapi-1.0.0/readme.md
--rw-r--r--   0        0        0    12455 1970-01-01 00:00:00.000000 donpapi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/__init__.py
+-rw-r--r--   0        0        0      283 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/config/donpapi_config.json
+-rw-r--r--   0        0        0   100868 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/database.py
+-rw-r--r--   0        0        0    14936 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/entry.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/__init__.py
+-rw-r--r--   0        0        0        2 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/__init__.py
+-rw-r--r--   0        0        0     5275 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/blob.py
+-rw-r--r--   0        0        0     3706 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credfile.py
+-rw-r--r--   0        0        0     4260 2023-07-06 08:25:26.651395 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credhist.py
+-rw-r--r--   0        0        0    15313 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/crypto.py
+-rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/eater.py
+-rw-r--r--   0        0        0    18015 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/masterkey.py
+-rw-r--r--   0        0        0      957 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/system.py
+-rw-r--r--   0        0        0    17204 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/DPAPI/vault.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/__init__.py
+-rw-r--r--   0        0        0     6449 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/change_privileges.py
+-rw-r--r--   0        0        0     2044 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/constant.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/__init__.py
+-rw-r--r--   0        0        0    32239 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyDes.py
+-rw-r--r--   0        0        0     2087 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/__init__.py
+-rw-r--r--   0        0        0    60310 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/aes.py
+-rw-r--r--   0        0        0     8123 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py
+-rw-r--r--   0        0        0     2060 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/util.py
+-rw-r--r--   0        0        0     1545 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/crypto/rc4.py
+-rw-r--r--   0        0        0     9631 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/dico.py
+-rw-r--r--   0        0        0     6595 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/dpapi_structure.py
+-rw-r--r--   0        0        0     3630 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/execute_cmd.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/__init__.py
+-rw-r--r--   0        0        0     3463 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Address.py
+-rw-r--r--   0        0        0     1798 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/BaseProcess.py
+-rw-r--r--   0        0        0    11069 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinProcess.py
+-rw-r--r--   0        0        0      427 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinStructures.py
+-rw-r--r--   0        0        0     3156 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Locator.py
+-rw-r--r--   0        0        0     8318 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/MemWorker.py
+-rw-r--r--   0        0        0     5948 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/OSXProcess.py
+-rw-r--r--   0        0        0      375 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Process.py
+-rw-r--r--   0        0        0     5069 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/SunProcess.py
+-rw-r--r--   0        0        0    11967 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinProcess.py
+-rw-r--r--   0        0        0     6155 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinStructures.py
+-rw-r--r--   0        0        0     1081 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/__init__.py
+-rw-r--r--   0        0        0      155 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/structures.py
+-rw-r--r--   0        0        0     3336 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/utils.py
+-rw-r--r--   0        0        0       92 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/version.py
+-rw-r--r--   0        0        0     1227 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/wintools.py
+-rw-r--r--   0        0        0     6004 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/manage_modules.py
+-rw-r--r--   0        0        0     1407 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/module_info.py
+-rw-r--r--   0        0        0    10076 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/run.py
+-rw-r--r--   0        0        0     2939 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/users.py
+-rw-r--r--   0        0        0    20971 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/winstructure.py
+-rw-r--r--   0        0        0    14449 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/config/write_output.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/__init__.py
+-rw-r--r--   0        0        0    10511 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/chromium_based.py
+-rw-r--r--   0        0        0     6989 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ie.py
+-rw-r--r--   0        0        0    23438 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/mozilla.py
+-rw-r--r--   0        0        0      880 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ucbrowser.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/pidgin.py
+-rw-r--r--   0        0        0     1993 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/psi.py
+-rw-r--r--   0        0        0     5133 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/chats/skype.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/__init__.py
+-rw-r--r--   0        0        0     2792 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/dbvis.py
+-rw-r--r--   0        0        0     1019 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/postgresql.py
+-rw-r--r--   0        0        0     3919 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/robomongo.py
+-rw-r--r--   0        0        0     4374 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/sqldeveloper.py
+-rw-r--r--   0        0        0      945 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/databases/squirrel.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/__init__.py
+-rw-r--r--   0        0        0     1828 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/galconfusion.py
+-rw-r--r--   0        0        0     1336 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/kalypsomedia.py
+-rw-r--r--   0        0        0     1378 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/roguestale.py
+-rw-r--r--   0        0        0     1776 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/games/turba.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/git/__init__.py
+-rw-r--r--   0        0        0     2263 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/git/gitforwindows.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/__init__.py
+-rw-r--r--   0        0        0     3662 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/outlook.py
+-rw-r--r--   0        0        0      280 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/mails/thunderbird.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/maven/__init__.py
+-rw-r--r--   0        0        0     5712 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/maven/mavenrepositories.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/keepass.py
+-rw-r--r--   0        0        0   361825 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/keethief.py
+-rw-r--r--   0        0        0     2159 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/__init__.py
+-rw-r--r--   0        0        0     9068 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/common.py
+-rw-r--r--   0        0        0     1638 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/crypto.py
+-rw-r--r--   0        0        0     4214 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/hbio.py
+-rw-r--r--   0        0        0    15332 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py
+-rw-r--r--   0        0        0    13773 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py
+-rw-r--r--   0        0        0     6259 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/memory/memorydump.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/__init__.py
+-rw-r--r--   0        0        0     4144 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/eyecon.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/php/__init__.py
+-rw-r--r--   0        0        0     2199 2023-07-06 08:25:26.655396 donpapi-1.0.1/donpapi/lazagne/softwares/php/composer.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/svn/__init__.py
+-rw-r--r--   0        0        0     2448 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/svn/tortoise.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/__init__.py
+-rw-r--r--   0        0        0     2409 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py
+-rw-r--r--   0        0        0     1950 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/coreftp.py
+-rw-r--r--   0        0        0     2107 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/cyberduck.py
+-rw-r--r--   0        0        0    13660 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/d3des.py
+-rw-r--r--   0        0        0     2049 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezilla.py
+-rw-r--r--   0        0        0     1493 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezillaserver.py
+-rw-r--r--   0        0        0     1640 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py
+-rw-r--r--   0        0        0     2454 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iisapppool.py
+-rw-r--r--   0        0        0     5312 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py
+-rw-r--r--   0        0        0     5427 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/keepassconfig.py
+-rw-r--r--   0        0        0     4016 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py
+-rw-r--r--   0        0        0     2109 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/openvpn.py
+-rw-r--r--   0        0        0     1628 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/puttycm.py
+-rw-r--r--   0        0        0     3610 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/rdpmanager.py
+-rw-r--r--   0        0        0     3184 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/unattended.py
+-rw-r--r--   0        0        0     6857 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/vnc.py
+-rw-r--r--   0        0        0     4078 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/winscp.py
+-rw-r--r--   0        0        0     1543 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/wsl.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/wifi/__init__.py
+-rw-r--r--   0        0        0     4629 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/wifi/wifi.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/__init__.py
+-rw-r--r--   0        0        0     1614 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/autologon.py
+-rw-r--r--   0        0        0      699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/cachedump.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/__init__.py
+-rw-r--r--   0        0        0     4434 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/addrspace.py
+-rw-r--r--   0        0        0    10218 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/newobj.py
+-rw-r--r--   0        0        0     4990 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/object.py
+-rw-r--r--   0        0        0     2542 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/types.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/__init__.py
+-rw-r--r--   0        0        0     4411 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py
+-rw-r--r--   0        0        0    10430 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py
+-rw-r--r--   0        0        0     5138 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py
+-rw-r--r--   0        0        0     2297 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py
+-rw-r--r--   0        0        0      899 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/credfiles.py
+-rw-r--r--   0        0        0     1455 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/credman.py
+-rw-r--r--   0        0        0      528 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/hashdump.py
+-rw-r--r--   0        0        0     1227 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/lsa_secrets.py
+-rw-r--r--   0        0        0     2717 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/ppypykatz.py
+-rw-r--r--   0        0        0     2942 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/vault.py
+-rw-r--r--   0        0        0      920 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/vaultfiles.py
+-rw-r--r--   0        0        0     3275 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lazagne/softwares/windows/windows.py
+-rw-r--r--   0        0        0     4974 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/RecentFiles.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/__init__.py
+-rw-r--r--   0        0        0    16870 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/adconnect.py
+-rw-r--r--   0        0        0    42137 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/certificates.py
+-rw-r--r--   0        0        0     4605 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/compliance_security.py
+-rw-r--r--   0        0        0     2141 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/defines.py
+-rw-r--r--   0        0        0    30179 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/__init__.py
+-rw-r--r--   0        0        0    11994 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/credhist.py
+-rw-r--r--   0        0        0    14585 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/crypto.py
+-rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/dpapi_pick/eater.py
+-rw-r--r--   0        0        0     4466 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/eater.py
+-rw-r--r--   0        0        0    10656 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/fileops.py
+-rw-r--r--   0        0        0     3938 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/neo4jconnection.py
+-rw-r--r--   0        0        0     3006 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/new_module.py
+-rw-r--r--   0        0        0    19699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/reg.py
+-rw-r--r--   0        0        0   116877 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/secretsdump.py
+-rw-r--r--   0        0        0     3542 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/toolbox.py
+-rw-r--r--   0        0        0     3484 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/lib/wmi.py
+-rw-r--r--   0        0        0   103749 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/myseatbelt.py
+-rw-r--r--   0        0        0     5699 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/myusers.py
+-rw-r--r--   0        0        0    52548 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/res/Logo_LOGIN.PNG
+-rw-r--r--   0        0        0     3429 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/res/style.css
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/__init__.py
+-rw-r--r--   0        0        0    10104 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/chrome_decrypt.py
+-rw-r--r--   0        0        0     7015 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/firefox_decrypt.py
+-rw-r--r--   0        0        0    17891 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/browser/mozilla.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/__init__.py
+-rw-r--r--   0        0        0    23725 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/keepass.py
+-rw-r--r--   0        0        0     4486 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/lastpass.py
+-rw-r--r--   0        0        0     5902 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/mRemoteNG-local.py
+-rw-r--r--   0        0        0    12420 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/manager/mRemoteNG.py
+-rw-r--r--   0        0        0        0 2023-07-06 08:25:26.659396 donpapi-1.0.1/donpapi/software/sysadmin/__init__.py
+-rw-r--r--   0        0        0    13660 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/d3des.py
+-rw-r--r--   0        0        0     6545 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/mobaxterm.py
+-rw-r--r--   0        0        0     2186 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/putty.py
+-rw-r--r--   0        0        0      210 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/teamviewer.py
+-rw-r--r--   0        0        0     2653 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/vnc-local.py
+-rw-r--r--   0        0        0     9808 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/vnc.py
+-rw-r--r--   0        0        0     6545 2023-07-06 08:25:26.663396 donpapi-1.0.1/donpapi/software/sysadmin/winscp.py
+-rw-r--r--   0        0        0     1015 2023-07-06 08:25:26.663396 donpapi-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    11514 2023-07-06 08:25:26.663396 donpapi-1.0.1/readme.md
+-rw-r--r--   0        0        0    12455 1970-01-01 00:00:00.000000 donpapi-1.0.1/PKG-INFO
```

### Comparing `donpapi-1.0.0/donpapi/database.py` & `donpapi-1.0.1/donpapi/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1116,1015 +1116,1015 @@
                         cur.execute(
                             f"INSERT INTO browser_version (browser_type,version,pillaged_from_computerid,pillaged_from_userid) VALUES ('{browser_type}', '{version}', '{pillaged_from_computerid}', {pillaged_from_userid})")
         except Exception as ex:
             self.logging.error(f"Exception in Add browser_version")
             self.logging.debug(ex)
 
 
-def add_computer(self, ip, hostname='', domain='', os='', default_user_id=0, dc=0, smb_signing_enabled=False,
-                 smbv1_enabled=False, is_admin=False, connectivity='Ok'):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(f"[{ip}] {bcolors.OKBLUE}Adding Computer {hostname}{bcolors.ENDC}")
-    try:
-        # domain = domain.split('.')[0].upper()
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(f'SELECT * FROM computers WHERE ip LIKE "{ip}"')
-            results = cur.fetchall()
-
-        if not len(results):
+    def add_computer(self, ip, hostname='', domain='', os='', default_user_id=0, dc=0, smb_signing_enabled=False,
+                    smbv1_enabled=False, is_admin=False, connectivity='Ok'):
+        """
+        Check if this host has already been added to the database, if not add it in.
+        """
+        self.logging.debug(f"[{ip}] {bcolors.OKBLUE}Adding Computer {hostname}{bcolors.ENDC}")
+        try:
+            # domain = domain.split('.')[0].upper()
             with self.conn:
                 cur = self.conn.cursor()
-                cur.execute(
-                    f"INSERT INTO computers (ip, hostname, domain, os, dc, default_user_id,smb_signing_enabled,is_admin,smbv1_enabled,connectivity) VALUES ('{ip}', '{hostname}', '{domain}', '{os}', {dc},{default_user_id},{smb_signing_enabled},{is_admin},{smbv1_enabled},'{connectivity}')")
-
-        return cur.lastrowid
-    except Exception as ex:
-        self.logging.error(f"Exception in Add Computeur")
-        self.logging.debug(ex)
-
-
-def update_computer(self, ip, hostname=None, domain=None, os=None, default_user_id=None, dc=None,
-                    smb_signing_enabled=None, smbv1_enabled=None, is_admin=None, connectivity=None):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(f"Updating Computer {ip}")
-    try:
-        # domain = domain.split('.')[0].upper()
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(f'SELECT * FROM computers WHERE ip LIKE "{ip}"')
-            results = cur.fetchall()
-
-        if len(results):
-            for host in results:
-                id_ = host[0]
-                hostname_ = host[2]
-                domain_ = host[3]
-                os_ = host[4]
-                dc_ = host[5]
-                is_admin_ = host[8]
-                connectivity_ = host[9]
-                for val in [(hostname, 'hostname'), (domain, 'domain'), (os, 'os'), (hostname, 'hostname'),
-                            (default_user_id, 'default_user_id'), (dc, 'dc'),
-                            (smb_signing_enabled, 'smb_signing_enabled'), (smbv1_enabled, 'smbv1_enabled'),
-                            (is_admin, 'is_admin'), (connectivity, 'connectivity')]:
-                    value = val[0]
-                    var = val[1]
-                    if value != None:
-                        with self.conn:
-                            cur = self.conn.cursor()
-                            cur.execute(f"UPDATE computers SET {var}='{value}' WHERE id={id_}")
-    except Exception as ex:
-        self.logging.error(f"Exception in Add Computeur")
-        self.logging.debug(ex)
-
-
-def add_file(self, file_path, filename, extension, pillaged_from_computerid=None, pillaged_from_computer_ip=None,
-             pillaged_from_userid=None, pillaged_from_username=None):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(
-        f"Adding file {filename} - path : {file_path} - {extension} - from user  {pillaged_from_username}")
-    try:
-        # domain = domain.split('.')[0].upper()
-        if pillaged_from_userid == None and pillaged_from_username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT id FROM users WHERE username='{pillaged_from_username}'")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_userid = result[0]
-            # print(f"{pillaged_from_userid} is {pillaged_from_username}")
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_computerid = result[0]
-        if pillaged_from_computerid != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(
-                    f'SELECT * FROM files WHERE filename LIKE "{filename}" AND pillaged_from_computerid={pillaged_from_computerid}')
+                cur.execute(f'SELECT * FROM computers WHERE ip LIKE "{ip}"')
                 results = cur.fetchall()
 
-                if not len(results):
-                    # self.logging.debug(f"inserting file {filename} - {file_path} -{extension}")
+            if not len(results):
+                with self.conn:
+                    cur = self.conn.cursor()
                     cur.execute(
-                        f"INSERT INTO files (file_path,filename,extension,pillaged_from_computerid,pillaged_from_userid) VALUES ('{file_path}', '{filename}', '{extension}', '{pillaged_from_computerid}', {pillaged_from_userid})")
-    except Exception as ex:
-        self.logging.error(f"Exception in Add Files")
-        self.logging.debug(ex)
-
-
-def add_masterkey(self, file_path, guid, status, decrypted_with='', decrypted_value='', pillaged_from_computerid=None,
-                  pillaged_from_computer_ip=None, pillaged_from_userid=None, pillaged_from_username=None):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(
-        f"[{pillaged_from_computer_ip}] Adding Masterkey {guid} - path : {file_path} - from user  {pillaged_from_username} - {status} ")
-    try:
-        # domain = domain.split('.')[0].upper()
-        if pillaged_from_userid == None and pillaged_from_username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT id FROM users WHERE username='{pillaged_from_username}'")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_userid = result[0]
-                    self.logging.debug(
-                        f"[{pillaged_from_computer_ip}] {pillaged_from_userid} is {pillaged_from_username}")
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_computerid = result[0]
-                    self.logging.debug(
-                        f"[{pillaged_from_computer_ip}] {pillaged_from_computer_ip} is {pillaged_from_computerid}")
-        if pillaged_from_computerid != None:
+                        f"INSERT INTO computers (ip, hostname, domain, os, dc, default_user_id,smb_signing_enabled,is_admin,smbv1_enabled,connectivity) VALUES ('{ip}', '{hostname}', '{domain}', '{os}', {dc},{default_user_id},{smb_signing_enabled},{is_admin},{smbv1_enabled},'{connectivity}')")
+
+            return cur.lastrowid
+        except Exception as ex:
+            self.logging.error(f"Exception in Add Computeur")
+            self.logging.debug(ex)
+
+
+    def update_computer(self, ip, hostname=None, domain=None, os=None, default_user_id=None, dc=None,
+                        smb_signing_enabled=None, smbv1_enabled=None, is_admin=None, connectivity=None):
+        """
+        Check if this host has already been added to the database, if not add it in.
+        """
+        self.logging.debug(f"Updating Computer {ip}")
+        try:
+            # domain = domain.split('.')[0].upper()
             with self.conn:
                 cur = self.conn.cursor()
-                cur.execute(
-                    f'SELECT * FROM masterkey WHERE guid LIKE "{guid}" AND pillaged_from_computerid={pillaged_from_computerid}')
+                cur.execute(f'SELECT * FROM computers WHERE ip LIKE "{ip}"')
                 results = cur.fetchall()
 
-                if not len(results):
-                    with self.conn:
-                        cur = self.conn.cursor()
-                        self.logging.debug(
-                            f"[{pillaged_from_computer_ip}] inserting Masterkey {guid} - {file_path} -{status} {pillaged_from_computerid}', {pillaged_from_userid},{decrypted_with},{decrypted_value}")
-                        cur.execute(
-                            f"INSERT INTO masterkey (file_path,guid,status,pillaged_from_computerid,pillaged_from_userid,decrypted_with,decrypted_value) VALUES ('{file_path}', '{guid}', '{status}', '{pillaged_from_computerid}', {pillaged_from_userid},'{decrypted_with}','{decrypted_value}')")
-                else:
-                    for masterkey in results:
-                        if (status != masterkey[3]) or (decrypted_with != masterkey[6]) or (
-                                decrypted_value != masterkey[7]):
+            if len(results):
+                for host in results:
+                    id_ = host[0]
+                    hostname_ = host[2]
+                    domain_ = host[3]
+                    os_ = host[4]
+                    dc_ = host[5]
+                    is_admin_ = host[8]
+                    connectivity_ = host[9]
+                    for val in [(hostname, 'hostname'), (domain, 'domain'), (os, 'os'), (hostname, 'hostname'),
+                                (default_user_id, 'default_user_id'), (dc, 'dc'),
+                                (smb_signing_enabled, 'smb_signing_enabled'), (smbv1_enabled, 'smbv1_enabled'),
+                                (is_admin, 'is_admin'), (connectivity, 'connectivity')]:
+                        value = val[0]
+                        var = val[1]
+                        if value != None:
                             with self.conn:
                                 cur = self.conn.cursor()
-                                cur.execute(
-                                    f"UPDATE masterkey SET status='{status}', decrypted_with='{decrypted_with}', decrypted_value='{decrypted_value}' WHERE id={masterkey[0]}")
-    except Exception as ex:
-        self.logging.error(f"Exception in Add Masterkey")
-        self.logging.debug(ex)
+                                cur.execute(f"UPDATE computers SET {var}='{value}' WHERE id={id_}")
+        except Exception as ex:
+            self.logging.error(f"Exception in Add Computeur")
+            self.logging.debug(ex)
 
 
-def update_masterkey(self, file_path, guid, status, decrypted_with=None, decrypted_value=None,
-                     pillaged_from_computerid=None, pillaged_from_computer_ip=None, pillaged_from_userid=None,
-                     pillaged_from_username=None):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(f"Updating Masterkey {guid} {status} {decrypted_value} {decrypted_with}")
-    try:
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_computerid = result[0]
-                    self.logging.debug(
-                        f"[{pillaged_from_computer_ip}] {pillaged_from_computer_ip} is {pillaged_from_computerid}")
-        if pillaged_from_computerid != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(
-                    f'SELECT * FROM masterkey WHERE guid LIKE "{guid}" AND pillaged_from_computerid={pillaged_from_computerid}')
-                results = cur.fetchall()
+    def add_file(self, file_path, filename, extension, pillaged_from_computerid=None, pillaged_from_computer_ip=None,
+                pillaged_from_userid=None, pillaged_from_username=None):
+        """
+        Check if this host has already been added to the database, if not add it in.
+        """
+        self.logging.debug(
+            f"Adding file {filename} - path : {file_path} - {extension} - from user  {pillaged_from_username}")
+        try:
+            # domain = domain.split('.')[0].upper()
+            if pillaged_from_userid == None and pillaged_from_username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT id FROM users WHERE username='{pillaged_from_username}'")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_userid = result[0]
+                # print(f"{pillaged_from_userid} is {pillaged_from_username}")
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_computerid = result[0]
+            if pillaged_from_computerid != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f'SELECT * FROM files WHERE filename LIKE "{filename}" AND pillaged_from_computerid={pillaged_from_computerid}')
+                    results = cur.fetchall()
 
-                if len(results):
-                    self.logging.debug("Found initial Masterkey")
-                    for masterkey in results:
+                    if not len(results):
+                        # self.logging.debug(f"inserting file {filename} - {file_path} -{extension}")
+                        cur.execute(
+                            f"INSERT INTO files (file_path,filename,extension,pillaged_from_computerid,pillaged_from_userid) VALUES ('{file_path}', '{filename}', '{extension}', '{pillaged_from_computerid}', {pillaged_from_userid})")
+        except Exception as ex:
+            self.logging.error(f"Exception in Add Files")
+            self.logging.debug(ex)
+
+
+    def add_masterkey(self, file_path, guid, status, decrypted_with='', decrypted_value='', pillaged_from_computerid=None,
+                    pillaged_from_computer_ip=None, pillaged_from_userid=None, pillaged_from_username=None):
+        """
+        Check if this host has already been added to the database, if not add it in.
+        """
+        self.logging.debug(
+            f"[{pillaged_from_computer_ip}] Adding Masterkey {guid} - path : {file_path} - from user  {pillaged_from_username} - {status} ")
+        try:
+            # domain = domain.split('.')[0].upper()
+            if pillaged_from_userid == None and pillaged_from_username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT id FROM users WHERE username='{pillaged_from_username}'")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_userid = result[0]
+                        self.logging.debug(
+                            f"[{pillaged_from_computer_ip}] {pillaged_from_userid} is {pillaged_from_username}")
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_computerid = result[0]
+                        self.logging.debug(
+                            f"[{pillaged_from_computer_ip}] {pillaged_from_computer_ip} is {pillaged_from_computerid}")
+            if pillaged_from_computerid != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f'SELECT * FROM masterkey WHERE guid LIKE "{guid}" AND pillaged_from_computerid={pillaged_from_computerid}')
+                    results = cur.fetchall()
+
+                    if not len(results):
                         with self.conn:
                             cur = self.conn.cursor()
+                            self.logging.debug(
+                                f"[{pillaged_from_computer_ip}] inserting Masterkey {guid} - {file_path} -{status} {pillaged_from_computerid}', {pillaged_from_userid},{decrypted_with},{decrypted_value}")
                             cur.execute(
-                                f"UPDATE masterkey SET status='{status}', decrypted_with='{decrypted_with}', decrypted_value='{decrypted_value}' WHERE id={masterkey[0]}")
-    except Exception as ex:
-        self.logging.debug(f"Exception in update Masterkey")
-        self.logging.debug(ex)
-
-
-def add_connected_user(self, ip, username):
-    """
-    Check if this host has already been added to the database, if not add it in.
-    """
-    self.logging.debug(f"Adding connected user {username} from {ip}")
-    ip = ip.replace('\\', '')
-    try:
-        # domain = domain.split('.')[0].upper()
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(f'SELECT * FROM connected_user WHERE username LIKE "{username}" AND ip LIKE "{ip}"')
-            results = cur.fetchall()
+                                f"INSERT INTO masterkey (file_path,guid,status,pillaged_from_computerid,pillaged_from_userid,decrypted_with,decrypted_value) VALUES ('{file_path}', '{guid}', '{status}', '{pillaged_from_computerid}', {pillaged_from_userid},'{decrypted_with}','{decrypted_value}')")
+                    else:
+                        for masterkey in results:
+                            if (status != masterkey[3]) or (decrypted_with != masterkey[6]) or (
+                                    decrypted_value != masterkey[7]):
+                                with self.conn:
+                                    cur = self.conn.cursor()
+                                    cur.execute(
+                                        f"UPDATE masterkey SET status='{status}', decrypted_with='{decrypted_with}', decrypted_value='{decrypted_value}' WHERE id={masterkey[0]}")
+        except Exception as ex:
+            self.logging.error(f"Exception in Add Masterkey")
+            self.logging.debug(ex)
 
-        if not len(results):
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"INSERT INTO connected_user (username, ip) VALUES ('{username}','{ip}')")
-        return cur.lastrowid
-    except Exception as ex:
-        self.logging.error(f"Exception in Add Connected users")
-        self.logging.debug(ex)
 
+    def update_masterkey(self, file_path, guid, status, decrypted_with=None, decrypted_value=None,
+                        pillaged_from_computerid=None, pillaged_from_computer_ip=None, pillaged_from_userid=None,
+                        pillaged_from_username=None):
+        """
+        Check if this host has already been added to the database, if not add it in.
+        """
+        self.logging.debug(f"Updating Masterkey {guid} {status} {decrypted_value} {decrypted_with}")
+        try:
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_computerid = result[0]
+                        self.logging.debug(
+                            f"[{pillaged_from_computer_ip}] {pillaged_from_computer_ip} is {pillaged_from_computerid}")
+            if pillaged_from_computerid != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f'SELECT * FROM masterkey WHERE guid LIKE "{guid}" AND pillaged_from_computerid={pillaged_from_computerid}')
+                    results = cur.fetchall()
 
-def add_user(self, domain='', username='', password='', credtype='', pillaged_from_computerid=None,
-             pillaged_from_computer_ip=None):
-    try:
-        # domain = domain.split('.')[0].upper()
-        user_rowid = None
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-                results = cur.fetchall()
-                if len(results) > 0:
-                    result = results[0]
-                    pillaged_from_computerid = result[0]
-        if pillaged_from_computerid != None:
-            query = f"SELECT * FROM users WHERE LOWER(domain)=LOWER('{domain}') AND LOWER(username)=LOWER('{username}') AND pillaged_from_computerid={pillaged_from_computerid}"
-            self.logging.debug(query)
+                    if len(results):
+                        self.logging.debug("Found initial Masterkey")
+                        for masterkey in results:
+                            with self.conn:
+                                cur = self.conn.cursor()
+                                cur.execute(
+                                    f"UPDATE masterkey SET status='{status}', decrypted_with='{decrypted_with}', decrypted_value='{decrypted_value}' WHERE id={masterkey[0]}")
+        except Exception as ex:
+            self.logging.debug(f"Exception in update Masterkey")
+            self.logging.debug(ex)
+
+
+    def add_connected_user(self, ip, username):
+        """
+        Check connected users to the machine
+        """
+        self.logging.info(f"Adding connected user {username} from {ip}")
+        ip = ip.replace('\\', '')
+        try:
+            # domain = domain.split('.')[0].upper()
             with self.conn:
                 cur = self.conn.cursor()
-                cur.execute(query)
+                cur.execute(f'SELECT * FROM connected_user WHERE username LIKE "{username}" AND ip LIKE "{ip}"')
                 results = cur.fetchall()
 
             if not len(results):
-                query = f"INSERT INTO users (domain, username, password, credtype, pillaged_from_computerid) VALUES ('{domain}','{username}','{password}','{credtype}',{pillaged_from_computerid})"
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"INSERT INTO connected_user (username, ip) VALUES ('{username}','{ip}')")
+            return cur.lastrowid
+        except Exception as ex:
+            self.logging.error(f"Exception in Add Connected users")
+            self.logging.debug(ex)
+
+
+    def add_user(self, domain='', username='', password='', credtype='', pillaged_from_computerid=None,
+                pillaged_from_computer_ip=None):
+        try:
+            # domain = domain.split('.')[0].upper()
+            user_rowid = None
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                    results = cur.fetchall()
+                    if len(results) > 0:
+                        result = results[0]
+                        pillaged_from_computerid = result[0]
+            if pillaged_from_computerid != None:
+                query = f"SELECT * FROM users WHERE LOWER(domain)=LOWER('{domain}') AND LOWER(username)=LOWER('{username}') AND pillaged_from_computerid={pillaged_from_computerid}"
                 self.logging.debug(query)
                 with self.conn:
                     cur = self.conn.cursor()
                     cur.execute(query)
-                user_rowid = cur.lastrowid
-                self.logging.debug('add_user(domain={}, username={}) => {}'.format(domain, username, user_rowid))
+                    results = cur.fetchall()
+
+                if not len(results):
+                    query = f"INSERT INTO users (domain, username, password, credtype, pillaged_from_computerid) VALUES ('{domain}','{username}','{password}','{credtype}',{pillaged_from_computerid})"
+                    self.logging.debug(query)
+                    with self.conn:
+                        cur = self.conn.cursor()
+                        cur.execute(query)
+                    user_rowid = cur.lastrowid
+                    self.logging.debug('add_user(domain={}, username={}) => {}'.format(domain, username, user_rowid))
+                else:
+                    self.logging.debug('add_user(domain={}, username={}) ALREADY EXIST'.format(domain, username))
             else:
-                self.logging.debug('add_user(domain={}, username={}) ALREADY EXIST'.format(domain, username))
-        else:
-            self.logging.error(f"user {username} associated computer not found ")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_user ")
-        self.logging.debug(ex)
-    return user_rowid
+                self.logging.error(f"user {username} associated computer not found ")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_user ")
+            self.logging.debug(ex)
+        return user_rowid
 
 
-def add_sid(self, username=None, user_id=None, sid=None):
-    try:
-        if user_id == None and username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT id FROM users WHERE LOWER(username)=LOWER('{username}')")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                user_id = result[0]
-        if user_id != None and sid != None:
-            # Deja en base ?
-            query = f"SELECT * FROM user_sid WHERE LOWER(sid)=LOWER('{sid}') AND user_id={user_id}"
-            self.logging.debug(query)
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(query)
-            results = cur.fetchall()
-            if not len(results):
-                query = f"INSERT INTO user_sid (user_id, sid) VALUES ('{user_id}','{sid}')"
+    def add_sid(self, username=None, user_id=None, sid=None):
+        try:
+            if user_id == None and username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT id FROM users WHERE LOWER(username)=LOWER('{username}')")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    user_id = result[0]
+            if user_id != None and sid != None:
+                # Deja en base ?
+                query = f"SELECT * FROM user_sid WHERE LOWER(sid)=LOWER('{sid}') AND user_id={user_id}"
                 self.logging.debug(query)
                 with self.conn:
                     cur = self.conn.cursor()
                     cur.execute(query)
-                user_rowid = cur.lastrowid
-                self.logging.debug(f'added SID {sid} for user id {user_id}')
-    except Exception as ex:
-        self.logging.error(f"Exception in add_sid ")
-        self.logging.debug(ex)
-    self.logging.debug(f"Added {username} sid {sid} to database")
-    return 1
-
+                results = cur.fetchall()
+                if not len(results):
+                    query = f"INSERT INTO user_sid (user_id, sid) VALUES ('{user_id}','{sid}')"
+                    self.logging.debug(query)
+                    with self.conn:
+                        cur = self.conn.cursor()
+                        cur.execute(query)
+                    user_rowid = cur.lastrowid
+                    self.logging.debug(f'added SID {sid} for user id {user_id}')
+        except Exception as ex:
+            self.logging.error(f"Exception in add_sid ")
+            self.logging.debug(ex)
+        self.logging.debug(f"Added {username} sid {sid} to database")
+        return 1
 
-def add_dpapi_hash(self, file_path=None, sid=None, guid=None, hash=None, context=None, pillaged_from_computerid=None,
-                   pillaged_from_computer_ip=None):
-    try:
-        # domain = domain.split('.')[0].upper()
-        user_rowid = None
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_computerid = result[0]
-        if pillaged_from_computerid != None and sid != None and guid != None and hash != None and context != None:
-            query = f"SELECT * FROM dpapi_hash WHERE LOWER(sid)=LOWER('{sid}') AND LOWER(guid)=LOWER('{guid}') AND LOWER(hash)=LOWER('{hash}') AND pillaged_from_computerid={pillaged_from_computerid} AND LOWER(context)=LOWER('{context}')"
-            self.logging.debug(query)
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(query)
-            results = cur.fetchall()
 
-            if not len(results):
-                query = f"INSERT INTO dpapi_hash (file_path, sid, guid, hash, context, pillaged_from_computerid) VALUES ('{file_path}','{sid}','{guid}','{hash}','{context}',{pillaged_from_computerid})"
+    def add_dpapi_hash(self, file_path=None, sid=None, guid=None, hash=None, context=None, pillaged_from_computerid=None,
+                    pillaged_from_computer_ip=None):
+        try:
+            # domain = domain.split('.')[0].upper()
+            user_rowid = None
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_computerid = result[0]
+            if pillaged_from_computerid != None and sid != None and guid != None and hash != None and context != None:
+                query = f"SELECT * FROM dpapi_hash WHERE LOWER(sid)=LOWER('{sid}') AND LOWER(guid)=LOWER('{guid}') AND LOWER(hash)=LOWER('{hash}') AND pillaged_from_computerid={pillaged_from_computerid} AND LOWER(context)=LOWER('{context}')"
                 self.logging.debug(query)
                 with self.conn:
                     cur = self.conn.cursor()
                     cur.execute(query)
-                user_rowid = cur.lastrowid
-                self.logging.debug(f'added DPAPI hash {hash}')
+                results = cur.fetchall()
+
+                if not len(results):
+                    query = f"INSERT INTO dpapi_hash (file_path, sid, guid, hash, context, pillaged_from_computerid) VALUES ('{file_path}','{sid}','{guid}','{hash}','{context}',{pillaged_from_computerid})"
+                    self.logging.debug(query)
+                    with self.conn:
+                        cur = self.conn.cursor()
+                        cur.execute(query)
+                    user_rowid = cur.lastrowid
+                    self.logging.debug(f'added DPAPI hash {hash}')
+                else:
+                    self.logging.debug(f'DPAPI hash {hash} ALREADY EXIST')
             else:
-                self.logging.debug(f'DPAPI hash {hash} ALREADY EXIST')
-        else:
-            self.logging.error(
-                f"missing infos to register DPAPI hash {hash} - {file_path},{sid},{guid},{hash},{context},{pillaged_from_computerid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_hash ")
-        self.logging.debug(ex)
-    return user_rowid
-
-
-def clear_input(self, data):
-    if isinstance(data, int):
-        return data
-    if data is None:
-        data = ''
-    result = data.replace('\x00', '')
-    return result
-
-
-def add_certificate(self, guid, pfx_file_path, issuer, subject, client_auth, pillaged_from_computerid=None,
-                    pillaged_from_userid=None, pillaged_from_computer_ip=None, pillaged_from_username=None):
-    """
-    Check if this cert has already been added to db, if not then add it
-    """
-    user_rowid = None
-    try:
-        guid = self.clear_input(guid)
-        pfx_file_path = self.clear_input(pfx_file_path)
-        issuer = self.clear_input(issuer)
-        subject = self.clear_input(subject)
-        self.logging.debug(f"{guid} - {binascii.hexlify(guid.encode('utf-8'))}")
-        self.logging.debug(f"{issuer} - {binascii.hexlify(issuer.encode('utf-8'))}")
-        self.logging.debug(f"{subject} - {binascii.hexlify(subject.encode('utf-8'))}")
-        self.logging.debug(f"{client_auth}")
-        self.logging.debug(f"{pfx_file_path} - {binascii.hexlify(pfx_file_path.encode('utf-8'))}")
-        self.logging.debug(
-            f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
-        self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
+                self.logging.error(
+                    f"missing infos to register DPAPI hash {hash} - {file_path},{sid},{guid},{hash},{context},{pillaged_from_computerid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_hash ")
+            self.logging.debug(ex)
+        return user_rowid
 
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_computerid = result[0]
-                self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_certificate 1")
-        self.logging.debug(ex)
 
-    try:
-        if pillaged_from_username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(
-                    f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_userid = result[0]
-                self.logging.debug(
-                    f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_certificate 2")
-        self.logging.debug(ex)
-        pass
-    if pillaged_from_computerid == None or pillaged_from_userid == None:
-        self.logging.debug(
-            f"[-] Missing computerId or UserId to register Certificate {pillaged_from_username} {pfx_file_path}")
-    # return None
+    def clear_input(self, data):
+        if isinstance(data, int):
+            return data
+        if data is None:
+            data = ''
+        result = data.replace('\x00', '')
+        return result
+
+
+    def add_certificate(self, guid, pfx_file_path, issuer, subject, client_auth, pillaged_from_computerid=None,
+                        pillaged_from_userid=None, pillaged_from_computer_ip=None, pillaged_from_username=None):
+        """
+        Check if this cert has already been added to db, if not then add it
+        """
+        user_rowid = None
+        try:
+            guid = self.clear_input(guid)
+            pfx_file_path = self.clear_input(pfx_file_path)
+            issuer = self.clear_input(issuer)
+            subject = self.clear_input(subject)
+            self.logging.debug(f"{guid} - {binascii.hexlify(guid.encode('utf-8'))}")
+            self.logging.debug(f"{issuer} - {binascii.hexlify(issuer.encode('utf-8'))}")
+            self.logging.debug(f"{subject} - {binascii.hexlify(subject.encode('utf-8'))}")
+            self.logging.debug(f"{client_auth}")
+            self.logging.debug(f"{pfx_file_path} - {binascii.hexlify(pfx_file_path.encode('utf-8'))}")
+            self.logging.debug(
+                f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
+            self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
 
-    try:
-        if pillaged_from_userid == None:
-            query = "SELECT * FROM certificates WHERE LOWER(guid)=LOWER(:guid) AND LOWER(subject)=LOWER(:subject) AND LOWER(issuer)=LOWER(:issuer) AND pillaged_from_computerid=:pillaged_from_computerid"
-            parameters = {
-                "guid": guid,
-                "subject": subject,
-                "issuer": issuer,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-            }
-        else:
-            query = "SELECT * FROM certificates WHERE LOWER(guid)=LOWER(:guid) AND LOWER(subject)=LOWER(:subject) AND LOWER(issuer)=LOWER(:issuer) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
-            parameters = {
-                "guid": guid,
-                "subject": subject,
-                "issuer": issuer,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-                "pillaged_from_userid": int(pillaged_from_userid)
-            }
-        self.logging.debug(query)
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(query, parameters)
-        results = cur.fetchall()
-    except Exception as ex:
-        self.logging.error(f"Exception in add_certificate 3")
-        self.logging.debug(ex)
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_computerid = result[0]
+                    self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_certificate 1")
+            self.logging.debug(ex)
 
-    try:
-        if not result or not len(results):
+        try:
+            if pillaged_from_username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_userid = result[0]
+                    self.logging.debug(
+                        f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_certificate 2")
+            self.logging.debug(ex)
+            pass
+        if pillaged_from_computerid == None or pillaged_from_userid == None:
+            self.logging.debug(
+                f"[-] Missing computerId or UserId to register Certificate {pillaged_from_username} {pfx_file_path}")
+        # return None
+
+        try:
             if pillaged_from_userid == None:
-                query = "INSERT INTO certificates (pfx_file_path, guid, issuer, subject, client_auth, pillaged_from_computerid) VALUES (:pfx_file_path, :guid, :issuer, :subject, :client_auth, :pillaged_from_computerid)"
+                query = "SELECT * FROM certificates WHERE LOWER(guid)=LOWER(:guid) AND LOWER(subject)=LOWER(:subject) AND LOWER(issuer)=LOWER(:issuer) AND pillaged_from_computerid=:pillaged_from_computerid"
                 parameters = {
-                    "pfx_file_path": pfx_file_path,
                     "guid": guid,
-                    "issuer": issuer,
                     "subject": subject,
-                    "client_auth": client_auth,
+                    "issuer": issuer,
                     "pillaged_from_computerid": int(pillaged_from_computerid),
                 }
             else:
-                query = "INSERT INTO certificates (pfx_file_path, guid, issuer, subject, client_auth, pillaged_from_computerid, pillaged_from_userid) VALUES (:pfx_file_path, :guid, :issuer, :subject, :client_auth, :pillaged_from_computerid, :pillaged_from_userid)"
+                query = "SELECT * FROM certificates WHERE LOWER(guid)=LOWER(:guid) AND LOWER(subject)=LOWER(:subject) AND LOWER(issuer)=LOWER(:issuer) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
                 parameters = {
-                    "pfx_file_path": pfx_file_path,
                     "guid": guid,
-                    "issuer": issuer,
                     "subject": subject,
-                    "client_auth": client_auth,
+                    "issuer": issuer,
+                    "pillaged_from_computerid": int(pillaged_from_computerid),
                     "pillaged_from_computerid": int(pillaged_from_computerid),
-                    "pillaged_from_userid": int(pillaged_from_userid),
+                    "pillaged_from_userid": int(pillaged_from_userid)
                 }
             self.logging.debug(query)
             with self.conn:
                 cur = self.conn.cursor()
                 cur.execute(query, parameters)
-            user_rowid = cur.lastrowid
-            self.logging.debug(
-                f'added_certificate(guid={guid}, issuer={issuer}, subject={subject}, client_auth={client_auth}) => {user_rowid}')
-        else:
-            self.logging.debug(
-                f'added_certificate(guid={guid}, issuer={issuer}, subject={subject}, client_auth={client_auth}) => ALREADY IN DB')
-
-    except Exception as ex:
-        self.logging.error(f"Exception in add_certificates 4")
-        self.logging.debug(ex)
-
-
-def add_credz(self, credz_type, credz_username, credz_password, credz_target, credz_path, pillaged_from_computerid=None,
-              pillaged_from_userid=None, pillaged_from_computer_ip=None, pillaged_from_username=None):
-    """
-    Check if this credential has already been added to the database, if not add it in.
-    """
-    user_rowid = None
-    try:
-        credz_username = self.clear_input(credz_username)
-        credz_password = self.clear_input(credz_password)
-        credz_target = self.clear_input(credz_target)
-        credz_path = self.clear_input(credz_path)
-        self.logging.debug(f"{credz_username} - {binascii.hexlify(credz_username.encode('utf-8'))}")
-        self.logging.debug(f"{credz_password} - {binascii.hexlify(credz_password.encode('utf-8'))}")
-        self.logging.debug(f"{credz_target} - {binascii.hexlify(credz_target.encode('utf-8'))}")
-        self.logging.debug(f"{credz_path} - {binascii.hexlify(credz_path.encode('utf-8'))}")
-        self.logging.debug(
-            f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
-        self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
-
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
             results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_computerid = result[0]
-                self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_credz 1")
-        self.logging.debug(ex)
+        except Exception as ex:
+            self.logging.error(f"Exception in add_certificate 3")
+            self.logging.debug(ex)
 
-    try:
-        if pillaged_from_username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(
-                    f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_userid = result[0]
+        try:
+            if not result or not len(results):
+                if pillaged_from_userid == None:
+                    query = "INSERT INTO certificates (pfx_file_path, guid, issuer, subject, client_auth, pillaged_from_computerid) VALUES (:pfx_file_path, :guid, :issuer, :subject, :client_auth, :pillaged_from_computerid)"
+                    parameters = {
+                        "pfx_file_path": pfx_file_path,
+                        "guid": guid,
+                        "issuer": issuer,
+                        "subject": subject,
+                        "client_auth": client_auth,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                    }
+                else:
+                    query = "INSERT INTO certificates (pfx_file_path, guid, issuer, subject, client_auth, pillaged_from_computerid, pillaged_from_userid) VALUES (:pfx_file_path, :guid, :issuer, :subject, :client_auth, :pillaged_from_computerid, :pillaged_from_userid)"
+                    parameters = {
+                        "pfx_file_path": pfx_file_path,
+                        "guid": guid,
+                        "issuer": issuer,
+                        "subject": subject,
+                        "client_auth": client_auth,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                        "pillaged_from_userid": int(pillaged_from_userid),
+                    }
+                self.logging.debug(query)
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(query, parameters)
+                user_rowid = cur.lastrowid
                 self.logging.debug(
-                    f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_credz 2")
-        self.logging.debug(ex)
-        pass
-    if pillaged_from_computerid == None or pillaged_from_userid == None:
-        self.logging.debug(
-            f"[-] Missing computerId or UserId to register Credz {credz_username} {credz_password} - {credz_target}")
-    # return None
-    try:
-        if pillaged_from_userid == None:
-            query = "SELECT * FROM credz WHERE LOWER(username)=LOWER(:credz_username) AND LOWER(password)=LOWER(:credz_password) AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid"
-            parameters = {
-                "credz_username": credz_username,
-                "credz_password": credz_password,
-                "credz_type": credz_type, "credz_target": credz_target,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-            }
-        else:
-            query = "SELECT * FROM credz WHERE LOWER(username)=LOWER(:credz_username) AND LOWER(password)=LOWER(:credz_password) AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
-            parameters = {
-                "credz_username": credz_username,
-                "credz_password": credz_password,
-                "credz_type": credz_type, "credz_target": credz_target,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-                "pillaged_from_userid": int(pillaged_from_userid)
-            }
-        self.logging.debug(query)
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(query, parameters)
-        results = cur.fetchall()
-    except Exception as ex:
-        self.logging.error(f"Exception in add_credz 3")
-        self.logging.debug(ex)
-    try:
-        if not len(results):
+                    f'added_certificate(guid={guid}, issuer={issuer}, subject={subject}, client_auth={client_auth}) => {user_rowid}')
+            else:
+                self.logging.debug(
+                    f'added_certificate(guid={guid}, issuer={issuer}, subject={subject}, client_auth={client_auth}) => ALREADY IN DB')
+
+        except Exception as ex:
+            self.logging.error(f"Exception in add_certificates 4")
+            self.logging.debug(ex)
+
+
+    def add_credz(self, credz_type, credz_username, credz_password, credz_target, credz_path, pillaged_from_computerid=None,
+                pillaged_from_userid=None, pillaged_from_computer_ip=None, pillaged_from_username=None):
+        """
+        Check if this credential has already been added to the database, if not add it in.
+        """
+        user_rowid = None
+        try:
+            credz_username = self.clear_input(credz_username)
+            credz_password = self.clear_input(credz_password)
+            credz_target = self.clear_input(credz_target)
+            credz_path = self.clear_input(credz_path)
+            self.logging.debug(f"{credz_username} - {binascii.hexlify(credz_username.encode('utf-8'))}")
+            self.logging.debug(f"{credz_password} - {binascii.hexlify(credz_password.encode('utf-8'))}")
+            self.logging.debug(f"{credz_target} - {binascii.hexlify(credz_target.encode('utf-8'))}")
+            self.logging.debug(f"{credz_path} - {binascii.hexlify(credz_path.encode('utf-8'))}")
+            self.logging.debug(
+                f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
+            self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
+
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_computerid = result[0]
+                    self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_credz 1")
+            self.logging.debug(ex)
+
+        try:
+            if pillaged_from_username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_userid = result[0]
+                    self.logging.debug(
+                        f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_credz 2")
+            self.logging.debug(ex)
+            pass
+        if pillaged_from_computerid == None or pillaged_from_userid == None:
+            self.logging.debug(
+                f"[-] Missing computerId or UserId to register Credz {credz_username} {credz_password} - {credz_target}")
+        # return None
+        try:
             if pillaged_from_userid == None:
-                query = "INSERT INTO credz (username, password, target, type, pillaged_from_computerid, file_path) VALUES (:credz_username, :credz_password, :credz_target, :credz_type, :pillaged_from_computerid, :credz_path)"
+                query = "SELECT * FROM credz WHERE LOWER(username)=LOWER(:credz_username) AND LOWER(password)=LOWER(:credz_password) AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid"
                 parameters = {
                     "credz_username": credz_username,
                     "credz_password": credz_password,
-                    "credz_target": credz_target,
-                    "credz_type": credz_type,
+                    "credz_type": credz_type, "credz_target": credz_target,
                     "pillaged_from_computerid": int(pillaged_from_computerid),
-                    "credz_path": credz_path,
                 }
             else:
-                query = "INSERT INTO credz (username, password, target, type, pillaged_from_computerid,pillaged_from_userid, file_path) VALUES (:credz_username, :credz_password, :credz_target, :credz_type, :pillaged_from_computerid, :pillaged_from_userid, :credz_path)"
+                query = "SELECT * FROM credz WHERE LOWER(username)=LOWER(:credz_username) AND LOWER(password)=LOWER(:credz_password) AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
                 parameters = {
                     "credz_username": credz_username,
                     "credz_password": credz_password,
-                    "credz_type": credz_type,
-                    "credz_target": credz_target,
+                    "credz_type": credz_type, "credz_target": credz_target,
                     "pillaged_from_computerid": int(pillaged_from_computerid),
-                    "pillaged_from_userid": int(pillaged_from_userid),
-                    "credz_path": credz_path,
+                    "pillaged_from_userid": int(pillaged_from_userid)
                 }
             self.logging.debug(query)
             with self.conn:
                 cur = self.conn.cursor()
                 cur.execute(query, parameters)
-            user_rowid = cur.lastrowid
-            self.logging.debug(
-                f'added_credential(credtype={credz_type}, target={credz_target}, username={credz_username}, password={credz_password}) => {user_rowid}')
-        else:
-            self.logging.debug(
-                f'added_credential(credtype={credz_type}, target={credz_target}, username={credz_username}, password={credz_password}) => ALREADY IN DB')
+            results = cur.fetchall()
+        except Exception as ex:
+            self.logging.error(f"Exception in add_credz 3")
+            self.logging.debug(ex)
+        try:
+            if not len(results):
+                if pillaged_from_userid == None:
+                    query = "INSERT INTO credz (username, password, target, type, pillaged_from_computerid, file_path) VALUES (:credz_username, :credz_password, :credz_target, :credz_type, :pillaged_from_computerid, :credz_path)"
+                    parameters = {
+                        "credz_username": credz_username,
+                        "credz_password": credz_password,
+                        "credz_target": credz_target,
+                        "credz_type": credz_type,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                        "credz_path": credz_path,
+                    }
+                else:
+                    query = "INSERT INTO credz (username, password, target, type, pillaged_from_computerid,pillaged_from_userid, file_path) VALUES (:credz_username, :credz_password, :credz_target, :credz_type, :pillaged_from_computerid, :pillaged_from_userid, :credz_path)"
+                    parameters = {
+                        "credz_username": credz_username,
+                        "credz_password": credz_password,
+                        "credz_type": credz_type,
+                        "credz_target": credz_target,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                        "pillaged_from_userid": int(pillaged_from_userid),
+                        "credz_path": credz_path,
+                    }
+                self.logging.debug(query)
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(query, parameters)
+                user_rowid = cur.lastrowid
+                self.logging.debug(
+                    f'added_credential(credtype={credz_type}, target={credz_target}, username={credz_username}, password={credz_password}) => {user_rowid}')
+            else:
+                self.logging.debug(
+                    f'added_credential(credtype={credz_type}, target={credz_target}, username={credz_username}, password={credz_password}) => ALREADY IN DB')
 
-    except Exception as ex:
-        self.logging.error(f"Exception in add_credz 4")
-        self.logging.debug(ex)
-
-    return None
-
-
-def add_cookies(self, credz_type, credz_name, credz_value, credz_expires_utc, credz_target, credz_path,
-                pillaged_from_computerid=None, pillaged_from_userid=None, pillaged_from_computer_ip=None,
-                pillaged_from_username=None):
-    """
-    Check if this credential has already been added to the database, if not add it in.
-    """
-    user_rowid = None
-    try:
-        credz_name = self.clear_input(credz_name)
-        self.logging.debug(f"{credz_name} - {binascii.hexlify(credz_name.encode('utf-8'))}")
-        credz_value = self.clear_input(credz_value)
-        self.logging.debug(f"{credz_value} - {binascii.hexlify(credz_value.encode('utf-8'))}")
-        credz_expires_utc = self.clear_input(credz_expires_utc)
-        self.logging.debug(f"{credz_expires_utc}")
-        credz_target = self.clear_input(credz_target)
-        self.logging.debug(f"{credz_target} - {binascii.hexlify(credz_target.encode('utf-8'))}")
-        credz_path = self.clear_input(credz_path)
-        self.logging.debug(f"{credz_path} - {binascii.hexlify(credz_path.encode('utf-8'))}")
-        self.logging.debug(
-            f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
-        self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_credz 4")
+            self.logging.debug(ex)
 
-        if pillaged_from_computer_ip != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_computerid = result[0]
-                self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_cookie 1")
-        self.logging.debug(ex)
+        return None
 
-    try:
-        if pillaged_from_username != None:
-            with self.conn:
-                cur = self.conn.cursor()
-                cur.execute(
-                    f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
-            results = cur.fetchall()
-            if len(results) > 0:
-                result = results[0]
-                pillaged_from_userid = result[0]
-                self.logging.debug(
-                    f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
-    except Exception as ex:
-        self.logging.error(f"Exception in add_cookies 2")
-        self.logging.debug(ex)
-        pass
-    if pillaged_from_computerid == None or pillaged_from_userid == None:
-        self.logging.debug(
-            f"[-] Missing computerId or UserId to register Cookie {credz_name} {credz_value} - {credz_target}")
-    # return None
-    try:
-        if pillaged_from_userid == None:
-            query = "SELECT * FROM cookies WHERE LOWER(name)=LOWER(:credz_name) AND LOWER(value)=LOWER(:credz_value) AND expires_utc=:credz_expires_utc AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid"
-            parameters = {
-                "credz_name": credz_name,
-                "credz_value": credz_value,
-                "credz_expires_utc": credz_expires_utc,
-                "credz_type": credz_type, "credz_target": credz_target,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-            }
-        else:
-            query = "SELECT * FROM cookies WHERE LOWER(name)=LOWER(:credz_name) AND LOWER(value)=LOWER(:credz_value) AND expires_utc=:credz_expires_utc AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
-            parameters = {
-                "credz_name": credz_name,
-                "credz_value": credz_value,
-                "credz_expires_utc": credz_expires_utc,
-                "credz_type": credz_type, "credz_target": credz_target,
-                "pillaged_from_computerid": int(pillaged_from_computerid),
-                "pillaged_from_userid": int(pillaged_from_userid)
-            }
-        self.logging.debug(query)
-        with self.conn:
-            cur = self.conn.cursor()
-            cur.execute(query, parameters)
-        results = cur.fetchall()
-    except Exception as ex:
-        self.logging.error(f"Exception in add_cookie 3")
-        self.logging.debug(ex)
-    try:
-        if not len(results):
+
+    def add_cookies(self, credz_type, credz_name, credz_value, credz_expires_utc, credz_target, credz_path,
+                    pillaged_from_computerid=None, pillaged_from_userid=None, pillaged_from_computer_ip=None,
+                    pillaged_from_username=None):
+        """
+        Check if this credential has already been added to the database, if not add it in.
+        """
+        user_rowid = None
+        try:
+            credz_name = self.clear_input(credz_name)
+            self.logging.debug(f"{credz_name} - {binascii.hexlify(credz_name.encode('utf-8'))}")
+            credz_value = self.clear_input(credz_value)
+            self.logging.debug(f"{credz_value} - {binascii.hexlify(credz_value.encode('utf-8'))}")
+            credz_expires_utc = self.clear_input(credz_expires_utc)
+            self.logging.debug(f"{credz_expires_utc}")
+            credz_target = self.clear_input(credz_target)
+            self.logging.debug(f"{credz_target} - {binascii.hexlify(credz_target.encode('utf-8'))}")
+            credz_path = self.clear_input(credz_path)
+            self.logging.debug(f"{credz_path} - {binascii.hexlify(credz_path.encode('utf-8'))}")
+            self.logging.debug(
+                f"pillaged_from_computer_ip {pillaged_from_computer_ip} - {binascii.hexlify(pillaged_from_computer_ip.encode('utf-8'))}")
+            self.logging.debug(f"pillaged_from_username {pillaged_from_username}")
+
+            if pillaged_from_computer_ip != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(f"SELECT * FROM computers WHERE LOWER(ip)=LOWER('{pillaged_from_computer_ip}')")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_computerid = result[0]
+                    self.logging.debug(f"[+] Resolved {pillaged_from_computer_ip} to id : {pillaged_from_computerid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_cookie 1")
+            self.logging.debug(ex)
+
+        try:
+            if pillaged_from_username != None:
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(
+                        f"SELECT * FROM users WHERE LOWER(username)=LOWER('{pillaged_from_username}') AND pillaged_from_computerid={pillaged_from_computerid}")
+                results = cur.fetchall()
+                if len(results) > 0:
+                    result = results[0]
+                    pillaged_from_userid = result[0]
+                    self.logging.debug(
+                        f"[+] Resolved {pillaged_from_username} on machine {pillaged_from_computerid} to id : {pillaged_from_userid}")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_cookies 2")
+            self.logging.debug(ex)
+            pass
+        if pillaged_from_computerid == None or pillaged_from_userid == None:
+            self.logging.debug(
+                f"[-] Missing computerId or UserId to register Cookie {credz_name} {credz_value} - {credz_target}")
+        # return None
+        try:
             if pillaged_from_userid == None:
-                query = "INSERT INTO cookies (name, value, expires_utc, target, type, pillaged_from_computerid, file_path) VALUES (:credz_name, :credz_value, :credz_expires_utc, :credz_target, :credz_type, :pillaged_from_computerid, :credz_path)"
+                query = "SELECT * FROM cookies WHERE LOWER(name)=LOWER(:credz_name) AND LOWER(value)=LOWER(:credz_value) AND expires_utc=:credz_expires_utc AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid"
                 parameters = {
                     "credz_name": credz_name,
                     "credz_value": credz_value,
                     "credz_expires_utc": credz_expires_utc,
-                    "credz_target": credz_target,
-                    "credz_type": credz_type,
+                    "credz_type": credz_type, "credz_target": credz_target,
                     "pillaged_from_computerid": int(pillaged_from_computerid),
-                    "credz_path": credz_path,
                 }
             else:
-                query = "INSERT INTO cookies (name, value, expires_utc, target, type, pillaged_from_computerid,pillaged_from_userid, file_path) VALUES (:credz_name, :credz_value, :credz_expires_utc, :credz_target, :credz_type, :pillaged_from_computerid, :pillaged_from_userid, :credz_path)"
+                query = "SELECT * FROM cookies WHERE LOWER(name)=LOWER(:credz_name) AND LOWER(value)=LOWER(:credz_value) AND expires_utc=:credz_expires_utc AND LOWER(type)=LOWER(:credz_type) AND LOWER(target)=LOWER(:credz_target) AND pillaged_from_computerid=:pillaged_from_computerid AND pillaged_from_userid=:pillaged_from_userid"
                 parameters = {
                     "credz_name": credz_name,
                     "credz_value": credz_value,
                     "credz_expires_utc": credz_expires_utc,
-                    "credz_type": credz_type,
-                    "credz_target": credz_target,
+                    "credz_type": credz_type, "credz_target": credz_target,
                     "pillaged_from_computerid": int(pillaged_from_computerid),
-                    "pillaged_from_userid": int(pillaged_from_userid),
-                    "credz_path": credz_path,
+                    "pillaged_from_userid": int(pillaged_from_userid)
                 }
             self.logging.debug(query)
             with self.conn:
                 cur = self.conn.cursor()
                 cur.execute(query, parameters)
-            user_rowid = cur.lastrowid
-            self.logging.debug(
-                f'added_cookies(credtype={credz_type}, target={credz_target}, name={credz_name}, value={credz_value}) => {user_rowid}')
-        else:
-            self.logging.debug(
-                f'added_credential(credtype={credz_type}, target={credz_target}, name={credz_name}, value={credz_value}) => ALREADY IN DB')
-
-    except Exception as ex:
-        self.logging.error(f"Exception in add_cookie 4")
-        self.logging.debug(ex)
-
-    return None
-
-
-def get_credz_old(self, filterTerm=None, credz_type=None):
-    """
-    Return credentials from the database.
-    """
-
-    cur = self.conn.cursor()
-
-    if credz_type:
-        cur.execute(f"SELECT * FROM credz WHERE credtype='{credz_type}'")
-
-    # if we're filtering by username
-    elif filterTerm and filterTerm != '':
-        cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
+            results = cur.fetchall()
+        except Exception as ex:
+            self.logging.error(f"Exception in add_cookie 3")
+            self.logging.debug(ex)
+        try:
+            if not len(results):
+                if pillaged_from_userid == None:
+                    query = "INSERT INTO cookies (name, value, expires_utc, target, type, pillaged_from_computerid, file_path) VALUES (:credz_name, :credz_value, :credz_expires_utc, :credz_target, :credz_type, :pillaged_from_computerid, :credz_path)"
+                    parameters = {
+                        "credz_name": credz_name,
+                        "credz_value": credz_value,
+                        "credz_expires_utc": credz_expires_utc,
+                        "credz_target": credz_target,
+                        "credz_type": credz_type,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                        "credz_path": credz_path,
+                    }
+                else:
+                    query = "INSERT INTO cookies (name, value, expires_utc, target, type, pillaged_from_computerid,pillaged_from_userid, file_path) VALUES (:credz_name, :credz_value, :credz_expires_utc, :credz_target, :credz_type, :pillaged_from_computerid, :pillaged_from_userid, :credz_path)"
+                    parameters = {
+                        "credz_name": credz_name,
+                        "credz_value": credz_value,
+                        "credz_expires_utc": credz_expires_utc,
+                        "credz_type": credz_type,
+                        "credz_target": credz_target,
+                        "pillaged_from_computerid": int(pillaged_from_computerid),
+                        "pillaged_from_userid": int(pillaged_from_userid),
+                        "credz_path": credz_path,
+                    }
+                self.logging.debug(query)
+                with self.conn:
+                    cur = self.conn.cursor()
+                    cur.execute(query, parameters)
+                user_rowid = cur.lastrowid
+                self.logging.debug(
+                    f'added_cookies(credtype={credz_type}, target={credz_target}, name={credz_name}, value={credz_value}) => {user_rowid}')
+            else:
+                self.logging.debug(
+                    f'added_credential(credtype={credz_type}, target={credz_target}, name={credz_name}, value={credz_value}) => ALREADY IN DB')
 
-    # otherwise return all credentials
-    else:
-        cur.execute("SELECT * FROM credz")
+        except Exception as ex:
+            self.logging.error(f"Exception in add_cookie 4")
+            self.logging.debug(ex)
 
-    results = cur.fetchall()
-    cur.close()
-    return results
+        return None
 
 
-def add_group(self, domain, name):
-    domain = domain.split('.')[0].upper()
-    cur = self.conn.cursor()
+    def get_credz_old(self, filterTerm=None, credz_type=None):
+        """
+        Return credentials from the database.
+        """
 
-    cur.execute("SELECT * FROM groups WHERE LOWER(domain)=LOWER(?) AND LOWER(name)=LOWER(?)", [domain, name])
-    results = cur.fetchall()
+        cur = self.conn.cursor()
 
-    if not len(results):
-        cur.execute("INSERT INTO groups (domain, name) VALUES (?,?)", [domain, name])
+        if credz_type:
+            cur.execute(f"SELECT * FROM credz WHERE credtype='{credz_type}'")
 
-    cur.close()
+        # if we're filtering by username
+        elif filterTerm and filterTerm != '':
+            cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
 
-    self.logging.debug('add_group(domain={}, name={}) => {}'.format(domain, name, cur.lastrowid))
+        # otherwise return all credentials
+        else:
+            cur.execute("SELECT * FROM credz")
 
-    return cur.lastrowid
+        results = cur.fetchall()
+        cur.close()
+        return results
 
 
-def add_admin_user(self, credtype, domain, username, password, host, userid=None):
-    domain = domain.split('.')[0].upper()
-    cur = self.conn.cursor()
+    def add_group(self, domain, name):
+        domain = domain.split('.')[0].upper()
+        cur = self.conn.cursor()
 
-    if userid:
-        cur.execute("SELECT * FROM users WHERE id=?", [userid])
-        users = cur.fetchall()
-    else:
-        cur.execute(
-            "SELECT * FROM users WHERE credtype=? AND LOWER(domain)=LOWER(?) AND LOWER(username)=LOWER(?) AND password=?",
-            [credtype, domain, username, password])
-        users = cur.fetchall()
+        cur.execute("SELECT * FROM groups WHERE LOWER(domain)=LOWER(?) AND LOWER(name)=LOWER(?)", [domain, name])
+        results = cur.fetchall()
 
-    cur.execute('SELECT * FROM computers WHERE ip LIKE ?', [host])
-    hosts = cur.fetchall()
+        if not len(results):
+            cur.execute("INSERT INTO groups (domain, name) VALUES (?,?)", [domain, name])
 
-    if len(users) and len(hosts):
-        for user, host in zip(users, hosts):
-            userid = user[0]
-            hostid = host[0]
+        cur.close()
 
-            # Check to see if we already added this link
-            cur.execute("SELECT * FROM admin_relations WHERE userid=? AND computerid=?", [userid, hostid])
-            links = cur.fetchall()
+        self.logging.debug('add_group(domain={}, name={}) => {}'.format(domain, name, cur.lastrowid))
 
-            if not len(links):
-                cur.execute("INSERT INTO admin_relations (userid, computerid) VALUES (?,?)", [userid, hostid])
+        return cur.lastrowid
 
-    cur.close()
 
+    def add_admin_user(self, credtype, domain, username, password, host, userid=None):
+        domain = domain.split('.')[0].upper()
+        cur = self.conn.cursor()
+
+        if userid:
+            cur.execute("SELECT * FROM users WHERE id=?", [userid])
+            users = cur.fetchall()
+        else:
+            cur.execute(
+                "SELECT * FROM users WHERE credtype=? AND LOWER(domain)=LOWER(?) AND LOWER(username)=LOWER(?) AND password=?",
+                [credtype, domain, username, password])
+            users = cur.fetchall()
+
+        cur.execute('SELECT * FROM computers WHERE ip LIKE ?', [host])
+        hosts = cur.fetchall()
+
+        if len(users) and len(hosts):
+            for user, host in zip(users, hosts):
+                userid = user[0]
+                hostid = host[0]
+
+                # Check to see if we already added this link
+                cur.execute("SELECT * FROM admin_relations WHERE userid=? AND computerid=?", [userid, hostid])
+                links = cur.fetchall()
 
-def get_admin_relations(self, userID=None, hostID=None):
-    cur = self.conn.cursor()
+                if not len(links):
+                    cur.execute("INSERT INTO admin_relations (userid, computerid) VALUES (?,?)", [userid, hostid])
 
-    if userID:
-        cur.execute("SELECT * FROM admin_relations WHERE userid=?", [userID])
+        cur.close()
 
-    elif hostID:
-        cur.execute("SELECT * FROM admin_relations WHERE computerid=?", [hostID])
 
-    results = cur.fetchall()
-    cur.close()
+    def get_admin_relations(self, userID=None, hostID=None):
+        cur = self.conn.cursor()
 
-    return results
+        if userID:
+            cur.execute("SELECT * FROM admin_relations WHERE userid=?", [userID])
 
+        elif hostID:
+            cur.execute("SELECT * FROM admin_relations WHERE computerid=?", [hostID])
 
-def get_group_relations(self, userID=None, groupID=None):
-    cur = self.conn.cursor()
+        results = cur.fetchall()
+        cur.close()
 
-    if userID and groupID:
-        cur.execute("SELECT * FROM group_relations WHERE userid=? and groupid=?", [userID, groupID])
+        return results
 
-    elif userID:
-        cur.execute("SELECT * FROM group_relations WHERE userid=?", [userID])
 
-    elif groupID:
-        cur.execute("SELECT * FROM group_relations WHERE groupid=?", [groupID])
+    def get_group_relations(self, userID=None, groupID=None):
+        cur = self.conn.cursor()
 
-    results = cur.fetchall()
-    cur.close()
+        if userID and groupID:
+            cur.execute("SELECT * FROM group_relations WHERE userid=? and groupid=?", [userID, groupID])
 
-    return results
+        elif userID:
+            cur.execute("SELECT * FROM group_relations WHERE userid=?", [userID])
 
+        elif groupID:
+            cur.execute("SELECT * FROM group_relations WHERE groupid=?", [groupID])
 
-def remove_admin_relation(self, userIDs=None, hostIDs=None):
-    cur = self.conn.cursor()
+        results = cur.fetchall()
+        cur.close()
 
-    if userIDs:
-        for userID in userIDs:
-            cur.execute("DELETE FROM admin_relations WHERE userid=?", [userID])
+        return results
 
-    elif hostIDs:
-        for hostID in hostIDs:
-            cur.execute("DELETE FROM admin_relations WHERE hostid=?", [hostID])
 
-    cur.close()
+    def remove_admin_relation(self, userIDs=None, hostIDs=None):
+        cur = self.conn.cursor()
 
+        if userIDs:
+            for userID in userIDs:
+                cur.execute("DELETE FROM admin_relations WHERE userid=?", [userID])
 
-def remove_group_relations(self, userID=None, groupID=None):
-    cur = self.conn.cursor()
+        elif hostIDs:
+            for hostID in hostIDs:
+                cur.execute("DELETE FROM admin_relations WHERE hostid=?", [hostID])
 
-    if userID:
-        cur.execute("DELETE FROM group_relations WHERE userid=?", [userID])
+        cur.close()
 
-    elif groupID:
-        cur.execute("DELETE FROM group_relations WHERE groupid=?", [groupID])
 
-    results = cur.fetchall()
-    cur.close()
+    def remove_group_relations(self, userID=None, groupID=None):
+        cur = self.conn.cursor()
 
-    return results
+        if userID:
+            cur.execute("DELETE FROM group_relations WHERE userid=?", [userID])
 
+        elif groupID:
+            cur.execute("DELETE FROM group_relations WHERE groupid=?", [groupID])
 
-def is_credential_valid(self, credentialID):
-    """
-    Check if this credential ID is valid.
-    """
-    cur = self.conn.cursor()
-    cur.execute('SELECT * FROM users WHERE id=? AND password IS NOT NULL LIMIT 1', [credentialID])
-    results = cur.fetchall()
-    cur.close()
-    return len(results) > 0
+        results = cur.fetchall()
+        cur.close()
 
+        return results
 
-def is_credential_local(self, credentialID):
-    cur = self.conn.cursor()
-    cur.execute('SELECT domain FROM users WHERE id=?', [credentialID])
-    user_domain = cur.fetchall()
 
-    if user_domain:
-        cur.execute('SELECT * FROM computers WHERE LOWER(hostname)=LOWER(?)', [user_domain])
+    def is_credential_valid(self, credentialID):
+        """
+        Check if this credential ID is valid.
+        """
+        cur = self.conn.cursor()
+        cur.execute('SELECT * FROM users WHERE id=? AND password IS NOT NULL LIMIT 1', [credentialID])
         results = cur.fetchall()
         cur.close()
         return len(results) > 0
 
 
-def get_credentials(self, filterTerm=None, credtype=None):
-    """
-    Return credentials from the database.
-    """
-
-    cur = self.conn.cursor()
+    def is_credential_local(self, credentialID):
+        cur = self.conn.cursor()
+        cur.execute('SELECT domain FROM users WHERE id=?', [credentialID])
+        user_domain = cur.fetchall()
 
-    # if we're returning a single credential by ID
-    if self.is_credential_valid(filterTerm):
-        cur.execute("SELECT * FROM users WHERE id=?", [filterTerm])
-
-    elif credtype:
-        cur.execute("SELECT * FROM users WHERE credtype=?", [credtype])
-
-    # if we're filtering by username
-    elif filterTerm and filterTerm != '':
-        cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
+        if user_domain:
+            cur.execute('SELECT * FROM computers WHERE LOWER(hostname)=LOWER(?)', [user_domain])
+            results = cur.fetchall()
+            cur.close()
+            return len(results) > 0
 
-    # otherwise return all credentials
-    else:
-        cur.execute("SELECT * FROM users")
 
-    results = cur.fetchall()
-    cur.close()
-    return results
+    def get_credentials(self, filterTerm=None, credtype=None):
+        """
+        Return credentials from the database.
+        """
 
+        cur = self.conn.cursor()
 
-def is_user_valid(self, userID):
-    """
-    Check if this User ID is valid.
-    """
-    cur = self.conn.cursor()
-    cur.execute('SELECT * FROM users WHERE id=? LIMIT 1', [userID])
-    results = cur.fetchall()
-    cur.close()
-    return len(results) > 0
+        # if we're returning a single credential by ID
+        if self.is_credential_valid(filterTerm):
+            cur.execute("SELECT * FROM users WHERE id=?", [filterTerm])
 
+        elif credtype:
+            cur.execute("SELECT * FROM users WHERE credtype=?", [credtype])
 
-def get_users(self, filterTerm=None):
-    cur = self.conn.cursor()
+        # if we're filtering by username
+        elif filterTerm and filterTerm != '':
+            cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
 
-    if self.is_user_valid(filterTerm):
-        cur.execute("SELECT * FROM users WHERE id=? LIMIT 1", [filterTerm])
+        # otherwise return all credentials
+        else:
+            cur.execute("SELECT * FROM users")
 
-    # if we're filtering by username
-    elif filterTerm and filterTerm != '':
-        cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
+        results = cur.fetchall()
+        cur.close()
+        return results
 
-    else:
-        cur.execute("SELECT * FROM users")
 
-    results = cur.fetchall()
-    cur.close()
-    return results
+    def is_user_valid(self, userID):
+        """
+        Check if this User ID is valid.
+        """
+        cur = self.conn.cursor()
+        cur.execute('SELECT * FROM users WHERE id=? LIMIT 1', [userID])
+        results = cur.fetchall()
+        cur.close()
+        return len(results) > 0
 
 
-def is_computer_valid(self, hostID):
-    """
-    Check if this host ID is valid.
-    """
-    cur = self.conn.cursor()
-    cur.execute('SELECT * FROM computers WHERE id=? LIMIT 1', [hostID])
-    results = cur.fetchall()
-    cur.close()
-    return len(results) > 0
+    def get_users(self, filterTerm=None):
+        cur = self.conn.cursor()
 
+        if self.is_user_valid(filterTerm):
+            cur.execute("SELECT * FROM users WHERE id=? LIMIT 1", [filterTerm])
 
-def get_computers(self, filterTerm=None, domain=None):
-    """
-    Return hosts from the database.
-    """
+        # if we're filtering by username
+        elif filterTerm and filterTerm != '':
+            cur.execute("SELECT * FROM users WHERE LOWER(username) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
 
-    cur = self.conn.cursor()
+        else:
+            cur.execute("SELECT * FROM users")
 
-    # if we're returning a single host by ID
-    if self.is_computer_valid(filterTerm):
-        cur.execute("SELECT * FROM computers WHERE id=? LIMIT 1", [filterTerm])
+        results = cur.fetchall()
+        cur.close()
+        return results
 
-    # if we're filtering by domain controllers
-    elif filterTerm == 'dc':
-        if domain:
-            cur.execute("SELECT * FROM computers WHERE dc=1 AND LOWER(domain)=LOWER(?)", [domain])
-        else:
-            cur.execute("SELECT * FROM computers WHERE dc=1")
 
-    # if we're filtering by ip/hostname
-    elif filterTerm and filterTerm != "":
-        cur.execute("SELECT * FROM computers WHERE ip LIKE ? OR LOWER(hostname) LIKE LOWER(?)",
-                    ['%{}%'.format(filterTerm), '%{}%'.format(filterTerm)])
+    def is_computer_valid(self, hostID):
+        """
+        Check if this host ID is valid.
+        """
+        cur = self.conn.cursor()
+        cur.execute('SELECT * FROM computers WHERE id=? LIMIT 1', [hostID])
+        results = cur.fetchall()
+        cur.close()
+        return len(results) > 0
 
-    # otherwise return all computers
-    else:
-        cur.execute("SELECT * FROM computers")
 
-    results = cur.fetchall()
-    cur.close()
-    return results
+    def get_computers(self, filterTerm=None, domain=None):
+        """
+        Return hosts from the database.
+        """
+
+        cur = self.conn.cursor()
+
+        # if we're returning a single host by ID
+        if self.is_computer_valid(filterTerm):
+            cur.execute("SELECT * FROM computers WHERE id=? LIMIT 1", [filterTerm])
+
+        # if we're filtering by domain controllers
+        elif filterTerm == 'dc':
+            if domain:
+                cur.execute("SELECT * FROM computers WHERE dc=1 AND LOWER(domain)=LOWER(?)", [domain])
+            else:
+                cur.execute("SELECT * FROM computers WHERE dc=1")
 
+        # if we're filtering by ip/hostname
+        elif filterTerm and filterTerm != "":
+            cur.execute("SELECT * FROM computers WHERE ip LIKE ? OR LOWER(hostname) LIKE LOWER(?)",
+                        ['%{}%'.format(filterTerm), '%{}%'.format(filterTerm)])
 
-def get_domain_controllers(self, domain=None):
-    return self.get_computers(filterTerm='dc', domain=domain)
+        # otherwise return all computers
+        else:
+            cur.execute("SELECT * FROM computers")
 
+        results = cur.fetchall()
+        cur.close()
+        return results
 
-def is_group_valid(self, groupID):
-    """
-    Check if this group ID is valid.
-    """
-    cur = self.conn.cursor()
-    cur.execute('SELECT * FROM groups WHERE id=? LIMIT 1', [groupID])
-    results = cur.fetchall()
-    cur.close()
 
-    self.logging.debug('is_group_valid(groupID={}) => {}'.format(groupID, True if len(results) else False))
-    return len(results) > 0
+    def get_domain_controllers(self, domain=None):
+        return self.get_computers(filterTerm='dc', domain=domain)
 
 
-def get_groups(self, filterTerm=None, groupName=None, groupDomain=None):
-    """
-    Return groups from the database
-    """
-    if groupDomain:
-        groupDomain = groupDomain.split('.')[0].upper()
+    def is_group_valid(self, groupID):
+        """
+        Check if this group ID is valid.
+        """
+        cur = self.conn.cursor()
+        cur.execute('SELECT * FROM groups WHERE id=? LIMIT 1', [groupID])
+        results = cur.fetchall()
+        cur.close()
 
-    cur = self.conn.cursor()
+        self.logging.debug('is_group_valid(groupID={}) => {}'.format(groupID, True if len(results) else False))
+        return len(results) > 0
 
-    if self.is_group_valid(filterTerm):
-        cur.execute("SELECT * FROM groups WHERE id=? LIMIT 1", [filterTerm])
 
-    elif groupName and groupDomain:
-        cur.execute("SELECT * FROM groups WHERE LOWER(name)=LOWER(?) AND LOWER(domain)=LOWER(?)",
-                    [groupName, groupDomain])
+    def get_groups(self, filterTerm=None, groupName=None, groupDomain=None):
+        """
+        Return groups from the database
+        """
+        if groupDomain:
+            groupDomain = groupDomain.split('.')[0].upper()
+
+        cur = self.conn.cursor()
+
+        if self.is_group_valid(filterTerm):
+            cur.execute("SELECT * FROM groups WHERE id=? LIMIT 1", [filterTerm])
+
+        elif groupName and groupDomain:
+            cur.execute("SELECT * FROM groups WHERE LOWER(name)=LOWER(?) AND LOWER(domain)=LOWER(?)",
+                        [groupName, groupDomain])
 
-    elif filterTerm and filterTerm != "":
-        cur.execute("SELECT * FROM groups WHERE LOWER(name) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
+        elif filterTerm and filterTerm != "":
+            cur.execute("SELECT * FROM groups WHERE LOWER(name) LIKE LOWER(?)", ['%{}%'.format(filterTerm)])
 
-    else:
-        cur.execute("SELECT * FROM groups")
+        else:
+            cur.execute("SELECT * FROM groups")
 
-    results = cur.fetchall()
-    cur.close()
-    self.logging.debug(
-        'get_groups(filterTerm={}, groupName={}, groupDomain={}) => {}'.format(filterTerm, groupName, groupDomain,
-                                                                               results))
-    return results
+        results = cur.fetchall()
+        cur.close()
+        self.logging.debug(
+            'get_groups(filterTerm={}, groupName={}, groupDomain={}) => {}'.format(filterTerm, groupName, groupDomain,
+                                                                                results))
+        return results
```

### Comparing `donpapi-1.0.0/donpapi/entry.py` & `donpapi-1.0.1/donpapi/entry.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/blob.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/blob.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/credfile.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credfile.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/credhist.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/credhist.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/crypto.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/eater.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/masterkey.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/masterkey.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/system.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/system.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/DPAPI/vault.py` & `donpapi-1.0.1/donpapi/lazagne/config/DPAPI/vault.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/change_privileges.py` & `donpapi-1.0.1/donpapi/lazagne/config/change_privileges.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/constant.py` & `donpapi-1.0.1/donpapi/lazagne/config/constant.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/pyDes.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyDes.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/__init__.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/aes.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/aes.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/blockfeeder.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/pyaes/util.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/pyaes/util.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/crypto/rc4.py` & `donpapi-1.0.1/donpapi/lazagne/config/crypto/rc4.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/dico.py` & `donpapi-1.0.1/donpapi/lazagne/config/dico.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/dpapi_structure.py` & `donpapi-1.0.1/donpapi/lazagne/config/dpapi_structure.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/execute_cmd.py` & `donpapi-1.0.1/donpapi/lazagne/config/execute_cmd.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/Address.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Address.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/BaseProcess.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/BaseProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/LinProcess.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/LinProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/Locator.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/Locator.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/MemWorker.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/MemWorker.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/OSXProcess.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/OSXProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/SunProcess.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/SunProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/WinProcess.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinProcess.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/WinStructures.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/WinStructures.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/__init__.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/utils.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/utils.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/lib/memorpy/wintools.py` & `donpapi-1.0.1/donpapi/lazagne/config/lib/memorpy/wintools.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/manage_modules.py` & `donpapi-1.0.1/donpapi/lazagne/config/manage_modules.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/module_info.py` & `donpapi-1.0.1/donpapi/lazagne/config/module_info.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/run.py` & `donpapi-1.0.1/donpapi/lazagne/config/run.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/users.py` & `donpapi-1.0.1/donpapi/lazagne/config/users.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/winstructure.py` & `donpapi-1.0.1/donpapi/lazagne/config/winstructure.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/config/write_output.py` & `donpapi-1.0.1/donpapi/lazagne/config/write_output.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/browsers/chromium_based.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/chromium_based.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/browsers/ie.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ie.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/browsers/mozilla.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/mozilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/browsers/ucbrowser.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/browsers/ucbrowser.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/chats/pidgin.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/chats/pidgin.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/chats/psi.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/chats/psi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/chats/skype.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/chats/skype.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/databases/dbvis.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/databases/dbvis.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/databases/postgresql.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/databases/postgresql.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/databases/robomongo.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/databases/robomongo.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/databases/sqldeveloper.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/databases/sqldeveloper.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/databases/squirrel.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/databases/squirrel.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/games/galconfusion.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/games/galconfusion.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/games/kalypsomedia.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/games/kalypsomedia.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/games/roguestale.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/games/roguestale.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/games/turba.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/games/turba.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/git/gitforwindows.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/git/gitforwindows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/mails/outlook.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/mails/outlook.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/maven/mavenrepositories.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/maven/mavenrepositories.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/keepass.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/keepass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/keethief.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/keethief.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/__init__.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/__init__.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/common.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/common.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/crypto.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/hbio.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/hbio.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/kdb4.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/libkeepass/pureSalsa20.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/memory/memorydump.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/memory/memorydump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/multimedia/eyecon.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/multimedia/eyecon.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/php/composer.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/php/composer.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/svn/tortoise.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/svn/tortoise.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/apachedirectorystudio.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/coreftp.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/coreftp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/cyberduck.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/cyberduck.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/d3des.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/d3des.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/filezilla.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/filezillaserver.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/filezillaserver.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/ftpnavigator.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/iisapppool.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iisapppool.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/iiscentralcertp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/keepassconfig.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/keepassconfig.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/opensshforwindows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/openvpn.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/openvpn.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/puttycm.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/puttycm.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/rdpmanager.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/rdpmanager.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/unattended.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/unattended.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/vnc.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/vnc.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/winscp.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/winscp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/sysadmin/wsl.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/sysadmin/wsl.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/wifi/wifi.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/wifi/wifi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/autologon.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/autologon.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/cachedump.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/cachedump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/addrspace.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/addrspace.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/newobj.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/newobj.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/object.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/object.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/types.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/types.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/domcachedump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/hashdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/lsasecrets.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/creddump7/win32/rawreg.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/credfiles.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/credfiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/credman.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/credman.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/hashdump.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/hashdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/lsa_secrets.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/lsa_secrets.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/ppypykatz.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/ppypykatz.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/vault.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/vault.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/vaultfiles.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/vaultfiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lazagne/softwares/windows/windows.py` & `donpapi-1.0.1/donpapi/lazagne/softwares/windows/windows.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/RecentFiles.py` & `donpapi-1.0.1/donpapi/lib/RecentFiles.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/adconnect.py` & `donpapi-1.0.1/donpapi/lib/adconnect.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/certificates.py` & `donpapi-1.0.1/donpapi/lib/certificates.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/compliance_security.py` & `donpapi-1.0.1/donpapi/lib/compliance_security.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/defines.py` & `donpapi-1.0.1/donpapi/lib/defines.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/dpapi.py` & `donpapi-1.0.1/donpapi/lib/dpapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,17 +154,17 @@
 		try:
 			if len(pwdhash) == 20:
 				# SHA1
 				key1 = HMAC.new(pwdhash, (sid + '\0').encode('utf-16le'), SHA1).digest()
 				key2 = None
 			else:
 				# Assume MD4
-				key1 = HMAC.new(pwdhash, (sid + '\0').encode('utf-16le'), SHA1).digest()
+				key1 = HMAC.new(pwdhash.encode('utf-16le'), (sid + '\0').encode('utf-16le'), SHA1).digest()
 				# For Protected users
-				tmpKey = pbkdf2_hmac('sha256', pwdhash, sid.encode('utf-16le'), 10000)
+				tmpKey = pbkdf2_hmac('sha256', pwdhash.encode('utf-16le'), sid.encode('utf-16le'), 10000)
 				tmpKey2 = pbkdf2_hmac('sha256', tmpKey, sid.encode('utf-16le'), 1)[:16]
 				key2 = HMAC.new(tmpKey2, (sid + '\0').encode('utf-16le'), SHA1).digest()[:20]
 		except Exception as e:
 			self.logging.error(f"derivekey exception : {str(e)}")
 		return key1, key2
```

### Comparing `donpapi-1.0.0/donpapi/lib/dpapi_pick/credhist.py` & `donpapi-1.0.1/donpapi/lib/dpapi_pick/credhist.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/dpapi_pick/crypto.py` & `donpapi-1.0.1/donpapi/lib/dpapi_pick/crypto.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/dpapi_pick/eater.py` & `donpapi-1.0.1/donpapi/lib/dpapi_pick/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/eater.py` & `donpapi-1.0.1/donpapi/lib/eater.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/fileops.py` & `donpapi-1.0.1/donpapi/lib/fileops.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/neo4jconnection.py` & `donpapi-1.0.1/donpapi/lib/neo4jconnection.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/new_module.py` & `donpapi-1.0.1/donpapi/lib/new_module.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/reg.py` & `donpapi-1.0.1/donpapi/lib/reg.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/secretsdump.py` & `donpapi-1.0.1/donpapi/lib/secretsdump.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/toolbox.py` & `donpapi-1.0.1/donpapi/lib/toolbox.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/lib/wmi.py` & `donpapi-1.0.1/donpapi/lib/wmi.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/myseatbelt.py` & `donpapi-1.0.1/donpapi/myseatbelt.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/myusers.py` & `donpapi-1.0.1/donpapi/myusers.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/res/Logo_LOGIN.PNG` & `donpapi-1.0.1/donpapi/res/Logo_LOGIN.PNG`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/res/style.css` & `donpapi-1.0.1/donpapi/res/style.css`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/browser/chrome_decrypt.py` & `donpapi-1.0.1/donpapi/software/browser/chrome_decrypt.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/browser/firefox_decrypt.py` & `donpapi-1.0.1/donpapi/software/browser/firefox_decrypt.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/browser/mozilla.py` & `donpapi-1.0.1/donpapi/software/browser/mozilla.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/manager/keepass.py` & `donpapi-1.0.1/donpapi/software/manager/keepass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/manager/lastpass.py` & `donpapi-1.0.1/donpapi/software/manager/lastpass.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/manager/mRemoteNG-local.py` & `donpapi-1.0.1/donpapi/software/manager/mRemoteNG-local.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/manager/mRemoteNG.py` & `donpapi-1.0.1/donpapi/software/manager/mRemoteNG.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/d3des.py` & `donpapi-1.0.1/donpapi/software/sysadmin/d3des.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/mobaxterm.py` & `donpapi-1.0.1/donpapi/software/sysadmin/mobaxterm.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/putty.py` & `donpapi-1.0.1/donpapi/software/sysadmin/putty.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/vnc-local.py` & `donpapi-1.0.1/donpapi/software/sysadmin/vnc-local.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/vnc.py` & `donpapi-1.0.1/donpapi/software/sysadmin/vnc.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/donpapi/software/sysadmin/winscp.py` & `donpapi-1.0.1/donpapi/software/sysadmin/winscp.py`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/pyproject.toml` & `donpapi-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "donpapi"
-version = "1.0.0"
+version = "1.0.1"
 description = "Dumping revelant information on compromised targets without AV detection"
 authors = ["Login Securite <contact@login-securite.com>"]
 readme = "readme.md"
 homepage = "https://github.com/login-securite/DonPAPI"
 repository = "https://github.com/login-securite/DonPAPI"
 exclude = []
 include = ["donpapi/config/*", "donpapi/res/*"]
```

### Comparing `donpapi-1.0.0/readme.md` & `donpapi-1.0.1/readme.md`

 * *Files identical despite different names*

### Comparing `donpapi-1.0.0/PKG-INFO` & `donpapi-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donpapi
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dumping revelant information on compromised targets without AV detection
 Home-page: https://github.com/login-securite/DonPAPI
 Author: Login Securite
 Author-email: contact@login-securite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
```

