# Comparing `tmp/CodeToCAD-0.2.1687027263.tar.gz` & `tmp/CodeToCAD-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CodeToCAD-0.2.1687027263.tar", last modified: Sat Jun 17 18:41:55 2023, max compression
+gzip compressed data, was "CodeToCAD-0.2.6.tar", last modified: Tue Mar 14 18:44:06 2023, max compression
```

## Comparing `CodeToCAD-0.2.1687027263.tar` & `CodeToCAD-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:41:55.106736 CodeToCAD-0.2.1687027263/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:41:55.106736 CodeToCAD-0.2.1687027263/CodeToCAD/
--rw-r--r--   0 runner    (1001) docker     (123)    58155 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/CodeToCAD/CodeToCADInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24610 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/CodeToCAD/CodeToCADProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)    36665 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/CodeToCAD/TestCodeToCADProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4390 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/CodeToCAD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33016 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/CodeToCAD/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 18:41:55.106736 CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-17 18:41:55.000000 CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-17 18:41:55.000000 CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 18:41:55.000000 CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 18:41:55.000000 CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-06-17 18:41:55.106736 CodeToCAD-0.2.1687027263/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 18:41:55.106736 CodeToCAD-0.2.1687027263/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-17 18:41:47.000000 CodeToCAD-0.2.1687027263/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-17 18:41:54.000000 CodeToCAD-0.2.1687027263/version.txt
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.653009 CodeToCAD-0.2.6/
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.651149 CodeToCAD-0.2.6/CodeToCAD/
+-rw-r--r--   0 shehab     (501) staff       (20)    52877 2023-03-14 17:49:23.000000 CodeToCAD-0.2.6/CodeToCAD/CodeToCADInterface.py
+-rw-r--r--   0 shehab     (501) staff       (20)    24176 2023-03-14 17:49:32.000000 CodeToCAD-0.2.6/CodeToCAD/CodeToCADProvider.py
+-rw-r--r--   0 shehab     (501) staff       (20)    33120 2023-03-14 17:49:27.000000 CodeToCAD-0.2.6/CodeToCAD/TestCodeToCADProvider.py
+-rw-r--r--   0 shehab     (501) staff       (20)     4039 2023-03-14 17:57:05.000000 CodeToCAD-0.2.6/CodeToCAD/__init__.py
+-rw-r--r--   0 shehab     (501) staff       (20)    27428 2023-03-10 02:21:17.000000 CodeToCAD-0.2.6/CodeToCAD/utilities.py
+drwxr-xr-x   0 shehab     (501) staff       (20)        0 2023-03-14 18:44:06.652343 CodeToCAD-0.2.6/CodeToCAD.egg-info/
+-rw-r--r--   0 shehab     (501) staff       (20)     5776 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/PKG-INFO
+-rw-r--r--   0 shehab     (501) staff       (20)      301 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/SOURCES.txt
+-rw-r--r--   0 shehab     (501) staff       (20)        1 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/dependency_links.txt
+-rw-r--r--   0 shehab     (501) staff       (20)       10 2023-03-14 18:44:06.000000 CodeToCAD-0.2.6/CodeToCAD.egg-info/top_level.txt
+-rw-r--r--   0 shehab     (501) staff       (20)    32473 2022-06-17 17:22:57.000000 CodeToCAD-0.2.6/LICENSE
+-rw-r--r--   0 shehab     (501) staff       (20)     5776 2023-03-14 18:44:06.652783 CodeToCAD-0.2.6/PKG-INFO
+-rw-r--r--   0 shehab     (501) staff       (20)     5242 2023-03-14 18:42:58.000000 CodeToCAD-0.2.6/README.md
+-rw-r--r--   0 shehab     (501) staff       (20)       38 2023-03-14 18:44:06.653087 CodeToCAD-0.2.6/setup.cfg
+-rw-r--r--   0 shehab     (501) staff       (20)      785 2023-03-14 18:44:05.000000 CodeToCAD-0.2.6/setup.py
```

### Comparing `CodeToCAD-0.2.1687027263/CodeToCAD/CodeToCADInterface.py` & `CodeToCAD-0.2.6/CodeToCAD/CodeToCADInterface.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,1773 +1,1719 @@
-# THIS IS AN AUTO-GENERATE FILE.
+# THIS IS AN AUTO-GENERATE FILE. 
 # DO NOT EDIT MANUALLY.
 # Please run development/capabilitiesJsonToPython/capabilitiesToPy.sh to generate this file.
 
 from abc import ABCMeta, abstractmethod
 from typing import Optional, TypeAlias, Union
 
-from CodeToCAD.utilities import (Angle, Axis, BoundaryBox, CurveTypes, Dimension, Dimensions, LengthUnit, Point, PresetLandmark)
+from CodeToCAD.utilities import (Angle, Axis, BoundaryBox, CurveTypes, Dimension,
+                            Dimensions, LengthUnit, Point)
 
 FloatOrItsStringValue: TypeAlias = Union[str, float]
 IntOrFloat: TypeAlias = Union[int, float]
 MaterialOrItsName: TypeAlias = Union[str, 'Material']
 PartOrItsName: TypeAlias = Union[str, 'Part']
 EntityOrItsName: TypeAlias = Union[str, 'Entity']
-SketchOrItsName: TypeAlias = Union[str, 'Sketch']
 LandmarkOrItsName: TypeAlias = Union[str, 'Landmark']
 AxisOrItsIndexOrItsName: TypeAlias = Union[str, int, Axis]
 DimensionOrItsFloatOrStringValue: TypeAlias = Union[str,float, Dimension]
 AngleOrItsFloatOrStringValue: TypeAlias = Union[str,float, Angle]
 EntityOrItsNameOrLandmark: TypeAlias = Union[str, 'Entity', 'Landmark']
 PointOrListOfFloatOrItsStringValue: TypeAlias = Union[str, list[FloatOrItsStringValue], Point]
 LengthUnitOrItsName: TypeAlias = Union[str,LengthUnit]
-PresetLandmarkOrItsName: TypeAlias = Union[str,PresetLandmark]
-CameraOrItsName:TypeAlias = Union[str, 'Camera']
 
 class Entity(metaclass=ABCMeta):
-    '''Capabilities shared between Parts and Sketches.'''
-
+    '''Capabilities shared between Parts, Sketches and Landmarks.'''
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @abstractmethod
-    def createFromFile(self, filePath:str, fileType:Optional[str]=None):
-        '''
-        Adds geometry to a part from a file. If the part does not exist, this will create it.
-        '''
-        
-        print("createFromFile is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def isExists(self) -> bool:
+    def isExists(self
+    ) -> bool:
         '''
         Check if an entity exists
         '''
         
         print("isExists is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def rename(self, newName:str, renamelinkedEntitiesAndLandmarks:bool=True):
+    def rename(self, newName:str, renamelinkedEntitiesAndLandmarks:bool=True
+    ):
         '''
         Rename the entity, with an option to rename linked landmarks and underlying data.
         '''
         
         print("rename is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def delete(self, removeChildren:bool):
+    def delete(self, removeChildren:bool
+    ):
         '''
         Delete the entity from the scene. You may need to delete an associated joint or other features.
         '''
         
         print("delete is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def isVisible(self) -> bool:
+    def isVisible(self
+    ) -> bool:
         '''
         Returns whether the entity is visible in the scene.
         '''
         
         print("isVisible is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def setVisible(self, isVisible:bool):
+    def setVisible(self, isVisible:bool
+    ):
         '''
         Toggles visibility of an entity in the scene.
         '''
         
         print("setVisible is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def apply(self, rotation:bool=True, scale:bool=True, location:bool=False, modifiers:bool=True):
+    def apply(self
+    ):
         '''
         Apply any modifications. This is application specific, but a general function is that it finalizes any changes made to an entity.
         '''
         
         print("apply is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def getNativeInstance(self) -> object:
+    def getNativeInstance(self
+    ):
         '''
         Get the native API's object instance. For example, in Blender API, this would return a bpy.object instance.
         '''
         
         print("getNativeInstance is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationWorld(self) -> 'Point':
+    def getLocationWorld(self
+    ) -> 'Point':
         '''
         Get the entities XYZ location relative to World Space.
         '''
         
         print("getLocationWorld is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationLocal(self) -> 'Point':
+    def getLocationLocal(self
+    ) -> 'Point':
         '''
         Get the entities XYZ location relative to Local Space.
         '''
         
         print("getLocationLocal is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def select(self):
+    def select(self
+    ):
         '''
         Select the entity (in UI).
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def export(self, filePath:str, overwrite:bool=True, scale:float=1.0):
+    def export(self, filePath:str, overwrite:bool=True, scale:float=1.0
+    ):
         '''
         Export Entity. Use the filePath to control the export type, e.g. '/path/to/cube.obj' or '/path/to/curve.svg'
         '''
         
         print("export is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def mirror(self, mirrorAcrossEntityOrLandmark:EntityOrItsNameOrLandmark, axis:AxisOrItsIndexOrItsName, resultingMirroredEntityName:Optional[str]=None):
+    def mirror(self, mirrorAcrossEntityOrLandmark:EntityOrItsNameOrLandmark, axis:AxisOrItsIndexOrItsName, resultingMirroredEntityName:Optional[str]=None
+    ):
         '''
         Mirror an existing entity with respect to a landmark. If a name is provided, the mirror becomes a separate entity.
         '''
         
         print("mirror is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def linearPattern(self, instanceCount:'int', offset:DimensionOrItsFloatOrStringValue, directionAxis:AxisOrItsIndexOrItsName="z"):
+    def linearPattern(self, instanceCount:'int', offset:DimensionOrItsFloatOrStringValue, directionAxis:AxisOrItsIndexOrItsName="z"
+    ):
         '''
         Pattern in a uniform direction.
         '''
         
         print("linearPattern is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def circularPattern(self, instanceCount:'int', separationAngle:AngleOrItsFloatOrStringValue, centerEntityOrLandmark:EntityOrItsNameOrLandmark, normalDirectionAxis:AxisOrItsIndexOrItsName="z"):
+    def circularPattern(self, instanceCount:'int', separationAngle:AngleOrItsFloatOrStringValue, centerEntityOrLandmark:EntityOrItsNameOrLandmark, normalDirectionAxis:AxisOrItsIndexOrItsName="z"
+    ):
         '''
         Pattern in a circular direction.
         '''
         
         print("circularPattern is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue):
+    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the XYZ directions. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("translateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateX(self, amount:DimensionOrItsFloatOrStringValue):
+    def translateX(self, amount:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the X direction. Pass a number or Dimension or Dimension-String (e.g. '2cm') to translate to a specific length.
         '''
         
         print("translateX is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateY(self, amount:DimensionOrItsFloatOrStringValue):
+    def translateY(self, amount:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the Y direction. Pass a number or Dimension or Dimension-String (e.g. '2cm') to translate to a specific length.
         '''
         
         print("translateY is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateZ(self, amount:DimensionOrItsFloatOrStringValue):
+    def translateZ(self, amount:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the z direction. Pass a number or Dimension or Dimension-String (e.g. '2cm') to translate to a specific length.
         '''
         
         print("translateZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue):
+    def scaleXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Scale in the XYZ directions. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("scaleXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleX(self, scale:DimensionOrItsFloatOrStringValue):
+    def scaleX(self, scale:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Scale in the X direction. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("scaleX is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleY(self, scale:DimensionOrItsFloatOrStringValue):
+    def scaleY(self, scale:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Scale in the Y direction. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("scaleY is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleZ(self, scale:DimensionOrItsFloatOrStringValue):
+    def scaleZ(self, scale:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Scale in the Z direction. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("scaleZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleXByFactor(self, scaleFactor:float):
+    def scaleXByFactor(self, scaleFactor:float
+    ):
         '''
         Scale in the X direction by a multiple.
         '''
         
         print("scaleXByFactor is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleYByFactor(self, scaleFactor:float):
+    def scaleYByFactor(self, scaleFactor:float
+    ):
         '''
         Scale in the Y direction by a multiple.
         '''
         
         print("scaleYByFactor is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleZByFactor(self, scaleFactor:float):
+    def scaleZByFactor(self, scaleFactor:float
+    ):
         '''
         Scale in the X direction by a multiple.
         '''
         
         print("scaleZByFactor is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def scaleKeepAspectRatio(self, scale:DimensionOrItsFloatOrStringValue, axis:AxisOrItsIndexOrItsName):
+    def scaleKeepAspectRatio(self, scale:DimensionOrItsFloatOrStringValue, axis:AxisOrItsIndexOrItsName
+    ):
         '''
         Scale in one axis and maintain the others. Pass a Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("scaleKeepAspectRatio is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue):
+    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the XYZ direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateX(self, rotation:AngleOrItsFloatOrStringValue):
+    def rotateX(self, rotation:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the X direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateX is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateY(self, rotation:AngleOrItsFloatOrStringValue):
+    def rotateY(self, rotation:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the Y direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateY is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateZ(self, rotation:AngleOrItsFloatOrStringValue):
+    def rotateZ(self, rotation:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the Z direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def twist(self, angle:AngleOrItsFloatOrStringValue, screwPitch:DimensionOrItsFloatOrStringValue, interations:'int'=1, axis:AxisOrItsIndexOrItsName="z"):
+    def twist(self, angle:AngleOrItsFloatOrStringValue, screwPitch:DimensionOrItsFloatOrStringValue, interations:'int'=1, axis:AxisOrItsIndexOrItsName="z"
+    ):
         '''
         AKA Helix, Screw. Revolve an entity
         '''
         
         print("twist is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def remesh(self, strategy:str, amount:float):
+    def remesh(self, strategy:str, amount:float
+    ):
         '''
         Remeshing should be capable of voxel or vertex based reconstruction, including decimating unnecessary vertices (if applicable).
         '''
         
         print("remesh is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createLandmark(self, landmarkName:str, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue) -> 'Landmark':
+    def createLandmark(self, landmarkName:str, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue
+    ) -> 'Landmark':
         '''
         Shortcut for creating and assigning a landmark to this entity. Returns a Landmark instance.
         '''
         
         print("createLandmark is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getBoundingBox(self) -> 'BoundaryBox':
+    def getBoundingBox(self
+    ) -> 'BoundaryBox':
         '''
         Get the Boundary Box around the entity.
         '''
         
         print("getBoundingBox is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getDimensions(self) -> 'Dimensions':
+    def getDimensions(self
+    ) -> 'Dimensions':
         '''
         Get the length span in each coordinate axis (X,Y,Z).
         '''
         
         print("getDimensions is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLandmark(self, landmarkName:PresetLandmarkOrItsName) -> 'Landmark':
+    def getLandmark(self, landmarkName:str
+    ) -> 'Landmark':
         '''
         Get the landmark by name
         '''
         
         print("getLandmark is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 class Part(Entity,metaclass=ABCMeta):
     '''Create and manipulate 3D shapes.'''
-
+    
     
 
     @abstractmethod
-    def createCube(self, width:DimensionOrItsFloatOrStringValue, length:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None):
+    def createFromFile(self, filePath:str, fileType:Optional[str]=None
+    ):
+        '''
+        Adds geometry to a part from a file. If the part does not exist, this will create it.
+        '''
+        
+        print("createFromFile is called in an abstract method. Please override this method.")
+        return self
+        
+
+    @abstractmethod
+    def createCube(self, width:DimensionOrItsFloatOrStringValue, length:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds cuboid geometry to a part.
         '''
         
         print("createCube is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createCone(self, radius:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, draftRadius:DimensionOrItsFloatOrStringValue=0, keywordArguments:Optional[dict]=None):
+    def createCone(self, radius:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, draftRadius:DimensionOrItsFloatOrStringValue=0, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds cone geometry to a part.
         '''
         
         print("createCone is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createCylinder(self, radius:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None):
+    def createCylinder(self, radius:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds cylinder geometry to a part.
         '''
         
         print("createCylinder is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createTorus(self, innerRadius:DimensionOrItsFloatOrStringValue, outerRadius:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None):
+    def createTorus(self, innerRadius:DimensionOrItsFloatOrStringValue, outerRadius:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds torus geometry to a part.
         '''
         
         print("createTorus is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createSphere(self, radius:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None):
+    def createSphere(self, radius:DimensionOrItsFloatOrStringValue, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds sphere geometry to a part.
         '''
         
         print("createSphere is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createGear(self, outerRadius:DimensionOrItsFloatOrStringValue, addendum:DimensionOrItsFloatOrStringValue, innerRadius:DimensionOrItsFloatOrStringValue, dedendum:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, pressureAngle:AngleOrItsFloatOrStringValue="20d", numberOfTeeth:'int'=12, skewAngle:AngleOrItsFloatOrStringValue=0, conicalAngle:AngleOrItsFloatOrStringValue=0, crownAngle:AngleOrItsFloatOrStringValue=0, keywordArguments:Optional[dict]=None):
+    def createGear(self, outerRadius:DimensionOrItsFloatOrStringValue, addendum:DimensionOrItsFloatOrStringValue, innerRadius:DimensionOrItsFloatOrStringValue, dedendum:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue, pressureAngle:AngleOrItsFloatOrStringValue="20d", numberOfTeeth:'int'=12, skewAngle:AngleOrItsFloatOrStringValue=0, conicalAngle:AngleOrItsFloatOrStringValue=0, crownAngle:AngleOrItsFloatOrStringValue=0, keywordArguments:Optional[dict]=None
+    ):
         '''
         Adds gear geometry to a part.
         '''
         
         print("createGear is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def clone(self, newName:str, copyLandmarks:bool=True) -> 'Part':
+    def clone(self, newName:str, copyLandmarks:bool=True
+    ) -> 'Part':
         '''
         Clone an existing Part with its geometry and properties. Returns the new Part.
         '''
         
         print("clone is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def loft(self, Landmark1:'Landmark', Landmark2:'Landmark'):
+    def loft(self, Landmark1:'Landmark', Landmark2:'Landmark'
+    ):
         '''
         Interpolate between two existing parts.
         '''
         
         print("loft is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def union(self, withPart:PartOrItsName, deleteAfterUnion:bool=True, isTransferLandmarks:bool=False):
+    def union(self, withPart:PartOrItsName, deleteAfterUnion:bool=True, isTransferLandmarks:bool=False
+    ):
         '''
         Boolean union
         '''
         
         print("union is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def subtract(self, withPart:PartOrItsName, deleteAfterSubtract:bool=True, isTransferLandmarks:bool=False):
+    def subtract(self, withPart:PartOrItsName, deleteAfterSubtract:bool=True, isTransferLandmarks:bool=False
+    ):
         '''
         Boolean subtraction
         '''
         
         print("subtract is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def intersect(self, withPart:PartOrItsName, deleteAfterIntersect:bool=True, isTransferLandmarks:bool=False):
+    def intersect(self, withPart:PartOrItsName, deleteAfterIntersect:bool=True, isTransferLandmarks:bool=False
+    ):
         '''
         Boolean intersection
         '''
         
         print("intersect is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def hollow(self, thicknessX:DimensionOrItsFloatOrStringValue, thicknessY:DimensionOrItsFloatOrStringValue, thicknessZ:DimensionOrItsFloatOrStringValue, startAxis:AxisOrItsIndexOrItsName="z", flipAxis:bool=False):
+    def hollow(self, thicknessX:DimensionOrItsFloatOrStringValue, thicknessY:DimensionOrItsFloatOrStringValue, thicknessZ:DimensionOrItsFloatOrStringValue, startAxis:AxisOrItsIndexOrItsName="z", flipAxis:bool=False
+    ):
         '''
         Remove vertices, if necessary, until the part has a specified wall thickness.
         '''
         
         print("hollow is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def hole(self, holeLandmark:LandmarkOrItsName, radius:DimensionOrItsFloatOrStringValue, depth:DimensionOrItsFloatOrStringValue, normalAxis:AxisOrItsIndexOrItsName="z", flipAxis:bool=False, initialRotationX:AngleOrItsFloatOrStringValue=0.0, initialRotationY:AngleOrItsFloatOrStringValue=0.0, initialRotationZ:AngleOrItsFloatOrStringValue=0.0, mirrorAboutEntityOrLandmark:Optional[EntityOrItsNameOrLandmark]=None, mirrorAxis:AxisOrItsIndexOrItsName="x", mirror:bool=False, circularPatternInstanceCount:'int'=1, circularPatternInstanceSeparation:AngleOrItsFloatOrStringValue=0.0, circularPatternInstanceAxis:AxisOrItsIndexOrItsName="z", circularPatternAboutEntityOrLandmark:Optional[EntityOrItsNameOrLandmark]=None, linearPatternInstanceCount:'int'=1, linearPatternInstanceSeparation:DimensionOrItsFloatOrStringValue=0.0, linearPatternInstanceAxis:AxisOrItsIndexOrItsName="x"):
+    def hole(self, holeLandmark:LandmarkOrItsName, radius:DimensionOrItsFloatOrStringValue, depth:DimensionOrItsFloatOrStringValue, normalAxis:AxisOrItsIndexOrItsName="z", flipAxis:bool=False, initialRotationX:AngleOrItsFloatOrStringValue=0.0, initialRotationY:AngleOrItsFloatOrStringValue=0.0, initialRotationZ:AngleOrItsFloatOrStringValue=0.0, mirrorAboutEntityOrLandmark:Optional[EntityOrItsNameOrLandmark]=None, mirrorAxis:AxisOrItsIndexOrItsName="x", mirror:bool=False, circularPatternInstanceCount:'int'=1, circularPatternInstanceSeparation:AngleOrItsFloatOrStringValue=0.0, circularPatternInstanceAxis:AxisOrItsIndexOrItsName="z", circularPatternAboutEntityOrLandmark:Optional[EntityOrItsNameOrLandmark]=None, linearPatternInstanceCount:'int'=1, linearPatternInstanceSeparation:DimensionOrItsFloatOrStringValue=0.0, linearPatternInstanceAxis:AxisOrItsIndexOrItsName="x"
+    ):
         '''
         Create a hole.
         '''
         
         print("hole is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setMaterial(self, materialName:MaterialOrItsName):
+    def setMaterial(self, materialName:MaterialOrItsName
+    ):
         '''
         Assign a known material to this part.
         '''
         
         print("setMaterial is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def isCollidingWithPart(self, otherPart:PartOrItsName) -> bool:
+    def isCollidingWithPart(self, otherPart:PartOrItsName
+    ):
         '''
         Check if this part is colliding with another.
         '''
         
         print("isCollidingWithPart is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def filletAllEdges(self, radius:DimensionOrItsFloatOrStringValue, useWidth:bool=False):
+    def filletAllEdges(self, radius:DimensionOrItsFloatOrStringValue, useWidth:bool=False
+    ):
         '''
         Fillet all edges.
         '''
         
         print("filletAllEdges is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def filletEdges(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearEdges:list[LandmarkOrItsName], useWidth:bool=False):
+    def filletEdges(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearEdges:list[LandmarkOrItsName], useWidth:bool=False
+    ):
         '''
         Fillet specific edges.
         '''
         
         print("filletEdges is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def filletFaces(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearFaces:list[LandmarkOrItsName], useWidth:bool=False):
+    def filletFaces(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearFaces:list[LandmarkOrItsName], useWidth:bool=False
+    ):
         '''
         Fillet specific faces.
         '''
         
         print("filletFaces is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def chamferAllEdges(self, radius:DimensionOrItsFloatOrStringValue):
+    def chamferAllEdges(self, radius:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Chamfer all edges.
         '''
         
         print("chamferAllEdges is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def chamferEdges(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearEdges:list[LandmarkOrItsName]):
+    def chamferEdges(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearEdges:list[LandmarkOrItsName]
+    ):
         '''
         Chamfer specific edges.
         '''
         
         print("chamferEdges is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def chamferFaces(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearFaces:list[LandmarkOrItsName]):
+    def chamferFaces(self, radius:DimensionOrItsFloatOrStringValue, landmarksNearFaces:list[LandmarkOrItsName]
+    ):
         '''
         Chamfer specific faces.
         '''
         
         print("chamferFaces is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def selectVertexNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None):
+    def selectVertexNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None
+    ):
         '''
         Select the vertex closest to a Landmark on the entity (in UI).
         '''
         
         print("selectVertexNearLandmark is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def selectEdgeNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None):
+    def selectEdgeNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None
+    ):
         '''
         Select an edge closest to a landmark on the entity (in UI).
         '''
         
         print("selectEdgeNearLandmark is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def selectFaceNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None):
+    def selectFaceNearLandmark(self, landmarkName:Optional[LandmarkOrItsName]=None
+    ):
         '''
         Select a face closest to a landmark on the entity (in UI).
         '''
         
         print("selectFaceNearLandmark is called in an abstract method. Please override this method.")
         return self
         
 class Sketch(Entity,metaclass=ABCMeta):
     '''Capabilities related to adding, multiplying, and/or modifying a curve.'''
-
+    
     
     name:str
     curveType:Optional['CurveTypes']=None
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, curveType:Optional['CurveTypes']=None, description:Optional[str]=None):
         super().__init__(name,description)
     
         self.name = name
         self.curveType = curveType
         self.description = description
 
     @abstractmethod
-    def clone(self, newName:str, copyLandmarks:bool=True) -> 'Sketch':
+    def clone(self, newName:str, copyLandmarks:bool=True
+    ) -> 'Sketch':
         '''
         Clone an existing sketch with its geometry and properties. Returns the new Sketch.
         '''
         
         print("clone is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def revolve(self, angle:AngleOrItsFloatOrStringValue, aboutEntityOrLandmark:EntityOrItsNameOrLandmark, axis:AxisOrItsIndexOrItsName="z"):
+    def revolve(self, angle:AngleOrItsFloatOrStringValue, aboutEntityOrLandmark:EntityOrItsNameOrLandmark, axis:AxisOrItsIndexOrItsName="z"
+    ):
         '''
         Revolve a Sketch around another Entity or Landmark
         '''
         
         print("revolve is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def thicken(self, radius:DimensionOrItsFloatOrStringValue):
-        '''
-        Uniformly add a wall around a sketch.
-        '''
-        
-        print("thicken is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def extrude(self, length:DimensionOrItsFloatOrStringValue) -> 'Part':
+    def extrude(self, length:DimensionOrItsFloatOrStringValue
+    ) -> 'Part':
         '''
         Extrude a curve by a specified length. Returns a Part type.
         '''
         
         print("extrude is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def sweep(self, profileNameOrInstance:SketchOrItsName, fillCap:bool=True):
+    def sweep(self, profileCurveName:str, fillCap:bool=False
+    ):
         '''
-        Extrude this Sketch along the path of another Sketch
+        Extrude this  curve along the path of another
         '''
         
         print("sweep is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def profile(self, profileCurveName:str):
+    def profile(self, profileCurveName:str
+    ):
         '''
         Bend this curve along the path of another
         '''
         
         print("profile is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createText(self, text:str, fontSize:DimensionOrItsFloatOrStringValue=1.0, bold:bool=False, italic:bool=False, underlined:bool=False, characterSpacing:'int'=1, wordSpacing:'int'=1, lineSpacing:'int'=1, fontFilePath:Optional[str]=None):
+    def createText(self, text:str, fontSize:DimensionOrItsFloatOrStringValue=1.0, bold:bool=False, italic:bool=False, underlined:bool=False, characterSpacing:'int'=1, wordSpacing:'int'=1, lineSpacing:'int'=1, fontFilePath:Optional[str]=None
+    ):
         '''
         Adds text to a sketch.
         '''
         
         print("createText is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createFromVertices(self, coordinates:list[PointOrListOfFloatOrItsStringValue], interpolation:'int'=64):
+    def createFromVertices(self, coordinates:list[PointOrListOfFloatOrItsStringValue], interpolation:'int'=64
+    ):
         '''
         Create a curve from 2D/3D points.
         '''
         
         print("createFromVertices is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createPoint(self, coordinate:PointOrListOfFloatOrItsStringValue):
+    def createPoint(self, coordinate:PointOrListOfFloatOrItsStringValue
+    ):
         '''
         Create a point
         '''
         
         print("createPoint is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createLine(self, length:DimensionOrItsFloatOrStringValue, angleX:AngleOrItsFloatOrStringValue=0.0, angleY:AngleOrItsFloatOrStringValue=0.0, symmetric:bool=False):
+    def createLine(self, length:DimensionOrItsFloatOrStringValue, angleX:AngleOrItsFloatOrStringValue=0.0, angleY:AngleOrItsFloatOrStringValue=0.0, symmetric:bool=False
+    ):
         '''
         Create a line
         '''
         
         print("createLine is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createLineBetweenPoints(self, endAt:PointOrListOfFloatOrItsStringValue, startAt:Optional[PointOrListOfFloatOrItsStringValue]=None):
+    def createLineBetweenPoints(self, endAt:PointOrListOfFloatOrItsStringValue, startAt:Optional[PointOrListOfFloatOrItsStringValue]=None
+    ):
         '''
         Create a line between two points
         '''
         
         print("createLineBetweenPoints is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createCircle(self, radius:DimensionOrItsFloatOrStringValue):
+    def createCircle(self, radius:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Create a circle
         '''
         
         print("createCircle is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createEllipse(self, radiusA:DimensionOrItsFloatOrStringValue, radiusB:DimensionOrItsFloatOrStringValue):
+    def createEllipse(self, radiusA:DimensionOrItsFloatOrStringValue, radiusB:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Create an ellipse
         '''
         
         print("createEllipse is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createArc(self, radius:DimensionOrItsFloatOrStringValue, angle:AngleOrItsFloatOrStringValue="180d"):
+    def createArc(self, radius:DimensionOrItsFloatOrStringValue, angle:AngleOrItsFloatOrStringValue="180d"
+    ):
         '''
         Create an arc
         '''
         
         print("createArc is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createArcBetweenThreePoints(self, pointA:'Point', pointB:'Point', centerPoint:'Point'):
+    def createArcBetweenThreePoints(self, pointA:'Point', pointB:'Point', centerPoint:'Point'
+    ):
         '''
         Create a 3-point arc
         '''
         
         print("createArcBetweenThreePoints is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createSegment(self, innerRadius:DimensionOrItsFloatOrStringValue, outerRadius:DimensionOrItsFloatOrStringValue, angle:AngleOrItsFloatOrStringValue="180d"):
+    def createSegment(self, innerRadius:DimensionOrItsFloatOrStringValue, outerRadius:DimensionOrItsFloatOrStringValue, angle:AngleOrItsFloatOrStringValue="180d"
+    ):
         '''
         Create a segment (intersection of two circles)
         '''
         
         print("createSegment is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createRectangle(self, length:DimensionOrItsFloatOrStringValue, width:DimensionOrItsFloatOrStringValue):
+    def createRectangle(self, length:DimensionOrItsFloatOrStringValue, width:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Create a rectangle
         '''
         
         print("createRectangle is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createPolygon(self, numberOfSides:'int', length:DimensionOrItsFloatOrStringValue, width:DimensionOrItsFloatOrStringValue):
+    def createPolygon(self, numberOfSides:'int', length:DimensionOrItsFloatOrStringValue, width:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Create an n-gon
         '''
         
         print("createPolygon is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createTrapezoid(self, lengthUpper:DimensionOrItsFloatOrStringValue, lengthLower:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue):
+    def createTrapezoid(self, lengthUpper:DimensionOrItsFloatOrStringValue, lengthLower:DimensionOrItsFloatOrStringValue, height:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Create a trapezoid
         '''
         
         print("createTrapezoid is called in an abstract method. Please override this method.")
         return self
         
-
-    @abstractmethod
-    def createSpiral(self, numberOfTurns:'int', height:DimensionOrItsFloatOrStringValue, radius:DimensionOrItsFloatOrStringValue, isClockwise:bool=True, radiusEnd:Optional[DimensionOrItsFloatOrStringValue]=None):
-        '''
-        Create a trapezoid
-        '''
-        
-        print("createSpiral is called in an abstract method. Please override this method.")
-        return self
-        
 class Landmark(metaclass=ABCMeta):
     '''Landmarks are named positions on an entity.'''
-
+    
     
     name:str
     parentEntity:EntityOrItsName
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, parentEntity:EntityOrItsName, description:Optional[str]=None):
         self.name = name
         self.parentEntity = parentEntity
         self.description = description
 
     @abstractmethod
-    def getLandmarkEntityName(self) -> str:
-        '''
-        Get the landmark object name in the scene, which may be different to the name of the landmark when it was first created. For example, the generated name may be {parentName}_{landmarkName}.
-        '''
+    def getLandmarkEntityName(self
+    ) -> str:
         
         print("getLandmarkEntityName is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getParentEntity(self) -> 'Entity':
-        '''
-        Get the name of the entity this landmark belongs to.
-        '''
+    def getParentEntity(self
+    ) -> 'Entity':
         
         print("getParentEntity is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def isExists(self) -> bool:
+    def isExists(self
+    ) -> bool:
         '''
         Check if an landmark exists
         '''
         
         print("isExists is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def rename(self, newName:str):
+    def rename(self, newName:str
+    ):
         '''
         Rename the landmark.
         '''
         
         print("rename is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def delete(self):
+    def delete(self
+    ):
         '''
         Delete the landmark from the scene.
         '''
         
         print("delete is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def isVisible(self) -> bool:
+    def isVisible(self
+    ) -> bool:
         '''
         Returns whether the landmark is visible in the scene.
         '''
         
         print("isVisible is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def setVisible(self, isVisible:bool):
+    def setVisible(self, isVisible:bool
+    ):
         '''
         Toggles visibility of an landmark in the scene.
         '''
         
         print("setVisible is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def getNativeInstance(self) -> object:
+    def getNativeInstance(self
+    ):
         '''
         Get the native API's object instance. For example, in Blender API, this would return a bpy.object instance.
         '''
         
         print("getNativeInstance is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationWorld(self) -> 'Point':
+    def getLocationWorld(self
+    ) -> 'Point':
         '''
         Get the landmark XYZ location relative to World Space.
         '''
         
         print("getLocationWorld is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationLocal(self) -> 'Point':
+    def getLocationLocal(self
+    ) -> 'Point':
         '''
         Get the landmark XYZ location relative to Local Space.
         '''
         
         print("getLocationLocal is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def select(self):
+    def select(self
+    ):
         '''
         Select the landmark (in UI).
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 class Joint(metaclass=ABCMeta):
     '''Joints define the relationships and constraints between entities.'''
-
+    
     
     entity1:EntityOrItsNameOrLandmark
     entity2:EntityOrItsNameOrLandmark
 
     @abstractmethod
     def __init__(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark):
         self.entity1 = entity1
         self.entity2 = entity2
 
     @abstractmethod
-    def translateLandmarkOntoAnother(self):
+    def translateLandmarkOntoAnother(self
+    ):
         '''
         Transforms one landmark onto another
         '''
         
         print("translateLandmarkOntoAnother is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def pivot(self):
+    def pivot(self
+    ):
         '''
         Constraint the rotation origin of entity B to entity A's landmark.
         '''
         
         print("pivot is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def gearRatio(self, ratio:float):
+    def gearRatio(self, ratio:float
+    ):
         '''
         Constraint the rotation of entity B to be a percentage of entity A's
         '''
         
         print("gearRatio is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitLocationXYZ(self, x:Optional[DimensionOrItsFloatOrStringValue]=None, y:Optional[DimensionOrItsFloatOrStringValue]=None, z:Optional[DimensionOrItsFloatOrStringValue]=None):
+    def limitLocationXYZ(self, x:Optional[DimensionOrItsFloatOrStringValue]=None, y:Optional[DimensionOrItsFloatOrStringValue]=None, z:Optional[DimensionOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the translation of entity B, relative to entity A's landmark.
         '''
         
         print("limitLocationXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitLocationX(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None):
+    def limitLocationX(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the translation of entity B, relative to entity A's landmark.
         '''
         
         print("limitLocationX is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitLocationY(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None):
+    def limitLocationY(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the translation of entity B, relative to entity A's landmark.
         '''
         
         print("limitLocationY is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitLocationZ(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None):
+    def limitLocationZ(self, min:Optional[DimensionOrItsFloatOrStringValue]=None, max:Optional[DimensionOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the translation of entity B, relative to entity A's landmark.
         '''
         
         print("limitLocationZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitRotationXYZ(self, x:Optional[AngleOrItsFloatOrStringValue]=None, y:Optional[AngleOrItsFloatOrStringValue]=None, z:Optional[AngleOrItsFloatOrStringValue]=None):
+    def limitRotationXYZ(self, x:Optional[AngleOrItsFloatOrStringValue]=None, y:Optional[AngleOrItsFloatOrStringValue]=None, z:Optional[AngleOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the rotation of entity B, relative to entity A's landmark.
         '''
         
         print("limitRotationXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitRotationX(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None):
+    def limitRotationX(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the rotation of entity B, relative to entity A's landmark.
         '''
         
         print("limitRotationX is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitRotationY(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None):
+    def limitRotationY(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the rotation of entity B, relative to entity A's landmark.
         '''
         
         print("limitRotationY is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def limitRotationZ(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None):
+    def limitRotationZ(self, min:Optional[AngleOrItsFloatOrStringValue]=None, max:Optional[AngleOrItsFloatOrStringValue]=None
+    ):
         '''
         Constraint the rotation of entity B, relative to entity A's landmark.
         '''
         
         print("limitRotationZ is called in an abstract method. Please override this method.")
         return self
         
 class Material(metaclass=ABCMeta):
     '''Materials affect the appearance and simulation properties of the parts.'''
-
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @abstractmethod
-    def assignToPart(self, partName:PartOrItsName):
-        '''
-        Assigns the material to a part.
-        '''
+    def assignToPart(self, partName:PartOrItsName
+    ):
         
         print("assignToPart is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setColor(self, rValue:IntOrFloat, gValue:IntOrFloat, bValue:IntOrFloat, aValue:IntOrFloat=1.0):
-        '''
-        Set the RGBA color of an entity. Supports 0-255 int or 0.0-1.0 float values.
-        '''
+    def setColor(self, rValue:IntOrFloat, gValue:IntOrFloat, bValue:IntOrFloat, aValue:IntOrFloat=1.0
+    ):
         
         print("setColor is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def addImageTexture(self, imageFilePath:str):
-        '''
-        Add a texture from an image file.
-        '''
+    def addImageTexture(self, imageFilePath:str
+    ):
         
         print("addImageTexture is called in an abstract method. Please override this method.")
         return self
         
 class Animation(metaclass=ABCMeta):
-    '''Animation related functionality.'''
-
+    '''Camera, lighting, rendering, animation related functionality.'''
+    
     
 
     @abstractmethod
     def __init__(self):
         pass
 
     @staticmethod
-    def default() -> 'Animation':
+    def default(
+    ) -> 'Animation':
         raise RuntimeError()
         
 
     @abstractmethod
-    def setFrameStart(self, frameNumber:'int'):
-        '''
-        Set the start animation frame in the scene.
-        '''
-        
-        print("setFrameStart is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setFrameEnd(self, frameNumber:'int'):
-        '''
-        Set the end animation frame in the scene.
-        '''
-        
-        print("setFrameEnd is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setFrameCurrent(self, frameNumber:'int'):
-        '''
-        Set the current animation frame in the scene.
-        '''
-        
-        print("setFrameCurrent is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def createKeyFrameLocation(self, entity:EntityOrItsName, frameNumber:'int'):
-        '''
-        Create an animation key-frame using the location of the entity.
-        '''
+    def createKeyFrameLocation(self, entity:EntityOrItsName, frameNumber:'int'
+    ):
         
         print("createKeyFrameLocation is called in an abstract method. Please override this method.")
-        return self
+        raise NotImplementedError()
         
 
     @abstractmethod
-    def createKeyFrameRotation(self, entity:EntityOrItsName, frameNumber:'int'):
-        '''
-        Create an animation key-frame using the rotation of the entity.
-        '''
+    def createKeyFrameRotation(self, entity:EntityOrItsName, frameNumber:'int'
+    ):
         
         print("createKeyFrameRotation is called in an abstract method. Please override this method.")
-        return self
+        raise NotImplementedError()
         
 class Light(metaclass=ABCMeta):
-    '''Manipulate a light object.'''
-
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @abstractmethod
-    def setColor(self, rValue:IntOrFloat, gValue:IntOrFloat, bValue:IntOrFloat):
-        '''
-        Set the color of an existing light.
-        '''
+    def setColor(self, rValue:IntOrFloat, gValue:IntOrFloat, bValue:IntOrFloat
+    ):
         
         print("setColor is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createSun(self, energyLevel:float):
-        '''
-        Create a Sun-type light.
-        '''
+    def createSun(self, energyLevel:float
+    ):
         
         print("createSun is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createSpot(self, energyLevel:float):
-        '''
-        Create a Spot-type light.
-        '''
+    def createSpot(self, energyLevel:float
+    ):
         
         print("createSpot is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createPoint(self, energyLevel:float):
-        '''
-        Create a Point-type light.
-        '''
+    def createPoint(self, energyLevel:float
+    ):
         
         print("createPoint is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createArea(self, energyLevel:float):
-        '''
-        Create an Area-type light.
-        '''
+    def createArea(self, energyLevel:float
+    ):
         
         print("createArea is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue):
+    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the XYZ directions. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("translateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue):
+    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the XYZ direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def isExists(self) -> bool:
+    def isExists(self
+    ) -> bool:
         '''
         Check if an light exists
         '''
         
         print("isExists is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def rename(self, newName:str):
+    def rename(self, newName:str
+    ):
         '''
         Rename the light.
         '''
         
         print("rename is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def delete(self):
+    def delete(self
+    ):
         '''
         Delete the light from the scene.
         '''
         
         print("delete is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def getNativeInstance(self) -> object:
+    def getNativeInstance(self
+    ):
         '''
         Get the native API's object instance. For example, in Blender API, this would return a bpy.object instance.
         '''
         
         print("getNativeInstance is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationWorld(self) -> 'Point':
+    def getLocationWorld(self
+    ) -> 'Point':
         '''
         Get the light XYZ location relative to World Space.
         '''
         
         print("getLocationWorld is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationLocal(self) -> 'Point':
+    def getLocationLocal(self
+    ) -> 'Point':
         '''
         Get the light XYZ location relative to Local Space.
         '''
         
         print("getLocationLocal is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def select(self):
+    def select(self
+    ):
         '''
         Select the light (in UI).
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
 class Camera(metaclass=ABCMeta):
-    '''Manipulate a camera object.'''
-
+    
     
     name:str
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:str, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @abstractmethod
-    def createPerspective(self):
-        '''
-        Create a perspective camera in the scene.
-        '''
+    def createPerspective(self
+    ):
         
         print("createPerspective is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createOrthogonal(self):
-        '''
-        Create an orthogonal camera in the scene.
-        '''
+    def createOrthogonal(self
+    ):
         
         print("createOrthogonal is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setFocalLength(self, length:float):
-        '''
-        Set the focal length of the camera.
-        '''
+    def setFocalLength(self, length:float
+    ):
         
         print("setFocalLength is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue):
+    def translateXYZ(self, x:DimensionOrItsFloatOrStringValue, y:DimensionOrItsFloatOrStringValue, z:DimensionOrItsFloatOrStringValue
+    ):
         '''
         Translate in the XYZ directions. Pass a number, Dimension or Dimension-String (e.g. '2cm') to scale to a specific length.
         '''
         
         print("translateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue):
+    def rotateXYZ(self, x:AngleOrItsFloatOrStringValue, y:AngleOrItsFloatOrStringValue, z:AngleOrItsFloatOrStringValue
+    ):
         '''
         Rotate in the XYZ direction. Default units is degrees. Pass in a number, Angle or Angle-String (e.g. 'PI/4radians' or 'PI/4r' or '90d'
         '''
         
         print("rotateXYZ is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def isExists(self) -> bool:
+    def isExists(self
+    ) -> bool:
         '''
         Check if an camera exists
         '''
         
         print("isExists is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def rename(self, newName:str):
+    def rename(self, newName:str
+    ):
         '''
         Rename the camera.
         '''
         
         print("rename is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def delete(self):
+    def delete(self
+    ):
         '''
         Delete the camera from the scene.
         '''
         
         print("delete is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def getNativeInstance(self) -> object:
+    def getNativeInstance(self
+    ):
         '''
         Get the native API's object instance. For example, in Blender API, this would return a bpy.object instance.
         '''
         
         print("getNativeInstance is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationWorld(self) -> 'Point':
+    def getLocationWorld(self
+    ) -> 'Point':
         '''
         Get the camera XYZ location relative to World Space.
         '''
         
         print("getLocationWorld is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getLocationLocal(self) -> 'Point':
+    def getLocationLocal(self
+    ) -> 'Point':
         '''
         Get the camera XYZ location relative to Local Space.
         '''
         
         print("getLocationLocal is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def select(self):
+    def select(self
+    ):
         '''
         Select the entity (in UI).
         '''
         
         print("select is called in an abstract method. Please override this method.")
         return self
         
-class Render(metaclass=ABCMeta):
-    '''Render the scene and export images or videos.'''
-
-    
-
-    @abstractmethod
-    def renderImage(self, outputFilePath:str, overwrite:bool=True, fileType:Optional[str]=None):
-        '''
-        Render a still image.
-        '''
-        
-        print("renderImage is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def renderVideoMp4(self, outputFilePath:str, startFrameNumber:'int'=1, endFrameNumber:'int'=100, stepFrames:'int'=1, overwrite:bool=True):
-        '''
-        Render an MP4 video.
-        '''
-        
-        print("renderVideoMp4 is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def renderVideoFrames(self, outputFolderPath:str, fileNamePrefix:str, startFrameNumber:'int'=1, endFrameNumber:'int'=100, stepFrames:'int'=1, overwrite:bool=True, fileType:Optional[str]=None):
-        '''
-        Render a video as image frame stills.
-        '''
-        
-        print("renderVideoFrames is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setFrameRate(self, frameRate:'int'):
-        '''
-        Set rendering framerate.
-        '''
-        
-        print("setFrameRate is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setResolution(self, x:'int', y:'int'):
-        '''
-        Set rendering resolution
-        '''
-        
-        print("setResolution is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setRenderQuality(self, quality:'int'):
-        '''
-        Set rendering quality.
-        '''
-        
-        print("setRenderQuality is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setRenderEngine(self, name:str):
-        '''
-        Set rendering engine name.
-        '''
-        
-        print("setRenderEngine is called in an abstract method. Please override this method.")
-        return self
-        
-
-    @abstractmethod
-    def setCamera(self, cameraNameOrInstance:CameraOrItsName):
-        '''
-        Set the rendering camera.
-        '''
-        
-        print("setCamera is called in an abstract method. Please override this method.")
-        return self
-        
 class Scene(metaclass=ABCMeta):
     '''Scene, camera, lighting, rendering, animation, simulation and GUI related functionality.'''
-
+    
     
     name:Optional[str]=None
     description:Optional[str]=None
 
     @abstractmethod
     def __init__(self, name:Optional[str]=None, description:Optional[str]=None):
         self.name = name
         self.description = description
 
     @staticmethod
-    def default() -> 'Scene':
+    def default(
+    ) -> 'Scene':
         raise RuntimeError()
         
 
     @abstractmethod
-    def create(self):
+    def create(self
+    ):
         '''
-        Creates a new scene.
+        Creates a new scene
         '''
         
         print("create is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def delete(self):
+    def delete(self
+    ):
         '''
-        Deletes a scene.
+        Deletes a scene
         '''
         
         print("delete is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def getSelectedEntity(self) -> 'Entity':
-        '''
-        Get the selected entity in the Scene.
-        '''
-        
-        print("getSelectedEntity is called in an abstract method. Please override this method.")
-        raise NotImplementedError()
-        
-
-    @abstractmethod
-    def export(self, filePath:str, entities:list[EntityOrItsName], overwrite:bool=True, scale:float=1.0):
+    def export(self, filePath:str, entities:list[EntityOrItsName], overwrite:bool=True, scale:float=1.0
+    ):
         '''
         Export the entire scene or specific entities.
         '''
         
         print("export is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setDefaultUnit(self, unit:LengthUnitOrItsName):
+    def setDefaultUnit(self, unit:LengthUnitOrItsName
+    ):
         '''
         Set the document's default measurements system.
         '''
         
         print("setDefaultUnit is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def createGroup(self, name:str):
+    def createGroup(self, name:str
+    ):
         '''
         Create a new group
         '''
         
         print("createGroup is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def deleteGroup(self, name:str, removeChildren:bool):
+    def deleteGroup(self, name:str, removeChildren:bool
+    ):
         '''
         Delete a new group
         '''
         
         print("deleteGroup is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def removeFromGroup(self, entityName:str, groupName:str):
+    def removeFromGroup(self, entityName:str, groupName:str
+    ):
         '''
         Removes an existing entity from a group
         '''
         
         print("removeFromGroup is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def assignToGroup(self, entities:list[EntityOrItsName], groupName:str, removeFromOtherGroups:Optional[bool]=True):
+    def assignToGroup(self, entities:list[EntityOrItsName], groupName:str, removeFromOtherGroups:Optional[bool]=True
+    ):
         '''
         Assigns an existing entity to a new group
         '''
         
         print("assignToGroup is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setVisible(self, entities:list[EntityOrItsName], isVisible:bool):
+    def setVisible(self, entities:list[EntityOrItsName], isVisible:bool
+    ):
         '''
         Change the visibiltiy of the entity.
         '''
         
         print("setVisible is called in an abstract method. Please override this method.")
         return self
         
 
     @abstractmethod
-    def setBackgroundImage(self, filePath:str, locationX:Optional[DimensionOrItsFloatOrStringValue]=0, locationY:Optional[DimensionOrItsFloatOrStringValue]=0):
+    def setBackgroundImage(self, filePath:str, locationX:Optional[DimensionOrItsFloatOrStringValue]=0, locationY:Optional[DimensionOrItsFloatOrStringValue]=0
+    ):
         '''
         Set the scene background image. This can be an image or an HDRI texture.
         '''
         
         print("setBackgroundImage is called in an abstract method. Please override this method.")
         return self
         
 class Analytics(metaclass=ABCMeta):
     '''Tools for collecting data about the entities and scene.'''
-
+    
     
 
     @abstractmethod
     def __init__(self):
         pass
 
     @abstractmethod
-    def measureDistance(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark) -> 'Dimensions':
+    def measureDistance(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark
+    ) -> 'Dimensions':
         '''
         The ubiquitous ruler.
         '''
         
         print("measureDistance is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def measureAngle(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark, pivot:Optional[EntityOrItsNameOrLandmark]=None) -> 'list[Angle]':
+    def measureAngle(self, entity1:EntityOrItsNameOrLandmark, entity2:EntityOrItsNameOrLandmark, pivot:Optional[EntityOrItsNameOrLandmark]=None
+    ) -> 'list[Angle]':
         '''
         The ubiquitous ruler.
         '''
         
         print("measureAngle is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getWorldPose(self, entity:EntityOrItsName) -> 'list[float]':
+    def getWorldPose(self, entity:EntityOrItsName
+    ) -> 'list[float]':
         '''
         Returns the world pose of an entity.
         '''
         
         print("getWorldPose is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getBoundingBox(self, entityName:EntityOrItsName) -> 'BoundaryBox':
+    def getBoundingBox(self, entityName:EntityOrItsName
+    ) -> 'BoundaryBox':
         '''
         Returns the bounding box of an entity.
         '''
         
         print("getBoundingBox is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
 
     @abstractmethod
-    def getDimensions(self, entityName:EntityOrItsName) -> 'Dimensions':
+    def getDimensions(self, entityName:EntityOrItsName
+    ) -> 'Dimensions':
         '''
         Returns the dimensions of an entity.
         '''
         
         print("getDimensions is called in an abstract method. Please override this method.")
         raise NotImplementedError()
         
-
-    @abstractmethod
-    def log(self, message:str):
-        '''
-        Write a message
-        '''
-        
-        print("log is called in an abstract method. Please override this method.")
-        return self
-
```

### Comparing `CodeToCAD-0.2.1687027263/CodeToCAD/TestCodeToCADProvider.py` & `CodeToCAD-0.2.6/CodeToCAD/TestCodeToCADProvider.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,23 +19,14 @@
         # inject provider?
         super().setUp()
 
 class TestEntity(TestProviderCase):
     
     
     @unittest.skip
-    def test_createFromFile(self):
-        instance = Part("name","description")
-
-        value = instance.createFromFile("filePath","fileType")
-
-        
-        assert value.isExists(), "Create method failed."
-        
-    @unittest.skip
     def test_isExists(self):
         instance = Part("name","description")
 
         value = instance.isExists("")
 
         
         assert value, "Get method failed."
@@ -72,15 +63,15 @@
         value = instance.setVisible("isVisible")
 
         
     @unittest.skip
     def test_apply(self):
         instance = Part("name","description")
 
-        value = instance.apply("rotation","scale","location","modifiers")
+        value = instance.apply("")
 
         
         assert value, "Modify method failed."
         
     @unittest.skip
     def test_getNativeInstance(self):
         instance = Part("name","description")
@@ -346,14 +337,23 @@
 
         
         assert value, "Get method failed."
         
 class TestPart(TestProviderCase):
     
     @unittest.skip
+    def test_createFromFile(self):
+        instance = Part("")
+
+        value = instance.createFromFile("filePath","fileType")
+
+        
+        assert value.isExists(), "Create method failed."
+        
+    @unittest.skip
     def test_createCube(self):
         instance = Part("")
 
         value = instance.createCube("width","length","height","keywordArguments")
 
         
         assert value.isExists(), "Create method failed."
@@ -577,36 +577,27 @@
 
         value = instance.revolve("angle","aboutEntityOrLandmark","axis")
 
         
         assert value, "Modify method failed."
         
     @unittest.skip
-    def test_thicken(self):
-        instance = Sketch("name","curveType","description")
-
-        value = instance.thicken("radius")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
     def test_extrude(self):
         instance = Sketch("name","curveType","description")
 
         value = instance.extrude("length")
 
         
         assert value, "Get method failed."
         
     @unittest.skip
     def test_sweep(self):
         instance = Sketch("name","curveType","description")
 
-        value = instance.sweep("profileNameOrInstance","fillCap")
+        value = instance.sweep("profileCurveName","fillCap")
 
         
         assert value, "Modify method failed."
         
     @unittest.skip
     def test_profile(self):
         instance = Sketch("name","curveType","description")
@@ -729,23 +720,14 @@
         instance = Sketch("name","curveType","description")
 
         value = instance.createTrapezoid("lengthUpper","lengthLower","height")
 
         
         assert value.isExists(), "Create method failed."
         
-    @unittest.skip
-    def test_createSpiral(self):
-        instance = Sketch("name","curveType","description")
-
-        value = instance.createSpiral("numberOfTurns","height","radius","isClockwise","radiusEnd")
-
-        
-        assert value.isExists(), "Create method failed."
-        
 class TestLandmark(TestProviderCase):
     
     
     @unittest.skip
     def test_getLandmarkEntityName(self):
         instance = Landmark("name","parentEntity","description")
 
@@ -971,61 +953,29 @@
         assert value, "Modify method failed."
         
 class TestAnimation(TestProviderCase):
     
     
     
     @unittest.skip
-    def test_setFrameStart(self):
-        instance = Animation("")
-
-        value = instance.setFrameStart("frameNumber")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setFrameEnd(self):
-        instance = Animation("")
-
-        value = instance.setFrameEnd("frameNumber")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setFrameCurrent(self):
-        instance = Animation("")
-
-        value = instance.setFrameCurrent("frameNumber")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
     def test_createKeyFrameLocation(self):
         instance = Animation("")
 
         value = instance.createKeyFrameLocation("entity","frameNumber")
 
         
-        assert value, "Modify method failed."
-        
     @unittest.skip
     def test_createKeyFrameRotation(self):
         instance = Animation("")
 
         value = instance.createKeyFrameRotation("entity","frameNumber")
 
         
-        assert value, "Modify method failed."
-        
 class TestLight(TestProviderCase):
     
-    
     @unittest.skip
     def test_setColor(self):
         instance = Light("name","description")
 
         value = instance.setColor("rValue","gValue","bValue")
 
         
@@ -1142,15 +1092,14 @@
         instance = Light("name","description")
 
         value = instance.select("")
 
         
 class TestCamera(TestProviderCase):
     
-    
     @unittest.skip
     def test_createPerspective(self):
         instance = Camera("name","description")
 
         value = instance.createPerspective("")
 
         
@@ -1247,82 +1196,14 @@
     @unittest.skip
     def test_select(self):
         instance = Camera("name","description")
 
         value = instance.select("")
 
         
-class TestRender(TestProviderCase):
-    
-    @unittest.skip
-    def test_renderImage(self):
-        instance = Render("")
-
-        value = instance.renderImage("outputFilePath","overwrite","fileType")
-
-        
-    @unittest.skip
-    def test_renderVideoMp4(self):
-        instance = Render("")
-
-        value = instance.renderVideoMp4("outputFilePath","startFrameNumber","endFrameNumber","stepFrames","overwrite")
-
-        
-    @unittest.skip
-    def test_renderVideoFrames(self):
-        instance = Render("")
-
-        value = instance.renderVideoFrames("outputFolderPath","fileNamePrefix","startFrameNumber","endFrameNumber","stepFrames","overwrite","fileType")
-
-        
-    @unittest.skip
-    def test_setFrameRate(self):
-        instance = Render("")
-
-        value = instance.setFrameRate("frameRate")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setResolution(self):
-        instance = Render("")
-
-        value = instance.setResolution("x","y")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setRenderQuality(self):
-        instance = Render("")
-
-        value = instance.setRenderQuality("quality")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setRenderEngine(self):
-        instance = Render("")
-
-        value = instance.setRenderEngine("name")
-
-        
-        assert value, "Modify method failed."
-        
-    @unittest.skip
-    def test_setCamera(self):
-        instance = Render("")
-
-        value = instance.setCamera("cameraNameOrInstance")
-
-        
-        assert value, "Modify method failed."
-        
 class TestScene(TestProviderCase):
     
     
     
     @unittest.skip
     def test_create(self):
         instance = Scene("name","description")
@@ -1336,38 +1217,27 @@
     def test_delete(self):
         instance = Scene("name","description")
 
         value = instance.delete("")
 
         
     @unittest.skip
-    def test_getSelectedEntity(self):
-        instance = Scene("name","description")
-
-        value = instance.getSelectedEntity("")
-
-        
-        assert value, "Get method failed."
-        
-    @unittest.skip
     def test_export(self):
         instance = Scene("name","description")
 
         value = instance.export("filePath","entities","overwrite","scale")
 
         
     @unittest.skip
     def test_setDefaultUnit(self):
         instance = Scene("name","description")
 
         value = instance.setDefaultUnit("unit")
 
         
-        assert value, "Modify method failed."
-        
     @unittest.skip
     def test_createGroup(self):
         instance = Scene("name","description")
 
         value = instance.createGroup("name")
 
         
@@ -1390,25 +1260,21 @@
     @unittest.skip
     def test_assignToGroup(self):
         instance = Scene("name","description")
 
         value = instance.assignToGroup("entities","groupName","removeFromOtherGroups")
 
         
-        assert value, "Modify method failed."
-        
     @unittest.skip
     def test_setVisible(self):
         instance = Scene("name","description")
 
         value = instance.setVisible("entities","isVisible")
 
         
-        assert value, "Modify method failed."
-        
     @unittest.skip
     def test_setBackgroundImage(self):
         instance = Scene("name","description")
 
         value = instance.setBackgroundImage("filePath","locationX","locationY")
 
         
@@ -1458,16 +1324,7 @@
         instance = Analytics("")
 
         value = instance.getDimensions("entityName")
 
         
         assert value, "Get method failed."
         
-    @unittest.skip
-    def test_log(self):
-        instance = Analytics("")
-
-        value = instance.log("message")
-
-        
-        assert value, "Modify method failed."
-
```

### Comparing `CodeToCAD-0.2.1687027263/CodeToCAD/__init__.py` & `CodeToCAD-0.2.6/CodeToCAD/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # This is the CodeToCAD provider.
 # Use the following import line in your CodeToCAD file:
 # from CodeToCAD import Part, Shape, Sketch, Curve, Landmark, Scene, Analytics, Joint, Material, Animation, min, max, center, Dimension, Dimensions, Angle
 
 min: str = Utilities.min
 max: str = Utilities.max
 center: str = Utilities.center
-PresetLandmark: Type[Utilities.PresetLandmark] = Utilities.PresetLandmark
 Dimension: Type[Utilities.Dimension] = Utilities.Dimension
 Dimensions: Type[Utilities.Dimensions] = Utilities.Dimensions
 Angle: Type[Utilities.Angle] = Utilities.Angle
 
 Part: Type[CodeToCADInterface.Part] = CodeToCADInterface.Part
 Shape: Type[CodeToCADInterface.Part] = CodeToCADInterface.Part
 Sketch: Type[CodeToCADInterface.Sketch] = CodeToCADInterface.Sketch
@@ -22,15 +21,14 @@
 Scene: Type[CodeToCADInterface.Scene] = CodeToCADInterface.Scene
 Analytics: Type[CodeToCADInterface.Analytics] = CodeToCADInterface.Analytics
 Joint: Type[CodeToCADInterface.Joint] = CodeToCADInterface.Joint
 Material: Type[CodeToCADInterface.Material] = CodeToCADInterface.Material
 Animation: Type[CodeToCADInterface.Animation] = CodeToCADInterface.Animation
 Camera: Type[CodeToCADInterface.Camera] = CodeToCADInterface.Camera
 Light: Type[CodeToCADInterface.Light] = CodeToCADInterface.Light
-Render: Type[CodeToCADInterface.Render] = CodeToCADInterface.Render
 
 
 def setPartProvider(provider: Type[CodeToCADInterface.Part], globalContext: Optional[dict]) -> None:
     global Part, Shape
     Part = provider
     Shape = provider
     if globalContext and "Part" in globalContext:
@@ -99,14 +97,7 @@
 
 
 def setLightProvider(provider, globalContext: Optional[dict]) -> None:
     global Light
     Light = provider
     if globalContext and "Light" in globalContext:
         globalContext["Light"] = provider
-
-
-def setRenderProvider(provider, globalContext: Optional[dict]) -> None:
-    global Render
-    Render = provider
-    if globalContext and "Render" in globalContext:
-        globalContext["Render"] = provider
```

### Comparing `CodeToCAD-0.2.1687027263/CodeToCAD/utilities.py` & `CodeToCAD-0.2.6/CodeToCAD/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,106 +10,46 @@
 from typing import Optional, Union
 
 
 min = "min"
 max = "max"
 center = "center"
 
-reservedWords = [min, max, center]
-
-
-class PresetLandmark(Enum):
-    left = 2
-    right = 4
-    top = 8
-    bottom = 16
-    front = 32
-    back = 64
-    center = 128
-    leftTop = left | top
-    leftBottom = left | bottom
-    leftFront = left | front
-    leftBack = left | back
-    rightTop = right | top
-    rightBottom = right | bottom
-    rightFront = right | front
-    rightBack = right | back
-    frontTop = front | top
-    backTop = back | top
-    frontBottom = front | bottom
-    backBottom = back | bottom
-    leftFrontTop = left | front | top
-    leftBackTop = left | back | top
-    leftFrontBottom = left | front | bottom
-    leftBackBottom = left | back | bottom
-    rightFrontTop = right | front | top
-    rightBackTop = right | back | top
-    rightFrontBottom = right | front | bottom
-    rightBackBottom = right | back | bottom
-
-    def __ror__(self, other):
-        return self.value | other.value
-
-    def __and__(self, other):
-        return self.value & other.value
-
-    def contains(self, other):
-        return (self & other == other.value)
-
-    @staticmethod
-    def fromString(landmarkName) -> Optional['PresetLandmark']:
-        for preset in PresetLandmark:
-            if preset.name == landmarkName:
-                return preset
-        return None
-
-    def getXYZ(self):
-        x = min if self.contains(PresetLandmark.left) else max if self.contains(
-            PresetLandmark.right) else center
-        y = min if self.contains(PresetLandmark.front) else max if self.contains(
-            PresetLandmark.back) else center
-        z = min if self.contains(PresetLandmark.bottom) else max if self.contains(
-            PresetLandmark.top) else center
-        return (x, y, z)
+reservedWords = ["min", "max", "center"]
 
 
 def isReservedWordInString(stringToCheck: str) -> bool:
     for word in reservedWords:
         if word in stringToCheck:
             return True
     return False
 
 
 def getFilename(relativeFilePath: str):
     path = Path(relativeFilePath)
     return path.stem
 
 
-def getFileExtension(filePath: str):
-    path = Path(filePath)
-    return path.suffix.replace(".", "")
+def createUUIDLikeId():
+    return str(uuid4()).replace("-", "")[:10]
+
+
+def formatLandmarkEntityName(parentEntityName: str, landmarkName: str):
+    return f"{parentEntityName}_{landmarkName}"
 
 
 def getAbsoluteFilepath(relativeFilePath: str):
     path = Path(relativeFilePath)
     absoluteFilePath = relativeFilePath
     if not path.is_absolute():
         absoluteFilePath = str(
             Path(sys.argv[0]).parent.joinpath(path).resolve())
     return absoluteFilePath
 
 
-def createUUIDLikeId():
-    return str(uuid4()).replace("-", "")[:10]
-
-
-def formatLandmarkEntityName(parentEntityName: str, landmarkName: str):
-    return f"{parentEntityName}_{landmarkName}"
-
-
 class EquittableEnum(Enum):
     # define the == operator, otherwise we can't compare enums, thanks python
     def __eq__(self, other):
         return type(self) == type(other) and self.value == other.value
 
 
 class Units(EquittableEnum):
@@ -134,15 +74,15 @@
             "d": AngleUnit.DEGREES
         }
 
         fromString: str = name.lower().replace("(s)", "")
 
         parsedUnit: Optional[AngleUnit] = aliases[fromString] if fromString in aliases else None
 
-        assert parsedUnit is not None, f"Could not parse unit {fromString}"
+        assert parsedUnit != None, f"Could not parse unit {fromString}"
 
         return parsedUnit
 
 
 class Angle():
 
     def toRadians(self) -> 'Angle':
@@ -228,37 +168,32 @@
         return Angle(pow(self.value, other.value, mod), self.unit)
 
     def __abs__(self):
         return Angle(abs(self.value), self.unit)
 
     def __lt__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value < other.value
 
     def __le__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value <= other.value
 
     def __gt__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value > other.value
 
     def __ge__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value >= other.value
 
     def __eq__(self, other):
         if other == None:
             return False
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value == other.value
 
     def __ne__(self, other):
         return not (self == other)
 
     def __copy__(self):
         return self.__deepcopy__()
@@ -326,15 +261,15 @@
 
     if type(angleString) == str:
         angleString = angleString.replace(" ", "").lower()
         angleString = re.search('[A-Za-z]+$', angleString)
 
         unitInString = AngleUnit.fromString(
             angleString[0]) if angleString else None
-        if unitInString is not None and angleString is not None:
+        if unitInString != None and angleString != None:
             defaultUnit = unitInString
             if len(angleString[0]) == len(anglesList[-1]):
                 anglesList.pop()
 
     parsedAngles = []
     for angle in anglesList:
         parsedAngles.append(Angle.fromString(angle, defaultUnit))
@@ -387,15 +322,15 @@
             "mi": LengthUnit.mi
         }
 
         fromString: str = name.lower().replace("(s)", "")
 
         parsedUnit: LengthUnit | None = aliases[fromString] if fromString in aliases else None
 
-        assert parsedUnit is not None, f"Could not parse unit {fromString}"
+        assert parsedUnit != None, f"Could not parse unit {fromString}"
 
         return parsedUnit
 
 
 class Axis(EquittableEnum):
     X = 0
     Y = 1
@@ -427,63 +362,37 @@
     Segment = 7
     Rectangle = 8
     Rhomb = 9
     Trapezoid = 10
     Polygon = 11
     Polygon_ab = 12
     Arc = 13
-    Spiral = 14
 
 
 class CurveTypes(EquittableEnum):
     POLY = 0
     NURBS = 1
     BEZIER = 2
 
 
-class FileFormats(EquittableEnum):
-    PNG = 0
-    JPEG = 1
-    OPEN_EXR = 2
-    MP4 = 3
-
-    @staticmethod
-    def fromString(name: str):
-        name = name.lower()
-        if name == "png":
-            return FileFormats.PNG
-        if name == "jpg" or name == "jpeg":
-            return FileFormats.JPEG
-        if name == "exr" or name == "openexr":
-            return FileFormats.OPEN_EXR
-        if name == "mp4" or "ffmpeg":
-            return FileFormats.MP4
-
-        raise TypeError(f"{name} is not a supported file type.")
-
-
 class ScalingMethods(Enum):
     toSpecificLength = 0
     scaleFactor = 1
     lockAspectRatio = 2  # scale one dimension, the others scale with it
 
 
 class ConstraintTypes(EquittableEnum):
     # Translation locked between specified start and end points in all axes.
-    LimitLocation = 0
+    Translation = 0
     # Rotation locked between specified start and end angles in all axes.
-    LimitRotation = 1
+    Rotation = 1
     # Rotation locked between specified start and end angles in all axes, but rotation origin is offset.
     Pivot = 2
     # Rotation of one object is a percentage of another's in a specified axis.
     Gear = 3
-    # Fixed position:
-    FixedPosition = 4
-    # Fixed rotation:
-    FixedRotation = 5
 
 
 class BoundaryAxis:
     min: float
     max: float
     unit: Optional[LengthUnit]
 
@@ -562,94 +471,89 @@
     def __str__(self) -> str:
         return f"{self.value}{' '+self.unit.name if self.unit else ''}"
 
     def __repr__(self) -> str:
         return self.__str__()
 
     def convertToUnit(self, targetUnit: LengthUnit) -> 'Dimension':
-        assert self.unit is not None, f"Current dimension does not have a unit."
+        assert self.unit != None, f"Current dimension does not have a unit."
         targetUnit = LengthUnit.fromString(targetUnit) if not isinstance(
             targetUnit, LengthUnit) else targetUnit
         assert isinstance(
             targetUnit, LengthUnit), f"Could not convert to unit {targetUnit}"
 
         newDimension = Dimension(
             self.value * (self.unit.value/targetUnit.value),
             targetUnit
         )
         return newDimension
 
     def arithmeticPrecheckAndUnitConversion(self, other) -> 'Dimension':
-        assert other is not None, "Right-hand value cannot be None."
+        assert other != None, "Right-hand value cannot be None."
         if not isinstance(other, Dimension):
             other = Dimension.fromString(other)
-        if other.unit is not None and self.unit is not None and other.unit != self.unit:
+        if other.unit != None and other.unit != self.unit:
             other = other.convertToUnit(self.unit)
         return other
 
     def __add__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value + other.value, self.unit or other.unit)
+        return Dimension(self.value + other.value, self.unit)
 
     def __sub__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value - other.value, self.unit or other.unit)
+        return Dimension(self.value - other.value, self.unit)
 
     def __mul__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value * other.value, self.unit or other.unit)
+        return Dimension(self.value * other.value, self.unit)
 
     def __truediv__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value / other.value, self.unit or other.unit)
+        return Dimension(self.value / other.value, self.unit)
 
     def __floordiv__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value // other.value, self.unit or other.unit)
+        return Dimension(self.value // other.value, self.unit)
 
     def __mod__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(self.value % other.value, self.unit or other.unit)
+        return Dimension(self.value % other.value, self.unit)
 
     # def __divmod__(self, other):
     #     other = self.arithmeticPrecheckAndUnitConversion(other)
     #     return Dimension(divmod(self.value, other.value), self.unit)
 
     def __pow__(self, other, mod=None):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        return Dimension(pow(self.value, other.value, mod), self.unit or other.unit)
+        return Dimension(pow(self.value, other.value, mod), self.unit)
 
     def __abs__(self):
         return Dimension(abs(self.value), self.unit)
 
     def __lt__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value < other.value
 
     def __le__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value <= other.value
 
     def __gt__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value > other.value
 
     def __ge__(self, other):
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value >= other.value
 
     def __eq__(self, other):
         if other == None:
             return False
         other = self.arithmeticPrecheckAndUnitConversion(other)
-        assert self.unit == other.unit, "Units are not matching for comparison."
         return self.value == other.value
 
     def __ne__(self, other):
         return not (self == other)
 
     def __copy__(self):
         return self.__deepcopy__()
@@ -691,20 +595,17 @@
         if unitInString:
             value = fromString[0:-1*len(unitInString)]
             unitInString = LengthUnit.fromString(unitInString)
             unit = unitInString or unit
 
         # if min,max,center is used, try to parse those words into their respective values.
         if isReservedWordInString(value):
-            assert boundaryAxis is not None, "min,max,center keywords used, but boundaryAxis is not known."
+            assert boundaryAxis != None, "min,max,center keywords used, but boundaryAxis is not known."
             if unit == None:
                 unit = boundaryAxis.unit
-
-            assert unit, "Could not determine the unit to convert the boundary axis."
-
             value = replaceMinMaxCenterWithRespectiveValue(
                 value, boundaryAxis, unit)
 
         assert len(value) > 0, f"Dimension value cannot be empty."
 
         # Make sure our value only contains math operations and numbers as a weak safety check before passing it to `eval`
         assert re.match(
@@ -729,110 +630,60 @@
         return [self.x, self.y, self.z]
 
     @classmethod
     def fromList(cls, pointList: list[Dimension]):
         assert len(pointList) == 3, "Point list must contain three Dimensions."
         return cls(pointList[0], pointList[1], pointList[2])
 
-    def arithmeticPrecheckAndUnitConversion(self, other) -> 'Point':
-        assert other is not None, "Right-hand value cannot be None."
-
-        if not isinstance(other, (int, float, str, Dimension, list, Point)):
-            raise TypeError(
-                "Only int/float, Dimension, or Dimension String, or a list of those types is allowed.")
-
-        if isinstance(other, (int, float)):
-            return Point(Dimension(other), Dimension(other), Dimension(other))
-
-        x = Dimension(0)
-        y = Dimension(0)
-        z = Dimension(0)
-
-        if isinstance(other, list):
-            [x, y, z] = getDimensionListFromStringList(other)
-
-        if isinstance(other, str):
-            if "," in other:
-                [x, y, z] = getDimensionListFromStringList(other)
-            else:
-                other = Dimension.fromString(other)
-
-        if isinstance(other, Dimension):
-            x = other
-            y = other
-            z = other
-
-        if isinstance(other, Point):
-            x = other.x
-            y = other.y
-            z = other.z
-
-        if x.unit is not None and self.x.unit is not None and x.unit != self.x.unit:
-            x: Dimension = x.convertToUnit(self.x.unit)
-        if y.unit is not None and self.y.unit is not None and y.unit != self.y.unit:
-            y: Dimension = y.convertToUnit(self.y.unit)
-        if z.unit is not None and self.z.unit is not None and z.unit != self.z.unit:
-            z: Dimension = z.convertToUnit(self.z.unit)
-        return Point(x, y, z)
-
     def __eq__(self, other) -> bool:
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         return self.x == other.x and self.y == other.y and self.z == other.z
 
     def __add__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x + other.x
         y = self.y + other.y
         z = self.z + other.z
         return Point(x, y, z)
 
     def __sub__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x - other.x
         y = self.y - other.y
         z = self.z - other.z
         return Point(x, y, z)
 
     def __mul__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x * other.x
         y = self.y * other.y
         z = self.z * other.z
         return Point(x, y, z)
 
     def __truediv__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x / other.x
         y = self.y / other.y
         z = self.z / other.z
         return Point(x, y, z)
 
     def __floordiv__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x // other.x
         y = self.y // other.y
         z = self.z // other.z
         return Point(x, y, z)
 
     def __mod__(self, other):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = self.x % other.x
         y = self.y % other.y
         z = self.z % other.z
         return Point(x, y, z)
 
-    # def __divmod__(self, other):
-    #     other = self.arithmeticPrecheckAndUnitConversion(other)
-    #     x = divmod(self.x, other.x)
-    #     y = divmod(self.y, other.y)
-    #     z = divmod(self.z, other.z)
-    #     return Point(x, y, z)
+    def __divmod__(self, other):
+        x = divmod(self.x, other.x)
+        y = divmod(self.y, other.y)
+        z = divmod(self.z, other.z)
+        return Point(x, y, z)
 
     def __pow__(self, other, mod=None):
-        other = self.arithmeticPrecheckAndUnitConversion(other)
         x = pow(self.x, other.x)
         y = pow(self.y, other.y)
         z = pow(self.z, other.z)
         return Point(x, y, z)
 
     def __abs__(self):
         x = abs(self.x)
@@ -1021,21 +872,21 @@
                       ), "Only a list of strings is allowed."
 
     parsedDimensions = []
 
     defaultUnit = None
 
     unitInString = getUnitInString(dimensions[-1])
-    if unitInString is not None:
+    if unitInString != None:
         defaultUnit = LengthUnit.fromString(unitInString)
         if len(unitInString) == len(dimensions[-1].replace(" ", "").lower()):
             dimensions.pop()
 
     for index, dimension in enumerate(dimensions):
-        if boundingBox is not None and index < 3:
+        if boundingBox != None and index < 3:
             boundaryAxis = getattr(boundingBox, "xyz"[index])
             parsedDimensions.append(Dimension.fromString(
                 dimension, defaultUnit, boundaryAxis))
             continue
 
         parsedDimensions.append(
             Dimension.fromString(dimension, defaultUnit, None))
```

### Comparing `CodeToCAD-0.2.1687027263/CodeToCAD.egg-info/PKG-INFO` & `CodeToCAD-0.2.6/CodeToCAD.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeToCAD
-Version: 0.2.1687027263
+Version: 0.2.6
 Summary: 3D modeling automation in your favorite modeling software.
 Home-page: https://github.com/CodeToCAD/CodeToCAD
 Author: CodeToCAD
 Author-email: shehab@codethatdown.com
 License: GPL v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,30 +13,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
-Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - the [documentation](https://codetocad.github.io/CodeToCAD/docs.html) will help you get started.
+Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
-## Documentation
-
-You can find the CodeToCAD documentation here: [https://codetocad.github.io/CodeToCAD/docs.html](https://codetocad.github.io/CodeToCAD/docs.html).
-
-You should browse the examples too! [https://codetocad.github.io/CodeToCAD/examples.html](https://codetocad.github.io/CodeToCAD/examples.html).
-
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml) [![Documentation Pages](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -45,51 +37,46 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/import_file_in_blender.png)
-
-> Note, you can also run CodeToCAD in Blender via cli: `blender -- --codetocad $(pwd)/yourScript.py`
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
-- [CodeToCAD-Blender](#blender)
-- Onshape (Work-in-progress)
+- [CodeToCAD-Blender](https://github.com/CodeToCad/CodeToCad-Blender)
 
-Future planned integrations (not in any order):
-- KiCAD
-- FreeCAD 
-- Cascade Studio
-- CADQuery
+Future planned integrations:
+- OnShape
 - ThreeJS
+- Electronic CAD (suggestions welcome)
 
 
 ## Benefits of code-based modeling with CodeToCAD:
 
 ✅ Simplified modeling interface - it's all text! No more scrolling and clicking into sub-menus to edit your models.
 
 🔓 Not vendor locked - your models are created in an open-source language. If you want to use another software, you do not lose the features you have defined. Note: There is no guarantee that a model created for, e.g. Blender, will work right away for another software, but with some refactoring, it theoretically should!
@@ -126,24 +113,18 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
-### Architecture
-
-CodeToCAD is an automation. Here is the high-level architecture for this tool.
-
-![Architecture](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/CodeToCAD%20architecture%20overview.drawio.png)
-
 ### Contributing
 
 If you would like to contribute to the project, please feel free to submit a PR. 
 
 Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
```

### Comparing `CodeToCAD-0.2.1687027263/LICENSE` & `CodeToCAD-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `CodeToCAD-0.2.1687027263/PKG-INFO` & `CodeToCAD-0.2.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CodeToCAD
-Version: 0.2.1687027263
+Version: 0.2.6
 Summary: 3D modeling automation in your favorite modeling software.
 Home-page: https://github.com/CodeToCAD/CodeToCAD
 Author: CodeToCAD
 Author-email: shehab@codethatdown.com
 License: GPL v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,30 +13,22 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
-Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - the [documentation](https://codetocad.github.io/CodeToCAD/docs.html) will help you get started.
+Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
-## Documentation
-
-You can find the CodeToCAD documentation here: [https://codetocad.github.io/CodeToCAD/docs.html](https://codetocad.github.io/CodeToCAD/docs.html).
-
-You should browse the examples too! [https://codetocad.github.io/CodeToCAD/examples.html](https://codetocad.github.io/CodeToCAD/examples.html).
-
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml) [![Documentation Pages](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -45,51 +37,46 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/import_file_in_blender.png)
-
-> Note, you can also run CodeToCAD in Blender via cli: `blender -- --codetocad $(pwd)/yourScript.py`
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
-- [CodeToCAD-Blender](#blender)
-- Onshape (Work-in-progress)
+- [CodeToCAD-Blender](https://github.com/CodeToCad/CodeToCad-Blender)
 
-Future planned integrations (not in any order):
-- KiCAD
-- FreeCAD 
-- Cascade Studio
-- CADQuery
+Future planned integrations:
+- OnShape
 - ThreeJS
+- Electronic CAD (suggestions welcome)
 
 
 ## Benefits of code-based modeling with CodeToCAD:
 
 ✅ Simplified modeling interface - it's all text! No more scrolling and clicking into sub-menus to edit your models.
 
 🔓 Not vendor locked - your models are created in an open-source language. If you want to use another software, you do not lose the features you have defined. Note: There is no guarantee that a model created for, e.g. Blender, will work right away for another software, but with some refactoring, it theoretically should!
@@ -126,24 +113,18 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
-### Architecture
-
-CodeToCAD is an automation. Here is the high-level architecture for this tool.
-
-![Architecture](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/CodeToCAD%20architecture%20overview.drawio.png)
-
 ### Contributing
 
 If you would like to contribute to the project, please feel free to submit a PR. 
 
 Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
```

### Comparing `CodeToCAD-0.2.1687027263/README.md` & `CodeToCAD-0.2.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,19 @@
 # CodeToCAD - Code-based modeling automation
 
 CodeToCAD brings intuitive and reliable code-based automation to your favorite 3D modeling software (e.g. Blender and OnShape). 
 
-Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - the [documentation](https://codetocad.github.io/CodeToCAD/docs.html) will help you get started.
+Unlike other code-based CAD (e.g. CADQuery and OpenSCAD), CodeToCAD interfaces directly with existing modeling software (like Blender and OnShape). Therefore, you can keep using the software you love, but leverage the power of code and automation in your work. You don't need to be a great programmer to use CodeToCAD - there will be a cheat-sheet and documentation to help you get started.
 
 <div align="center">
-<image src="https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/three_axis_mill.gif"/>
+<image src="./documentation/three_axis_mill.gif"/>
 </div>
 
-## Documentation
-
-You can find the CodeToCAD documentation here: [https://codetocad.github.io/CodeToCAD/docs.html](https://codetocad.github.io/CodeToCAD/docs.html).
-
-You should browse the examples too! [https://codetocad.github.io/CodeToCAD/examples.html](https://codetocad.github.io/CodeToCAD/examples.html).
-
 ## Getting Started
 
-[![Release Version and Blender Addon](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml/badge.svg?branch=develop)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/on-pr-resolved.yml) [![Documentation Pages](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/CodeToCAD/CodeToCAD/actions/workflows/pages/pages-build-deployment)
-
 > Pre-requisites: Python 3.10 or newer. 
 
 1. Install the [CodeToCAD PIP Package](https://pypi.org/project/CodeToCAD/) to get intellisense syntax highlighting.
 
     `pip install CodeToCAD`
 
 2. Create your own CodeToCAD python file and save it:
@@ -30,51 +22,46 @@
     # This is also the examples/materials.py example
     from CodeToCAD import *
 
     myMaterial = Material("material").setColor(169, 76, 181, 0.8)
     Part("Cube").createCube(1, 1, 1).setMaterial(myMaterial)
     ```
 
-    ![Material Cube](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/materialCube.png)
+    ![Material Cube](./documentation/materialCube.png)
 
-3. Run your script in your modeling software. If you are using Blender, check out the instructions for installing the [Blender Addon](#blender) addon below.
+3. Run your script in your modeling software. See instructions for installing the [Blender Addon](#blender) addon below.
 
 ### Blender
 
 > Note: Blender 3.1 or newer is required.
 
-1. Download a release and install the Blender Addon from [CodeToCADBlenderAddon.zip](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/CodeToCADBlenderAddon.zip) or from the latest Release (see the sidebar).
-    > If you're a developer, instead of downloading a release, you can clone this repository. [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+1. Download a release (Check Releases in the repository side-bar) and install the Blender Addon from [./providers/blender/CodeToCADBlenderAddon.py](./providers/blender/CodeToCADBlenderAddon.py). [Video Guide](https://youtu.be/YD_4nj0QUJ4)
+    > If you're a developer, instead of downloading a release, you can clone this repository.
 
 2. Import your script using the file menu > import > CodeToCAD or the CodeToCAD menu in the sidebar.
-    ![import_file](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/import_file_in_blender.png)
-
-> Note, you can also run CodeToCAD in Blender via cli: `blender -- --codetocad $(pwd)/yourScript.py`
+    ![import_file](./documentation/import_file_in_blender.png)
 
 ## What do I do next?
 
 - Run or browse the [examples](./examples/)! 
 
-    ![Stacked Cubes](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/stackedCubes.png)
+    ![Stacked Cubes](./documentation/stackedCubes.png)
 
 - Join the [Discord Server](https://discord.gg/MnZEtqwt74) to receive updates and help from the community! [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
 
 
 ## Integrations
 
 Current integrations:
-- [CodeToCAD-Blender](#blender)
-- Onshape (Work-in-progress)
+- [CodeToCAD-Blender](https://github.com/CodeToCad/CodeToCad-Blender)
 
-Future planned integrations (not in any order):
-- KiCAD
-- FreeCAD 
-- Cascade Studio
-- CADQuery
+Future planned integrations:
+- OnShape
 - ThreeJS
+- Electronic CAD (suggestions welcome)
 
 
 ## Benefits of code-based modeling with CodeToCAD:
 
 ✅ Simplified modeling interface - it's all text! No more scrolling and clicking into sub-menus to edit your models.
 
 🔓 Not vendor locked - your models are created in an open-source language. If you want to use another software, you do not lose the features you have defined. Note: There is no guarantee that a model created for, e.g. Blender, will work right away for another software, but with some refactoring, it theoretically should!
@@ -111,24 +98,18 @@
 
 ### Running Tests
 
 Run tests using `sh runTests.sh`.
 
 ### Capabilities.json and Jinja2 templates
 
-[CodeToCAD/capabilities.json](./CodeToCAD/capabilities.json) is a schema used to generate the [CodeToCAD interface](./CodeToCAD/CodeToCADInterface.py).
+[core/capabilities.json](./core/capabilities.json) is a schema used to generate the [CodeToCAD interface](./core/CodeToCADInterface.py).
 
 Jinja2 templates are used to turn capabilities.json into an interface, as well as templates for CodeToCAD Providers and Tests.
 
 You can generate the Jinja2 templates by running the "Capabilities.json to Python" task in VSCode, or `sh development/capabilitiesJsonToPython/capabilitiesToPy.sh`
 
-### Architecture
-
-CodeToCAD is an automation. Here is the high-level architecture for this tool.
-
-![Architecture](https://raw.githubusercontent.com/CodeToCAD/CodeToCAD/develop/docs/images/CodeToCAD%20architecture%20overview.drawio.png)
-
 ### Contributing
 
 If you would like to contribute to the project, please feel free to submit a PR. 
 
-Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
+Please join the Discord Server if you have any questions or suggestions: [https://discord.gg/MnZEtqwt74](https://discord.gg/MnZEtqwt74)
```

