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
     :scale: 100%
     :alt: Shelf

* Use this Shelf for creating RenderOverride nodes, switching active nodes, etc.


Description of each tool
************************

1. Node Editor
==============

  .. figure:: ../../_images/shelf_editor_icon.png
     :scale: 100%
     :alt: ShelfNodeEditorIcon

  * Clicking on the icon opens a window that looks like this

    .. figure:: ../../_images/NodeEditorAll_EN.png
       :scale: 100%
       :alt: NodeEditorAll

    * **Node List**

      * A list of RenderOverride nodes present in the Maya scene is displayed.
      * The checkbox for each item represents the **on** / **off** of the ``Enable`` attribute.
      * Clicking on a node in the list selects it and makes it active.

        * (The ``Enable`` attribute of the selected node will be **on** and the other nodes will be **off**)

    * **Create RenderOverride Node**

      * Creates a RenderOverride node
      * The created node becomes active

    * **Refresh UI**

      * Update the UI to the latest state

    * **Close**

      * Close window

2. Refresh
==========

  .. figure:: ../../_images/shelf_refresh_icon.png
     :scale: 100%
     :alt: ShelfRefreshIcon

  * Click the icon to refresh the view
  * If the view does not refresh after changing the attribute of the RenderOverride node, click this button to refresh the view

