# Comparing `tmp/reddit_decider-1.4.0.tar.gz` & `tmp/reddit_decider-1.4.1.tar.gz`

## Comparing `reddit_decider-1.4.0.tar` & `reddit_decider-1.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/local_dependencies/decider/Cargo.toml
--rw-r--r--   0        0        0       19 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/.gitignore
--rw-r--r--   0        0        0      323 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/Makefile
--rw-r--r--   0        0        0      710 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/README.md
--rw-r--r--   0        0        0     6097 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/benches/decider.rs
--rw-r--r--   0        0        0     9514 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/context.rs
--rw-r--r--   0        0        0    48184 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/events.rs
--rw-r--r--   0        0        0   110863 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/local_dependencies/decider/src/lib.rs
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/Cargo.toml
--rw-r--r--   0        0        0      112 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/.gitignore
--rw-r--r--   0        0        0      786 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/Makefile
--rw-r--r--   0        0        0     6041 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/README.md
--rw-r--r--   0        0        0      273 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    22412 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/python/rust_decider/__init__.py
--rw-r--r--   0        0        0      259 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/python/rust_decider/prometheus_metrics.py
--rw-r--r--   0        0        0      177 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/requirements-dev.txt
--rw-r--r--   0        0        0       40 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/setup.cfg
--rw-r--r--   0        0        0     1300 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/setup.py
--rw-r--r--   0        0        0    34812 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/src/lib.rs
--rw-r--r--   0        0        0    40966 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/decider_unit_test.py
--rw-r--r--   0        0        0    10110 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/integration_test.py
--rw-r--r--   0        0        0     2903 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/test_rust.py
--rw-r--r--   0        0        0    34128 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/unit_test.py
--rw-r--r--   0        0        0     3088 2023-07-05 18:59:38.000000 reddit_decider-1.4.0/test/utils.py
--rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/local_dependencies/decider/Cargo.toml
+-rw-r--r--   0        0        0       19 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/.gitignore
+-rw-r--r--   0        0        0      323 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/Makefile
+-rw-r--r--   0        0        0      710 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/README.md
+-rw-r--r--   0        0        0     6097 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/benches/decider.rs
+-rw-r--r--   0        0        0     9514 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/context.rs
+-rw-r--r--   0        0        0    48184 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/events.rs
+-rw-r--r--   0        0        0   111863 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/local_dependencies/decider/src/lib.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/Cargo.toml
+-rw-r--r--   0        0        0      112 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/.gitignore
+-rw-r--r--   0        0        0      786 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/Makefile
+-rw-r--r--   0        0        0     6041 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/README.md
+-rw-r--r--   0        0        0      273 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    22412 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/python/rust_decider/__init__.py
+-rw-r--r--   0        0        0      259 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/python/rust_decider/prometheus_metrics.py
+-rw-r--r--   0        0        0      177 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/requirements-dev.txt
+-rw-r--r--   0        0        0       40 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/setup.cfg
+-rw-r--r--   0        0        0     1300 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/setup.py
+-rw-r--r--   0        0        0    34812 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/src/lib.rs
+-rw-r--r--   0        0        0    42128 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/decider_unit_test.py
+-rw-r--r--   0        0        0    10110 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/integration_test.py
+-rw-r--r--   0        0        0     2903 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/test_rust.py
+-rw-r--r--   0        0        0    34128 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/unit_test.py
+-rw-r--r--   0        0        0     3088 2023-07-06 18:25:28.000000 reddit_decider-1.4.1/test/utils.py
+-rw-r--r--   0        0        0     6238 1970-01-01 00:00:00.000000 reddit_decider-1.4.1/PKG-INFO
```

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/Cargo.toml` & `reddit_decider-1.4.1/local_dependencies/decider/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "decider"
-version = "1.4.0"
+version = "1.4.1"
 edition = "2021"
 description = "a package for AB-testing and dynamic config"
 homepage = "https://mattknox.com"
 license = "MIT"
 documentation = "https://mattknox.com/decider"
 readme = "README.md"
```

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/README.md` & `reddit_decider-1.4.1/local_dependencies/decider/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/benches/decider.rs` & `reddit_decider-1.4.1/local_dependencies/decider/benches/decider.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/src/context.rs` & `reddit_decider-1.4.1/local_dependencies/decider/src/context.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/src/events.rs` & `reddit_decider-1.4.1/local_dependencies/decider/src/events.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/local_dependencies/decider/src/lib.rs` & `reddit_decider-1.4.1/local_dependencies/decider/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -73,34 +73,34 @@
     }
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct Metadata {
     pub id: u32,
     pub name: String,
-    pub enabled: bool,
     pub version: u32,
     pub owner: String,
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct DynamicConfig {
     metadata: Metadata,
+    enabled: bool,
     value: Value,
     value_type: ValueType,
 }
 
 /// RangeVariant represent a unit of controllable code, that we might want to turn off, make
 /// available only to some users, etc..  This is what FeatureFlags/AB tests control.
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub struct RangeVariant {
     metadata: Metadata,
     pub emit_event: bool,
     pub variant_set: VariantSet,
-    enabled: bool, // is this just for darkmode?
+    enabled: bool,
     targeting: Option<TargetingTree>,
     overrides: Option<Vec<HashMap<String, TargetingTree>>>,
 }
 
 #[derive(Serialize, Deserialize, Debug, Clone)]
 pub enum Feature {
     RangeVariant(RangeVariant),
@@ -165,16 +165,16 @@
 impl DynamicConfig {
     fn default_decision(&self, events: Vec<ExperimentEvent>) -> InternalDecision {
         InternalDecision {
             feature_id: self.metadata.id,
             feature_name: self.metadata.name.clone(),
             feature_version: self.metadata.version,
             variant_name: None,
-            value: self.value.clone(),
-            value_type: Some(self.value_type),
+            value: Value::Null,
+            value_type: None,
             events,
         }
     }
 }
 
 impl Feature {
     pub fn metadata(&self) -> &Metadata {
@@ -424,42 +424,44 @@
     targeting: Option<TargetingTree>,
     overrides: Option<Vec<HashMap<String, TargetingTree>>>,
     variant_set: Option<VariantSet>,
 }
 
 impl From<&Feature> for LegacyExperiment {
     fn from(f: &Feature) -> Self {
-        let (feature_type, emit_event, value, value_type, targeting, overrides, variant_set) =
+        let (feature_type, enabled, emit_event, value, value_type, targeting, overrides, variant_set) =
             match f {
                 Feature::RangeVariant(rv) => (
                     ExperimentType::RangeVariant,
+                    rv.enabled,
                     rv.emit_event,
                     None,
                     None,
                     rv.targeting.clone(),
                     rv.overrides.clone(),
                     Some(rv.variant_set.clone()),
                 ),
                 Feature::DynamicConfig(dc) => (
                     ExperimentType::DynamicConfig,
+                    dc.enabled,
                     false,
                     Some(dc.value.clone()),
                     Some(dc.value_type),
                     None,
                     None,
                     None,
                 ),
             };
 
         LegacyExperiment {
             id: f.metadata().id,
             name: f.metadata().name.to_string(),
-            enabled: f.metadata().enabled,
             version: f.metadata().version,
             owner: f.metadata().owner.to_string(),
+            enabled,
             feature_type,
             emit_event,
             value,
             value_type,
             targeting,
             overrides,
             variant_set,
@@ -1150,15 +1152,19 @@
             },
         }
     }
 }
 
 impl Decide for DynamicConfig {
     fn darkmode(&self, _d: &Decider, _ctx: &Context) -> Result<Choice, DeciderError> {
-        Ok(Choice::None)
+        if self.enabled {
+            Ok(Choice::Pass("darkmode:enabled"))
+        } else {
+            Ok(Choice::None)
+        }
     }
 
     fn fractional_availability(
         &self,
         _d: &Decider,
         _ctx: &Context,
     ) -> Result<Choice, DeciderError> {
@@ -1396,15 +1402,14 @@
 }
 
 impl From<&Experiment> for Metadata {
     fn from(exp: &Experiment) -> Self {
         Metadata {
             id: exp.id,
             name: exp.name.clone(),
-            enabled: exp.enabled,
             version: exp.experiment.experiment_version,
             owner: exp.owner.clone(),
         }
     }
 }
 
 impl From<&serde_json::Value> for ValueType {
@@ -1432,14 +1437,15 @@
         .clone()
         .map(Value::from)
         .unwrap_or_else(|| Value::from(exp.value_type.unwrap_or(ValueType::Null)));
     let value_type = value.borrow().into();
 
     Ok(DynamicConfig {
         metadata: exp.into(),
+        enabled: exp.enabled,
         value,
         value_type,
     })
 }
 
 fn experiment_to_multivariant_choice(
     exp: &Experiment,
@@ -1524,15 +1530,14 @@
             range: 0..100,
         };
 
         Feature::RangeVariant(RangeVariant {
             metadata: Metadata {
                 id: 1,
                 name: "first_feature".to_string(),
-                enabled: true,
                 version: 1,
                 owner: "test".to_string(),
             },
             emit_event: true,
             variant_set: VariantSet {
                 start_ts: 0,
                 stop_ts: 2147483648, // 2 ** 31 - far future.
@@ -1602,18 +1607,18 @@
             }
         };
 
         Feature::DynamicConfig(DynamicConfig {
             metadata: Metadata {
                 id: 2,
                 name: name_str + "_dynamic_config",
-                enabled: true,
                 version: 1,
                 owner: "test".to_string(),
             },
+            enabled: true,
             value: value,
             value_type: value_type,
         })
     }
 
     fn make_experiment(name: String, meg: Option<String>, hg: Option<String>) -> Experiment {
         let c = Variant {
@@ -2556,14 +2561,48 @@
             ..Context::default()
         };
         let decision = decider.choose("x0", ctx, None).unwrap();
         assert_eq!(decision.variant_name, None);
     }
 
     #[test]
+    fn dc_darkmode() {
+        let cgf = json!({
+            "dc": {
+                "id": 1337,
+                "value": {
+                    "map": {
+                        "foo": "bar",
+                    }
+                },
+                "type": "dynamic_config",
+                "version": "1",
+                "enabled": false,
+                "owner": "test",
+                "name": "dc",
+                "value_type": "Map",
+                "experiment": {
+                    "experiment_version": 1
+                }
+            }
+        });
+
+        let json_str = serde_json::to_string(&cgf).unwrap();
+        let json_bytes = json_str.as_bytes();
+        let decider = Decider::from_bytes(json_bytes).unwrap();
+
+        let ctx = &Context {
+            user_id: Some("t2_id_1".to_string()),
+            ..Context::default()
+        };
+
+        assert_eq!(true, decider.get_map("dc", ctx).is_err());
+    }
+
+    #[test]
     fn decider_override_groups() {
         let cgf = json!({
             "$override_groups": {
                 "id": 1337,
                 "value": {
                     "$ads_admins": {
                         "name": "$ads_admins",
@@ -2571,15 +2610,15 @@
                         "field": "user_id"
                     }
                 },
                 "type": "dynamic_config",
                 "version": "1",
                 "enabled": false,
                 "owner": "test",
-                "name": "$override_group",
+                "name": "$override_groups",
                 "value_type": "Map",
                 "experiment": {
                     "experiment_version": 1
                 }
             },
             "x0": {
                 "id": 1,
```

### Comparing `reddit_decider-1.4.0/Makefile` & `reddit_decider-1.4.1/Makefile`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/README.md` & `reddit_decider-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/python/rust_decider/__init__.py` & `reddit_decider-1.4.1/python/rust_decider/__init__.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/setup.py` & `reddit_decider-1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/src/lib.rs` & `reddit_decider-1.4.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/test/decider_unit_test.py` & `reddit_decider-1.4.1/test/decider_unit_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -461,14 +461,48 @@
             with self.assertRaises(DeciderException) as e:
                 decider.choose("genexp_business_id", ctx)
             self.assertEqual(
                 str(e.exception),
                 'Missing field "business_id" in context for bucket_val = business_id',
             )
 
+    def test_choose_with_other_fields_for_bucketing(self):
+        cfg = self.genexp_0_cfg
+        cfg["genexp_0"]["experiment"].update(
+            {
+                "bucket_val": "foo",
+                "variants": [
+                    {"range_start": 0.0, "range_end": 1.0, "name": "control_1"},
+                ],
+            }
+        )
+
+        with create_temp_config_file(cfg) as f:
+            decider = setup_decider_class(f.name)
+            ctx = self.valid_ctx_dict
+
+            # include bucket_val value in "other_fields"
+            ctx.update({"other_fields": {"foo": "bar"}})
+
+            choice = decider.choose("genexp_0", ctx)
+
+            self.assertEqual(
+                dict(choice),
+                {
+                    "variant": "control_1",
+                    "value": None,
+                    "feature_id": 6299,
+                    "feature_name": "genexp_0",
+                    "feature_version": 5,
+                    "events": [
+                        "0::::6299::::genexp_0::::5::::control_1::::bar::::foo::::0::::2147483648::::test"
+                    ],
+                },
+            )
+
     def test_choose_with_other_fields_for_targeting(self):
         cfg = self.genexp_0_cfg
         cfg["genexp_0"]["experiment"].update(
             {"targeting": {"ALL": [{"EQ": {"field": "foo", "values": ["bar"]}}]}}
         )
 
         with create_temp_config_file(cfg) as f:
@@ -510,14 +544,15 @@
                 },
             )
 
     def test_choose_with_other_fields_for_overrides(self):
         cfg = self.genexp_0_cfg
         cfg["genexp_0"]["experiment"].update(
             {
+                "bucket_val": "foo",
                 "overrides": [
                     {
                         "variant_5": {
                             "ANY": [{"EQ": {"field": "foo", "values": ["bar"]}}]
                         }
                     }
                 ],
@@ -542,15 +577,15 @@
                 {
                     "variant": "variant_5",
                     "value": None,
                     "feature_id": 6299,
                     "feature_name": "genexp_0",
                     "feature_version": 5,
                     "events": [
-                        "1::::6299::::genexp_0::::5::::variant_5::::795244::::user_id::::0::::2147483648::::test"
+                        "1::::6299::::genexp_0::::5::::variant_5::::bar::::foo::::0::::2147483648::::test"
                     ],
                 },
             )
 
             # override doesn't match
             ctx.update({"other_fields": {"foo": "huh"}})
```

### Comparing `reddit_decider-1.4.0/test/integration_test.py` & `reddit_decider-1.4.1/test/integration_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/test/test_rust.py` & `reddit_decider-1.4.1/test/test_rust.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/test/unit_test.py` & `reddit_decider-1.4.1/test/unit_test.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/test/utils.py` & `reddit_decider-1.4.1/test/utils.py`

 * *Files identical despite different names*

### Comparing `reddit_decider-1.4.0/PKG-INFO` & `reddit_decider-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reddit-decider
-Version: 1.4.0
+Version: 1.4.1
 Requires-Dist: prometheus-client>=0.12.0,<1.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # rust_decider
 
 Rust implementation of bucketing, targeting, overrides, and dynamic config logic.
```

