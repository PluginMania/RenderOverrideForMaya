.. _sample_Action_en:

Actions (using external Python files)
#####################################

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++

Overview
********

* Python scripts can be used to generate and display text tailored to the situation
* This example shows how to output action information in combination with the ``Actions`` Attribute of the RenderOverride node

  .. figure:: ../../_gif/renderoverride_actionsSampleResult.gif
     :scale: 70%
     :alt: ActionsResult

     The text display can be switched as shown in the upper right corner.

++++

Project file
************

* This is the finished scene of this project (saved in Maya2022)

  * :download:`MayaScene(2022) <../../_download/cube_animation_sample_actions_maya2022_v001.zip>`

++++

Process
*******

1. Actions Attribute Settings
=============================

* Add information to the ``Actions`` attribute

  .. figure:: ../../_images/sample_actions_attrs.png
     :alt: ActionsAttr

     Enter ActionName/ StartFrame/ EndFrame

2. Preparing Python Scripts
===========================

* This time, we will use the ``renderoverride_actions.py`` provided by the plugin

  * The Python files are installed in ``C:/ProgramData/Autodesk/ApplicationPlugins/RenderOverride/Contents/plug-ins/[OS-MAYA VERSION]/python/``.
  * The ``PYTHONPATH`` is passed when RenderOverride is loaded, so you can use it right away.

    * (If you want to run your own Python code, it is recommended that you use ``PYTHONPATH`` or similar to pass it through.)

3. Setting Text Attributes
==========================

1. Check ``Enable`` of Text.
2. Set ``Generate Type`` of Text to **Python**.
3. Enter the following code in the ``Text String`` Attribute

   .. code-block:: python

      import renderoverride_actions;renderoverride_actions.actions_text()

   .. figure:: ../../_images/sample_actions_textAttrs.png
      :alt: TextAttr

   * Right click on the text box to select a template (choose ``Python: Actions``)

     .. figure:: ../../_images/sample_actions_textRightClicked.png
        :alt: TextRightClicked

4. Check display
================

* Play the timeline, and if the display changes to look like the text in the upper right corner of the next video, you have succeeded.

  .. figure:: ../../_gif/renderoverride_actionsSampleResult.gif
     :scale: 70%
     :alt: ActionsResult

++++

.. seealso::
   :ref:`notes_python_en`
