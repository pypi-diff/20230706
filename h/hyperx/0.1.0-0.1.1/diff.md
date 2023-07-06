# Comparing `tmp/hyperx-0.1.0.tar.gz` & `tmp/hyperx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperx-0.1.0.tar", last modified: Fri Jun 30 15:47:45 2023, max compression
+gzip compressed data, was "hyperx-0.1.1.tar", last modified: Thu Jul  6 15:54:45 2023, max compression
```

## Comparing `hyperx-0.1.0.tar` & `hyperx-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.221887 hyperx-0.1.0/
--rw-rw-rw-   0        0        0      535 2023-06-30 15:47:45.221887 hyperx-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.186131 hyperx-0.1.0/hyperx/
--rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.0/hyperx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.206360 hyperx-0.1.0/hyperx/api/
--rw-rw-rw-   0        0        0   145913 2023-06-30 15:38:21.000000 hyperx-0.1.0/hyperx/api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.209350 hyperx-0.1.0/hyperx/api/types/
--rw-rw-rw-   0        0        0    24178 2023-06-29 20:33:40.000000 hyperx-0.1.0/hyperx/api/types/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.215329 hyperx-0.1.0/hyperx/library/
--rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/__init__.py
--rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/find.py
--rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/library/library.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.219894 hyperx-0.1.0/hyperx/utils/
--rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.0/hyperx/utils/__init__.py
--rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.0/hyperx/utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-30 15:47:45.204370 hyperx-0.1.0/hyperx.egg-info/
--rw-rw-rw-   0        0        0      535 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-30 15:47:45.000000 hyperx-0.1.0/hyperx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      660 2023-06-30 15:47:20.000000 hyperx-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-30 15:47:45.222885 hyperx-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.803233 hyperx-0.1.1/
+-rw-rw-rw-   0        0        0      535 2023-07-06 15:54:45.802233 hyperx-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-03-28 13:10:57.000000 hyperx-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.767609 hyperx-0.1.1/hyperx/
+-rw-rw-rw-   0        0        0      747 2023-06-29 20:58:54.000000 hyperx-0.1.1/hyperx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.789003 hyperx-0.1.1/hyperx/api/
+-rw-rw-rw-   0        0        0   145708 2023-07-06 15:54:30.000000 hyperx-0.1.1/hyperx/api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.791234 hyperx-0.1.1/hyperx/api/types/
+-rw-rw-rw-   0        0        0    24178 2023-06-29 20:33:40.000000 hyperx-0.1.1/hyperx/api/types/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.797234 hyperx-0.1.1/hyperx/library/
+-rw-rw-rw-   0        0        0      125 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/__init__.py
+-rw-rw-rw-   0        0        0     1587 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/find.py
+-rw-rw-rw-   0        0        0     1395 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/library/library.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.800233 hyperx-0.1.1/hyperx/utils/
+-rw-rw-rw-   0        0        0       50 2023-03-28 13:10:57.000000 hyperx-0.1.1/hyperx/utils/__init__.py
+-rw-rw-rw-   0        0        0     2410 2023-06-30 13:01:12.000000 hyperx-0.1.1/hyperx/utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-06 15:54:45.786194 hyperx-0.1.1/hyperx.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-07-06 15:54:45.000000 hyperx-0.1.1/hyperx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      660 2023-07-06 15:19:27.000000 hyperx-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 15:54:45.803233 hyperx-0.1.1/setup.cfg
```

### Comparing `hyperx-0.1.0/PKG-INFO` & `hyperx-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.0
+Version: 0.1.1
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.0/hyperx/__init__.py` & `hyperx-0.1.1/hyperx/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.0/hyperx/api/__init__.py` & `hyperx-0.1.1/hyperx/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,33 +196,33 @@
 
 class JointAnalysisResult(AnalysisResult):
 	def __init__(self, jointAnalysisResult: _api.JointAnalysisResult):
 		self._Entity = jointAnalysisResult
 
 	@property
 	def ObjectId(self) -> types.JointObject:
-		return types.JointObject[self._Entity.JointObject.ToString()]
+		return types.JointObject[self._Entity.ObjectId.ToString()]
 
 
 class ZoneAnalysisConceptResult(AnalysisResult):
 	def __init__(self, zoneAnalysisConceptResult: _api.ZoneAnalysisConceptResult):
 		self._Entity = zoneAnalysisConceptResult
 
 	@property
 	def ConceptId(self) -> types.FamilyConceptUID:
-		return types.FamilyConceptUID[self._Entity.FamilyConceptUID.ToString()]
+		return types.FamilyConceptUID[self._Entity.ConceptId.ToString()]
 
 
 class ZoneAnalysisObjectResult(AnalysisResult):
 	def __init__(self, zoneAnalysisObjectResult: _api.ZoneAnalysisObjectResult):
 		self._Entity = zoneAnalysisObjectResult
 
 	@property
 	def ObjectId(self) -> types.FamilyObjectUID:
-		return types.FamilyObjectUID[self._Entity.FamilyObjectUID.ToString()]
+		return types.FamilyObjectUID[self._Entity.ObjectId.ToString()]
 
 
 class AssignableProperty(IdNameEntity):
 	def __init__(self, assignableProperty: _api.AssignableProperty):
 		self._Entity = assignableProperty
 
 
@@ -258,29 +258,29 @@
 
 	@property
 	def CategoryId(self) -> int:
 		return self._Entity.CategoryId
 
 	@property
 	def DataType(self) -> types.UserConstantDataType:
-		return types.UserConstantDataType[self._Entity.UserConstantDataType.ToString()]
+		return types.UserConstantDataType[self._Entity.DataType.ToString()]
 
 	@property
 	def DefaultValue(self) -> str:
 		return self._Entity.DefaultValue
 
 	@property
 	def Description(self) -> str:
 		return self._Entity.Description
 
 	@property
 	def EnumValues(self) -> dict[int, str]:
 		enumValuesDict = {}
 		for kvp in self._Entity.EnumValues:
-			enumValuesDict[int[kvp.Key.ToString()]] = str(kvp.Value)
+			enumValuesDict[int(kvp.Key)] = str(kvp.Value)
 
 		return enumValuesDict
 
 	@property
 	def PackageId(self) -> int:
 		return self._Entity.PackageId
 
@@ -658,15 +658,15 @@
 
 	@property
 	def RunDeckOrder(self) -> int:
 		return self._Entity.RunDeckOrder
 
 	@property
 	def SolutionType(self) -> types.FeaSolutionType:
-		return types.FeaSolutionType[self._Entity.FeaSolutionType.ToString()]
+		return types.FeaSolutionType[self._Entity.SolutionType.ToString()]
 
 
 class DesignLoadSubcaseMultiplier(IdNameEntity):
 	def __init__(self, designLoadSubcaseMultiplier: _api.DesignLoadSubcaseMultiplier):
 		self._Entity = designLoadSubcaseMultiplier
 
 	@property
@@ -828,33 +828,33 @@
 	def __init__(self, discreteFieldTable: _api.DiscreteFieldTable):
 		self._Entity = discreteFieldTable
 
 	@property
 	def Columns(self) -> dict[int, str]:
 		columnsDict = {}
 		for kvp in self._Entity.Columns:
-			columnsDict[int[kvp.Key.ToString()]] = str(kvp.Value)
+			columnsDict[int(kvp.Key)] = str(kvp.Value)
 
 		return columnsDict
 
 	@property
 	def ColumnCount(self) -> int:
 		return self._Entity.ColumnCount
 
 	@property
 	def DataType(self) -> types.DiscreteFieldDataType:
-		return types.DiscreteFieldDataType[self._Entity.DiscreteFieldDataType.ToString()]
+		return types.DiscreteFieldDataType[self._Entity.DataType.ToString()]
 
 	@property
 	def PhysicalEntityType(self) -> types.DiscreteFieldPhysicalEntityType:
-		return types.DiscreteFieldPhysicalEntityType[self._Entity.DiscreteFieldPhysicalEntityType.ToString()]
+		return types.DiscreteFieldPhysicalEntityType[self._Entity.PhysicalEntityType.ToString()]
 
 	@property
 	def PointIds(self) -> list[Vector3d]:
-		return [Vector3d[vector3d.ToString()] for vector3d in self._Entity.PointIds]
+		return [Vector3d(vector3d) for vector3d in self._Entity.PointIds]
 
 	@property
 	def RowCount(self) -> int:
 		return self._Entity.RowCount
 
 	@property
 	def RowIds(self) -> list[int]:
@@ -2374,36 +2374,36 @@
 
 	@property
 	def CorrectionId(self) -> types.CorrectionId:
 		return types.CorrectionId[self._Entity.CorrectionId.ToString()]
 
 	@property
 	def PropertyId(self) -> types.CorrectionProperty:
-		return types.CorrectionProperty[self._Entity.CorrectionProperty.ToString()]
+		return types.CorrectionProperty[self._Entity.PropertyId.ToString()]
 
 
 class OrthotropicCorrectionFactorValue:
 	def __init__(self, orthotropicCorrectionFactorValue: _api.OrthotropicCorrectionFactorValue):
 		self._Entity = orthotropicCorrectionFactorValue
 
 	@property
 	def Property(self) -> types.CorrectionProperty:
-		return types.CorrectionProperty[self._Entity.CorrectionProperty.ToString()]
+		return types.CorrectionProperty[self._Entity.Property.ToString()]
 
 	@property
 	def Correction(self) -> types.CorrectionId:
-		return types.CorrectionId[self._Entity.CorrectionId.ToString()]
+		return types.CorrectionId[self._Entity.Correction.ToString()]
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
-		return types.CorrectionEquation[self._Entity.CorrectionEquation.ToString()]
+		return types.CorrectionEquation[self._Entity.Equation.ToString()]
 
 	@property
 	def EquationParameter(self) -> types.EquationParameterId:
-		return types.EquationParameterId[self._Entity.EquationParameterId.ToString()]
+		return types.EquationParameterId[self._Entity.EquationParameter.ToString()]
 
 	@property
 	def Value(self) -> float:
 		return self._Entity.Value
 
 	@Value.setter
 	def Value(self, value: float) -> None:
@@ -2412,15 +2412,15 @@
 
 class OrthotropicEquationCorrectionFactor(OrthotropicCorrectionFactorBase):
 	def __init__(self, orthotropicEquationCorrectionFactor: _api.OrthotropicEquationCorrectionFactor):
 		self._Entity = orthotropicEquationCorrectionFactor
 
 	@property
 	def Equation(self) -> types.CorrectionEquation:
-		return types.CorrectionEquation[self._Entity.CorrectionEquation.ToString()]
+		return types.CorrectionEquation[self._Entity.Equation.ToString()]
 
 	def AddCorrectionFactorValue(self, equationParameterName: types.EquationParameterId, valueToAdd: float) -> OrthotropicCorrectionFactorValue:
 		return OrthotropicCorrectionFactorValue(self._Entity.AddCorrectionFactorValue(_types.EquationParameterId(equationParameterName.value), valueToAdd))
 
 
 class TabularCorrectionFactorRow:
 	def __init__(self, tabularCorrectionFactorRow: _api.TabularCorrectionFactorRow):
@@ -2435,15 +2435,15 @@
 	def __init__(self, orthotropicTabularCorrectionFactor: _api.OrthotropicTabularCorrectionFactor):
 		self._Entity = orthotropicTabularCorrectionFactor
 
 	@property
 	def CorrectionFactorRows(self) -> dict[int, TabularCorrectionFactorRow]:
 		correctionFactorRowsDict = {}
 		for kvp in self._Entity.CorrectionFactorRows:
-			correctionFactorRowsDict[int[kvp.Key.ToString()]] = TabularCorrectionFactorRow(kvp.Value)
+			correctionFactorRowsDict[int(kvp.Key)] = TabularCorrectionFactorRow(kvp.Value)
 
 		return correctionFactorRowsDict
 
 	@property
 	def CorrectionIndependentDefinitions(self) -> set[types.CorrectionIndependentDefinition]:
 		return {types.CorrectionIndependentDefinition(correctionIndependentDefinition) for correctionIndependentDefinition in self._Entity.CorrectionIndependentDefinitions}
 
@@ -2474,15 +2474,15 @@
 
 class OrthotropicAllowableCurvePoint:
 	def __init__(self, orthotropicAllowableCurvePoint: _api.OrthotropicAllowableCurvePoint):
 		self._Entity = orthotropicAllowableCurvePoint
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
-		return types.AllowablePropertyName[self._Entity.AllowablePropertyName.ToString()]
+		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
 
 	@property
 	def Temperature(self) -> float:
 		return self._Entity.Temperature
 
 	@property
 	def X(self) -> float:
@@ -2511,19 +2511,19 @@
 
 class OrthotropicLaminateAllowable:
 	def __init__(self, orthotropicLaminateAllowable: _api.OrthotropicLaminateAllowable):
 		self._Entity = orthotropicLaminateAllowable
 
 	@property
 	def Property_ID(self) -> types.AllowablePropertyName:
-		return types.AllowablePropertyName[self._Entity.AllowablePropertyName.ToString()]
+		return types.AllowablePropertyName[self._Entity.Property_ID.ToString()]
 
 	@property
 	def Method_ID(self) -> types.AllowableMethodName:
-		return types.AllowableMethodName[self._Entity.AllowableMethodName.ToString()]
+		return types.AllowableMethodName[self._Entity.Method_ID.ToString()]
 
 	@Property_ID.setter
 	def Property_ID(self, value: types.AllowablePropertyName) -> None:
 		self._Entity.Property_ID = _types.AllowablePropertyName(value.value)
 
 	@Method_ID.setter
 	def Method_ID(self, value: types.AllowableMethodName) -> None:
@@ -3252,15 +3252,15 @@
 
 class SectionCut(IdNameEntity):
 	def __init__(self, sectionCut: _api.SectionCut):
 		self._Entity = sectionCut
 
 	@property
 	def ReferencePoint(self) -> types.SectionCutPropertyLocation:
-		return types.SectionCutPropertyLocation[self._Entity.SectionCutPropertyLocation.ToString()]
+		return types.SectionCutPropertyLocation[self._Entity.ReferencePoint.ToString()]
 
 	@property
 	def HorizontalVector(self) -> Vector3d:
 		return Vector3d(self._Entity.HorizontalVector)
 
 	@property
 	def NormalVector(self) -> Vector3d:
@@ -4351,15 +4351,15 @@
 
 	@property
 	def LoadProperties(self) -> LoadPropertyCol:
 		return LoadPropertyCol(self._Entity.LoadProperties)
 
 	@property
 	def FemFormat(self) -> types.ProjectModelFormat:
-		return types.ProjectModelFormat[self._Entity.ProjectModelFormat.ToString()]
+		return types.ProjectModelFormat[self._Entity.FemFormat.ToString()]
 
 	def Upload(self, uploadSetName: str, company: str, program: str, tags: list[str], notes: str, zoneIds: set[int], jointIds: set[int]) -> bool:
 		tagsList = List[str]()
 		if tags is not None:
 			for thing in tags:
 				if thing is not None:
 					tagsList.Add(thing)
@@ -5037,15 +5037,15 @@
 
 	@property
 	def IntValue(self) -> int:
 		return self._Entity.IntValue
 
 	@property
 	def ValueType(self) -> types.CorrectionValueType:
-		return types.CorrectionValueType[self._Entity.CorrectionValueType.ToString()]
+		return types.CorrectionValueType[self._Entity.ValueType.ToString()]
 
 
 class OrthotropicEffectiveLaminate:
 	def __init__(self, orthotropicEffectiveLaminate: _api.OrthotropicEffectiveLaminate):
 		self._Entity = orthotropicEffectiveLaminate
 
 	@property
```

### Comparing `hyperx-0.1.0/hyperx/api/types/__init__.py` & `hyperx-0.1.1/hyperx/api/types/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.0/hyperx/library/find.py` & `hyperx-0.1.1/hyperx/library/find.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.0/hyperx/library/library.py` & `hyperx-0.1.1/hyperx/library/library.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.0/hyperx/utils/utils.py` & `hyperx-0.1.1/hyperx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `hyperx-0.1.0/hyperx.egg-info/PKG-INFO` & `hyperx-0.1.1/hyperx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperx
-Version: 0.1.0
+Version: 0.1.1
 Summary: HyperX scripting for Python
 Author-email: Kelly Ann Smith <kellyann.smith@collieraerospace.com>, Noah Prezant <noah.prezant@collieraerospace.com>
 Project-URL: Homepage, https://collieraerospace.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `hyperx-0.1.0/pyproject.toml` & `hyperx-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyperx"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Kelly Ann Smith", email="kellyann.smith@collieraerospace.com" },
   { name="Noah Prezant", email="noah.prezant@collieraerospace.com" },
 ]
 description = "HyperX scripting for Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

