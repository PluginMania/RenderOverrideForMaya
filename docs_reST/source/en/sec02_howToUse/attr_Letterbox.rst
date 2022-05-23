.. _attr_Letterbox_en:

Letterbox
#########

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++


Overview
********

* Letterboxes can be displayed on the top, bottom, left, and right
* The standard for displaying the borders is ResolutionGate.
* The width/height of the letterbox is specified by the ratio of the width/height of the ResolutionGate.

  * For example, if you enter ``10`` for Top, the letterbox will be displayed with a thickness of 10% of the ResolutionGate height.

.. figure:: ../../_gif/_tmp_gif.gif
   :alt: letterbox

++++

Attribute
**********************

.. figure:: ../../_images/letterboxAttr.png
   :alt: letterbox

Color
=====

* Letterbox Color

Opacity
=======

* Letterbox opacity

Top (%)
=======

* Specify the height of the letterbox to be displayed at the top
* Specified as a percentage of the ResolutionGate height.

Left (%)
========

* Specify the width of the letterbox to be displayed on the left side
* Specified as a percentage of the width of the ResolutionGate.

Right (%)
=========

* Specify the width of the letterbox to be displayed on the right side
* Specified as a percentage of the width of the ResolutionGate.

Bottom (%)
==========

* Specify the height of the letterbox to be displayed at the bottom.
* Specified as a percentage of the ResolutionGate height.
