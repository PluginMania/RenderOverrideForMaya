.. _knownIssues_en:

Known Issues
############

.. contents:: Contents of this page:
   :depth: 2
   :local:

++++

Changing the color of the "Color" attribute is not immediately reflected in the view.
*************************************************************************************

* This is a specification of the attribute editor and is caused by the screen not being refreshed immediately.
* Click the ``Refresh`` button on the Shelf or change any attribute except the color to refresh the screen.

  .. figure:: ../../_images/shelf_refresh_icon.png
     :alt: shelf_editor_icon


++++

Foreground and background images are not displayed even if they are set in the file node.
*****************************************************************************************


* This error is occurring in **Maya2023**.
* Click the ``Refresh`` button on the Shelf to refresh the screen

  .. figure:: ../../_images/shelf_refresh_icon.png
     :alt: shelf_editor_icon


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
   If you have any bugs or troubles that are not mentioned here, please report them from `Issues`_.
   We accept reports of bugs and troubles only from this page.



.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues

