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

  * You can retrieve information from the Maya scene, retrieve information from the web, or retrieve information from a database.

* This example shows how to output action information in combination with the ``Actions`` Attribute of the RenderOverride node

++++

Process
*******

1. Actions Attribute Settings
=============================

* Add information to the ``Actions`` attribute


2. Preparing Python Scripts
===========================

* This time, we will use the ``renderoverride_actions.py`` provided by the plugin

  * The Python files are installed in ``C:/ProgramData/Autodesk/ApplicationPlugins/RenderOverride/Contents/plug-ins/[OS-MAYA VERSION]/python/``.
  * The ``PYTHONPATH`` is passed when RenderOverride is loaded, so you can use it right away!

    * (If you want to run your own Python code, it is recommended that you use ``PYTHONPATH`` or similar to pass it through.)


3. Setting Text Attributes
==========================

1. Check ``Enable`` of Text.
2. Set ``Generate Type`` of Text to **Python**.
3. Enter the following code in the ``Text String`` Attribute

   * (Right click on the text box to select a template (choose ``Python: Actions``)).

   .. code-block:: python

      import renderoverride_actions;renderoverride_actions.actions_text()

4. Check display
================

* Play the timeline, and if the display changes as shown in the attached video, you have succeeded!

++++

Python Scripting Notes
**************************

See :ref:`here<notes_python_en>`
