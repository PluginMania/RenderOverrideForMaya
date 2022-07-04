Load plug-ins
##################

.. contents:: Contents of this page:
   :depth: 2
   :local:

++++

* Complete the plugin installation before launching Maya®.

  * (:ref:`how-to-plugin-install_en`)

* Once installed, launch Maya®.


How to load plug-ins
**********************

1. Launch **Plug-in Manager** (``Windows > Settings/Preferences > Plug-in Manager``)
2. In the Plug-in Manager dialog, check the **Loaded** or **Auto load** checkboxes for ``RenderOverride.py`` and ``RenderOverrideNode.py``.

   .. figure:: ../../_images/pluginManager.png
      :alt: PluginManager

++++

License Authentication
**********************

* Activation is performed when the plugin is loaded


  .. warning::
     * Software downloaded from the Trial version page will be activated as a trial version without being activated, even if you have paid for the paid version license.
     * If you have paid for the paid version license, please uninstall the Trial version and download and install the paid version software.

* ScriptEditor outputs the authentication history

  .. figure:: ../../_images/licenseAuthScriptEditor.png
     :alt: licenseAuthFlowJP

     (If the license of the paid version is valid, the history will be displayed as shown in the figure)

* If the following dialog box appears during activation, please update to a newer version.

  * This dialog will appear so that you can use a version with new features and increased stability.
  * We also ask you to update your software periodically to avoid security issues.

  .. figure:: ../../_images/licenseAuth_newRelease1.png
     :alt: licenseAuth_newRelease

     (If you get this indication, please update within a month.)

  .. figure:: ../../_images/licenseAuth_newRelease2.png
     :alt: licenseAuth_newRelease

     (If you see this message, please update your software immediately. Commercial use is no longer available and a watermark will be displayed)

.. note::
   * If you encounter any trouble with activation, please report it to us at " :ref:`bugReport_en`".
   * If you attach a snapshot of ScriptEditor, it will be easier for us to respond.


++++

Shelf
*****

* When RenderOverride is successfully loaded, the "RenderOverride" shelf is automatically loaded.

  * (may be loaded automatically when Maya® is launched after the plug-in is installed)

* Please make sure that the Shelf is loaded as shown below.
* Use this Shelf to create RenderOverride nodes, switch active nodes, etc.

  .. figure:: ../../_images/shelf_all.png
     :scale: 100%
     :alt: Shelf

  .. seealso::
     Click here for a description of each Shelf feature > :ref:`shelf_en`.


.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues
