# Comparing `tmp/BLACKFORGE2-0.1.post3.tar.gz` & `tmp/BLACKFORGE2-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.1.post3.tar", last modified: Thu Jun 15 14:15:10 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.2.0.tar", last modified: Tue Jun 20 22:08:05 2023, max compression
```

## Comparing `BLACKFORGE2-0.1.post3.tar` & `BLACKFORGE2-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.928119 BLACKFORGE2-0.1.post3/
-drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.916617 BLACKFORGE2-0.1.post3/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14363 2023-06-15 14:13:08.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 14:15:10.926128 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      316 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 14:15:10.000000 BLACKFORGE2-0.1.post3/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.post3/LICENSE
--rw-rw-rw-   0        0        0      316 2023-06-15 14:15:10.927123 BLACKFORGE2-0.1.post3/PKG-INFO
--rw-rw-rw-   0        0        0     8041 2023-06-13 07:29:39.000000 BLACKFORGE2-0.1.post3/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-15 14:15:10.928119 BLACKFORGE2-0.1.post3/setup.cfg
--rw-rw-rw-   0        0        0      496 2023-06-15 14:15:04.000000 BLACKFORGE2-0.1.post3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.261164 BLACKFORGE2-0.2.0/
+drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.242713 BLACKFORGE2-0.2.0/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14335 2023-06-20 22:06:51.000000 BLACKFORGE2-0.2.0/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.2.0/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 22:08:05.258172 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      312 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 22:08:04.000000 BLACKFORGE2-0.2.0/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      312 2023-06-20 22:08:05.260165 BLACKFORGE2-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8967 2023-06-16 21:39:12.000000 BLACKFORGE2-0.2.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-20 22:08:05.261164 BLACKFORGE2-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2023-06-20 22:07:27.000000 BLACKFORGE2-0.2.0/setup.py
```

### Comparing `BLACKFORGE2-0.1.post3/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.2.0/BLACKFORGE2/FORGE.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,17 @@
 class Physics():
 
 	def __init__(self):
 		pass
 
 	def apply_gravity(self, entity, gravity_value:float, delta_time:float):
 		entity.velocity.y += gravity_value * delta_time
-		entity.rect.y += entity.velocity.y
 
 	def horizontal_movement_collision(self, entity, collision_tiles:pygame.sprite.Group):
 		entity = entity
-		entity.rect.x += entity.velocity.x * entity.speed
-
 		for sprite in collision_tiles.sprites():
 			if sprite.rect.colliderect(entity.rect):
 				if entity.velocity.x < 0: 
 					entity.rect.left = sprite.rect.right
 					entity.collide_left = True
 					self.current_x = entity.rect.left
 				elif entity.velocity.x > 0:
@@ -86,27 +83,27 @@
 	def draw(self, surface:pygame.Surface):
 		surface.blit(self.image, self.rect.topleft)
 
 	def update(self):
 		pass
 
 class StaticTile(pygame.sprite.Sprite):
-	def __init__(self, pos:tuple, groups:list, surface:pygame.Surface):
+	def __init__(self, position:tuple, groups:list, surface:pygame.Surface):
 		super().__init__(groups)
 		self.image = surface
-		self.rect = self.image.get_rect(topleft=pos)
-		self.pos = pygame.math.Vector2(pos)  # Initial position of the tile
+		self.rect = self.image.get_rect(topleft=position)
+		self.position = pygame.math.Vector2(position)  # Initial position of the tile
 
 	def update(self, world_shift):
 		self.rect.x += world_shift.x
 		self.rect.y += world_shift.y
 
 class MovingTile(StaticTile):
 	def __init__(self, pos:tuple, groups:list, direction:str, speed:int, delta_time:float, surface:pygame.Surface):
-		super().__init__(pos, groups, surface)
+		super().__init__(position, groups, surface)
 		self.image = surface
 		self.delta_time = delta_time
 		self.direction = direction  # Movement direction ('up', 'down', 'left', 'right')
 		self.speed = speed  # Movement speed (pixels per frame)
 
 	def move(self, constraints:list):
 		for constraint in constraints:
@@ -198,18 +195,18 @@
 				light_layer.blit(self.generate_glow(self.intensity, self.radius*2), (pos_x-100, pos_y-100), special_flags=pygame.BLEND_RGB_ADD)
 
 		# Blit the overlay with the glows on the surface
 		surface.blit(light_layer, (0,0), special_flags=pygame.BLEND_RGB_MULT)
 
 """ USER INTERFACE """
 class Button():
-	def __init__(self, game, text:str, pos:tuple, function, base=(0,0,300,81), hovered=(0,0,300,81), base_color=(77,77,255,50), hover_color=(77, 77, 80), text_color=(255,255,255), text_size=60, hovered_pos=None, id=None):
+	def __init__(self, game, text:str, position:tuple, function, base=(0,0,300,81), hovered=(0,0,300,81), base_color=(77,77,255,50), hover_color=(77, 77, 80), text_color=(255,255,255), text_size=60, hovered_pos=None, id=None):
 		self.game = game
 		self.text = text
-		self.pos = pos
+		self.position = position
 		self.id = id
 		self.function = function
 		if isinstance(base, str):
 			self.base = pygame.transform.scale(get_image(base), (128,64))
 			self.rect = self.base.get_rect()
 		else:
 			self.base = base
@@ -228,28 +225,28 @@
 		if isinstance(hovered, str):
 			self.hovered = pygame.transform.scale(get_image('../assets/ui/buttons/button_plate2.png'), (128,64))
 			self.hover_func = self.draw_image
 		else:
 			self.hovered = pygame.Rect(hovered)
 			self.hover_func = self.draw_rect
 
-		self.rect.center = self.pos
+		self.rect.center = self.position
 		self.text_color = text_color
 		self.base_color = base_color
 		self.hover_color = hover_color
 		self.size = text_size
 		if hovered_pos is None:
-			self.hovered_pos = pos
+			self.hovered_pos = position
 		else:
 			self.hovered_pos = hovered_pos
 		self.is_hovered = False
 	
 	def update(self, event:pygame.event) -> None:
-		pos = pygame.mouse.get_pos()
-		if self.rect.collidepoint(pos[0], pos[1]):
+		position = pygame.mouse.get_pos()
+		if self.rect.collidepoint(position[0], position[1]):
 			self.is_hovered = True
 			if event.type == pygame.MOUSEBUTTONDOWN and event.button == 1:
 				#play_sound("Assets/sounds/click.mp3")
 				
 				if isinstance(self.function, type):
 					self.game.sceneManager.scene = self.function(self.game)
 					return
```

### Comparing `BLACKFORGE2-0.1.post3/LICENSE` & `BLACKFORGE2-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BLACKFORGE2-0.1.post3/README.rst` & `BLACKFORGE2-0.2.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,117 +1,159 @@
-# BLACKFORGE2
-A framework for developing 2d games with python+pygame.
+# Quick-Guide
 
+# Basic Platformer With BLACKFORGE2
 
-# Simple Platformer Tutorial With BLACKFORGE2
 *This framework assumes you have an understanding of the following: ( **python**, **pygame**, **Object Oriented Programming**, **Classes** and **Inheritance** )*
 
-- *This is meant to show you some attributes, classes and functions provided by BLACKFORGE2. There are many more tools included to help you out with making your game. Go to definition on the BLACKFORGE2 import and check out some of the code to learn more about them. I will be creating documentation soon.*
+*This is meant to give you an understanding of how this framework was intended to be used while also showing you some attributes, classes and functions provided by BLACKFORGE2. There are many more tools included to help you out with making your game. You can find out more about them in the* [Documentation](https://www.notion.so/Documentation-0-1-3-40543d6137f84918bd900931ec93e02d?pvs=21)*.*
 
-- *I have provided comments within the code to explain whats going on*
+<aside>
+💡 *I have provided comments within the code to explain whats going on.*
+
+</aside>
+
+### First we get our imports ready and our project settings
 
-- First we get our imports ready and our project settings
 ---
+
 ```python
 from BLACKFORGE2 import *
 
 """ Settings """
 FPS = 60
-SCREEN_SIZE = (1000,800)
-GRAVITY = 0.62
+SCREEN_SIZE = (1000,800) # x,y
+GRAVITY = 0.62  # the gravity constant for our game
+
 ```
-- The development branch of pygame *pygame-ce* is installed when you install BLACKFORGE2.
-*If you are experiencing issues/conflicts, it is reccomended to delete pygame by running the following command:* ``` pip uninstall pygame ```
+
+<aside>
+💡 *The development branch of pygame, pygame-ce, is installed with BLACKFORGE2.
+If you are experiencing issues/conflicts, it is reccomended to delete pygame by running the following command: `pip uninstall pygame`*
+
+</aside>
+
 ---
-- First lets create a simple Player class
-*Within this Player class we will use the Physics class, and the Entity class along with their attributes to get our player set up quick and clean.*
+
+### First lets create a simple Player class
+
+<aside>
+💡 *Within this Player class we will use the [Physics](https://www.notion.so/969eff6f2dd94aa8ba95f9f88be430b8?pvs=21) class, and the [Entity](https://www.notion.so/969eff6f2dd94aa8ba95f9f88be430b8?pvs=21) class along with their attributes to get our player set up quick and clean.*
+
+</aside>
+
 ---
+
 ```python
 class Player(Entity):
     def __init__(self, game, size:int, position:tuple, speed:int, group:pygame.sprite.Group()):
         super().__init__(size, position, speed, group)
         self.game = game  # passing an instance of your main game class can give you access to other classes without imports e.g(self.game.level.level_width)
         self.image.fill([255,0,255]) # the Entity() class has a default image attribute which is just a pygame surface
         self.jump_force = -13  # the force upwards the player has when jumping
         # go to definition on the Entity class to see what other useful attributes it has
 
     def move(self):
         keys = pygame.key.get_pressed()
 
         if keys[pygame.K_d]:
-            self.velocity.x = self.speed  # the velocity attribute is used to control the speed the player will move in a certain direction
+            self.velocity.x = self.speed  # the velocity attribute is used to control 
+															#  the speed the player will move in a certain direction
         elif keys[pygame.K_a]:
             self.velocity.x = -self.speed
         else:
             self.velocity.x = 0
-        
+
         # the Entity class has atttributes to verify where a collision is happening.
-        if keys[pygame.K_SPACE] and self.collide_bottom:  # here we can implement a jump by checking the key pressed and the player's bottom collision attribute
+        if keys[pygame.K_SPACE] and self.collide_bottom:  # here we can implement a jump 
+							#  by checking the key pressed and the player's bottom collision attribute
             self.velocity.y = self.jump_force
-    
-    def update(self, terrain):  # pass the sprite group containing sprites you want the player to collide with for the collision methods to check
+
+    def update(self, terrain):  # pass the sprite group containing sprites you want the collision methods to check
         self.move()  # call the players move method which alters its velocity
         self.rect.x += self.velocity.x  # move the player's rect according to its velocity (this is done for the y direction on any Entity() that calls the apply_gravity() method.)
         # the Entity class has a physics attribute by default which comes with gravity application, and 2d collision checks
         self.physics.horizontal_movement_collision(self, terrain)  # for the collision checks, you pass the entity to perform the checks on (as the Physics class can be used alone) and the sprites to check collisions with
         self.physics.apply_gravity(self, GRAVITY)  # for gravity application you pass the entity to apply gravity to as well as the gravity constant of your game
         self.physics.vertical_movement_collision(self, terrain)
-
 ```
+
 ---
-- We can now set up a Level class which will handle creating the "layers" or sprite groups for our game, and drawing them at the correct position based on *level_data* that we pass it.
-*In this class we will use the StaticTile class to create some tiles for our player to interact with.*
+
+<aside>
+💡 *The entity class comes with a handful of attributes already set up. One of those attributes is physics. Check out the [Physics](https://www.notion.so/969eff6f2dd94aa8ba95f9f88be430b8?pvs=21) class to learn how it works.*
+
+</aside>
+
 ---
+
+### We can now set up a Level class which will handle creating the "layers" or sprite groups for our game, and drawing them at the correct position based on *level_data* that we pass it.
+
+<aside>
+💡 *In this class we will use the [StaticTile](https://www.notion.so/969eff6f2dd94aa8ba95f9f88be430b8?pvs=21) class to create some tiles for our player to interact with.*
+
+</aside>
+
+---
+
 ```python
 class Level():
     def __init__(self, game, level_data, surface):
                         # here i pass the data for the level and the surface it should be drawn to
         self.game = game
         self.level_data = level_data
         self.display_surface = surface
 
         # sprite groups setup
         self.terrain = pygame.sprite.Group()  # terrain sprites group
         self.create_tile_group(self.level_data, 'terrain', 64)
-    
+
     def create_tile_group(self, level_data, tile_type:str, tile_size:int):
-        # create a group of tile sprites based on the layout and type
+        # create a group of tile sprites based on the data and type
         tile = pygame.Surface((tile_size, tile_size))  # tile graphics
         tile.fill((25,0,50))
 
         for row_index, row in enumerate(level_data):  # iterate over each row
             for col_index, value in enumerate(row):        # and then over each column
                 if value != '0':  # here we check if a tile should be placed
                     x = col_index * tile_size
                     y = row_index * tile_size
 
-                    # use match case to handle different tile types e.g(foreground/background tiles)
+                    # use match case to handle different tile types 
+										#  e.g(foreground/background tiles)
                     match tile_type:
                         case 'terrain':
                             sprite = StaticTile((x, y), [self.terrain], tile)  # here we use the StaticTile class to create a tile that has no special properties
-                                # we pass the position, sprite group, and tile surface (the .image attribute)
+                                # we pass the position, sprite group(s), and tile surface (the .image attribute)
 
     def draw_level(self, surface:pygame.Surface):
         self.terrain.draw(surface)
-
 ```
+
 ---
-- Then we can set up a basic Game class that will contain our game loop.
+
+### Then we can set up a basic Game class that will contain our game loop.
+
+<aside>
+💡 This class is the home of our game loop, and acts as a medium between other classes.
+
+</aside>
+
 ---
+
 ```python
 class Game():
     def __init__(self):
-        # pygame.init()  # no need to init as its done for you
+        # pygame.init()  # no need to init all modules, the ones you will need have been initialized
         self.screen = pygame.display.set_mode(SCREEN_SIZE)
         pygame.display.set_caption("Example")
         self.clock = pygame.time.Clock()
         self.player_sprite_group = pygame.sprite.GroupSingle()
         self.player = Player(self, 32, (200,150), 3, [self.player_sprite_group])  # create an instance of the player class
-                          # (size, position, speed, spritegroup)
-        
+                          # (size, position, speed, sprite group(s))
+
         # sample game map (if your using tiled, you can use csv files the same way)
         game_map = [
             "1000000000000001",
             "1011110000111101",
             "1000000000000001",
             "1000000000000001",
             "1111000000001111",
@@ -140,28 +182,45 @@
             self.level.draw_level(self.screen)  # call the level's draw method
             self.player.draw(self.screen)  # call the player's draw method
             self.player.update(self.level.terrain)  # call the player's update method and pass the terrain "layer"(sprite group)
 
             self.clock.tick(FPS)
             pygame.display.flip()
 ```
+
 ---
-- Finally we can create an instance of our game class.
+
+### Finally we can create an instance of our game class.
+
 ---
-```python
+
+```
 if __name__ == "__main__":
 	game = Game()
 	game.run()
 ```
+
 ---
-- Save your project, and run the following command in the *root directiory* of said project:
+
+### Save your project, and run the following command in the *root directiory* of said project:
+
 ---
+
 ```
 python3 *filename*.py
 ```
+
 ---
-- This is the end result.
----
-![ezgif-5-358a3857db](https://github.com/setoyuma/BLACKFORGE2/assets/118138305/583399ea-3eb3-4988-92a4-4d0bbe29d083)
+
+### This is the end result.
+
 ---
-- Hopefully this tutorial provided some form of insight into some of the useful methods and classes that come with BLACKFORGE2. Feel free to check out the GitHub repo here:  https://github.com/setoyuma/BLACKFORGE2
+
+https://github.com/setoyuma/BLACKFORGE2/assets/118138305/583399ea-3eb3-4988-92a4-4d0bbe29d083
+
+Hopefully this tutorial provided some form of insight into some of the useful methods and classes that come with BLACKFORGE2 and how they are intended to be used. 
+
+Feel free to check out the GitHub repo here: https://github.com/setoyuma/BLACKFORGE2
+
 ---
+
+[Documentation](https://www.notion.so/Documentation-0-1-3-40543d6137f84918bd900931ec93e02d?pvs=21)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

