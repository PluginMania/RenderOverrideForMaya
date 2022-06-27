.. _knownIssues_en:

Known Issues
############

.. contents:: Contents of this page:
   :depth: 2
   :local:

++++

.. _knownIssues_colorAttr_en:

Changing the color of the "Color" attribute is not immediately reflected in the view.
*************************************************************************************

* This is a specification of the attribute editor and is caused by the screen not being refreshed immediately.

.. sep

* Solution

  * Change attributes other than color
  * Click the ``Refresh`` button on the shelf.

    .. figure:: ../../_images/shelf_refresh_icon.png
       :alt: shelf_editor_icon

  * Click the "**Refresh the scene and UI**" button in the NodeEditor.

    .. figure:: ../../_images/NodeEditor_refresh.png
       :alt: NodeEditor_refesh

++++

.. _knownIssues_fgBgImg_en:

Foreground and background images are not displayed even if they are set in the file node.
*****************************************************************************************


* This error is occurring in **Maya®2023**.
* Images may load slowly and take some time to display.

.. sep

* Solution

  * Change attributes other than color
  * Click the ``Refresh`` button on the shelf.

    .. figure:: ../../_images/shelf_refresh_icon.png
       :alt: shelf_editor_icon

  * Click the "**Refresh the scene and UI**" button in the NodeEditor.

    .. figure:: ../../_images/NodeEditor_refresh.png
       :alt: NodeEditor_refesh

++++

When multiple Grids are set, some of them are not displayed.
************************************************************

* The following two grids will not be drawn unless specified at the beginning.

  * ``Golden Spiral(A)``
  * ``Golden Spiral(B)`` (Mirror)

    .. figure:: ../../_images/gridTroubleA.png
       :alt: gridTroubleA

       (``Golden Spiral(A)`` is set to second, so it will not appear in the view)


* The reason is that the drawing process is different from other Grids.
* Please change the order in which Grids are drawn.

    .. figure:: ../../_images/gridTroubleB.png
       :alt: gridTroubleB

       (If ``Golden Spiral(A)`` is specified at the beginning, it will be displayed in the view.)

++++

.. note::
   * If you have any bugs or troubles that are not mentioned here, please report them from ":ref:`bugReport_en`".
   * You can check the status of reported bugs and troubles at "`Issues`_".

.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues
