# Comparing `tmp/Lopster-0.1.5.tar.gz` & `tmp/Lopster-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.1.5.tar", last modified: Sat Jul  1 18:47:27 2023, max compression
+gzip compressed data, was "Lopster-0.1.6.tar", last modified: Sat Jul  8 15:49:39 2023, max compression
```

## Comparing `Lopster-0.1.5.tar` & `Lopster-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.342308 Lopster-0.1.5/
-drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.311022 Lopster-0.1.5/Lopster/
--rw-rw-rw-   0        0        0    11911 2023-07-01 18:47:06.000000 Lopster-0.1.5/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 18:47:27.342308 Lopster-0.1.5/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 18:47:27.000000 Lopster-0.1.5/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-07-01 18:47:27.342308 Lopster-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-07-01 18:47:27.342308 Lopster-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-07-01 18:23:27.000000 Lopster-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:49:39.261372 Lopster-0.1.6/
+drwxrwxrwx   0        0        0        0 2023-07-08 15:49:39.230156 Lopster-0.1.6/Lopster/
+-rw-rw-rw-   0        0        0    10237 2023-07-08 15:48:05.000000 Lopster-0.1.6/Lopster/Lopster.py
+-rw-rw-rw-   0        0        0       22 2023-07-08 15:48:38.000000 Lopster-0.1.6/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 15:49:39.245750 Lopster-0.1.6/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-07-08 15:49:39.000000 Lopster-0.1.6/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-07-08 15:49:39.000000 Lopster-0.1.6/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 15:49:39.000000 Lopster-0.1.6/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-08 15:49:39.000000 Lopster-0.1.6/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-08 15:49:39.000000 Lopster-0.1.6/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-07-08 15:49:39.261372 Lopster-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-08 15:49:39.261372 Lopster-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-07-08 15:48:56.000000 Lopster-0.1.6/setup.py
```

### Comparing `Lopster-0.1.5/Lopster/__init__.py` & `Lopster-0.1.6/Lopster/Lopster.py`

 * *Files 18% similar despite different names*

```diff
@@ -131,29 +131,14 @@
         def is_clicked(window, eve):
             if self.x <= eve.pos[0] <= self.x + self.w and self.y <= eve.pos[1] <= self.y + self.h:
                 event(window, eve)
 
         mouse = Mouse()
         mouse.leftDown(is_clicked)
 
-    def cash(self):
-        text = []
-
-        text.append("Enemy\n")
-        text.append("x = " + str(self.x) + "\n")
-        text.append("y = " + str(self.y) + "\n")
-        text.append("h = " + str(self.h) + "\n")
-        text.append("w = " + str(self.w) + "\n")
-        text.append("func update = " +
-                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
-        text.append("init @x @y @h @w @update\n")
-        text.append(";")
-
-        return "".join(text)
-
 
 class FakeEnemy:
     typ = "Enemy"
     x = 0
     y = 0
     h = 0
     w = 0
@@ -168,29 +153,14 @@
 
     def hide(self):
         self.typ = "NoN"
 
     def visible(self, typ):
         self.typ = typ
 
-    def cash(self):
-        text = []
-
-        text.append("FakeEnemy\n")
-        text.append("x = " + self.x + "\n")
-        text.append("y = " + self.y + "\n")
-        text.append("h = " + self.h + "\n")
-        text.append("w = " + self.w + "\n")
-        text.append("func update = " +
-                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
-        text.append("init @x @y @h @w @update\n")
-        text.append(";")
-
-        return "".join(text)
-
 
 class Player(Enemy):
     typ = "EnemyPlayer"
     speed = 5
 
     def __init__(self, _x, _y, _h, _w, _update, speed):
         super().__init__(_x, _y, _h, _w, _update)
@@ -228,30 +198,14 @@
 
     def moveUp(self):
         self.y -= self.speed
 
     def moveDown(self):
         self.y += self.speed
 
-    def cash(self):
-        text = []
-
-        text.append("Player\n")
-        text.append("x = " + str(self.x) + "\n")
-        text.append("y = " + str(self.y) + "\n")
-        text.append("h = " + str(self.h) + "\n")
-        text.append("w = " + str(self.w) + "\n")
-        text.append("speed = " + str(self.speed) + "\n")
-        text.append("func update = " +
-                    inspect.getsource(self.update).replace("\n", "/../+o+/../") + "\n")
-        text.append("init @x @y @h @w @speed @update\n")
-        text.append(";")
-
-        return "".join(text)
-
 class Sprite(Enemy):
     def __init__(self, _x, _y, _h, _w, src, size, _update, speed):
         super().__init__(_x, _y, _h, _w, _update)
         self.speed = speed
         self.src = src
         self.size = size
         self.srcList = []
@@ -399,11 +353,8 @@
 
             for obj in Enemy._object:
                 if obj.typ != "NoN":
                     obj.update(window, obj)
 
             pygame.display.update()
 
-        pygame.quit()
-
-
-__all__ = ['Enemy', 'FakeEnemy', 'Player', 'MathMap', 'Map', 'RunLopster']
+        pygame.quit()
```

