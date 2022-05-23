Overview
########

.. contents:: Contents of this page:
   :depth: 2
   :local:

++++

Functions
*********

* RenderOverride overrides the viewport display. It has the following functions

  * Text (HUD) display
  * Letterbox display
  * Grid display
  * Display of images (Foreground/ Background)

.. sep

* **RenderOverride node** can be used to customize the text to be displayed, etc.
* There is no change in the Viewport 2.0 display (object visibility)


.. figure:: ../../_gif/_tmp_gif.gif
   :scale: 100%
   :alt: overview
   :align: left


Supported Versions / OS
****************************

+------+-------------------+-----------+---------+---------------------------------+
| Maya | OS                | Operation | Support | Source code                     |
+======+===================+===========+=========+=================================+
| 2022 | Windows10 (64bit) | ✅        | Active  | Python3.7 + MayaAPI2.0 + Cython |
+------+-------------------+-----------+---------+---------------------------------+
| 2023 | Windows10 (64bit) | ✅        | Active  | Python3.9 + MayaAPI2.0 + Cython |
+------+-------------------+-----------+---------+---------------------------------+


* RenderOverride is designed for use with Maya 2022 and later
* Code is written in Python3, API 2.0, and Cython and has been optimized

  * Nearly 2x performance improvement over Maya2020 (Python2)
  * Due to Python version and performance reasons, versions prior to Maya2022 are not supported.

* Windows 10 is the only OS currently supported.

  * Windows 11 has not been tested, but may work (Currently not supported).

* The supported Maya versions are basically three generations, from the latest version to the previous two generations.

  * Maya versions that have been supported in the past can continue to be used, but there is a possibility that bugs may not be addressed if they are discovered.

.. note::
   * MacOS will not be supported in the future.
   * Linux (CentOS, Rocky Linux) support will be considered when we get some builders to help us.

     * If you have any requests for Linux version, or if you want to help us to build it, please report them in `Issues`_.


.. _Issues: https://github.com/PluginMania/RenderOverrideMaya/issues
