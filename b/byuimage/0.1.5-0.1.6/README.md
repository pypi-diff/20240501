# Comparing `tmp/byuimage-0.1.5.tar.gz` & `tmp/byuimage-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byuimage-0.1.5.tar", max compression
+gzip compressed data, was "byuimage-0.1.6.tar", max compression
```

## Comparing `byuimage-0.1.5.tar` & `byuimage-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0     1066 2021-12-21 16:42:19.652632 byuimage-0.1.5/LICENSE
--rw-r--r--   0        0        0     4956 2022-02-11 22:27:06.747704 byuimage-0.1.5/byuimage.py
--rw-r--r--   0        0        0      402 2022-02-11 22:28:02.706699 byuimage-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      602 2022-02-11 22:29:07.663774 byuimage-0.1.5/setup.py
--rw-r--r--   0        0        0      479 2022-02-11 22:29:07.663989 byuimage-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     5079 2024-05-01 18:25:29.000000 byuimage-0.1.6/byuimage.py
+-rw-r--r--   0        0        0     1087 2024-04-30 17:21:43.000000 byuimage-0.1.6/LICENSE
+-rw-r--r--   0        0        0      455 2024-05-01 18:40:43.000000 byuimage-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      575 1970-01-01 00:00:00.000000 byuimage-0.1.6/PKG-INFO
```

### Comparing `byuimage-0.1.5/LICENSE` & `byuimage-0.1.6/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 BYU-CS110
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 BYU-CS110
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `byuimage-0.1.5/byuimage.py` & `byuimage-0.1.6/byuimage.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,148 @@
-from PIL import Image as PILImage
-
-""" A simple image library that is built on top of pillow. For details, see
-    https://python-pillow.org
-"""
-
-# Constants that represent the first (X) and second (Y) tuple in a location
-# coordinate (X, Y)
-X = 0
-Y = 1
-
-# Constants that represent the red (R), green (G), and blue (B) portions of
-# a pixel color
-R = 0
-G = 1
-B = 2
-
-
-class ImageInitializationError(Exception):
-    """ Exception used when initializing an image without a required filename """
-    def __init__(self, message="Must supply a filename"):
-        self.message = message
-        super().__init__(self.message)
-
-
-class Pixel:
-    """ The Pixel class is used to represent a single pixel in an image. It
-        has a location (X,Y) coordinate and references the image in which
-        it is located. Users can get or set the RGB values of a pixel.
-    """
-    def __init__(self, location, image):
-        """ Initialize a pixel with location (X,Y) coordinate and an image """
-        self.location = location
-        self.image = image
-
-    @property
-    def red(self):
-        """ gets the red portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        return rgb[R]
-
-    @red.setter
-    def red(self, value):
-        """ sets the red portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        self.image.putpixel(self.location, (int(value), rgb[G], rgb[B]))
-
-    @property
-    def green(self):
-        """ gets the green portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        return rgb[G]
-
-    @green.setter
-    def green(self, value):
-        """ sets the green portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        self.image.putpixel(self.location, (rgb[R], int(value), rgb[B]))
-
-    @property
-    def blue(self):
-        """ gets the blue portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        return rgb[B]
-
-    @blue.setter
-    def blue(self, value):
-        """ sets the blue portion of the pixel value """
-        rgb = self.image.getpixel(self.location)
-        self.image.putpixel(self.location, (rgb[R], rgb[G], int(value)))
-
-
-class Image:
-    """ The SimpleImage class provides a simplified interface to interact with
-        images. Users can iterate over the pixels in the image, get the pixel at
-        a particular (X, Y) coordinate, and get image properties such as height
-        and width. Users interact with the Pixel class to get or change the RGB
-        values of individual pixels.
-    """
-    def __init__(self, filename: str, image=None):
-        """ Initialize an image with either a filename or an image. If given a
-            filename, the image is initialized from the file. If given an image,
-            the image is initialized as a copy of this image. If neither a
-            filename or an image is supplied, an exception is raised.
-
-            image - a reference to a pillow image
-            pixels - the pixels in the image
-            location - the (X, Y) coordinate of the current pixel, used when
-                iterating over all pixels; initialized to (0, 0)
-        """
-        if filename:
-            self.image = PILImage.open(filename).convert('RGB')
-        elif image:
-            self.image = image
-        else:
-            raise ImageInitializationError
-        self.pixels = self.image.load()
-        self.location = (0, 0)
-
-    @property
-    def height(self):
-        """ Get the height of the image in pixels """
-        return self.image.height
-
-    @property
-    def width(self):
-        """ Get the width of the image in pixels """
-        return self.image.width
-
-    def __iter__(self):
-        """ Return an iterator """
-        return self
-
-    def __next__(self):
-        """ Get the next pixel in the image, based on the (X, Y) coordinate of
-            the current pixel. Used for an iterator.
-            """
-        loc = self.location
-        if self.location[Y] == self.height:
-            self.location = (0, 0)
-            raise StopIteration
-        self.location = (self.location[X] + 1, self.location[Y])
-        if self.location[X] == self.width:
-            self.location = (0, self.location[Y] + 1)
-        return Pixel(loc, self.image)
-
-    def show(self):
-        """ Shows the image in a window. """
-        self.image.show()
-
-    def save(self, filename):
-        self.image.save(filename, quality=100)
-
-    def get_pixel(self, x, y):
-        """ Returns the pixel at the given (X, Y) coordinate """
-        return Pixel((x, y), self.image)
-
-    @staticmethod
-    def blank(width, height):
-        """ Creates a blank (white) image of a given width and height. Can
-            be passed an optional color to make an image of the desired color.
-        """
-        image = PILImage.new(mode="RGB", size=(width, height), color="white")
-        i = Image(filename=None, image=image)
-        return i
+from PIL import Image as PILImage
+
+""" A simple image library that is built on top of pillow. For details, see
+    https://python-pillow.org
+"""
+
+# Constants that represent the first (X) and second (Y) tuple in a location
+# coordinate (X, Y)
+X = 0
+Y = 1
+
+# Constants that represent the red (R), green (G), and blue (B) portions of
+# a pixel color
+R = 0
+G = 1
+B = 2
+
+
+class ImageInitializationError(Exception):
+    """ Exception used when initializing an image without a required filename """
+    def __init__(self, message="Must supply a filename"):
+        self.message = message
+        super().__init__(self.message)
+
+
+class Pixel:
+    """ The Pixel class is used to represent a single pixel in an image. It
+        has a location (X,Y) coordinate and references the image in which
+        it is located. Users can get or set the RGB values of a pixel.
+    """
+    def __init__(self, location, image_data):
+        """ Initialize a pixel with location (X,Y) coordinate and an image """
+        self.location = location
+        self.image_data = image_data
+
+    @property
+    def red(self):
+        """ gets the red portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        return r
+
+    @red.setter
+    def red(self, value):
+        """ sets the red portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        self.image_data[self.location] = (int(value), g, b)
+
+    @property
+    def green(self):
+        """ gets the green portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        return g
+
+    @green.setter
+    def green(self, value):
+        """ sets the green portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        self.image_data[self.location] = (r, int(value), b)
+
+    @property
+    def blue(self):
+        """ gets the blue portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        return b
+
+    @blue.setter
+    def blue(self, value):
+        """ sets the blue portion of the pixel value """
+        r, g, b = self.image_data[self.location]
+        self.image_data[self.location] = (r, g, int(value), 255)
+
+    @property
+    def color(self):
+        """ gets the full rgb color of the pixel """
+        return self.image_data[self.location]
+    
+    @color.setter
+    def color(self, value):
+        """ sets the full rgb color of a pixel at once """
+        self.image_data[self.location] = value
+
+
+class Image:
+    """ The SimpleImage class provides a simplified interface to interact with
+        images. Users can iterate over the pixels in the image, get the pixel at
+        a particular (X, Y) coordinate, and get image properties such as height
+        and width. Users interact with the Pixel class to get or change the RGB
+        values of individual pixels.
+    """
+    def __init__(self, filename: str, image=None):
+        """ Initialize an image with either a filename or an image. If given a
+            filename, the image is initialized from the file. If given an image,
+            the image is initialized as a copy of this image. If neither a
+            filename or an image is supplied, an exception is raised.
+
+            image - a reference to a pillow image
+            pixels - the pixels in the image
+            location - the (X, Y) coordinate of the current pixel, used when
+                iterating over all pixels; initialized to (0, 0)
+        """
+        if filename:
+            self.image = PILImage.open(filename).convert('RGB')
+        elif image:
+            self.image = image
+        else:
+            raise ImageInitializationError
+        self.pixels = self.image.load()
+        self.location = (0, 0)
+        self.generator = self.pixel_generator()
+
+    @property
+    def height(self):
+        """ Get the height of the image in pixels """
+        return self.image.height
+
+    @property
+    def width(self):
+        """ Get the width of the image in pixels """
+        return self.image.width
+    
+    def pixel_generator(self):
+        for y in range(self.height):
+            for x in range(self.width):
+                yield Pixel((x, y), self.pixels)
+
+    def __iter__(self):
+        """ Return an iterator """
+        return self.pixel_generator()
+
+    def show(self):
+        """ Shows the image in a window. """
+        self.image.show()
+
+    def save(self, filename):
+        self.image.save(filename, quality=100)
+
+    def get_pixel(self, x, y):
+        """ Returns the pixel at the given (X, Y) coordinate """
+        return Pixel((x, y), self.pixels)
+
+    @staticmethod
+    def blank(width, height):
+        """ Creates a blank (white) image of a given width and height. Can
+            be passed an optional color to make an image of the desired color.
+        """
+        image = PILImage.new(mode="RGB", size=(width, height), color="white")
+        i = Image(filename=None, image=image)
+        return i
```

