# Comparing `tmp/cmo_dataviz-0.1.0.tar.gz` & `tmp/cmo_dataviz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmo_dataviz-0.1.0.tar", last modified: Wed Jun 14 07:51:57 2023, max compression
+gzip compressed data, was "cmo_dataviz-0.1.1.tar", last modified: Mon Jul 17 13:30:45 2023, max compression
```

## Comparing `cmo_dataviz-0.1.0.tar` & `cmo_dataviz-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.659214 cmo_dataviz-0.1.0/
--rw-rw-rw-   0        0        0     2985 2023-06-14 07:51:57.657195 cmo_dataviz-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2643 2023-04-25 10:48:58.000000 cmo_dataviz-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.602691 cmo_dataviz-0.1.0/cmo_dataviz/
--rw-rw-rw-   0        0        0       22 2023-04-24 09:23:29.000000 cmo_dataviz-0.1.0/cmo_dataviz/__init__.py
--rw-rw-rw-   0        0        0    25658 2023-06-14 07:22:39.000000 cmo_dataviz-0.1.0/cmo_dataviz/dataviz.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.653051 cmo_dataviz-0.1.0/cmo_dataviz/notebooks/
--rw-rw-rw-   0        0        0    94012 2023-06-12 13:01:16.000000 cmo_dataviz-0.1.0/cmo_dataviz/notebooks/Cmotions Dataviz tutorial.ipynb
--rw-rw-rw-   0        0        0     1354 2023-04-25 10:48:58.000000 cmo_dataviz-0.1.0/cmo_dataviz/resources.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.650694 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/
--rw-rw-rw-   0        0        0     2985 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      139 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-14 07:51:57.000000 cmo_dataviz-0.1.0/cmo_dataviz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 07:51:57.659214 cmo_dataviz-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1293 2023-06-14 07:24:42.000000 cmo_dataviz-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 07:51:57.655061 cmo_dataviz-0.1.0/tests/
--rw-rw-rw-   0        0        0     4075 2023-06-14 06:50:17.000000 cmo_dataviz-0.1.0/tests/test_dataviz.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:30:45.282980 cmo_dataviz-0.1.1/
+-rw-rw-rw-   0        0        0     3674 2023-07-17 13:30:45.282980 cmo_dataviz-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3332 2023-07-17 13:24:52.000000 cmo_dataviz-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 13:30:45.192088 cmo_dataviz-0.1.1/cmo_dataviz/
+-rw-rw-rw-   0        0        0       22 2023-04-24 09:23:29.000000 cmo_dataviz-0.1.1/cmo_dataviz/__init__.py
+-rw-rw-rw-   0        0        0    27677 2023-07-17 13:21:43.000000 cmo_dataviz-0.1.1/cmo_dataviz/dataviz.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:30:45.274895 cmo_dataviz-0.1.1/cmo_dataviz/notebooks/
+-rw-rw-rw-   0        0        0   143818 2023-07-17 13:11:12.000000 cmo_dataviz-0.1.1/cmo_dataviz/notebooks/Cmotions Dataviz tutorial.ipynb
+-rw-rw-rw-   0        0        0     1354 2023-04-25 10:48:58.000000 cmo_dataviz-0.1.1/cmo_dataviz/resources.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:30:45.248074 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/
+-rw-rw-rw-   0        0        0     3674 2023-07-17 13:30:44.000000 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-17 13:30:45.000000 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 13:30:44.000000 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      139 2023-07-17 13:30:44.000000 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-17 13:30:44.000000 cmo_dataviz-0.1.1/cmo_dataviz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 13:30:45.282980 cmo_dataviz-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1293 2023-07-17 13:25:13.000000 cmo_dataviz-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 13:30:45.274895 cmo_dataviz-0.1.1/tests/
+-rw-rw-rw-   0        0        0     4945 2023-07-17 13:13:58.000000 cmo_dataviz-0.1.1/tests/test_dataviz.py
```

### Comparing `cmo_dataviz-0.1.0/cmo_dataviz/dataviz.py` & `cmo_dataviz-0.1.1/cmo_dataviz/dataviz.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import warnings
 import matplotlib.pyplot as plt
 import numpy as np
 import seaborn as sns
 from pandas.api.types import is_numeric_dtype
 import pandas as pd
+import networkx as nx
 
 
 def import_style(filepath: str) -> None:
     """
     This function imports a style file for matplotlib plots.
 
     Args:
@@ -25,27 +26,27 @@
     title="",
     titlefontsize=12,
     figsize=(10, 10),
     ax=None,
 ) -> plt.Axes:
     """
     This function creates a horizontal bar plot using the input data and variables.
-    
+
     Args:
       data: The data to be plotted, in the form of a pandas DataFrame or a dictionary.
       x_var: The variable to be plotted on the x-axis.
       y_var: The variable used for the y-axis of the horizontal barplot.
       x_label: The label for the x-axis of the horizontal barplot.
       title: The title of the horizontal bar plot.
       titlefontsize: The font size of the title of the horizontal bar plot. Defaults to 12
       figsize: The size of the figure in inches (width, height).
       ax: The ax parameter is an optional parameter that allows the user to pass in an existing
     matplotlib Axes object to plot on. If this parameter is not provided, the function will create a new
     figure and Axes object to plot on.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
@@ -57,30 +58,32 @@
         ax.set_yticklabels(data[y_var])
         ax.invert_yaxis()
         ax.set_xlabel(x_label)
         ax.set_title(title, fontsize=titlefontsize)
         return ax
 
 
-def create_scatterplot(data, x_var, y_var, title="", titlefontsize=12, figsize=(10, 10), ax=None) -> plt.Axes:
+def create_scatterplot(
+    data, x_var, y_var, title="", titlefontsize=12, figsize=(10, 10), ax=None
+) -> plt.Axes:
     """
     This function creates a scatterplot with specified data, x and y variables, title, and axis
     parameters.
-    
+
     Args:
       data: The dataset that contains the variables to be plotted.
       x_var: The name of the variable to be plotted on the x-axis of the scatterplot.
       y_var: The variable to be plotted on the y-axis of the scatterplot.
       title: The title of the scatterplot (default is an empty string).
       titlefontsize: The font size of the title of the scatterplot. Defaults to 12
       figsize: The size of the figure in inches (width, height).
       ax: The ax parameter is an optional parameter that allows the user to specify an existing
     matplotlib Axes object to plot the scatterplot on. If ax is not provided, a new figure and Axes
     object will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
@@ -99,26 +102,26 @@
     title="",
     titlefontsize=12,
     figsize=(10, 10),
     ax=None,
 ) -> plt.Axes:
     """
     This function creates a heatmap with customizable options using the Seaborn library in Python.
-    
+
     Args:
       data: The data to be plotted in the heatmap. It should be a 2D array or a pandas DataFrame.
       complete: A boolean parameter that determines whether to show the complete heatmap or only the
     bottom half of it. If set to True, the complete heatmap will be shown. If set to False, only the
     bottom half of the heatmap will be shown. Defaults to True
       title: The title of the heatmap plot.
       titlefontsize: The font size of the title of the heatmap. Defaults to 12
       figsize: The size of the figure (width, height) in inches.
       ax: The matplotlib Axes object to plot the heatmap on. If None, a new figure and Axes object will
     be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if complete:
@@ -259,29 +262,29 @@
     title="",
     titlefontsize=12,
     figsize=(10, 10),
     ax=None,
 ) -> plt.Axes:
     """
     This function creates a swarmplot using seaborn library with customizable parameters.
-    
+
     Args:
       data: The dataset that contains the variables to be plotted.
       x_var: The variable to be plotted on the x-axis of the swarmplot.
       y_var: The variable to be plotted on the y-axis. It is optional and can be left as None if only
     the x-axis variable is to be plotted.
       color_by: The variable used to color the points in the swarmplot. If not specified, all points
     will have the same color.
       title: The title of the plot.
       titlefontsize: The font size of the title of the plot. Defaults to 12
       figsize: The size of the figure in inches (width, height).
       ax: The ax parameter is an optional parameter that allows the user to specify the matplotlib Axes
     object on which the swarmplot will be drawn. If ax is not provided, a new figure and Axes object
     will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
@@ -312,30 +315,30 @@
     titlefontsize=12,
     figsize=(10, 10),
     ax=None,
 ) -> plt.Axes:
     """
     The function creates a histogram plot of a given variable in a dataset, with options for
     color-coding and binning.
-    
+
     Args:
       data: The input data for creating the histogram.
       var: The variable/column name from the input data that will be used to create the histogram.
       color_by: The variable to use for coloring the histogram bars or stacking them. If None or the
     same as the variable being plotted, the bars will not be colored or stacked.
       bins: The number of bins to use for the histogram. Defaults to 10
       max_categories: The maximum number of categories allowed in the histogram. If the number of
     categories exceeds this value, an option to replace the longtail into "OTHER" is created. Defaults
     to 50
       title: The title of the histogram plot.
       titlefontsize: The font size of the title of the histogram. Defaults to 12
       figsize: The size of the figure in inches (width, height).
       ax: The matplotlib Axes object to plot the histogram on. If None, a new figure and Axes object
     will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
@@ -394,23 +397,23 @@
 
 
 def create_confusion_matrix_heatmap(
     conf_matrix, model_accuracy=None, figsize=(10, 10), ax=None
 ) -> plt.Axes:
     """
     This function creates a heatmap of a confusion matrix with optional model accuracy score.
-    
+
     Args:
       conf_matrix: The confusion matrix to be visualized as a heatmap.
       model_accuracy: The accuracy score of the model, expressed as a percentage. It is an optional
     parameter that can be used to add a title to the heatmap.
       figsize: The size of the figure in inches (width, height).
       ax: An optional parameter that specifies the matplotlib Axes object to plot the heatmap on. If not
     provided, a new figure and Axes object will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     if ax is None:
         fig = plt.figure(figsize=figsize)
         ax = fig.add_subplot(111)
     sns.heatmap(
@@ -431,23 +434,23 @@
         plt.title(all_sample_title, size=15)
     return ax
 
 
 def create_tableplot(data, colLabels=None, figsize=(10, 10), ax=None) -> plt.Axes:
     """
     The function creates a table plot using the given data and column labels.
-    
+
     Args:
       data: a pandas DataFrame containing the data to be plotted in the table
       colLabels: A list of column labels for the tableplot. If not provided, the column labels will be
     the column names of the input data.
       figsize: The size of the figure in inches (width, height).
       ax: An optional parameter that specifies the matplotlib Axes object to plot the table on. If it is
     not provided, a new figure and Axes object will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     if ax is None:
         fig = plt.figure(figsize=figsize)
         ax = fig.add_subplot(111)
     if colLabels is None:
@@ -457,20 +460,20 @@
     ax.axis("off")
     return ax
 
 
 def create_single_tableplot(data, colLabels=None):
     """
     The function creates a table plot with given data and column labels.
-    
+
     Args:
       data: a pandas DataFrame containing the data to be plotted in a table format
       colLabels: A list of column labels for the table. If not provided, the column labels will be the
     column names of the input data.
-    
+
     Returns:
       a matplotlib figure object.
     """
     if colLabels is None:
         colLabels = data.columns
     if len(data) + 1 > len(colLabels):
         nrows, ncols = len(data) + 1, len(colLabels)
@@ -484,20 +487,20 @@
     tableplot.scale(2, 2)
     return fig
 
 
 def create_pairplot(data, figtitle=""):
     """
     This function creates a pairplot using seaborn library with customized settings and a given title.
-    
+
     Args:
       data: The data to be plotted in the pairplot.
       figtitle: The title of the figure. It is an optional parameter and if not provided, the figure
     will not have a title.
-    
+
     Returns:
       a matplotlib figure object.
     """
     with plt.rc_context(
         {
             "axes.labelcolor": "black",
             "ytick.labelleft": True,
@@ -524,28 +527,28 @@
     x_label="",
     title="",
     figsize=(10, 10),
     ax=None,
 ) -> plt.Axes:
     """
     The function creates a bar plot with optional value labels and customizable labels and title.
-    
+
     Args:
       data: The data to be plotted in the barplot.
       x_var: The variable to be plotted on the x-axis of the barplot.
       y_var: The variable used for the height of the bars in the barplot.
       add_value_labels: A boolean parameter that determines whether or not to add labels to the top of
     each bar in the barplot indicating the height of the bar. Defaults to True
       x_label: The label for the x-axis of the barplot.
       title: The title of the barplot.
       figsize: The size of the figure (width, height) in inches.
       ax: The ax parameter is an optional parameter that allows the user to pass in an existing
     matplotlib Axes object to plot on. If this parameter is not provided, a new figure and Axes object
     will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
     ):
         if ax is None:
@@ -573,26 +576,26 @@
 
 def create_stacked_barplot(
     data, x_var, y_var, color_by, x_label="", title="", figsize=(10, 10), ax=None
 ) -> plt.Axes:
     """
     This function creates a stacked barplot with multiple categories and colors based on a given
     dataset.
-    
+
     Args:
       data: The input data for the plot.
       x_var: The variable to be plotted on the x-axis.
       y_var: The variable to be plotted on the y-axis of the stacked barplot.
       color_by: The variable used to determine the color of the bars in the stacked barplot.
       x_label: The label for the x-axis of the plot.
       title: The title of the stacked barplot.
       figsize: The size of the figure (width, height) in inches.
       ax: The ax parameter is an optional parameter that allows the user to specify the matplotlib Axes
     object on which to draw the plot. If it is not specified, a new Axes object will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     categories = data[color_by].unique()
     init_data = pd.DataFrame(data[x_var].unique(), columns=[x_var]).sort_values(
         by=x_var
     )
@@ -639,28 +642,28 @@
 
 def create_lineplot(
     data, x_var, y_var, color_by=None, x_label="", title="", figsize=(10, 10), ax=None
 ) -> plt.Axes:
     """
     This function creates a line plot with optional color grouping based on a specified data set and
     variables.
-    
+
     Args:
       data: The data to be plotted in the line plot.
       x_var: The variable to be plotted on the x-axis of the line plot.
       y_var: The variable to be plotted on the y-axis of the line plot.
       color_by: The variable used to color the lines in the line plot. If this parameter is not
     specified, all lines will have the same color.
       x_label: The label for the x-axis of the line plot.
       title: The title of the line plot.
       figsize: The size of the figure in inches (width, height).
       ax: The ax parameter is an optional parameter that allows the user to pass in an existing
     matplotlib Axes object to plot the lineplot on. If ax is not provided, a new figure and Axes object
     will be created.
-    
+
     Returns:
       a matplotlib Axes object.
     """
     categories = data[color_by].unique()
 
     with plt.rc_context(
         {"axes.labelcolor": "black", "ytick.labelleft": True, "xtick.labelbottom": True}
@@ -675,7 +678,83 @@
         _ = ax.set_xlabel(x_label)
         _ = ax.set_xticks(
             ax.get_xticks(), ax.get_xticklabels(), rotation=45, ha="right"
         )
         _ = ax.set_title(title)
         _ = ax.legend(loc="upper right", ncol=len(categories))
         return ax
+
+
+def create_network_graph(
+    data,
+    node_1,
+    node_2,
+    edge_weight,
+    edge_label,
+    title="",
+    figsize=(10, 10),
+    ax=None,
+    seed=None,
+) -> plt.Axes:
+    if ax is None:
+        fig = plt.figure(figsize=figsize)
+        ax = fig.add_subplot(111)
+
+    # add an adjustment to the position to prevent overlapping edges
+    data["position_adjustment"] = data.groupby([node_1, node_2]).cumcount() * 0.15
+
+    # determine the network and position of nodes
+    ng = nx.from_pandas_edgelist(
+        data,
+        node_1,
+        node_2,
+        edge_attr=[edge_weight, edge_label, "position_adjustment"],
+        create_using=nx.MultiDiGraph(),
+    )
+    pos = nx.spring_layout(ng, scale=2, k=1, iterations=10, seed=seed)
+
+    # draw the nodes including their name
+    _ = nx.draw_networkx_labels(ng, pos, font_size=10)
+    _ = nx.draw_networkx_nodes(
+        ng, pos, node_color="lightblue", node_size=500, alpha=0.8
+    )
+
+    # add the edges between the nodes, including the label
+    for u, v, attr in ng.edges(data=True):
+        pos_adjust = attr["position_adjustment"]
+
+        # calculate the midpoint of the edge
+        x1, y1 = pos[u]
+        x2, y2 = pos[v]
+        cx = (x1 + x2) / 2
+        cy = (y1 + y2) / 2
+
+        # set the label position
+        text_pos = (cx + pos_adjust, cy + pos_adjust)
+
+        # draw the edge with connectionstyle
+        arrowprops = dict(
+            arrowstyle="->",
+            color="0.5",
+            shrinkA=5,
+            shrinkB=5,
+            patchA=None,
+            patchB=None,
+            connectionstyle=f"arc3,rad={pos_adjust}",
+        )
+        _ = ax.annotate(
+            "",
+            xy=pos[u],
+            xycoords="data",
+            xytext=pos[v],
+            textcoords="data",
+            arrowprops=arrowprops,
+        )
+
+        # draw the edge label
+        text_label = attr[edge_label]
+        _ = ax.text(text_pos[0], text_pos[1], text_label)
+
+    _ = ax.set_title(title)
+    _ = ax.set_axis_off()
+
+    return ax
```

### Comparing `cmo_dataviz-0.1.0/cmo_dataviz/resources.py` & `cmo_dataviz-0.1.1/cmo_dataviz/resources.py`

 * *Files identical despite different names*

### Comparing `cmo_dataviz-0.1.0/setup.py` & `cmo_dataviz-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # read the contents of the README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="cmo_dataviz",
-    version="0.1.0",
+    version="0.1.1",
     python_requires='>=3.6',
     description='Easily create graphs using custom styling',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Jeanine Schoonemann',
     author_email='service@cmotions.nl',
     url='https://Cmotions@dev.azure.com/Cmotions/Packages/_git/cmo_dataviz',
```

