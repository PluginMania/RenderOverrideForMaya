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


.. _shelf_letterboxSettings_en:

2. Letterbox Settings
=====================

*[New in version* :ref:`v1.1.0<release_1_1_0_en>` *]*

.. figure:: ../../_images/shelf_letterbox_icon.png
    :alt: ShelfLetterboxIcon

* A tool to set up Letterbox as described in "How to set up Letterbox".

  * Clicking on the icon opens a window that looks like this.

    .. figure:: ../../_images/shelf_letter_all.png
       :alt: LetterboxSettingsAll

    1. **Preset**

       * Switches render size and letterbox values to preset values.

    2. **Render (WxH)**

       * Render Resolution.
       * Sets the final rendering resolution or a multiple of it.

    3. **Letterbox Height (%)**

       * Specifies the thickness of the letterbox to be displayed at the top and bottom, as a percentage.

    4. **Letterbox Width (%)**

       * Specifies the thickness of the letterboxes to be displayed on the left and right sides, in percentage.

    5. **RenderOverride Node**

       * Specifies the RenderOverride node to which the Letterbox values will be applied.
       * By default, the currently active node is specified.
       * Selecting the ``[Create New Node]`` item creates a new RenderOverride node and applies the letterbox settings to the new node.

         .. figure:: ../../_images/shelf_letter_renderoverride_comb.png
            :alt: LetterboxSettings_RenderOverrrideCombobox

    6. **Set the camera's Overscan attribute to 1.0**

       * Check if you want to set the ``Overscan`` attribute of the camera to ``1.0``.

    7. **Camera**

       * Select the camera to which you want to apply ``Set the camera's Overscan attribute to 1.0``.

    8. **Apply**

       * Applies the values specified in the various settings.

    9. **Refresh**

       * Refresh the Maya® scene and bring the UI up to date.

    10. **Close**

        * Close window.

3. Refresh
==========

.. figure:: ../../_images/shelf_refresh_icon.png
    :alt: ShelfRefreshIcon

* Refresh the view

  * If the view does not refresh after changing the attribute of the RenderOverride node, click this button to refresh the view

4. Help
=======

.. figure:: ../../_images/shelf_help_icon.png
    :alt: ShelfRefreshIcon

* Opens an online table of contents in an HTML browser.
