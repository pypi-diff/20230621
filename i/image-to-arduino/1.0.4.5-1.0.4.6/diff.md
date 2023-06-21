# Comparing `tmp/image-to-arduino-1.0.4.5.tar.gz` & `tmp/image-to-arduino-1.0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image-to-arduino-1.0.4.5.tar", last modified: Mon Jun 19 15:58:12 2023, max compression
+gzip compressed data, was "image-to-arduino-1.0.4.6.tar", last modified: Wed Jun 21 15:31:25 2023, max compression
```

## Comparing `image-to-arduino-1.0.4.5.tar` & `image-to-arduino-1.0.4.6.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/LICENSE
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/MANIFEST.in
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2489 2023-06-19 15:52:12.000000 image-to-arduino-1.0.4.5/README.md
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/image_to_arduino/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/image_to_arduino/__init__.py
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/image_to_arduino/__main__.py
--rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)    14653 2023-06-19 15:57:42.000000 image-to-arduino-1.0.4.5/image_to_arduino/main.py
-drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/PKG-INFO
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      380 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/SOURCES.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/dependency_links.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/entry_points.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/requires.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-06-19 15:58:12.000000 image-to-arduino-1.0.4.5/image_to_arduino.egg-info/top_level.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.5/requirements.txt
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-19 15:58:12.265240 image-to-arduino-1.0.4.5/setup.cfg
--rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      972 2023-06-19 15:57:18.000000 image-to-arduino-1.0.4.5/setup.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1066 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.6/LICENSE
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       25 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.6/MANIFEST.in
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     2782 2023-06-21 14:46:50.000000 image-to-arduino-1.0.4.6/README.md
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/image_to_arduino/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        0 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.6/image_to_arduino/__init__.py
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       78 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.6/image_to_arduino/__main__.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/image_to_arduino/icon/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     6620 2023-06-21 11:56:34.000000 image-to-arduino-1.0.4.6/image_to_arduino/icon/icon.png
+-rwxrwxr-x   0 wiktor    (1000) wiktor    (1000)    14543 2023-06-21 15:30:36.000000 image-to-arduino-1.0.4.6/image_to_arduino/main.py
+drwxrwxr-x   0 wiktor    (1000) wiktor    (1000)        0 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      364 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/PKG-INFO
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)      411 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)        1 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       68 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/entry_points.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       73 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/requires.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       17 2023-06-21 15:31:25.000000 image-to-arduino-1.0.4.6/image_to_arduino.egg-info/top_level.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       77 2023-05-19 14:21:54.000000 image-to-arduino-1.0.4.6/requirements.txt
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)       38 2023-06-21 15:31:25.815269 image-to-arduino-1.0.4.6/setup.cfg
+-rw-rw-r--   0 wiktor    (1000) wiktor    (1000)     1062 2023-06-21 15:01:33.000000 image-to-arduino-1.0.4.6/setup.py
```

### Comparing `image-to-arduino-1.0.4.5/LICENSE` & `image-to-arduino-1.0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `image-to-arduino-1.0.4.5/README.md` & `image-to-arduino-1.0.4.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+![{0ximage, 0xto, 0xarduino} (2)](https://github.com/WiktorK02/image-to-arduino/assets/123249470/0d7c1363-9f5e-4ce6-9d60-7f8a966d54be)
 # Image Converter GUI APP for Arduino oled display ssd1306 128x64
 ## About Project
 Application has been created in order to easy convert images into your <strong>Arduino</strong> project with <strong>oled displays</strong>
 ### How does it work:
 While you open .png and .jpg (others extensions in the future) image in app, the algorithm convert it to hexdeicmal array. Then it             returns full     code, ready to copy and put into the Arduino IDE. You can also preview how image will you like on your dislplay
 ## Demo
- <p align="center">
-<img src="https://user-images.githubusercontent.com/123249470/232137289-ff2707a7-a4bf-4e55-88a5-a469f54c3c3d.gif" width="350" height="560">
-</p>
+![1](https://github.com/WiktorK02/image-to-arduino/assets/123249470/13ef2888-5a98-4d0a-a8c5-c2dc26e7ea3c)
+![3](https://github.com/WiktorK02/image-to-arduino/assets/123249470/1e1bb538-91c3-4565-840a-62a25afd3da4)
+![4](https://github.com/WiktorK02/image-to-arduino/assets/123249470/580678dc-633b-4454-9760-37843860272c)
 
 ## Getting Started
 ### Prerequisites
 Download python, pip and check version
 ```
 $ pip3 --version 
 $ python --version
@@ -52,26 +53,26 @@
 4. Make changes and test<br>
 5. Submit Pull Request with comprehensive description of change
 
 ## Task list
 * add more than one display size<br>
 * make icon of the app<br>
 * make app as .exe <br>
-* fix issue with generating dark png images with trancparency
 * resize window (width)
 * optimize gif extension option (or remove it)
 * test software
+* <del> fix issue with generating dark png images with trancparency <del>
 * <del> reverse color of image </del><br>
 * <del> create function which generate full arduino code(not only arduino array) and connect it to switch button</del>
 * <del> show preview of an image </del> <br>
 * <del> upgrade graphics and style </del><br>
 * <del> add more functions </del><br>
 ## What I have learned
 *	tkinter library skills 
-*	basics of UX and GUI
+*	basics of GUI
 *	image processing 
 ## Used libraries
 * tkinter 
 * customtkinter
 * openCV
 * numpy
 ## License
```

### Comparing `image-to-arduino-1.0.4.5/image_to_arduino/main.py` & `image-to-arduino-1.0.4.6/image_to_arduino/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,25 @@
-#!/usr/bin/env python3
+
 import tkinter as tk
 import customtkinter 
 from tkinter            import filedialog
 import cv2
 import numpy            as np
 from PIL                import Image, ImageTk, ImageOps
 import os
 import imghdr
-import traceback
-
 
 file_path = ''
 image_tk = ''
-left_switch_state = False
-right_switch_state = False
-png_switch_state = False
+rvrs_colors_state = False
+full_code_state = False
+rmv_bckg_state = False
 
 def main():
-
-
+    
     def open_file():
         global file_path
         file_path = filedialog.askopenfilename()
         if file_path:
             # If file name len is greater than 15: return ... + extension
             file_label.configure(
                 text="File: "
@@ -30,107 +27,86 @@
                     os.path.basename(file_path)
                     if len(os.path.basename(file_path)) < 15
                     else "..." + imghdr.what(file_path)
                 )
             )
         else:
             file_label.configure(text="No file selected")
-    def image_conv():
-        if not png_switch_state:
+
+    def image_to_hex():
+        if not rmv_bckg_state:
             img = Image.open(file_path).convert("RGBA")
             img = img.resize((128, 64))
             img = ImageOps.grayscale(img)
-            if left_switch_state:
+            if rvrs_colors_state:
             # Reverse the colors of the image
                 img= ImageOps.invert(img)
             
             # Convert the PIL Image to a NumPy array and apply thresholding
             img_arr = np.array(img)
             _, thresholded_image = cv2.threshold(img_arr, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
             
             # Convert the thresholded image to a binary array (0s and 1s)
             binary_array = np.where(thresholded_image > 0, 1, 0)
-            
-            # Convert the binary array to a 1D array
-            one_d_array = binary_array.flatten()
-            
-            # Split the binary alpha values into 8-byte arrays
-            byte_arrays = np.packbits(one_d_array)
-            
-            # Convert byte arrays to hexadecimal format
-            hex_byte_arrays = ['0x' + format(byte, '02x') for byte in byte_arrays]
-            
-            cpp_array = ', '.join(hex_byte_arrays)
-            
-            # Insert newline after every 10 hexadecimal numbers
-            cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
-            cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
-            cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
-            
-            return cpp_array
+                
         else:
             image = cv2.imread(file_path, cv2.IMREAD_UNCHANGED)
             image = cv2.resize(image, (128, 64))
             
             # Split the image into channels
             b, g, r, a = cv2.split(image)
-        
-            
+    
             # Convert the thresholded image to a binary array (0s and 1s)
             binary_array = np.where(a > 0, 1, 0)
             
-            # Convert the binary array to a 1D array
-            one_d_array = binary_array.flatten()
-            
-            if left_switch_state:
-                one_d_array = 1 - one_d_array
-            
-            # Split the binary alpha values into 8-bit arrays
-            byte_arrays = np.packbits(one_d_array)
-            
-            # Convert byte arrays to hexadecimal format
-            hex_byte_arrays = ['0x' + format(byte, '02x') for byte in byte_arrays]
-            
-            cpp_array = ', '.join(hex_byte_arrays)
-            
-            # Insert newline after every 10 hexadecimal numbers
-            cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
-            cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
-            cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
+        # Convert the binary array to a 1D array
+        one_d_array = binary_array.flatten()
             
-            return cpp_array
+        if rvrs_colors_state and rmv_bckg_state:
+            one_d_array = 1 - one_d_array
+        
+        # Split the binary alpha values into 8-bit arrays
+        byte_arrays = np.packbits(one_d_array)
+        
+        # Convert byte arrays to hexadecimal format
+        hex_byte_arrays = ['0x' + format(byte, '02x') for byte in byte_arrays]
+        
+        cpp_array = ', '.join(hex_byte_arrays)
+        
+        # Insert newline after every 10 hexadecimal numbers
+        cpp_array = [cpp_array[i:i+2] for i in range(0, len(cpp_array), 2)]  # Split into pairs of hexadecimal numbers
+        cpp_array = [''.join(cpp_array[i:i+30]) for i in range(0, len(cpp_array), 30)]  # Join pairs with space, and group every 10 pairs
+        cpp_array = '\n'.join(cpp_array)  # Join groups with newline character
+        
+        return cpp_array
 
-    def update_img_pre():
-        if not png_switch_state:
+    def update_img_preview():
+        if not rmv_bckg_state:
             img = Image.open(file_path).convert("RGBA")
             
             img = img.resize((128, 64))
             img = ImageOps.grayscale(img)
             
-            if left_switch_state:
+            if rvrs_colors_state:
                 # Reverse the colors of the image
                 img = ImageOps.invert(img)
             
             # Convert the PIL Image to a NumPy array and apply thresholding
             img_arr = np.array(img)
             _, thresholded_image = cv2.threshold(img_arr, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
             
             image_preview_label.config(image="")
             bw_img = Image.fromarray(thresholded_image)
             
-            # Update image preview
-            image_pre = ImageTk.PhotoImage(bw_img)
-            image_preview_label.config(image=image_pre)
-            image_preview_label.image = image_pre
         else:    
             image = cv2.imread(file_path, cv2.IMREAD_UNCHANGED)
             # Split the image into channels
             b, g, r, a = cv2.split(image)
             # Check if the image has an alpha channel
-            if image.shape[2] == 4 and left_switch_state:
+            if image.shape[2] == 4 and rvrs_colors_state:
                 
                 # Set transparent pixels to white
                 white_mask = (a == 0)
                 b[white_mask] = 255
                 g[white_mask] = 255
                 r[white_mask] = 255
                 
@@ -139,15 +115,15 @@
                 b[non_transparent_mask] = 0
                 g[non_transparent_mask] = 0
                 r[non_transparent_mask] = 0
                 # Set white pixels to non-transparent (alpha to 255)
                 white_pixels = (b == 255) & (g == 255) & (r == 255)
                 a[white_pixels] = 255
                 
-            elif not left_switch_state:
+            elif not rvrs_colors_state:
                 # Set transparent pixels to white
                 white_mask = (a == 0)
                 b[white_mask] = 0
                 g[white_mask] = 0
                 r[white_mask] = 0
                 
                 # Set non-transparent pixels to black
@@ -163,88 +139,87 @@
             # Convert the image to a NumPy array
             img_arr = np.array(image)
 
             image_preview_label.config(image="")
             resized_image = cv2.resize(img_arr, (128, 64))
             bw_img = Image.fromarray(resized_image)
             
-            # Update image preview
-            image_pre = ImageTk.PhotoImage(bw_img)
-            image_preview_label.config(image=image_pre)
-            image_preview_label.image = image_pre
-   
-    def update_gif():
-        global image_previews
-        frames_list = []
-        image_previews = []
-        # open the GIF file
-        gif_file = Image.open(file_path)
-
-        # loop through each frame of the GIF
-        for frame in range(0, gif_file.n_frames):
-            gif_file.seek(frame)
-
-            # extract the transparency mask if it exists
-            transparency_mask = gif_file.convert("RGBA").split()[-1] if gif_file.info.get("transparency") else None
-
-            # create a new RGBA image with the same size as the original
-            new_image = Image.new("RGBA", gif_file.size)
-
-            # paste the current frame onto the new image, preserving transparency
-            new_image.paste(gif_file, (0, 0), transparency_mask)
-
-                # Replace transparent pixels with white
-            new_image = Image.alpha_composite(Image.new("RGBA", new_image.size, (255, 255, 255, 255)), new_image)
-
-            new_image = new_image.resize((128, 64))
-
-            new_image = ImageOps.grayscale(new_image)
-            if left_switch_state == True:
-                # Reverse the colors of the image
-                new_image= ImageOps.invert(new_image)
-            # Convert the PIL Image to a NumPy array and apply thresholding
-            img_arr = np.array(new_image)
-            _, thresholded_image = cv2.threshold(img_arr, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
-            
-            image_preview_label.config(image="")
-            bw_img = Image.fromarray(thresholded_image).convert('L')
-            photo = ImageTk.PhotoImage(bw_img)
-            image_previews.append(photo)
-
-        # Display the first frame preview
-        current_frame = 0
-
-
-        def update_preview():
-            nonlocal current_frame
-            current_frame = (current_frame+1) % len(image_previews)
-            image_preview_label.config(image=image_previews[current_frame])
-            image_preview_label.after(100, update_preview)  # Update every 100 ms
+        # Update image preview
+        image_pre = ImageTk.PhotoImage(bw_img)
+        image_preview_label.config(image=image_pre)
+        image_preview_label.image = image_pre
+
+    # def update_gif():
+    #     global image_previews
+    #     frames_list = []
+    #     image_previews = []
+    #     # open the GIF file
+    #     gif_file = Image.open(file_path)
+
+    #     # loop through each frame of the GIF
+    #     for frame in range(0, gif_file.n_frames):
+    #         gif_file.seek(frame)
+
+    #         # extract the transparency mask if it exists
+    #         transparency_mask = gif_file.convert("RGBA").split()[-1] if gif_file.info.get("transparency") else None
+
+    #         # create a new RGBA image with the same size as the original
+    #         new_image = Image.new("RGBA", gif_file.size)
+
+    #         # paste the current frame onto the new image, preserving transparency
+    #         new_image.paste(gif_file, (0, 0), transparency_mask)
+
+    #             # Replace transparent pixels with white
+    #         new_image = Image.alpha_composite(Image.new("RGBA", new_image.size, (255, 255, 255, 255)), new_image)
+
+    #         new_image = new_image.resize((128, 64))
+
+    #         new_image = ImageOps.grayscale(new_image)
+    #         if rvrs_colors_state == True:
+    #             # Reverse the colors of the image
+    #             new_image= ImageOps.invert(new_image)
+    #         # Convert the PIL Image to a NumPy array and apply thresholding
+    #         img_arr = np.array(new_image)
+    #         _, thresholded_image = cv2.threshold(img_arr, 0, 255, cv2.THRESH_BINARY + cv2.THRESH_OTSU)
+            
+    #         image_preview_label.config(image="")
+    #         bw_img = Image.fromarray(thresholded_image).convert('L')
+    #         photo = ImageTk.PhotoImage(bw_img)
+    #         image_previews.append(photo)
+
+    #     # Display the first frame preview
+    #     current_frame = 0
+
+    #     def update_preview():
+    #         nonlocal current_frame
+    #         current_frame = (current_frame+1) % len(image_previews)
+    #         image_preview_label.config(image=image_previews[current_frame])
+    #         image_preview_label.after(100, update_preview)  # Update every 100 ms
         
-        # Start updating the preview
-        image_preview_label.after(100, update_preview)
+    #     # Start updating the preview
+    #     image_preview_label.after(100, update_preview)
 
-    def generate_text():
+    def generate_hex_array():
         global image_tk, switch_var
         if not file_path == '':    
             try:
                 # To check extenxion
                 extension = imghdr.what(file_path)
                 if  extension == "jpeg" or extension == "png":
-                    update_img_pre()
-                    if right_switch_state == False:
+                    update_img_preview()
+                    if full_code_state == False:
                         # Generate C++ array
-                        cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + image_conv() + '\n};' 
-                    elif right_switch_state == True:
+                        cpp_array = 'const unsigned char PROGMEM ' + os.path.splitext(os.path.basename(file_path))[0] + ' [] = {\n' + image_to_hex() + '\n};' 
+                    elif full_code_state == True:
                         # Generate full code ready to use 
                         cpp_array = '''#include <Adafruit_SSD1306.h>
 #include <Adafruit_GFX.h>
 #define OLED_RESET 4
 Adafruit_SSD1306 display(OLED_RESET);
-const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {\n''' +  image_conv() + ''' };
+const unsigned char PROGMEM ''' + os.path.splitext(os.path.basename(file_path))[0] + '''[] = {\n''' +  image_to_hex() + ''' };
 void setup() 
 {
     display.begin(SSD1306_SWITCHCAPVCC, 0x3C);
     display.display();
     delay(2000);
     display.clearDisplay();}
 void loop() 
@@ -253,71 +228,108 @@
     display.display();
     delay(5000);
     display.clearDisplay();
     delay(5000);}'''        
 
                     output_text.delete(1.0, tk.END)
                     output_text.insert(tk.END, cpp_array)
-                elif extension == "gif":
-                    update_gif()
+                # elif extension == "gif":
+                #     update_gif()
             # In case of error or invalid extension         
             except:
                 output_text.delete(1.0, tk.END)
                 output_text.insert(tk.END, "Error generating text")
         else: 
             output_text.delete(1.0, tk.END)
             output_text.insert(tk.END, "Select any file")
+    
     def copy_all():
         if not file_path:
             copied_all_label.configure(text="No text to copy")
             return
 
         root.clipboard_clear()
         root.clipboard_append(output_text.get(1.0, tk.END))
         copied_all_label.configure(text="✓ Copied")
 
-    def toggle_left_switch():
-        global left_switch_state
-        left_switch_state = not left_switch_state
-
-    def toggle_right_switch():
-        global right_switch_state
-        right_switch_state = not right_switch_state
+    def toggle_rvrs_colors_switch():
+        global rvrs_colors_state
+        rvrs_colors_state = not rvrs_colors_state
+
+    def toggle_full_code_switch():
+        global full_code_state
+        full_code_state = not full_code_state
     
-    def toggle_png_switch():
-        global png_switch_state
-        png_switch_state = not png_switch_state
+    def toggle_rmv_bckg_switch():
+        global rmv_bckg_state
+        rmv_bckg_state = not rmv_bckg_state
 
     def clear_all():
         global image_previews
         # Clear output text and image preview
         output_text.delete(1.0, tk.END)
         image_preview_label.config(image="")
         image_previews = []
+    
+    def callback():
+        global after_id
+        var.set(var.get() + 1)
+        after_id = root.after(500, callback)
+
+    def quit():
+        """Cancel all scheduled callbacks and quit."""
+        root.after_cancel(after_id)
+        root.destroy()
 
     customtkinter.set_appearance_mode("dark")  
     customtkinter.set_default_color_theme("dark-blue")  
 
     # Create customtkinter window
     root = customtkinter.CTk() 
+
+    w = 340 # Width for the Tk root
+    h = 600 # Height for the Tk root
+
+    # Get screen width and height
+    ws = root.winfo_screenwidth() # width of the screen
+    hs = root.winfo_screenheight() # height of the screen
+
+    # Calculate x and y coordinates for the Tk root window
+    x = (ws/2) - (w/2)
+    y = (hs/2) - (h/2)
+
+    # Set where it is placed
+    root.geometry('%dx%d+%d+%d' % (w, h, x, y))
     root.title("Image to arduino")
+   
+    var = tk.IntVar()
 
     # Set window size
-    root.geometry("340x600") # Set width and height as desired
+    root.geometry(f"{w}x{h}") # Set width and height as desired
+    
+    # Configure the window to not be resizable
+    root.resizable(False, False)  
+    
+    # Icon app
+    current_file = __file__
+    current_dir = os.path.dirname(current_file)
+    icon_file = os.path.join(current_dir, 'icon', 'icon.png')
+    icon = tk.PhotoImage(file=icon_file)
+    root.iconphoto(False, icon, icon)
 
     # Label for displaying selected file path
     file_label =  customtkinter.CTkLabel(root, text="No file selected")
     file_label.grid(row=0, column=0, padx=10, columnspan=1, sticky="nsew", pady=5)
 
     # "Open File" button
     open_file_button = customtkinter.CTkButton(root, text="Open File", command=open_file)
     open_file_button.grid(row=0, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")
 
     # "Generate" button
-    generate_button = customtkinter.CTkButton(root, text="Generate Code", command=generate_text)
+    generate_button = customtkinter.CTkButton(root, text="Generate Code", command=generate_hex_array)
     generate_button.grid(row=3, column=0, padx=10, pady=5, columnspan=1, sticky="nsew")
 
     # "Copy All" button
     copy_all_button = customtkinter.CTkButton(root, text="Copy All", command=copy_all)
     copy_all_button.grid(row=3, column=1, padx=10, pady=5, columnspan=1, sticky="nsew")  
 
     # Output text 
@@ -333,26 +345,28 @@
     preview_text_label.grid(row=6, column=0, pady=5, padx=10)
 
     # Label to display the image
     image_preview_label = tk.Label(root, bg="#1b1a1b")
     image_preview_label.grid(row=7, column=0, columnspan=1, padx=10)
 
     # Switch label left
-    switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_left_switch)
+    switch = customtkinter.CTkSwitch(root, text="Reverse colors", command=toggle_rvrs_colors_switch)
     switch.grid(row=1, column=0, padx=10, sticky="nsew")
 
     # Switch label png
-    switch = customtkinter.CTkSwitch(root, text="Remove background", command=toggle_png_switch)
+    switch = customtkinter.CTkSwitch(root, text="Remove background", command=toggle_rmv_bckg_switch)
     switch.grid(row=2, column=0, padx=10, sticky="nsew")
 
     # Switch label right 
-    switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_right_switch)
+    switch_right = customtkinter.CTkSwitch(root, text="Full arduino code", command=toggle_full_code_switch)
     switch_right.grid(row=1, column=1, padx=10, sticky="nsew")
 
     # "Clear all" button 
     clear_all_button = customtkinter.CTkButton(root, text="Clear All", command=clear_all)
     clear_all_button.grid(row=5, column=0, pady=5, padx=10, columnspan=1, sticky="nsew")  
 
-    # Configure the window to not be resizable
-    root.resizable(False, False)
+
+    callback()
+    root.protocol('WM_DELETE_WINDOW', quit)
 
     root.mainloop()
+
```

### Comparing `image-to-arduino-1.0.4.5/setup.py` & `image-to-arduino-1.0.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,24 +6,26 @@
 with open(req_file, 'r') as f:
     REQUIREMENTS = [line.strip() for line in f.readlines()]
 
 LONG_DESCRIPTION = 'About Image converter GUI App to arduino oled display ssd1306 128x64'
 
 setup(
    name='image-to-arduino',
-   version='1.0.4.5',
+   version='1.0.4.6',
    description='Image converter to arduino',
    license="MIT",
    author='WiktorK02',
    author_email='wiktor.kidon@hotmail.com',
    url="https://github.com/WiktorK02/Image_Converter_App.git",
    long_description_content_type="text/markdown",
    long_description=LONG_DESCRIPTION,
-   packages=['image_to_arduino'],
-   package_data={'image_to_arduino': ['data/*.dat']},
+   packages=find_packages(),
+   include_package_data=True,
+   package_data={'gravitypy': ['*']},
+   data_files=[('image_to_arduino/icon', ['image_to_arduino/icon/icon.png'])],
    install_requires=REQUIREMENTS, 
     entry_points={
         'console_scripts': [
             'image-to-arduino = image_to_arduino.__main__:main'
         ]
     },
```

