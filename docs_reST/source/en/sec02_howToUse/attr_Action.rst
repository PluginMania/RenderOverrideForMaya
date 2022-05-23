.. _attr_Action_en:

Action List
###########


.. contents:: Contents of this page:
   :depth: 3
   :local:

++++


Overview
********

* This attribute does not directly affect the view
* Can be combined with Python or MEL scripts to customize the view

  * This Attribute is often used when creating animations for games.
  * See [:ref:`sample_Action_en`] for specific usage


++++


Attribute
*********

.. figure:: ../../_images/actionAttr1.png
   :alt: actionAttr1


[Add New Item] button
=====================

* Add an Action item

++++


Attribute (Actions[*] in frame)
*******************************

.. figure:: ../../_images/actionAttr2.png
   :alt: actionAttr2


Action Name
===========

* Enter an action name

  * ``Walk`` ``Jump`` etc.

Start Frame
===========

* Enter the start frame of the action

  .. note::
     * If you need ``End Frame`` attributes, please report them in `Issues`_.
     * (The author thinks it can be controlled by a script ( :ref:`sample_Action_en` ))

       .. code-block:: python

          # basic
          cur_actions_end_frame = next_actions_start_frame - 1

          # has margin frame?
          cur_actions_end_frame = next_actions_start_frame - margin_time - 1



"Trash" icon
============

* Delete Action


.. _Issues: https://github.com/PluginMania/RenderOverrideMaya/issues

