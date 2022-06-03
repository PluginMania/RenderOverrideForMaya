Load plug-ins
##################

.. contents:: Contents of this page:
   :depth: 2
   :local:

++++

* Complete the plugin installation before launching Maya.

  * (:ref:`how-to-plugin-install_en`)

* Once installed, launch Maya.


How to load plug-ins
**********************

1. From the Maya menu, navigate to ``Windows > Settings/Preferences > Plug-in Manager``
2. In the Plug-in Manager dialog, check the **Loaded** or **Auto load** checkboxes for ``RenderOverride.py`` and ``RenderOverrideNode.py``.

   .. figure:: ../../_images/pluginManager.png
      :alt: PluginManager

++++

License Authentication
**********************

* Activation is performed when the plugin is loaded
* The authorization procedure is as follows

  1. Check LICENSE file

     * If a LICENSE file exists, check if the license is valid
     * If it is valid, you can use it as a commercial version
     * If the LICENSE file is valid, the authorization process to the Autodesk App Store in (2.) will be skipped

  2. Go to the Autodesk App Store to check for a commercial license

     * Access Autodesk's server over the network to check if your license is valid
     * Make sure you are connected to the network.
     * Enter your Autodesk user ID (email address) and click the OK button.

       .. figure:: ../../_images/licenseAuthUserIdDialog.png
          :alt: AutodeskUserID

     * If certified, you can use it for commercial purposes.
     * If not certified, it will be for trial use (watermark will be displayed)

* The diagram is as follows

  .. figure:: ../../_images/licenseAuthFlowEN.PNG
     :alt: licenseAuthFlowEN

* When the plugin is loaded, the ScriptEditor outputs the authentication history

  .. figure:: ../../_images/licenseAuthScriptEditor.png
     :alt: licenseAuthFlowJP

  .. note::
     If you have any trouble with activation, please report it to us through `Issues`_.
     If you attach a snapshot of ScriptEditor, it will be easier for us to respond.

++++

Shelf
*****

* When RenderOverride is successfully loaded, the "RenderOverride" shelf is automatically loaded.

  * (may be loaded automatically when Maya is launched after the plug-in is installed)

* Please make sure that the Shelf is loaded as shown below.
* Use this Shelf to create RenderOverride nodes, switch active nodes, etc.

  .. figure:: ../../_images/shelf_all.png
     :scale: 100%
     :alt: Shelf

  .. seealso::
     Click here for a description of each Shelf feature > :ref:`shelf_en`.


.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues
