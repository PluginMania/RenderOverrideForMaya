.. _shelf_en:

Shelf
#####

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++

Overview
********

* When the RenderOverride plug-in is successfully loaded, the "RenderOverride" Shelf is automatically loaded
* Please make sure that the following Shelf is loaded

  .. figure:: ../../_images/shelf_all.png
     :alt: Shelf

++++

Description of each tool
************************

1. Node Editor
==============

.. figure:: ../../_images/shelf_editor_icon.png
    :alt: ShelfNodeEditorIcon

* Use this tool for creating RenderOverride nodes, switching active nodes, etc.

  * Clicking on the icon opens a window that looks like this

    .. figure:: ../../_images/NodeEditorAll.png
       :alt: NodeEditorAll

    1. **Node List**

       * A list of RenderOverride nodes present in the Maya® scene is displayed.
       * The checkbox for each item represents the **on** / **off** of the ``Enable`` attribute.
       * Clicking on a node in the list selects it and makes it active.

         * (The ``Enable`` attribute of the selected node will be **on** and the other nodes will be **off**)

    2. **Create RenderOverride Node**

       * Creates a RenderOverride node
       * The created node becomes active

    3. **Delete Selected Node**

       * Delete the node selected in the UI

    4. **Refresh the scene and UI**

       * Refresh Maya® scene and UI

    5. **Close**

       * Close window

2. Refresh
==========

.. figure:: ../../_images/shelf_refresh_icon.png
    :alt: ShelfRefreshIcon

* Refresh the view

  * If the view does not refresh after changing the attribute of the RenderOverride node, click this button to refresh the view

3. Help
=======

.. figure:: ../../_images/shelf_help_icon.png
    :alt: ShelfRefreshIcon

* Opens an online table of contents in an HTML browser.
