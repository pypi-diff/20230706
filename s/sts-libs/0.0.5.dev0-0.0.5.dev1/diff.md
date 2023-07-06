# Comparing `tmp/sts_libs-0.0.5.dev0.tar.gz` & `tmp/sts_libs-0.0.5.dev1.tar.gz`

## Comparing `sts_libs-0.0.5.dev0.tar` & `sts_libs-0.0.5.dev1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/__about__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/__init__.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/__init__.py
--rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/dm.py
--rw-r--r--   0        0        0    42311 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/dmpd.py
--rw-r--r--   0        0        0    17423 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/fc.py
--rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/fio.py
--rw-r--r--   0        0        0    49941 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/iscsi.py
--rw-r--r--   0        0        0    47069 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/linux.py
--rw-r--r--   0        0        0    66802 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lio.py
--rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/loopdev.py
--rw-r--r--   0        0        0    36092 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lsm.py
--rw-r--r--   0        0        0    36659 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/lvm.py
--rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/md.py
--rw-r--r--   0        0        0    42761 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/mp.py
--rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/net.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/qemu_img.py
--rw-r--r--   0        0        0    29049 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi.py
--rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi_debug.py
--rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/stratis.py
--rw-r--r--   0        0        0    23144 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/vdo.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/__init__.py
--rw-r--r--   0        0        0     6081 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/atomic_run.py
--rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/beaker.py
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cli_tools.py
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cmdline.py
--rw-r--r--   0        0        0    12501 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/logchecker.py
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/persistent_vars.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/restraint.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/size.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/tmt.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/__init__.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/cmdline_test.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/fio_test.py
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/iscsi_test.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/linux_test.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/logchecker_test.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/loopdev_test.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/lvm_test.py
--rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/md_test.py
--rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/net_test.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/persistent_vars_test.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/tests/scsi_test.py
--rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/LICENSE
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/pyproject.toml
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/sts_libs/README.md
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/__init__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/__init__.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/__about__.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/__init__.py
+-rw-r--r--   0        0        0    20700 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/dm.py
+-rw-r--r--   0        0        0    42305 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/dmpd.py
+-rw-r--r--   0        0        0    17423 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/fc.py
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/fio.py
+-rw-r--r--   0        0        0    50253 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/iscsi.py
+-rw-r--r--   0        0        0    46948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/linux.py
+-rw-r--r--   0        0        0    66740 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/lio.py
+-rw-r--r--   0        0        0     6836 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/loopdev.py
+-rw-r--r--   0        0        0    36092 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/lsm.py
+-rw-r--r--   0        0        0    36657 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/lvm.py
+-rw-r--r--   0        0        0     6194 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/md.py
+-rw-r--r--   0        0        0    42709 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/mp.py
+-rw-r--r--   0        0        0    18789 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/net.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/qemu_img.py
+-rw-r--r--   0        0        0    28690 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/scsi.py
+-rw-r--r--   0        0        0     4102 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/scsi_debug.py
+-rw-r--r--   0        0        0    17167 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/stratis.py
+-rw-r--r--   0        0        0    23142 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/vdo.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/__init__.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/atomic_run.py
+-rw-r--r--   0        0        0     3915 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/beaker.py
+-rw-r--r--   0        0        0     4501 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/cli_tools.py
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/cmdline.py
+-rw-r--r--   0        0        0    12491 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/logchecker.py
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/persistent_vars.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/restraint.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/size.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/tmt.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/__init__.py
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/cmdline_test.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/fio_test.py
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/iscsi_test.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/linux_test.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/logchecker_test.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/loopdev_test.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/lvm_test.py
+-rw-r--r--   0        0        0     4495 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/md_test.py
+-rw-r--r--   0        0        0     3987 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/net_test.py
+-rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/persistent_vars_test.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/tests/scsi_test.py
+-rw-r--r--   0        0        0     2021 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/LICENSE
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/pyproject.toml
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/sts_libs/README.md
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 sts_libs-0.0.5.dev1/PKG-INFO
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/dm.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/dm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/dmpd.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/dmpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -906,15 +906,15 @@
             print("FAIL: Source file is not a file.")
             return False
         device = source_file
 
     regions = region.split(".")
     try:
         int(regions[0])
-        if regions[1] != "":
+        if regions[1]:
             raise ValueError  # noqa: TRY301
         int(regions[2])
         if regions[3] is not None:
             raise ValueError  # noqa: TRY301
     except ValueError:
         print("FAIL: Region must be in format 'INT..INT'")
         return False
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/fc.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/fc.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/fio.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/fio.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/iscsi.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/iscsi.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,107 +152,166 @@
 
     def iface_update_ip(self, iface: str, ip: str) -> StsCompletedProcess:
         return self.iface_update(iface=iface, name="iface.ipaddress", value=ip)
 
     def discovery(
         self,
         portal: str,
-        discovery_type: str = "st",
-        iface: Optional[str] = None,
+        type: str = "st",
+        interface: Optional[str] = None,
         **kwargs: str,
     ) -> StsCompletedProcess:
-        arguments = {"-t": discovery_type, "-p": portal, **kwargs}
-        if iface:
-            arguments.update({"-I": iface})
+        arguments = {"-t": type, "-p": portal, **kwargs}
+        if interface:
+            arguments.update({"-I": interface})
         return self._run(mode="discovery", arguments=arguments)
 
     def node(self, **kwargs: Union[str, Optional[str]]) -> StsCompletedProcess:
         return self._run(mode="node", arguments={**kwargs})
 
     def node_login(self, **kwargs: str) -> StsCompletedProcess:
         arguments = {"--login": None, **kwargs}
         return self.node(**arguments)
 
     def node_logout(self, **kwargs: str) -> StsCompletedProcess:
         arguments = {"--logout": None, **kwargs}
         return self.node(**arguments)
 
 
-def get_env_vars() -> dict:
-    """Parse general environmental variables needed for iscsi initiator
-    Accepts following env vars:
-    'ISCSI_INITIATORNAME': str
-    'ISCSI_TARGET': str
-    'ISCSI_IFACES': list[dict]
-    returns dict of all found variables.
-    """
-    vars_to_return: dict = {}
-    iqn_in_iface_vars = False
-    initiatorname: Optional[str] = getenv("ISCSI_INITIATORNAME")
-    if initiatorname:
-        vars_to_return.update({"initiatorname": initiatorname})
-        print(f"INFO: Detected initiatorname: {initiatorname}")
-
-    target_portal: Optional[str] = getenv("ISCSI_TARGET")
-    if target_portal:
-        vars_to_return.update({"target_portal": target_portal})
-        print(f"INFO: Detected target portal: {target_portal}")
-
-    iface_data: Optional[str] = getenv("ISCSI_IFACES")
-    if iface_data:
-        iqn_in_iface_vars = True  # Setting back to False below, in case at least one iface does not have iqn
-        ifaces: List[dict] = literal_eval(iface_data)
-        vars_to_return.update({"ifaces": ifaces})
-        print("INFO: Detected ifaces:")
-        for iface_dict in ifaces:
-            print(iface_dict)
-            if "iqn" not in iface_dict:
-                iqn_in_iface_vars = False
-
-    # Check if we have necessary initiator iqns
-    if not initiatorname and not iqn_in_iface_vars:
-        print("WARN: No iSCSI initiator iqn specified")
+class ConfVars(TypedDict):
+    initiatorname: str  # iqn.1994-05.redhat:example
+    targets: List[TargetVars]
+    ifaces: List[IfaceVars]
+
+
+class IfaceVars(TypedDict):
+    hwaddress: str
+    iscsi_ifacename: str
+    net_ifacename: str
+    transport_name: str
+    initiatorname: str
+    isid: str
+    bootproto: str
+    ipaddress: str
+    prefix_len: str
+    subnet_mask: str
+    gateway: str
+    primary_dns: str
+    secondary_dns: str
+    vlan_id: str
+    vlan_priority: str
+    vlan_state: str
+    ipv6_linklocal: str
+    ipv6_router: str
+    ipv6_autocfg: str
+    linklocal_autocfg: str
+    router_autocfg: str
+    state: str
+    iface_num: str
+    mtu: str
+    port: str
+    delayed_ack: str
+    tcp_nagle: str
+    tcp_wsf_state: str
+    tcp_wsf: str
+    tcp_timer_scale: str
+    tcp_timestamp: str
+    dhcp_dns: str
+    dhcp_slp_da: str
+    tos_state: str
+    tos: str
+    gratuitous_arp: str
+    dhcp_alt_client_id_state: str
+    dhcp_alt_client_id: str
+    dhcp_req_vendor_id_state: str
+    dhcp_vendor_id_state: str
+    dhcp_vendor_id: str
+    dhcp_learn_iqn: str
+    fragmentation: str
+    incoming_forwarding: str
+    ttl: str
+    gratuitous_neighbor_adv: str
+    redirect: str
+    ignore_icmp_echo_request: str
+    mld: str
+    flow_label: str
+    traffic_class: str
+    hop_limit: str
+    nd_reachable_tmo: str
+    nd_rexmit_time: str
+    nd_stale_tmo: str
+    dup_addr_detect_cnt: str
+    router_adv_link_mtu: str
+    def_task_mgmt_timeout: str
+    header_digest: str
+    data_digest: str
+    immediate_data: str
+    initial_r2t: str
+    data_seq_inorder: str
+    data_pdu_inorder: str
+    erl: str
+    max_receive_data_len: str
+    first_burst_len: str
+    max_outstanding_r2t: str
+    max_burst_len: str
+    chap_auth: str
+    bidi_chap: str
+    strict_login_compliance: str
+    discovery_auth: str
+    discovery_logout: str
+
+
+class TargetVars(TypedDict):
+    name: str  # iqn
+    interface: str
+    portal: str  # ip or hostname
+    type: str  # discovery type
+
+
+class AuthFields(TypedDict):
+    tbl_idx: str
+    authmethod: str
+    username: str
+    password: str
+    password_length: str
+    username_in: str
+    password_in: str
 
-    return vars_to_return
 
-
-def setup(env_vars: Optional[dict] = None, discover_targets: bool = False) -> bool:
+def setup(variables: ConfVars) -> bool:
     """Configure iSCSI initiator based on env variables."""
     iscsiadm = IscsiAdm(verbose=True)
-    if not env_vars:
-        env_vars = get_env_vars()
-    if "initiatorname" in env_vars:
-        if not set_initiatorname(env_vars["initiatorname"]):
+
+    if "initiatorname" in variables:
+        if not set_initiatorname(variables["initiatorname"]):
             return False
         linux.service_restart(ISCSID_SERVICE_NAME, verbose=False)
-    if "ifaces" in env_vars:
-        for iface in env_vars["ifaces"]:
-            ifacename = iface["iscsi_ifacename"]
+
+    if "ifaces" in variables:
+        for iface in variables["ifaces"]:
+            ifacename = iface["name"]
             if ("qedi" in ifacename or "bnx2i" in ifacename) and not linux.is_service_running(ISCSIUIO_SERVICE_NAME):
                 linux.service_enable(ISCSIUIO_SERVICE_NAME, now=True)
-            values_to_set: Optional[dict] = iface["setup"]
-            if not values_to_set:
-                continue
             if "hwaddress" in values_to_set:
                 create_iscsi_iface(iface_name=ifacename)
-            for n, v in values_to_set.items():
+            for n, v in iface.items():
+                if n == "ifacename":
+                    continue
                 completed_process = iscsiadm.iface_update(iface=ifacename, name=n, value=v)
                 ret = completed_process.returncode
                 out = completed_process.output
                 if ret != 0:
                     print(f"FAIL: iscsi update command returned {ret}. Output: {out}")
                     return False
-            if discover_targets:
-                iface_targets = iface["targets"]
-                for t in iface_targets:
-                    if not t["portal"]:
-                        print(f"FAIL: No portal specified for iSCSI discovery: {iface}")
-                        return False
-                    if iscsiadm.discovery(iface=ifacename, portal=t["portal"]) != 0:
-                        return False
+
+    if "targets" in variables:
+        for target in variables["targets"]:
+            if iscsiadm.discovery(**target) != 0:
+                return False
+
     if not linux.is_service_enabled(ISCSID_SERVICE_NAME):
         linux.service_enable(ISCSID_SERVICE_NAME)
     return True
 
 
 def discovery_login(iface_name, portal, iqn, iface_ip=None, subnet_mask=None, gateway=None) -> bool:  # noqa: ANN001
     if not iface_name or not portal or not iqn:
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/linux.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/linux.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,22 +346,16 @@
       equal: return value if packaged are equal version (default 'True').
     """
     pkg = package_version(package)
     if pkg is None:
         return None
     if any(True for x in pkg if not isinstance(x, int)):
         # cut ending of package name containing string, parse_version() does not work with ints and strings at once
-        pack = []
-        for p in pkg[:].split("."):
-            try:
-                int(p)
-            except ValueError:
-                break
-            pack.append(p)
-        pkg = ".".join(pack)
+        pack = [int(p) for p in pkg.split(".") if p.isdigit()]
+        pkg = ".".join(map(str, pack))
     if equal:
         return parse_version(version + "." + release) <= parse_version(pkg)
     return parse_version(version + "." + release) < parse_version(pkg)
 
 
 def wait_udev(sleeptime=15):  # noqa: ANN001, ANN201
     """Wait udev to finish. Often used after scsi rescan."""
@@ -966,15 +960,15 @@
     if only_direct:
         cmd = f"lsblk -nsl {child_device} -o KNAME | sed -n 2p"  # if no parent, returns nothing
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: run {cmd}")
         print(output)
         return None
-    if output == "" or output == child_device:
+    if not output or output == child_device:
         print("WARN: get_parent_device - device has no parent")
         return None
     return output
 
 
 def get_udev_property(device_name: str, property_key: str) -> Union[str, None]:
     """Given an /dev device name, returns specified property using udevadm.
@@ -1325,15 +1319,15 @@
     None: systemctl is not installed or timestamp does not exist
     """
     if not exists("systemctl"):
         cmd = f"systemctl show {service_name} --property=ActiveEnterTimestamp"
         ret, data = run_ret_out(cmd, return_output=True)
         if ret == 0:
             timestamp = data.split("=")
-            if timestamp[1] != "":
+            if timestamp[1]:
                 return timestamp[1]
             return None
         print(f"WARN: Could not get active enter timestamp of service: {service_name}")
     return None
 
 
 def get_system_logs(
@@ -1444,25 +1438,25 @@
     except OSError as e:
         print("FAIL: Unable to open {}. It might not exist")
         print(e)
         return False
 
     config.filename = file
     fail = False
-    for param in parameters_to_remove:
-        print(f'INFO: Removing "{param}" from {file}')
-        try:
+    try:
+        for param in parameters_to_remove:
+            print(f'INFO: Removing "{param}" from {file}')
             if section:
                 config[section].pop(param)
             else:
                 config.pop(param)
-        except KeyError:
-            if warn:
-                print("WARN: Parameter to remove is not in config")
-            fail = True
+    except KeyError:
+        if warn:
+            print("WARN: Parameter to remove is not in config")
+        fail = True
 
     config.write()
     if fail:
         return False
     return True
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/lio.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/lio.py`

 * *Files 0% similar despite different names*

```diff
@@ -876,15 +876,15 @@
     """
     cmd = f"targetcli /iscsi/{tgt_iqn}/tpg{tpg}/acls/{init_iqn} ls | grep {tgt_lun_id}"
     retcode, output = run_ret_out(cmd, return_output=True, verbose=False)
     if retcode != 0:
         print(f"FAIL: Could not get mapping for lun {tgt_lun_id} on iSCSI target {tgt_iqn}/{init_iqn}")
         return False
 
-    if output == "":
+    if not output:
         return False
     return True
 
 
 def lio_add_iscsi_target(  # noqa: ANN201
     tgt_iqn=None,  # noqa: ANN001
     init_iqn=None,  # noqa: ANN001
@@ -1818,21 +1818,21 @@
                         "lun": False,
                         "add_mapped_luns": False,
                     }
             else:
                 keys = {"wwn": False}
         else:
             keys = {"wwn": False}
-        for key in keys:
-            try:
+        try:
+            for key in keys:
                 cmd += f"{key}={kwargs[key]} "
-            except KeyError:
-                if not self.disable_check and keys[key]:
-                    print(f"FAIL: Create on path '{self.path}' requires argument {key}.")
-                    return 1
+        except KeyError:
+            if not self.disable_check and keys[key]:
+                print(f"FAIL: Create on path '{self.path}' requires argument {key}.")
+                return 1
         return self._run(cmd, **arguments)
 
     def delete(self, **kwargs):  # noqa: ANN003, ANN201
         keys = None
         cmd = "delete "
         arguments, kwargs = self._extract_args(kwargs)
         # the following ensures the ordering is correct in correct paths
@@ -1868,21 +1868,21 @@
                 if "luns" in self.path:
                     keys = {"lun": True}
             else:
                 keys = {"wwn": False}
         else:
             keys = {"wwn": True}
 
-        for key in keys:
-            try:
+        try:
+            for key in keys:
                 cmd += f"{key}={kwargs[key]} "
-            except KeyError:
-                if not self.disable_check and keys[key]:
-                    print(f"FAIL: Delete on path '{self.path}' requires argument {key}.")
-                    return 1
+        except KeyError:
+            if not self.disable_check and keys[key]:
+                print(f"FAIL: Delete on path '{self.path}' requires argument {key}.")
+                return 1
 
         return self._run(cmd, **arguments)
 
     def help(self, topic="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
         return self._run(f"help {topic}", **kwargs)
 
     def saveconfig(self, savefile=None, **kwargs):  # noqa: ANN001, ANN003, ANN201
@@ -1911,17 +1911,15 @@
     def get(self, group="", **kwargs):  # noqa: ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
         cmd = f"get {group} {' '.join(kwargs.keys())}"
         return self._run(cmd, **arguments)
 
     def set(self, group="", **kwargs):  # noqa: A003, ANN001, ANN003, ANN201
         arguments, kwargs = self._extract_args(kwargs)
-        params = [
-            f"{kwarg}='{kwargs[kwarg]}'" if kwargs[kwarg] != "" else f"{kwarg}='{kwargs[kwarg]}'" for kwarg in kwargs
-        ]
+        params = [f"{kwarg}='{kwargs[kwarg]}'" if kwargs[kwarg] else f"{kwarg}='{kwargs[kwarg]}'" for kwarg in kwargs]
         cmd = f"set {group} {' '.join(params)}"
         return self._run(cmd, **arguments)
 
     def info(self, **kwargs):  # noqa: ANN003, ANN201
         return self._run("info", **kwargs)
 
     def version(self, **kwargs):  # noqa: ANN003, ANN201
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/loopdev.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/loopdev.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/lsm.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/lsm.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/lvm.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/lvm.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     cmd = f"pvcreate {options} {pv_name}"
     if run(cmd, verbose=verbose).returncode != 0:
         # print ("FAIL: Could not create %s" % pv_name)
         return False
     return True
 
 
-def pv_remove(pv_name: str, force=None, verbose=True):  # noqa: ANN001, ANN201
+def pv_remove(pv_name: str, force=None, verbose=True) -> bool:  # noqa: ANN001
     """Delete a Volume Group.
     The arguments are:
     VG name
     force (boolean)
     verbose (boolean).
 
     Returns:
@@ -560,15 +560,15 @@
     """Get all the configuration types from lvm.conf file."""
     out = run("lvmconfig --type full", capture_output=True, verbose=False).output
 
     options = {}
     category = ""
     for line in out.split("\n"):
         line = line.strip()  # noqa: PLW2901
-        if line == "" or "}" in line:
+        if not line or "}" in line:
             # skip empty or end of list line
             continue
         if "{" in line:
             # category part
             category = line[:-2]  # removing "allocation {"[:-2] == "allocation"
             options[category] = []
         elif "=" in line:
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/md.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/md.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/mp.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/mp.py`

 * *Files 1% similar despite different names*

```diff
@@ -566,20 +566,19 @@
         print("FAIL: mpath_names_of_vendor() - requires vendor parameter")
         return None
 
     mp_devs = multipath_query_all()
     if not mp_devs:
         return None
 
-    mpaths = []
-    for mpath_info in list(mp_devs["by_mpath_name"].values()):
-        if "vendor" in list(mpath_info.keys()) and mpath_info["vendor"] == vendor:
-            mpaths.append(mpath_info["mpath_name"])
-
-    return mpaths
+    return [
+        mpath_info["mpath_name"]
+        for mpath_info in mp_devs["by_mpath_name"].values()
+        if "vendor" in mpath_info and mpath_info["vendor"] == vendor
+    ]
 
 
 def mpath_check_disk_status(mpath_name, scsi_disk):  # noqa: ANN001, ANN201
     """Check the online status of a specific SCSI disk from a mpath device."""
     if not mpath_name or not scsi_disk:
         print("FAIL: mpath_check_disk_status() - requires mpath_name and scsi_disk parameters")
         return None
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/net.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/net.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/qemu_img.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/qemu_img.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/scsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,19 +154,20 @@
     if not vendor:
         print("FAIL: get_scsi_name_by_vendor() - requires vendor parameter")
         return None
 
     all_scsi_disks_info = query_all_scsi_disks()
     if not all_scsi_disks_info:
         return None
-    scsi_names = []
-    for scsi_info in list(all_scsi_disks_info.values()):
-        if "vendor" in list(scsi_info.keys()) and scsi_info["vendor"] == vendor:
-            scsi_names.append(scsi_info["name"])
-    return scsi_names
+
+    return [
+        scsi_info["name"]
+        for scsi_info in all_scsi_disks_info.values()
+        if "vendor" in scsi_info and scsi_info["vendor"] == vendor
+    ]
 
 
 def scsi_host_of_scsi_name(scsi_name):  # noqa: ANN001, ANN201
     if not scsi_name:
         print("FAIL: scsi_host_of_scsi_name() - requires scsi_name parameter")
         return None
 
@@ -321,15 +322,15 @@
     scsi_drv_sysfs = f"/sys/class/scsi_host/host{host_id}/proc_name"
     if not Path(scsi_drv_sysfs).is_file():
         print(f"FAIL: {scsi_drv_sysfs} is not a valid path")
         return None
 
     output = run(f"cat {scsi_drv_sysfs}", capture_output=True, verbose=False).output
     scsi_driver = output
-    if scsi_driver == "(null)" or scsi_driver == "":
+    if not scsi_driver or scsi_driver == "(null)":
         # Driver information was not exported, let try to find it out some other way
         lpfc_sysfs_file = f"/sys/class/scsi_host/host{host_id}/lpfc_drvr_version"
         if Path(lpfc_sysfs_file).is_file():
             return "lpfc"
 
         driver_sysfs_file = f"/sys/class/scsi_host/host{host_id}/driver_name"
         if Path(driver_sysfs_file).is_file():
@@ -415,21 +416,15 @@
     If no host is given it will scan all SCSI hosts
     The arguments are:
     Host:      e.g. 1 for host1
     Returns:
     True if no problem executing command
     False if something went wrong.
     """
-    host_list = []
-    if host:
-        host_list = [host]
-    else:
-        scsi_hosts = get_hosts()
-        for host in scsi_hosts:
-            host_list.append(host)
+    host_list = [host] if host else list(get_hosts())
 
     error = 0
 
     if not host_list:
         print("WARN: No host found on server to rescan")
         return True
 
@@ -452,22 +447,15 @@
     If no disk is given, rescann all SCSI disks
     echo 1 > /sys/block/<scsi_disk>/device/rescan
     Host:      e.g. 1 for host1
     Returns:
     True if no problem executing command
     False if something went wrong.
     """
-    scsi_disks = []
-
-    if scsi_disk:
-        scsi_disks = [scsi_disk]
-    else:
-        ids = get_scsi_disk_ids()
-        for _id in ids:
-            scsi_disks.append(get_scsi_disk_name(_id))
+    scsi_disks = [scsi_disk] if scsi_disk else [get_scsi_disk_name(_id) for _id in get_scsi_disk_ids()]
 
     error = 0
     for scsi_disk in scsi_disks:
         cmd = f"echo 1 > /sys/block/{scsi_disk}/device/rescan"
         if run(cmd).returncode != 0:
             print(f"FAIL: Could not rescan {scsi_disk}")
             error += 1
@@ -552,17 +540,16 @@
 
     scsi_ids = []
     all_scsi_info = query_all_scsi_disks()
     if not all_scsi_info:
         # Could not find any SCSI device
         return None
 
-    for _id in list(all_scsi_info.keys()):
-        if all_scsi_info[_id]["wwid"] == wwid:
-            scsi_ids.append(_id)
+    scsi_ids = [_id for _id in all_scsi_info if all_scsi_info[_id]["wwid"] == wwid]
+
     if scsi_ids:
         scsi_ids = list(set(scsi_ids))  # dedup
     return scsi_ids
 
 
 def wwn_of_disk(scsi_disk):  # noqa: ANN001, ANN201
     """Usage
@@ -656,19 +643,16 @@
         return None
 
     all_scsi_host_ids = get_hosts()
     if not all_scsi_host_ids:
         print("FAIL: query_scsi_driver_info() - Host does not have any SCSI host")
         return None
 
-    driver_host_ids = []
     # Check which SCSI hosts are using the driver we want
-    for host_id in all_scsi_host_ids:
-        if scsi_driver_of_host_id(host_id) == driver:
-            driver_host_ids.append(host_id)
+    driver_host_ids = [host_id for host_id in all_scsi_host_ids if scsi_driver_of_host_id(host_id) == driver]
 
     if not driver_host_ids:
         print(f"FAIL:  No SCSI disk found from driver {driver}")
         return None
 
     scsi_driver_info = {"scsi_host": {}}
     for host_id in driver_host_ids:
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/scsi_debug.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/scsi_debug.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/stratis.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/stratis.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/vdo.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/vdo.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     status_old = [x for x in status_old.splitlines() if changed_var in x]
     status_new = [x for x in status_new.splitlines() if changed_var in x]
     print(f"Before: {', '.join(status_old)}")
     print(f"After:  {', '.join(status_new)}")
     diff = list(context_diff(status_old, status_new))
     difference = "\n".join([x for x in diff if x.startswith("!")])
 
-    if difference == "":
+    if not difference:
         error = f"WARN: Modifying VDO to {changed_argument} did nothing."
         print(error)
         errors.append(error)
 
 
 def minimum_slab_size(device, default_to_2g=True):  # noqa: ANN001, ANN201
     def _get_raid_device(device):  # noqa: ANN001, ANN202
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/atomic_run.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/atomic_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,20 +108,19 @@
     if isinstance(success, bool):
         success = switcher[success]
 
     # match expected_ret to success in case we do not specify it
     if expected_ret is None:
         expected_ret = success
 
-    params = []
-    for a in kwargs:
-        params.append(str(a) + " = " + str(kwargs[a]))
-    if len(params) != 0:
-        params = ", ".join([str(i) for i in params])
+    params = [str(a) + " = " + str(kwargs[a]) for a in kwargs]
+    if params:
+        params = ", ".join(params)
         message += f" with params {params}"
+
     logger.info("\n" + message)  # noqa: G003
 
     try:
         ret, output = command(return_output=True, **kwargs)
     except TypeError as e:
         if "takes no keyword arguments" in str(e):
             # this function takes no keyword arguments
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/beaker.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/beaker.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cli_tools.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/cli_tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """cli_tools.py: Module to provide tools of wrapping command line tools for further usage."""
+from typing import List, Optional
 
 #  Copyright: Contributors to the sts project
 #  GNU General Public License v3.0+ (see LICENSE or https://www.gnu.org/licenses/gpl-3.0.txt)
 
 
 class WrongCommandExceptionError(Exception):
     def __init__(self, cmd) -> None:  # noqa: ANN001
@@ -68,21 +69,18 @@
         try:
             value = return_type(_value)
         except ValueError as e:
             print(f"WARN: Got ValueError: {e}.")
             return None
         return value
 
-    def _get_possible_arguments(self, command=None):  # noqa: ANN001, ANN202
-        # Returns possible arguments for said command if specified
-        args = []
+    def _get_possible_arguments(self, command: Optional[str] = None) -> List[str]:
+        # Returns possible arguments for the specified command if provided
         if command:
-            for key in list(self.arguments.keys()):
-                if list(self.commands.keys())[list(self.commands.values()).index(command)] in self._get_cmd(key):
-                    args.append(key)
+            args = [key for key in self.arguments if self._get_cmd(key) == command]
         else:
             args = list(self.arguments.keys())
         return args
 
     @staticmethod
     def _add_value(value, command, argument):  # noqa: ANN001, ANN205
         if argument[-1:] in ["=", "&"]:
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/cmdline.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/cmdline.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,20 @@
             timeout=timeout,
         )
         ret_out = StsCompletedProcess(returncode=cp.returncode, output=cp.stdout.rstrip() if cp.stdout else None)
 
         if not capture_output and verbose and ret_out.output:
             print(ret_out.output)
 
-        return ret_out
-
     except subprocess.TimeoutExpired as e:
         return StsCompletedProcess(returncode=124, output=e.output if e.output else None)
 
+    else:
+        return ret_out
+
 
 def run_ret_out(
     cmd: str,
     timeout: Optional[int] = None,
     return_output: bool = False,
     use_popen: bool = False,
     verbose: bool = True,
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/logchecker.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/logchecker.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,19 +242,19 @@
     log_msg_file = "/var/log/messages"
     if not Path(log_msg_file).is_file():
         print(f"WARN: Could not open {log_msg_file}")
         return True
 
     with Path(log_msg_file).open("rb") as log_file:
         log = ""
-        for line in log_file.readlines():
-            try:
+        try:
+            for line in log_file.readlines():
                 log += line.decode("UTF-8")
-            except UnicodeDecodeError:
-                log += line.decode("latin-1")
+        except UnicodeDecodeError:
+            log += line.decode("latin-1")
 
     begin_tag = "\\[ cut here \\]"
     end_tag = "\\[ end trace "
 
     if not Path(previous_time_file).is_file():
         first_time = "Jan 01 00:00:00"
         time = _date2num(first_time)
@@ -318,15 +318,15 @@
         print("INFO: No kdump log found for this server")
         return True
 
     ret, output = run_ret_out(f"ls -l {kdump_dir}/{hostname} |  awk '{{print$9}}'", return_output=True)
     kdumps = output.split("\n")
     kdump_dates = []
     for kdump in kdumps:
-        if kdump == "":
+        if not kdump:
             continue
         # parse on the date, remove the ip of the uploader
         m = re.match(".*?-(.*)", kdump)
         if not m:
             print(f"WARN: unexpected format for kdump ({kdump})")
             continue
         date = m.group(1)
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/persistent_vars.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/persistent_vars.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/restraint.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/restraint.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/size.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/size.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/src/sts/utils/tmt.py` & `sts_libs-0.0.5.dev1/sts_libs/src/sts/utils/tmt.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/cmdline_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/cmdline_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/fio_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/fio_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/iscsi_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/iscsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/linux_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/linux_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/logchecker_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/logchecker_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/lvm_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/lvm_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/md_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/md_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/net_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/net_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/persistent_vars_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/persistent_vars_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/sts_libs/tests/scsi_test.py` & `sts_libs-0.0.5.dev1/sts_libs/tests/scsi_test.py`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/.gitignore` & `sts_libs-0.0.5.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/LICENSE` & `sts_libs-0.0.5.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/pyproject.toml` & `sts_libs-0.0.5.dev1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -40,19 +40,27 @@
   "netifaces2==0.0.16",
   "six==1.16.0",
     # via configobj
   "typing-extensions==4.5.0",
     # via netifaces2
 ]
 
+# pytest-plugins
+# https://github.com/pytest-dev/pyfakefs
+# https://github.com/pytest-dev/pytest-testinfra
+# https://github.com/CFMTech/pytest-monitor
+# https://github.com/omarkohl/pytest-datafiles
+# pytest-sugar
+# https://pypi.org/project/pytest-benchmark/
+
 [project.urls]
 Repository = "https://gitlab.com/rh-kernel-stqe/sts/"
 
 [tool.hatch.version]
-path = "sts_libs/__about__.py"
+path = "sts_libs/src/sts/__about__.py"
 
 [tool.hatch.build.targets.sdist]
 include = ["sts_libs", "requirements-stable.txt", "LICENSE"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["sts_libs/src/sts"]
 
@@ -60,67 +68,67 @@
 line-length = 120
 target-version = ["py311", "py39", "py38"]
 
 [tool.ruff]
 line-length = 120
 namespace-packages = ["sts_libs"]
 src = ["sts_libs/src"]
-target-version = "py38"
 select = [
   "F",  # Pyflakes
   "E",  # pycodestyle
   "W",  # pycodestyle
   #"C90",  # mccabe
   "I",  # isort
   "N",  # pep8-naming
   "D",  # pydocstyle
   "UP",  # pyupgrade
   "YTT",  # flake8-2020
   "ANN",  # flake8-annotations
-  #"BLE",  # flake8-blind-except
+  #"BLE",  # flake8-blind-except -> TODO
+  #"FBT",  # flake8-boolean-trap
   "B",  # flake8-bugbear
   "A",  # flake8-builtins
   "COM",  # flake8-commas
   "C4",  # flake8-comprehensions
   "DTZ",  # flake8-datetimez
   "T10",  # flake8-debugger
-  "DJ",  # flake8-django
   "EM",  # flake8-errmsg
-  "EXE",  # flake8-executable
   "ISC",  # flake8-implicit-str-concat
   "ICN",  # flake8-import-conventions
   "G",  # flake8-logging-format
   "INP",  # flake8-no-pep420
   "PIE",  # flake8-pie
+  #"T20",  # flake8-print -> TODO
   "PT",  # flake8-pytest-style
   "Q",  # flake8-quotes
   "RSE",  # flake8-raise
   "RET",  # flake8-return
   "SLF",  # flake8-self
+  "SLOT",  # flake8-slots
   "SIM",  # flake8-simplify
   "TID",  # flake8-tidy-imports
   "TCH",  # flake8-type-checking
   "INT",  # flake8-gettext
   "ARG",  # flake8-unused-arguments
   "PTH",  # flake8-use-pathlib
   #"ERA",  # eradicate
   "PGH",  # pygrep-hooks
   "PL",  # Pylint
   "TRY",  # tryceratops
+  "FLY",  # flynt
+  "PERF",  # perflint
   "RUF",  # Ruff-specific rules
 ]
 ignore = [
-  "D10",  # Missing docstring
-  "D205",  # 1 blank line required between summary line and description
+  "D10",  # Missing docstring -> TODO
+  "D205",  # 1 blank line required between summary line and description -> TODO
   "D417",  # Missing argument descriptions -> Do not use docstring description for well type-annotated args
-  "PLR09",  # pylint-refactor too-many
-  "PLC1901",  # compare-to-empty-string
-  "PLR2004",  # magic value
-  "TRY300",  # Consider moving this statement to an `else` block. Seems to be broken?
-  "ANN101",  # Missing type annotation for `self` in method
+  "PLR09",  # pylint-refactor too-many -> TODO
+  "PLR2004",  # magic value -> TODO
+  "ANN101",  # Missing type annotation for `self` in method -> Not necessary
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = ["INP001"]
 
 [tool.ruff.flake8-builtins]
 builtins-ignorelist = ["id"]
@@ -138,10 +146,14 @@
 [tool.mypy]
 ignore_missing_imports = true
 # strict = true  # TODO -> Will require a lot of effort
 show_error_codes = true
 python_version = "3.8"
 
 [tool.yamlfix]
-explicit_start = "false"
-line_length = 120
-sequence_style = "block_style"
+explicit_start = "false"  # '---' at the beggining of the file
+line_length = 62  # 62 makes multiline text blocks <= 72 chars
+preserve_quotes = "true"  # otherwise can remove necessary quotes
+whitelines = 1 # allow no more than n whiteline(s)
+#comments_whitelines = 1
+#section_whitelines = 0  # force n whitelines between top-level sections
+sequence_style = "keep_style"  # "block_style" to force idented lists
```

### Comparing `sts_libs-0.0.5.dev0/sts_libs/README.md` & `sts_libs-0.0.5.dev1/sts_libs/README.md`

 * *Files identical despite different names*

### Comparing `sts_libs-0.0.5.dev0/PKG-INFO` & `sts_libs-0.0.5.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sts-libs
-Version: 0.0.5.dev0
+Version: 0.0.5.dev1
 Project-URL: Repository, https://gitlab.com/rh-kernel-stqe/sts/
 Author-email: Bruno Goncalves <bgoncalv@redhat.com>, Filip Suba <fsuba@redhat.com>, Jakub Krysl <jkrysl@redhat.com>, Martin Hoyer <mhoyer@redhat.com>
 Maintainer-email: Martin Hoyer <mhoyer@redhat.com>, Filip Suba <fsuba@redhat.com>, Bruno Goncalves <bgoncalv@redhat.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE
 Classifier: Framework :: Hatch
 Classifier: Intended Audience :: Developers
```

