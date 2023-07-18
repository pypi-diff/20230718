# Comparing `tmp/pynamicui-0.0.2.tar.gz` & `tmp/pynamicui-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamicui-0.0.2.tar", last modified: Tue Jul 18 07:36:37 2023, max compression
+gzip compressed data, was "pynamicui-0.0.3.tar", last modified: Tue Jul 18 07:42:25 2023, max compression
```

## Comparing `pynamicui-0.0.2.tar` & `pynamicui-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.806503 pynamicui-0.0.2/
--rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      775 2023-07-18 07:36:37.807505 pynamicui-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    17677 2023-07-18 01:40:07.000000 pynamicui-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.760503 pynamicui-0.0.2/pynamicui/
--rw-rw-rw-   0        0        0      386 2023-07-18 07:32:34.000000 pynamicui-0.0.2/pynamicui/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-18 07:36:37.804508 pynamicui-0.0.2/pynamicui.egg-info/
--rw-rw-rw-   0        0        0      775 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-18 07:36:37.000000 pynamicui-0.0.2/pynamicui.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      779 2023-07-18 07:32:57.000000 pynamicui-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0     1108 2023-07-18 07:36:37.811506 pynamicui-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.385733 pynamicui-0.0.3/
+-rw-rw-rw-   0        0        0    11542 2023-07-18 06:19:12.000000 pynamicui-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      775 2023-07-18 07:42:25.385733 pynamicui-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    17583 2023-07-18 07:39:19.000000 pynamicui-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.303646 pynamicui-0.0.3/pynamicui/
+-rw-rw-rw-   0        0        0      386 2023-07-18 07:40:33.000000 pynamicui-0.0.3/pynamicui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.356649 pynamicui-0.0.3/pynamicui/createDom/
+-rw-rw-rw-   0        0        0       32 2023-07-18 06:04:50.000000 pynamicui-0.0.3/pynamicui/createDom/__init__.py
+-rw-rw-rw-   0        0        0     1899 2023-07-18 01:43:07.000000 pynamicui-0.0.3/pynamicui/createDom/createDom.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.374733 pynamicui-0.0.3/pynamicui/createElement/
+-rw-rw-rw-   0        0        0       40 2023-07-18 06:04:41.000000 pynamicui-0.0.3/pynamicui/createElement/__init__.py
+-rw-rw-rw-   0        0        0     3302 2023-07-18 01:43:31.000000 pynamicui-0.0.3/pynamicui/createElement/createElement.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.382736 pynamicui-0.0.3/pynamicui/createStylesheet/
+-rw-rw-rw-   0        0        0       46 2023-07-18 06:04:27.000000 pynamicui-0.0.3/pynamicui/createStylesheet/__init__.py
+-rw-rw-rw-   0        0        0      522 2023-07-18 02:33:30.000000 pynamicui-0.0.3/pynamicui/createStylesheet/createStylesheet.py
+drwxrwxrwx   0        0        0        0 2023-07-18 07:42:25.337647 pynamicui-0.0.3/pynamicui.egg-info/
+-rw-rw-rw-   0        0        0      775 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      456 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-18 07:42:25.000000 pynamicui-0.0.3/pynamicui.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      779 2023-07-18 07:41:55.000000 pynamicui-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1185 2023-07-18 07:42:25.389735 pynamicui-0.0.3/setup.cfg
```

### Comparing `pynamicui-0.0.2/LICENSE` & `pynamicui-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamicui-0.0.2/PKG-INFO` & `pynamicui-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.2
+Version: 0.0.3
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `pynamicui-0.0.2/README.md` & `pynamicui-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,22 +10,22 @@
     - [Creating Components](#creating-components)
       - [Example: Creating a Navigation Bar Component](#example-creating-a-navigation-bar-component)
       - [Example: Creating a Counter Page Component](#example-creating-a-counter-page-component)
     - [The `App` Class](#the-app-class)
       - [Example:](#example-1)
     - [Running the App](#running-the-app)
     - [Conclusion](#conclusion)
-- [PyDynamicUI: An In-Depth Look](#pydynamicui-an-in-depth-look)
+- [PynamicUI: An In-Depth Look](#pynamicui-an-in-depth-look)
   - [Introduction](#introduction)
   - [Inspirations from React](#inspirations-from-react)
   - [Inspirations from CSS and HTML](#inspirations-from-css-and-html)
   - [Use of CustomTkinter](#use-of-customtkinter)
   - [Facilitating Application Development](#facilitating-application-development)
   - [Conclusion](#conclusion-1)
-- [PyDynamicUI: What Sets It Apart](#pydynamicui-what-sets-it-apart)
+- [PynamicUI: What Sets It Apart](#pynamicui-what-sets-it-apart)
   - [1. Dynamic User Interfaces with Virtual DOM](#1-dynamic-user-interfaces-with-virtual-dom)
   - [2. Component-Based Architecture](#2-component-based-architecture)
   - [3. CSS-Inspired Styling](#3-css-inspired-styling)
   - [4. Integration with Tkinter via CustomTkinter](#4-integration-with-tkinter-via-customtkinter)
   - [5. Streamlined Application Development](#5-streamlined-application-development)
   - [6. Active Development and Community Support](#6-active-development-and-community-support)
   - [7. Lightweight and Non-Intrusive](#7-lightweight-and-non-intrusive)
@@ -44,27 +44,27 @@
 
 - **Routing and Navigation:** PynamicUI supports routing and navigation, allowing you to create multi-page applications. You can define routes and associate them with specific UI components, enabling seamless navigation between different pages.
 
 - **Stylesheets and nested styles** PynamicUI supports mapped stylesheets, allowing you to create fast and smooth style transitions. Most importantly it helps keep your different modules readable and in scope.
 
 
 ## Developer Guide
-An extensive developer guide for PyDynamicUI. We'll cover the main classes and their methods, along with examples to demonstrate how to use them effectively.
+An extensive developer guide for PynamicUI. We'll cover the main classes and their methods, along with examples to demonstrate how to use them effectively.
 
 ### Installation
 
-Before you begin, make sure you have installed PyDynamicUI. You can install it using pip:
+Before you begin, make sure you have installed PynamicUI. You can install it using pip:
 
 ```bash
-pip install PyDynamicUI
+pip install PynamicUI
 ```
 
 ### Importing the Library
 
-To use PyDynamicUI, import the necessary elements from the library:
+To use PynamicUI, import the necessary elements from the library:
 
 ```python
 from pynamicui.pynamicui import *
 ```
 
 ### Creating a Stylesheet
 
@@ -93,15 +93,15 @@
 styles.addNestedStyle("PrimaryButton", "NestedPrimaryButton", {
     "fg_color": "darkblue",
 })
 ```
 
 ### Creating Components
 
-Components are the building blocks of your user interface. In PyDynamicUI, you create components using classes that represent different parts of your application.
+Components are the building blocks of your user interface. In PynamicUI, you create components using classes that represent different parts of your application.
 
 #### Example: Creating a Navigation Bar Component
 
 ```python
 class NavBar:
     def __init__(self, dom):
         self.dom = dom
@@ -233,82 +233,82 @@
 To run the app, create an instance of the `App` class:
 
 ```python
 if __name__ == "__main__":
     App()
 ```
 
-Now you have a complete example of creating a dynamic user interface using PyDynamicUI. You can further extend the application by adding more components, styles, and interactions based on your specific use case.
+Now you have a complete example of creating a dynamic user interface using PynamicUI. You can further extend the application by adding more components, styles, and interactions based on your specific use case.
 
 ### Conclusion
 
-Congratulations! You have successfully learned how to create dynamic user interfaces using PyDynamicUI. You can now build complex and interactive applications with ease by leveraging the power of virtual DOM and dynamic component creation. Explore the documentation for more advanced features and customization options. Happy coding!
+Congratulations! You have successfully learned how to create dynamic user interfaces using PynamicUI. You can now build complex and interactive applications with ease by leveraging the power of virtual DOM and dynamic component creation. Explore the documentation for more advanced features and customization options. Happy coding!
 
-# PyDynamicUI: An In-Depth Look
+# PynamicUI: An In-Depth Look
 
 ## Introduction
 
-PyDynamicUI is a Python library that simplifies the process of creating dynamic user interfaces for desktop applications. It takes inspiration from popular web development frameworks like React, the styling capabilities of CSS, and the structure of HTML. The library also utilizes CustomTkinter as a widget library to ensure cross-compatibility and seamless integration with Tkinter, one of the standard GUI frameworks in Python.
+PynamicUI is a Python library that simplifies the process of creating dynamic user interfaces for desktop applications. It takes inspiration from popular web development frameworks like React, the styling capabilities of CSS, and the structure of HTML. The library also utilizes CustomTkinter as a widget library to ensure cross-compatibility and seamless integration with Tkinter, one of the standard GUI frameworks in Python.
 
 ## Inspirations from React
 
-React is a widely-used JavaScript library for building user interfaces, known for its component-based architecture and the concept of a virtual DOM. PyDynamicUI borrows the idea of components and implements a similar virtual DOM approach to efficiently update and render UI elements when their state changes. Components in PyDynamicUI are classes that represent different parts of the user interface, and they can be dynamically created and updated.
+React is a widely-used JavaScript library for building user interfaces, known for its component-based architecture and the concept of a virtual DOM. PynamicUI borrows the idea of components and implements a similar virtual DOM approach to efficiently update and render UI elements when their state changes. Components in PynamicUI are classes that represent different parts of the user interface, and they can be dynamically created and updated.
 
-React's unidirectional data flow principle is also reflected in PyDynamicUI, where changes to the application's state trigger re-rendering of the virtual DOM and subsequently update the user interface. This helps in maintaining a clear separation of concerns and facilitates the building of complex UIs with ease.
+React's unidirectional data flow principle is also reflected in PynamicUI, where changes to the application's state trigger re-rendering of the virtual DOM and subsequently update the user interface. This helps in maintaining a clear separation of concerns and facilitates the building of complex UIs with ease.
 
 ## Inspirations from CSS and HTML
 
-Styling in PyDynamicUI takes inspiration from CSS. Styles are defined using dictionaries containing key-value pairs for attributes such as font, color, padding, etc. The StylesheetConstructor class allows for dynamic creation and management of styles, offering a similar experience to working with CSS.
+Styling in PynamicUI takes inspiration from CSS. Styles are defined using dictionaries containing key-value pairs for attributes such as font, color, padding, etc. The StylesheetConstructor class allows for dynamic creation and management of styles, offering a similar experience to working with CSS.
 
-PyDynamicUI's createElement function is reminiscent of HTML, where you can create elements like Buttons, Labels, Frames, etc., and define their properties and styles in a familiar HTML-like syntax. This makes it intuitive for developers with experience in web development to transition into creating desktop applications with PyDynamicUI.
+PynamicUI's createElement function is reminiscent of HTML, where you can create elements like Buttons, Labels, Frames, etc., and define their properties and styles in a familiar HTML-like syntax. This makes it intuitive for developers with experience in web development to transition into creating desktop applications with PynamicUI.
 
 ## Use of CustomTkinter
 
-CustomTkinter is a widget library developed for PyDynamicUI that sits on top of the standard Tkinter library. It extends the functionality of Tkinter and introduces additional features required to implement the dynamic nature of PyDynamicUI.
+CustomTkinter is a widget library developed for PynamicUI that sits on top of the standard Tkinter library. It extends the functionality of Tkinter and introduces additional features required to implement the dynamic nature of PynamicUI.
 
-By using CustomTkinter, PyDynamicUI ensures cross-compatibility and maintains the robustness of the Tkinter framework. CustomTkinter is well-maintained and designed to seamlessly integrate with PyDynamicUI, providing developers with a stable and consistent experience when building GUI applications.
+By using CustomTkinter, PynamicUI ensures cross-compatibility and maintains the robustness of the Tkinter framework. CustomTkinter is well-maintained and designed to seamlessly integrate with PynamicUI, providing developers with a stable and consistent experience when building GUI applications.
 
 ## Facilitating Application Development
 
-PyDynamicUI is a facilitator that aims to simplify the process of creating Python GUI desktop applications. By taking inspiration from popular web development frameworks and adopting familiar concepts from CSS and HTML, PyDynamicUI reduces the learning curve for developers. Its component-based architecture and virtual DOM approach make it easy to build interactive and responsive user interfaces.
+PynamicUI is a facilitator that aims to simplify the process of creating Python GUI desktop applications. By taking inspiration from popular web development frameworks and adopting familiar concepts from CSS and HTML, PynamicUI reduces the learning curve for developers. Its component-based architecture and virtual DOM approach make it easy to build interactive and responsive user interfaces.
 
-The library does not aim to introduce overly complex or fancy features; instead, it focuses on making the development workflow more accessible and efficient. PyDynamicUI streamlines the UI creation process, allowing developers to focus on the core logic of their applications without worrying about the intricacies of GUI design.
+The library does not aim to introduce overly complex or fancy features; instead, it focuses on making the development workflow more accessible and efficient. PynamicUI streamlines the UI creation process, allowing developers to focus on the core logic of their applications without worrying about the intricacies of GUI design.
 
 ## Conclusion
 
-In conclusion, PyDynamicUI is a powerful yet straightforward library that empowers Python developers to create dynamic user interfaces for desktop applications. Taking inspiration from React, CSS, and HTML, PyDynamicUI offers a familiar development experience while leveraging CustomTkinter for cross-compatibility and reliable integration with Tkinter. By serving as a facilitator, PyDynamicUI aims to make GUI desktop application development in Python easier, faster, and more enjoyable for developers of all levels of experience.
+In conclusion, PynamicUI is a powerful yet straightforward library that empowers Python developers to create dynamic user interfaces for desktop applications. Taking inspiration from React, CSS, and HTML, PynamicUI offers a familiar development experience while leveraging CustomTkinter for cross-compatibility and reliable integration with Tkinter. By serving as a facilitator, PynamicUI aims to make GUI desktop application development in Python easier, faster, and more enjoyable for developers of all levels of experience.
 
-# PyDynamicUI: What Sets It Apart
+# PynamicUI: What Sets It Apart
 
-PyDynamicUI stands out as a unique and viable option for developers looking to build dynamic user interfaces for Python desktop applications. Its distinctive features and benefits make it an excellent choice for various use cases. Let's explore what sets PyDynamicUI apart and why it's a viable option for developers:
+PynamicUI stands out as a unique and viable option for developers looking to build dynamic user interfaces for Python desktop applications. Its distinctive features and benefits make it an excellent choice for various use cases. Let's explore what sets PynamicUI apart and why it's a viable option for developers:
 
 ## 1. Dynamic User Interfaces with Virtual DOM
 
-One of the key differentiators of PyDynamicUI is its adoption of the virtual DOM approach. Inspired by web development frameworks like React, PyDynamicUI efficiently manages updates and re-renders only the necessary components when the application's state changes. This dynamic nature significantly enhances the performance and responsiveness of the user interface, making it ideal for applications with complex and interactive UI requirements.
+One of the key differentiators of PynamicUI is its adoption of the virtual DOM approach. Inspired by web development frameworks like React, PynamicUI efficiently manages updates and re-renders only the necessary components when the application's state changes. This dynamic nature significantly enhances the performance and responsiveness of the user interface, making it ideal for applications with complex and interactive UI requirements.
 
 ## 2. Component-Based Architecture
 
-PyDynamicUI embraces a component-based architecture, mirroring React's paradigm. Components are modular building blocks of the user interface, encapsulating their own logic, styles, and state. This promotes code reusability, maintainability, and separation of concerns, enabling developers to build complex applications in a structured and organized manner.
+PynamicUI embraces a component-based architecture, mirroring React's paradigm. Components are modular building blocks of the user interface, encapsulating their own logic, styles, and state. This promotes code reusability, maintainability, and separation of concerns, enabling developers to build complex applications in a structured and organized manner.
 
 ## 3. CSS-Inspired Styling
 
-Styling in PyDynamicUI draws inspiration from CSS, providing developers with a familiar and intuitive way to define styles for UI elements. Styles are created using dictionaries containing key-value pairs for various attributes, such as font, color, padding, etc. The StylesheetConstructor class allows for the dynamic creation and management of styles, streamlining the process of designing visually appealing and consistent user interfaces.
+Styling in PynamicUI draws inspiration from CSS, providing developers with a familiar and intuitive way to define styles for UI elements. Styles are created using dictionaries containing key-value pairs for various attributes, such as font, color, padding, etc. The StylesheetConstructor class allows for the dynamic creation and management of styles, streamlining the process of designing visually appealing and consistent user interfaces.
 
 ## 4. Integration with Tkinter via CustomTkinter
 
-PyDynamicUI leverages CustomTkinter, a well-maintained widget library that extends the functionality of the standard Tkinter library. By building on top of Tkinter, PyDynamicUI ensures cross-compatibility and stability. Developers can seamlessly use PyDynamicUI's features alongside Tkinter's existing components and functionalities, making it a viable option for those already familiar with Tkinter.
+PynamicUI leverages CustomTkinter, a well-maintained widget library that extends the functionality of the standard Tkinter library. By building on top of Tkinter, PynamicUI ensures cross-compatibility and stability. Developers can seamlessly use PynamicUI's features alongside Tkinter's existing components and functionalities, making it a viable option for those already familiar with Tkinter.
 
 ## 5. Streamlined Application Development
 
-PyDynamicUI is designed to facilitate the creation of Python GUI desktop applications by minimizing the complexity of UI development. By providing developers with familiar concepts from web development and simplifying the creation and management of styles and components, PyDynamicUI streamlines the application development workflow. This allows developers to focus more on application logic and functionality and less on the intricacies of GUI design.
+PynamicUI is designed to facilitate the creation of Python GUI desktop applications by minimizing the complexity of UI development. By providing developers with familiar concepts from web development and simplifying the creation and management of styles and components, PynamicUI streamlines the application development workflow. This allows developers to focus more on application logic and functionality and less on the intricacies of GUI design.
 
 ## 6. Active Development and Community Support
 
-PyDynamicUI benefits from active development and a growing community of contributors and users. This active community ensures that the library is regularly updated, improved, and supported. Developers can rely on PyDynamicUI as a viable long-term option for building Python desktop applications, knowing that it will continue to evolve and adapt to their needs.
+PynamicUI benefits from active development and a growing community of contributors and users. This active community ensures that the library is regularly updated, improved, and supported. Developers can rely on PynamicUI as a viable long-term option for building Python desktop applications, knowing that it will continue to evolve and adapt to their needs.
 
 ## 7. Lightweight and Non-Intrusive
 
-PyDynamicUI is lightweight and non-intrusive, allowing developers to integrate it seamlessly into their existing projects. The library does not impose heavy dependencies or substantial changes to the development environment. Developers can easily adopt PyDynamicUI without disrupting their existing workflow, making it an attractive option for both new and existing projects.
+PynamicUI is lightweight and non-intrusive, allowing developers to integrate it seamlessly into their existing projects. The library does not impose heavy dependencies or substantial changes to the development environment. Developers can easily adopt PynamicUI without disrupting their existing workflow, making it an attractive option for both new and existing projects.
 
 ## Conclusion
 
-PyDynamicUI's dynamic user interfaces, component-based architecture, CSS-inspired styling, integration with Tkinter via CustomTkinter, streamlined development process, and active community support make it a standout and viable option for developers. Its ability to simplify and enhance the creation of Python GUI desktop applications sets it apart and positions it as an excellent choice for projects of all sizes and complexities. Whether you are a seasoned developer or new to GUI application development, PyDynamicUI empowers you to build engaging and interactive user interfaces with ease and efficiency.
+PynamicUI's dynamic user interfaces, component-based architecture, CSS-inspired styling, integration with Tkinter via CustomTkinter, streamlined development process, and active community support make it a standout and viable option for developers. Its ability to simplify and enhance the creation of Python GUI desktop applications sets it apart and positions it as an excellent choice for projects of all sizes and complexities. Whether you are a seasoned developer or new to GUI application development, PynamicUI empowers you to build engaging and interactive user interfaces with ease and efficiency.
```

### Comparing `pynamicui-0.0.2/pynamicui.egg-info/PKG-INFO` & `pynamicui-0.0.3/pynamicui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamicui
-Version: 0.0.2
+Version: 0.0.3
 Summary: dynamic web-like UIs using a declarative syntax
 Home-page: https://github.com/zacharie410/PynamicUI
 Author: zacharie410
 License: Apache Software License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `pynamicui-0.0.2/pyproject.toml` & `pynamicui-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.tbump]
 github_url = "https://github.com/zacharie410/PynamicUI"
 
 [tool.tbump.version]
-current = "0.0.2"
+current = "0.0.3"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `pynamicui-0.0.2/setup.cfg` & `pynamicui-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pynamicui
-version = 0.0.2
+version = 0.0.3
 description = dynamic web-like UIs using a declarative syntax
 long_description = PynamicUI is a lightweight Python library that provides a dynamic user interface (UI) framework for creating interactive and responsive applications. It simplifies the process of building user interfaces by abstracting away the complexities of working directly with a UI toolkit like Tkinter.
 long_description_content_type = text/markdown
 url = https://github.com/zacharie410/PynamicUI
 author = zacharie410
 license = Apache Software License
 license_file = LICENSE
@@ -18,14 +18,17 @@
 documentation = https://github.com/zacharie410/PynamicUI
 repository = https://github.com/zacharie410/PynamicUI
 
 [options]
 python_requires = >=3.7
 packages = 
 	pynamicui
+	pynamicui.createDom
+	pynamicui.createElement
+	pynamicui.createStylesheet
 install_requires = 
 	customtkinter
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

