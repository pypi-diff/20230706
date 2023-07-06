# Comparing `tmp/pydelorean-0.3.1.tar.gz` & `tmp/pydelorean-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydelorean-0.3.1.tar", last modified: Sun Jul  2 15:28:56 2023, max compression
+gzip compressed data, was "pydelorean-1.1.0.tar", last modified: Thu Jul  6 11:16:54 2023, max compression
```

## Comparing `pydelorean-0.3.1.tar` & `pydelorean-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-06-10 12:13:51.000000 pydelorean-0.3.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-07-02 15:28:56.380357 pydelorean-0.3.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-11 13:16:27.000000 pydelorean-0.3.1/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.378357 pydelorean-0.3.1/pydelorean/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1974 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3903 2023-07-02 13:53:53.000000 pydelorean-0.3.1/pydelorean/delorean.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.379357 pydelorean-0.3.1/pydelorean/parser/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-10 12:14:10.000000 pydelorean-0.3.1/pydelorean/parser/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1311 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/parser/parser.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     4865 2023-07-02 13:55:11.000000 pydelorean-0.3.1/pydelorean/parser/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/pydelorean/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       21 2023-06-10 12:13:51.000000 pydelorean-0.3.1/pydelorean/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2789 2023-06-10 16:47:52.000000 pydelorean-0.3.1/pydelorean/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-14 12:58:48.000000 pydelorean-0.3.1/pydelorean/utils.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.379357 pydelorean-0.3.1/pydelorean.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2532 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      421 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-02 15:28:56.000000 pydelorean-0.3.1/pydelorean.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-02 15:28:56.380357 pydelorean-0.3.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      951 2023-07-02 15:28:29.000000 pydelorean-0.3.1/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-02 15:28:56.380357 pydelorean-0.3.1/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1198 2023-06-11 13:13:52.000000 pydelorean-0.3.1/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 12:19:37.000000 pydelorean-1.1.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-07-06 11:16:54.113550 pydelorean-1.1.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2108 2023-06-12 11:33:27.000000 pydelorean-1.1.0/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1947 2023-07-03 11:53:35.000000 pydelorean-1.1.0/pydelorean/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3897 2023-07-03 11:53:12.000000 pydelorean-1.1.0/pydelorean/delorean.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/parser/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       22 2023-06-12 11:33:27.000000 pydelorean-1.1.0/pydelorean/parser/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1672 2023-07-03 11:09:36.000000 pydelorean-1.1.0/pydelorean/parser/parser.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6017 2023-07-06 10:23:48.000000 pydelorean-1.1.0/pydelorean/parser/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/tools/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2602 2023-07-06 11:15:07.000000 pydelorean-1.1.0/pydelorean/tools/__init__.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       42 2023-07-04 11:20:36.000000 pydelorean-1.1.0/pydelorean/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1509 2023-07-04 11:22:10.000000 pydelorean-1.1.0/pydelorean/tree/forest.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1916 2023-07-03 11:09:58.000000 pydelorean-1.1.0/pydelorean/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      245 2023-06-21 00:15:53.000000 pydelorean-1.1.0/pydelorean/utils.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-07-06 11:16:54.113550 pydelorean-1.1.0/pydelorean.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2551 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      455 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       32 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       11 2023-07-06 11:16:54.000000 pydelorean-1.1.0/pydelorean.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-07-06 11:16:54.113550 pydelorean-1.1.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      971 2023-07-06 11:16:39.000000 pydelorean-1.1.0/setup.py
```

### Comparing `pydelorean-0.3.1/LICENSE` & `pydelorean-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydelorean-0.3.1/PKG-INFO` & `pydelorean-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.3.1
+Version: 1.1.0
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.3.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.1.0.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -101,7 +102,8 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
+
```

### Comparing `pydelorean-0.3.1/README.rst` & `pydelorean-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pydelorean-0.3.1/pydelorean/__init__.py` & `pydelorean-1.1.0/pydelorean/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bs4 import BeautifulSoup
 from .delorean import mdtreeify, findMetadata
-from .tree.types import MarkdownForest
-from .utils import FileType
+from .tree.forest import MarkdownForest
 import re
 
 def treeify(name:str, md:str, *args, **kwargs) -> MarkdownForest:
     """Converts a markdown document into a MarkdownForest object.
 
     Args:
         name (str, optional): Name of the document.
```

### Comparing `pydelorean-0.3.1/pydelorean/delorean.py` & `pydelorean-1.1.0/pydelorean/delorean.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 """
     
 import re
 
 import frontmatter
 from treelib import Tree
 from .utils import *
-from .tree.types import MarkdownForest, TextNode, HeaderNode, Node
+from .tree import MarkdownForest, TextNode, HeaderNode
 from .parser import *
 
 # ==================================================================================================
 #                                           TREEIFY
 # ==================================================================================================
 
 # TODO: Rename to snake_case in the future.
@@ -86,15 +86,15 @@
     return returnForest
 
 
 # ==================================================================================================
 #                                           TEXTIFY
 # ==================================================================================================
 
-def convertRootToText(rootNode: Node) -> str:
+def convertRootToText(rootNode: HeaderNode) -> str:
     
     # BASE CASE: We just have text node.
     if isinstance(rootNode, TextNode):
         return repr(rootNode) + "\n"
     
     # For the header node
     headerLevel = rootNode.get_header_level()
```

### Comparing `pydelorean-0.3.1/pydelorean/parser/parser.py` & `pydelorean-1.1.0/pydelorean/parser/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     
     def __init__(self, document_name:str, text:str):
         self.document_name = document_name
         self.text = text
         
     def parse(self) -> Tree:
         pass
-    
-    
+
+   
 class MarkdownParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Tree:
         HEADER_PATTERN = r"^(#+\s+)(.*)"
@@ -47,8 +47,26 @@
 class YAMLParser(Parser):
     
     def __init__(self, document_name:str, text:str):
         super().__init__(document_name, text)
         
     def parse(self) -> Tree:
         pass
-        
+
+
+class JSONParser(Parser):
+    
+    def __init__(self, document_name:str, text:str):
+        super().__init__(document_name, text)
+        
+    def parse(self) -> Tree:
+        pass
+    
+
+class XMLParser(Parser):
+    
+    def __init__(self, document_name:str, text:str):
+        super().__init__(document_name, text)
+        
+    def parse(self) -> Tree:
+        pass
+
```

### Comparing `pydelorean-0.3.1/pydelorean/parser/utils.py` & `pydelorean-1.1.0/pydelorean/parser/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,113 +1,144 @@
 import re
-from treelib import Tree
 from pydelorean.tree import TextNode, HeaderNode
+from bigtree import Node, print_tree
 
-
-def buildTree(inputText:str, name:str, *args, **kwargs) -> Tree:
+def buildTree(inputText:str, *args, **kwargs) -> HeaderNode:
     """ Function to build the provides tree varaible from the inputText. 
     Works for Github Flavored Markdown (GFM). 
 
     Args:
         inputText (str): Input text to be parsed
         name (Str): Name of the document
         
     """
     assert isinstance(inputText, str), "inputText must be a string"
     if inputText == "":
         return None
     
-    tree = Tree()
-    root_id = tree.create_node(tag=name, identifier="root").identifier
+    root = Node("root")
 
     # Default to the GFM header pattern
     HEADER_PATTERN = kwargs['header_pattern'] if 'header_pattern' in kwargs else r"^(#+\s+)(.*)"
     
+    inputText = inputText.strip()
     matches = re.finditer(HEADER_PATTERN, inputText, re.MULTILINE)
         
     # Get all the indices of the headers
     indices = [(match.start(), match.end()) for match in matches]
     
     # BASE CASE
     # Check if it is only text (since there are no header indices)
     if len(indices) == 0:
-        tree.create_node(tag=inputText[0:min(10, len(inputText))],
-                         data=TextNode(inputText),
-                         parent=root_id)
-        return tree
+        text_node = TextNode(name=inputText, text=inputText)
+        root >> text_node
+        return root
     
     # Is there text before the first header?
     if indices[0][0] != 0:
         textBefore = inputText[0:indices[0][0]]
-        tree.create_node(tag=textBefore[0:min(10, len(textBefore))],
-                        data=TextNode(textBefore),
-                        parent=root_id)
+        node = TextNode(name=textBefore, text=textBefore)
+        root >> node
 
     # Use a stack to keep track of the header levels.
     stack = []
 
     # Iterate over all the headers and accordingly build the tree.
     for currHeader in indices:
    
         currHeaderText = inputText[currHeader[0]:currHeader[1]]
         currHeaderLevel = len(currHeaderText) - len(currHeaderText.replace("#", ""))
         
-        # If this is the first header then create the root node automatically.
+        # If this is the first header then create the header node automatically.
         if len(stack) == 0:
              # Create the header node with the current header.
-            node = tree.create_node(tag=currHeaderText,
-                                    data=HeaderNode(currHeaderText, currHeaderLevel, root_id),
-                                    parent=root_id)
+            node = HeaderNode(name=currHeaderText, header=currHeaderText, headerNumber=currHeaderLevel)
+            root >> node
 
             # Add the node to the stack
-            stack.append((currHeaderLevel, currHeader, node.identifier))
+            stack.append((currHeaderLevel, currHeader, node))
             continue
         else:
             lastHeader = stack[-1]
         
         # CASE 1: If the current header level is greater than the starting header level then keep going.
         if currHeaderLevel > lastHeader[0]:
             
             # Extract the text between the current header and the previous header
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
-                tree.create_node(tag=textBetween[0:min(10, len(textBetween))],
-                                 data=TextNode(textBetween),
-                                 parent=lastHeader[-1])
+                node = TextNode(name=textBetween, text=textBetween)
+                lastHeader[-1] >> node
 
             # Create the header node and add it to the stack
-            node = tree.create_node(tag=currHeaderText,
-                                    data=HeaderNode(currHeaderText, currHeaderLevel, lastHeader[-1]),
-                                    parent=lastHeader[-1])
-            stack.append((currHeaderLevel, currHeader, node.identifier))
+            node = HeaderNode(name=currHeaderText, header=currHeaderText, headerNumber=currHeaderLevel)
+            lastHeader[-1] >> node
+            
+            stack.append((currHeaderLevel, currHeader, node))
             
         # CASE 2: If the current header level is less than or equal to the starting header level then we need to create a new tree.
         elif currHeaderLevel <= lastHeader[0]:
             
             # Get the text between 
             textBetween = inputText[lastHeader[1][1]:currHeader[0]].strip()
             if textBetween != "":
-                tree.create_node(tag=textBetween[0:min(10, len(textBetween))],
-                                 data=TextNode(textBetween),
-                                 parent=lastHeader[-1])
-            
+                node = TextNode(name=textBetween, text=textBetween)
+                lastHeader[-1] >> node
+                            
             # Pop off until you get to the node with a lower level than the current header level
             while len(stack) > 0:
                 if stack[-1][0] >= currHeaderLevel:
                     stack.pop()
                 else:
                     break
             
             if len(stack) == 0:
                 
-                node = tree.create_node(currHeaderText, data=HeaderNode(currHeaderText, currHeaderLevel, root_id), parent=root_id)
+                node = HeaderNode(name=currHeaderText, header=currHeaderText, headerNumber=currHeaderLevel)
+                root >> node
             else:
-                node = tree.create_node(currHeaderText, data=HeaderNode(currHeaderText, currHeaderLevel, stack[-1][-1]), parent=stack[-1][-1])
-            stack.append((currHeaderLevel, currHeader, node.identifier))
+                node = HeaderNode(name=currHeaderText, header=currHeaderText, headerNumber=currHeaderLevel)
+                stack[-1][-1] >> node
+            stack.append((currHeaderLevel, currHeader, node))
                 
                 
     # Check if there is any text after the last header
     if indices[-1][1] != len(inputText):
         textEnd = inputText[indices[-1][1]:].strip()
-        tree.create_node(tag=textEnd[:min(10, len(textEnd))], data=TextNode(textEnd), parent=stack[-1][-1])
+        node = TextNode(name=textEnd, text=textEnd)
+        stack[-1][-1] >> node
         
-    return tree
+    return root
+
+
+text=  """
+# Appendices
+
+The appendix begins with an epigraph by Pardot Kynes in which he considers the kind of existence available when humans increase in number in a finite environment.
+
+## Appendix I: The Ecology of Dune.
+This appendix details “the ecology of Dune.” It is heavily focused on the story of Pardot Kynes, Arrakis's first planetologist.
+
+## Appendix II: The Religion of Dune.
+Before the coming of [[Muad'Dib]], the Fremen of Arrakis practiced a religion whose roots in the Maometh Saari are there for any scholar to see. Many have traced the extensive borrowings from other religions. The most common example is the Hymn to Water, a direct copy from the Orange Catholic Liturgical Manual, calling for rain clouds which Arrakis had never seen. But there are more profound points of accord between the Kitab al-Ibar of the Fremen and the teachings of Bible, Ilm, and Fiqh.
+
+## Appendix III: Report on Bene Gesserit Motives and Purposes.
+This appendix details a “report on Bene Gesserit motives and purpose.”
+The narrator introduces it by noting that Lady Jessica commissioned the report directly after the “Arrakis Affair.” 
+
+### Narratives
+The document is noted as being extremely honest in tone.
+
+## Appendix IV: The Almanak eb-Ashraf (Selected Excerpts of the Noble Houses)
+This appendix details selected excerpts about the noble Houses of Dune. The first entry discusses the Padishah Emperor Shaddam IV of House Corrino. His rule is most significant for the “Arrakis Revolt,” which historians ascribe to his poor court politics. 
+
+# Terminology of the Imperium
+
+Hello there
+
+## Another One
+asda
+# """
+
+root = buildTree(text)
+
+print_tree(root)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydelorean-0.3.1/pydelorean/tree/types.py` & `pydelorean-1.1.0/pydelorean/tree/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,15 @@
 """_summary_
 
 """
 
-from treelib import Tree
+from bigtree import BaseNode, Node
 
 # TODO: Add all the documentation and convert to snake case soon.
 
-class Node:
-    """_summary_
-    """
-    
-    def __init__(self):
-        pass
-                   
-    def __str__(self):
-        return f"{self.__class__.__name__}()"
-
 
 class TextNode(Node):
     """_summary_
 
     Args:
         Node (_type_): _description_
 
@@ -28,16 +18,18 @@
 
     Returns:
         _type_: _description_
     """
     
     FRACTION_PRINTABLE = 0.25
     
-    def __init__(self, text:str):
+    def __init__(self, name:str, text:str, **kwargs):
         self.text = text
+        super().__init__(name, **kwargs)
+        
         
     def __getitem__(self, index:int):
         if index < 0 or index >= len(self.text):
             raise IndexError("Index out of bounds")
         return self.text[index]
            
     def __str__(self):
@@ -57,19 +49,20 @@
 class HeaderNode(Node):
     """_summary_
 
     Args:
         Node (_type_): _description_
     """
     
-    def __init__(self, header:str, headerNumber:int, parentID):
-        self.parentID = parentID
+    def __init__(self, name:str, header:str, headerNumber:int, **kwargs):
         self.header = header
         self.headerNumber = headerNumber
+        self.name = header
         self.corpus = []
+        super().__init__(name, **kwargs)
         
     def __str__(self):
         return self.header
     
     def __repr__(self):
         return f"(h{self.headerNumber}) {self.header}"
     
@@ -84,41 +77,9 @@
     def get_corpus(self) -> list:
         return self.corpus
     
     def add_to_corpus(self, text:str) -> None:
         self.corpus.append(text)
 
 
-class MarkdownForest:
-    
-    def __init__(self, root:Tree, documentName:str="[document]", metadata:dict=None):
-        self.documentName = documentName
-        self.metadata = metadata
-        self.root = root
-        self.treeCount = len(root.children('root'))
-        self.backlinks = []
-        self.tags = []
-        
-    def __str__(self):
-        return str(self.root)
-    
-    def __len__(self):
-        return self.treeCount
 
-    def add_root(self, root:Tree):
-        self.root = root
-
-    def get_metadata(self):
-        return self.metadata
-    
-    def add_backlink(self, backlink:str):
-        self.backlinks.append(backlink)
-    
-    def get_backlinks(self):
-        return self.backlinks
-    
-    def add_tag(self, tag:str):
-        self.tags.append(tag)
-        
-    def get_tags(self):
-        return self.tags
```

### Comparing `pydelorean-0.3.1/pydelorean.egg-info/PKG-INFO` & `pydelorean-1.1.0/pydelorean.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pydelorean
-Version: 0.3.1
+Version: 1.1.0
 Summary: A package to convert between markup language documents and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/delorean
-Download-URL: https://github.com/kj3moraes/delorean/archive/0.3.1.zip
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
+Download-URL: https://github.com/kj3moraes/delorean/archive/1.1.0.zip
+Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 .. image:: media/image.png
    :width: 200
 
 delorean
@@ -101,7 +102,8 @@
 3. Traverse and edit the Python data structure.
 
 License
 -------
 
 This project is licensed under the Apache 2.0 License. A copy of the license 
 can be found in the LICENSE file.
+
```

### Comparing `pydelorean-0.3.1/setup.py` & `pydelorean-1.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '0.3.1'
+VERSION = '1.1.0'
 DESCRIPTION = 'A package to convert between markup language documents and a forest data structure for efficient processing.'
 
 setup(
     name = "pydelorean",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     license = "Apache 2.0",
     url = "http://github.com/kj3moraes/delorean",
-    packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser'],
+    packages = ['pydelorean', 'pydelorean.tree', 'pydelorean.parser', 'pydelorean.tools'],
     tests_require = ['unittest'],
-    install_requires = ['markdown', 'treelib', 'beautifulsoup4'],
+    install_requires = ['markdown', 'bigtree', 'beautifulsoup4'],
     download_url = 'https://github.com/kj3moraes/delorean/archive/%s.zip' % VERSION,
     classifiers = [
         "Topic :: Utilities",
     ],
 )
```

