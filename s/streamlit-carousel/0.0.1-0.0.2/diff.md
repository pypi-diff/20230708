# Comparing `tmp/streamlit_carousel-0.0.1.tar.gz` & `tmp/streamlit_carousel-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_carousel-0.0.1.tar", last modified: Sat Jul  8 16:21:17 2023, max compression
+gzip compressed data, was "streamlit_carousel-0.0.2.tar", last modified: Sat Jul  8 16:46:06 2023, max compression
```

## Comparing `streamlit_carousel-0.0.1.tar` & `streamlit_carousel-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:21:17.024811 streamlit_carousel-0.0.1/
--rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       63 2023-07-08 13:29:37.000000 streamlit_carousel-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4906 2023-07-08 16:21:17.023805 streamlit_carousel-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-07-08 16:14:36.000000 streamlit_carousel-0.0.1/README.md
--rw-rw-rw-   0        0        0      895 2023-07-08 13:28:44.000000 streamlit_carousel-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-08 16:21:17.024811 streamlit_carousel-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      740 2023-07-08 13:26:46.000000 streamlit_carousel-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:21:17.004803 streamlit_carousel-0.0.1/streamlit_carousel/
--rw-rw-rw-   0        0        0     4863 2023-07-08 16:19:18.000000 streamlit_carousel-0.0.1/streamlit_carousel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:21:17.021802 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/
--rw-rw-rw-   0        0        0     4906 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       60 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-07-08 16:21:16.000000 streamlit_carousel-0.0.1/streamlit_carousel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/
+-rw-rw-rw-   0        0        0     1076 2023-07-03 17:27:05.000000 streamlit_carousel-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       53 2023-07-08 16:44:00.000000 streamlit_carousel-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4918 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2997 2023-07-08 16:34:50.000000 streamlit_carousel-0.0.2/README.md
+-rw-rw-rw-   0        0        0      907 2023-07-08 16:36:00.000000 streamlit_carousel-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      740 2023-07-08 16:35:57.000000 streamlit_carousel-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.244831 streamlit_carousel-0.0.2/streamlit_carousel/
+-rw-rw-rw-   0        0        0     4863 2023-07-08 16:19:18.000000 streamlit_carousel-0.0.2/streamlit_carousel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.229206 streamlit_carousel-0.0.2/streamlit_carousel/carousel/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/
+-rw-rw-rw-   0        0        0     1058 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/asset-manifest.json
+-rw-rw-rw-   0        0        0     1910 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/index.html
+-rw-rw-rw-   0        0        0      660 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/precache-manifest.22851dbcebea0476fd3c97bc108bb6e8.js
+-rw-rw-rw-   0        0        0     1183 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.229206 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/
+-rw-rw-rw-   0        0        0   241050 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css
+-rw-rw-rw-   0        0        0   583870 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/css/2.777d1846.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.291706 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/
+-rw-rw-rw-   0        0        0   616599 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js
+-rw-rw-rw-   0        0        0     2181 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1664534 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/2.4dc317cb.chunk.js.map
+-rw-rw-rw-   0        0        0     1351 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js
+-rw-rw-rw-   0        0        0     3998 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/main.f596a625.chunk.js.map
+-rw-rw-rw-   0        0        0     1578 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js
+-rw-rw-rw-   0        0        0     8297 2023-07-08 16:31:21.000000 streamlit_carousel-0.0.2/streamlit_carousel/carousel/build/static/js/runtime-main.5e408f89.js.map
+drwxrwxrwx   0        0        0        0 2023-07-08 16:46:06.260454 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/
+-rw-rw-rw-   0        0        0     4918 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1201 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       60 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-07-08 16:46:06.000000 streamlit_carousel-0.0.2/streamlit_carousel.egg-info/top_level.txt
```

### Comparing `streamlit_carousel-0.0.1/LICENSE` & `streamlit_carousel-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.1/PKG-INFO` & `streamlit_carousel-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit_carousel
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
+Project-URL: Homepage, https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel
 Keywords: python,streamlit,react,bootstrap,carousel,gallery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -81,18 +81,18 @@
 - Only url images are supported for now (not local files)
 - A 'use_container_width' argument needs to be added
 - If an item's text is too long, it overflows on other items
 
 ## Contributing
 Contributions to Streamlit Carousel are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
 
-Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/README.md) for more information.
+Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/README.md) for more information.
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/LICENSE) for more information.
+This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/LICENSE) for more information.
 
 ## Credits
 Streamlit Carousel is created and maintained by Thomas Bouamoud. 
 It leverages the [React Bootstrap Carousel component](https://react-bootstrap.netlify.app/docs/components/carousel/) and utilizes the Streamlit Custom Components feature.
 
 ## Contact
 If you have any questions or inquiries, feel free to reach out to thomas.bouamoud@gmail.com.
```

### Comparing `streamlit_carousel-0.0.1/README.md` & `streamlit_carousel-0.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -46,18 +46,18 @@
 - Only url images are supported for now (not local files)
 - A 'use_container_width' argument needs to be added
 - If an item's text is too long, it overflows on other items
 
 ## Contributing
 Contributions to Streamlit Carousel are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
 
-Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/README.md) for more information.
+Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/README.md) for more information.
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/LICENSE) for more information.
+This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/LICENSE) for more information.
 
 ## Credits
 Streamlit Carousel is created and maintained by Thomas Bouamoud. 
 It leverages the [React Bootstrap Carousel component](https://react-bootstrap.netlify.app/docs/components/carousel/) and utilizes the Streamlit Custom Components feature.
 
 ## Contact
 If you have any questions or inquiries, feel free to reach out to thomas.bouamoud@gmail.com.
```

### Comparing `streamlit_carousel-0.0.1/pyproject.toml` & `streamlit_carousel-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "streamlit_carousel"
-version = "0.0.1"
+version = "0.0.2"
 description = "A Streamlit implementation of the React Bootstrap Carousel component."
 readme = "README.md"
 authors = [{ name = "Thomas Bouamoud", email = "thomas.bouamoud@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -19,11 +19,11 @@
 ]
 requires-python = ">=3.6"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
-Homepage = "https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel"
+Homepage = "https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel"
 
 [project.scripts]
 realpython = "reader.__main__:main"
```

### Comparing `streamlit_carousel-0.0.1/setup.py` & `streamlit_carousel-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit_carousel",
-    version="0.0.1",
+    version="0.0.2",
     author="Thomas Bouamoud",
     author_email="thomas.bouamoud@gmail.com",
     description="A Streamlit implementation of the React Bootstrap Carousel component.",
     long_description="https://react-bootstrap.netlify.app/docs/components/carousel/",
     long_description_content_type="text/plain",
     url="https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit_carousel-0.0.1/streamlit_carousel/__init__.py` & `streamlit_carousel-0.0.2/streamlit_carousel/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_carousel-0.0.1/streamlit_carousel.egg-info/PKG-INFO` & `streamlit_carousel-0.0.2/streamlit_carousel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-carousel
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit implementation of the React Bootstrap Carousel component.
 Home-page: https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
 Author: Thomas Bouamoud
 Author-email: Thomas Bouamoud <thomas.bouamoud@gmail.com>
 License: Copyright (c) 2023 Thomas Bouamoud
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -20,15 +20,15 @@
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
-Project-URL: Homepage, https://github.com/thomasbs17/streamlit-contributions/bootstrap_carousel
+Project-URL: Homepage, https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel
 Keywords: python,streamlit,react,bootstrap,carousel,gallery
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
@@ -81,18 +81,18 @@
 - Only url images are supported for now (not local files)
 - A 'use_container_width' argument needs to be added
 - If an item's text is too long, it overflows on other items
 
 ## Contributing
 Contributions to Streamlit Carousel are welcome! If you find any issues or have suggestions for improvements, please open an issue on the [GitHub repository](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel). If you'd like to contribute code, you can fork the repository, make your changes, and submit a pull request.
 
-Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/README.md) for more information.
+Before contributing, please review the [Contributing Guidelines](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/README.md) for more information.
 
 ## License
-This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/blob/master/bootstrap_carousel/LICENSE) for more information.
+This package is licensed under the MIT License. See the [LICENSE file](https://github.com/thomasbs17/streamlit-contributions/tree/master/bootstrap_carousel/LICENSE) for more information.
 
 ## Credits
 Streamlit Carousel is created and maintained by Thomas Bouamoud. 
 It leverages the [React Bootstrap Carousel component](https://react-bootstrap.netlify.app/docs/components/carousel/) and utilizes the Streamlit Custom Components feature.
 
 ## Contact
 If you have any questions or inquiries, feel free to reach out to thomas.bouamoud@gmail.com.
```

