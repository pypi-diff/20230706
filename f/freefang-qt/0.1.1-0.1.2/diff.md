# Comparing `tmp/freefang_qt-0.1.1.tar.gz` & `tmp/freefang_qt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freefang_qt-0.1.1.tar", last modified: Mon Jul  3 21:27:29 2023, max compression
+gzip compressed data, was "freefang_qt-0.1.2.tar", last modified: Wed Jul  5 22:45:26 2023, max compression
```

## Comparing `freefang_qt-0.1.1.tar` & `freefang_qt-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:27:29.769328 freefang_qt-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-03 21:27:29.769328 freefang_qt-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:27:29.765328 freefang_qt-0.1.1/freefang_qt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/game_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/game_join.py
--rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/gameloop.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/packets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:27:29.769328 freefang_qt-0.1.1/freefang_qt/qml/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/ActionButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Create_Game.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Game_UI.qml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/HunterKill.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Join_Game.qml
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/ProtectorProtect.qml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/SeerReveal.qml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Vote.qml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Werewolfvote.qml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Witch_kill.qml
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/Witch_revive.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/qml/main.qml
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/freefang_qt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 21:27:29.765328 freefang_qt-0.1.1/freefang_qt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 21:27:29.000000 freefang_qt-0.1.1/freefang_qt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 21:27:29.769328 freefang_qt-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-03 21:27:20.000000 freefang_qt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/game_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/game_join.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/gameloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/packets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt/qml/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/ActionButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Create_Game.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Game_UI.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/HunterKill.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Join_Game.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/ProtectorProtect.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/SeerReveal.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Vote.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Werewolfvote.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Witch_kill.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/Witch_revive.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/qml/main.qml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/freefang_qt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/freefang_qt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-05 22:45:26.000000 freefang_qt-0.1.2/freefang_qt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-05 22:45:26.973519 freefang_qt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-05 22:45:17.000000 freefang_qt-0.1.2/setup.py
```

### Comparing `freefang_qt-0.1.1/LICENSE` & `freefang_qt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/PKG-INFO` & `freefang_qt-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang_qt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PySide client for the FreeFang werewolf gameserver.
 Author-email: Solaris <iusegentoobtw@protonmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-qt
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-qt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `freefang_qt-0.1.1/freefang_qt/game_creation.py` & `freefang_qt-0.1.2/freefang_qt/game_creation.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/gameloop.py` & `freefang_qt-0.1.2/freefang_qt/gameloop.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 	witchaction = Signal(list, arguments=['nightdeaths'])
 	remove_buttons = Signal()
 	playername = ""
 	time = ""
 	up = ""
 	role = ""
 	players = []
+	werewolves = [] #Only used if the player is a werewolf
 	game_started = False
 
 
 	def __init__(self):
 		super(Game_loop, self).__init__()
 		
 	def handle_time_change(self, packet):
@@ -121,14 +122,24 @@
 	# This function should be the one that creates the buttons allowing the witch to do its action
 	def handle_witch_send_dead(self, packet):
 		deadplayers = " ".join(packet.dead)
 		self.chatupdate.emit(f"The following players {deadplayers} died during this night.")
 		self.chatupdate.emit(f"Would you like to revive someone, kill someone else, or pass?")
 
 		self.witchaction.emit(packet.dead)
+
+	# Handle the packet that is sent to all werewolves on game start
+	# Which contains the names of all other werewolves
+	def handle_show_werewolves(self, packet):
+		for i in packet.headers.werewolves:
+		 	if i != self.playername:
+					self.werewolves.append(i)
+			
+		if len(self.werewolves) > 0:
+			self.chatupdate.emit(f"Your fellow werewolves are {' '.join(self.werewolves)}")
 		
 
 	def getplayerbyname(self, player):
 		return [i for i in self.players if i.name == player][0]
 
 	@Slot(str, result=bool)
 	def isalive(self, player):
@@ -147,15 +158,16 @@
 			"added_to_game": self.handle_added_to_game,
 			"player_join": self.handle_player_join,
 			"chat_message": self.handle_chat_message,
 			"seer_role_reveal": self.handle_seer_role_reveal,
 			"town_vote_begin": self.begin_town_vote,
 			"player_leave": self.handle_leave,
 			"werewolf_vote": self.handle_werewolf_vote,
-			"witch_send_dead": self.handle_witch_send_dead
+			"witch_send_dead": self.handle_witch_send_dead,
+			"show_werewolves": self.handle_show_werewolves
 		}
 		if packet_to_func.get(packet.action):
 			packet_to_func[packet.action](packet)
 			return 0
 		else:
 			return 1
 
@@ -239,7 +251,10 @@
 			
 	@Slot(str)
 	def witch_revive(self, player):
 		self.remove_buttons.emit()
 		packet = utils.object_to_json(packets.Witch_revive(player))
 		net.send_packet(packet, global_data.socket)		
 			
+	@Slot(str, result=bool)
+	def iswerewolf(self, player):
+		return player in self.werewolves
```

### Comparing `freefang_qt-0.1.1/freefang_qt/main.py` & `freefang_qt-0.1.2/freefang_qt/main.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/net.py` & `freefang_qt-0.1.2/freefang_qt/net.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/packets.py` & `freefang_qt-0.1.2/freefang_qt/packets.py`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/qml/Create_Game.qml` & `freefang_qt-0.1.2/freefang_qt/qml/Create_Game.qml`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/qml/Game_UI.qml` & `freefang_qt-0.1.2/freefang_qt/qml/Game_UI.qml`

 * *Files 2% similar despite different names*

```diff
@@ -162,14 +162,17 @@
 							if (!game_loop.isalive(game_loop.playername)){
 								return;
 							}
 							for( var i = 0; i < playermodel.rowCount(); i++ ) {
 								if (playermodel.get(i).player != game_loop.playername && game_loop.isalive(playermodel.get(i).player)){
 									playermodel.get(i).buttonsrc = btn;
 								}
+								if (act == "Werewolfvote" && game_loop.iswerewolf(playermodel.get(i).player)){
+									playermodel.get(i).buttonsrc = "";
+								}
 							}
 						}
 						function onRemove_buttons(){
 							for( var i = 0; i < playermodel.rowCount(); i++ ) {
 								playermodel.get(i).buttonsrc = "";
 							}
 						}
```

### Comparing `freefang_qt-0.1.1/freefang_qt/qml/Join_Game.qml` & `freefang_qt-0.1.2/freefang_qt/qml/Join_Game.qml`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt/qml/main.qml` & `freefang_qt-0.1.2/freefang_qt/qml/main.qml`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/freefang_qt.egg-info/PKG-INFO` & `freefang_qt-0.1.2/freefang_qt.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freefang-qt
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PySide client for the FreeFang werewolf gameserver.
 Author-email: Solaris <iusegentoobtw@protonmail.com>
 Project-URL: Homepage, https://github.com/FreeFangGame/freefang-qt
 Project-URL: Bug Tracker, https://github.com/FreeFangGame/freefang-qt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `freefang_qt-0.1.1/freefang_qt.egg-info/SOURCES.txt` & `freefang_qt-0.1.2/freefang_qt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freefang_qt-0.1.1/pyproject.toml` & `freefang_qt-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name  = "freefang_qt"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Solaris", email="iusegentoobtw@protonmail.com" }
 ]
 dependencies = [
 	"pyside6"
 ]
```

