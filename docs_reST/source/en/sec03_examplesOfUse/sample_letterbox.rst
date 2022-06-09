.. _sample_letterbox_en:

How to set up Letterbox
#######################

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++

Overview
********

* This section describes how to calculate the resolution and other settings when using letterboxes.
* Letterboxes at the top and bottom of the screen at ResolutionGate's ``10%`` ratio.
* Here are the steps to output with Playblast.

.. sep

* Please create a RenderOverride node.

++++

Process
*******

1. First, check the "Resolution" in ResolutionGate

   * Basically, it is the resolution or its magnification at the time of final rendering.
   * In this case, we will use ``1920 x 1080``.

2. To add letterboxes to the top and bottom of the screen by 10%, we multiply the previous resolution height by ``1.2``.

   * The result is ``1296`` (px).

3. Set the ImageSize in RenderSettings to the resolution you just set (``1920 x 1296``)

   * (The resolution setting is necessary because the position of the letterbox is based on ResolutionGate)

   .. figure:: ../../_images/sample_letterbox_renderSettings.png
      :alt: RenderSettings

4. Set the **Top** and **Bottom** attributes of the RenderOverride node's letterbox to ``108`` respectively

   * The width of the letterbox is calculated based on the resolution value in the RenderSettings.
   * Based on the value of ``1296``, the letterboxes will be displayed in ``108`` increments above and below

     * (* based on ResolutionGate height ratios)

   .. figure:: ../../_images/sample_letterbox_changeAttr.png
      :alt: LetterboxAttr

   .. figure:: ../../_images/sample_letterbox_viewPx.png
      :alt: LetterboxView

5. Enter the text you want to display in the ``Text String`` attribute of the RenderOverride node and see if the text appears on the letterbox.

   * Set the ``Fit text size to letterbox`` attribute to **on** if you want the text size to match the letterbox height.
   * Adjust the ``Text Scale`` and ``Offset`` attributes as needed.

   .. figure:: ../../_images/sample_letterbox_textAttr.png
      :alt: TextAttr

   .. figure:: ../../_images/sample_letterbox_displayText.png
      :alt: DisplayText

6. Set the ``Overscan`` attribute of the camera to ``1``.

   * This setting will crop the view with the ResolutionGate border during the playblast (without having to crop it with AfterEffects or other editing software).

   .. figure:: ../../_images/sample_letterbox_camOverscanAttr.png
      :alt: CameraOverscanAttr

7. Open Playblast options and set the "**Display size**" attribute to ``From Render Settings``.

   .. figure:: ../../_images/sample_letterbox_playblastOpt.png
      :alt: PlayblastOption

      (Other options are at your disposal)

8. Click the ``Playblast`` or ``Apply`` button in the options dialog to run Playblast

   * Check the output video
