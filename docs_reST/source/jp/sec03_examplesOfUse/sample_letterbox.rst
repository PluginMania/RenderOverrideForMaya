.. _sample_letterbox_jp:

Letterboxの設定方法
###################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

概要
*****

* レターボックスを使う際の、解像度の計算や各種設定方法を紹介します
* レターボックスを画面の上下に、 ``10%`` の高さで表示させる場合の設定方法になります
* Playblastで出力するまでの手順を紹介します

++++

手順
*****

1. まず、ResolutionGateの"解像度"を確認します

   * 基本的に、最終レンダリングする時の解像度になります
   * 今回は ``1920 x 1080`` とします

2. レターボックスを画面の上下に10%ずつ加えるため、先ほどの解像度の高さを ``1.2倍`` します

   * 計算結果は ``1296`` (px)になります

3. RenderSettingsのImageSizeに、先ほどの解像度(``1920 x 1296``)を設定します

   * (レターボックスの表示位置はResolutionGateが基準になっているため、解像度の設定が必要になります)

   .. figure:: ../../_images/sample_letterbox_renderSettings.png
      :alt: RenderSettings

4. RenderOverrideノードのレターボックスの **Top** と **Bottom** アトリビュートの値を、それぞれ ``108`` に設定します

   * レターボックスの幅は、RenderSettingsの解像度の値を基準に計算されます
   * ``1296`` の値を基に、上下に ``108`` 分ずつレターボックスを表示させます

     * (※ResolutionGateの高さの比率に基づいて表示されます)

   .. figure:: ../../_images/sample_letterbox_changeAttr.png
      :alt: LetterboxAttr

   .. figure:: ../../_images/sample_letterbox_viewPx.png
      :alt: LetterboxView
      :scale: 70%

5. RenderOverrideノードの ``Text String`` アトリビュートに表示させたいテキストを入力し、レターボックス上に文字が表示されるか確認します

   * 文字の大きさをレターボックスの高さに合わせたい場合は、 ``Fit text size to letterbox`` アトリビュートを **on** にします
   * 必要に応じて ``Text Scale`` や ``Offset`` アトリビュートを調整してください

   .. figure:: ../../_images/sample_letterbox_textAttr.png
      :alt: TextAttr

   .. figure:: ../../_images/sample_letterbox_displayText.png
      :alt: DisplayText

6. カメラの ``Overscan`` アトリビュートを ``1`` に設定します

   * この設定をすることで、Playblast時にResolutionGateの枠でビューが切り抜かれます(AfterEffectsなどの編集ソフトで切り抜き作業を行わずに済みます)

   .. figure:: ../../_images/sample_letterbox_camOverscanAttr.png
      :alt: CameraOverscanAttr

7. Playblastのオプションを開き、"**Display size**"アトリビュートを ``From Render Settings`` に設定します

   .. figure:: ../../_images/sample_letterbox_playblastOpt.png
      :alt: PlayblastOption

      (他のオプションは自由に設定してください)

8. オプションダイアログの ``Playblast`` もしくは ``Apply`` ボタンをクリックし、Playblastを実行します

   * 出力された動画を確認してください
