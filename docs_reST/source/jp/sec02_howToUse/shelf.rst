.. _shelf_jp:

Shelf
#####

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

概要
*****

* RenderOverrideのプラグインが正常にロードされると、"RenderOverride"のShelfが自動的に読み込まれます
* 次のようなShelfが読み込まれていることを確認してください

  .. figure:: ../../_images/shelf_all.png
     :alt: Shelf

++++

各ツールの説明
**************

1. Node Editor
==============

.. figure:: ../../_images/shelf_editor_icon.png
    :alt: ShelfNodeEditorIcon

* RenderOverrideノードの作成や、アクティブなノードの切り替えなどでこのツールを使います


  * アイコンをクリックすると、次のようなウィンドウが開きます

    .. figure:: ../../_images/NodeEditorAll.png
       :alt: NodeEditorAll

    1. **ノードのリスト**

       * Maya®シーンに存在するRenderOverrideノードのリストが表示されます
       * 各項目のチェックボックスは、 ``Enable`` アトリビュートの **on** / **off** を表しています
       * リストをクリックすると、そのノードが選択され、アクティブになります

         * (選択したノードの ``Enable`` アトリビュートが **on** になり、その他のノードは **off** になります)

    2. **Create RenderOverride Node**

       * RenderOverrideノードを作成します
       * 作成されたノードがアクティブになります

    3. **Delete Selected Node**

       * UIで選択されているノードを削除します

    4. **Refresh the scene and UI**

       * Maya®のシーンをリフレッシュし、UIを最新の状態に更新します

    5. **Close**

       * ウィンドウを閉じます


.. _shelf_letterboxSettings_jp:

2. Letterbox Settings
=====================

*[* :ref:`v1.1.0<release_1_1_0_jp>` *で追加]*

.. figure:: ../../_images/shelf_letterbox_icon.png
    :alt: ShelfLetterboxIcon

* 「:ref:`sample_letterbox_jp`」で紹介されているような、Letterboxの設定を行うためのツールです

  * アイコンをクリックすると、次のようなウィンドウが開きます

    .. figure:: ../../_images/shelf_letter_all.png
       :alt: LetterboxSettingsAll

    1. **Preset**

       * レンダリングサイズとレターボックスの値を、プリセット値に切り替えます

    2. **Render (WxH)**

       * レンダリング解像度
       * 最終的にレンダリングする時の解像度、もしくはその倍数を設定します

    3. **Letterbox Height (%)**

       * 上下に表示させるレターボックスの厚みを、パーセンテージで指定します

    4. **Letterbox Width (%)**

       * 左右に表示させるレターボックスの厚みを、パーセンテージで指定します

    5. **RenderOverride Node**

       * Letterboxの値を適用させる、RenderOverrideノードを指定します
       * デフォルトでは、現在アクティブになっているノードが指定されます
       * ``[Create New Node]`` の項目を選択すると、新しくRenderOverrideノードが作成され、新しいノードに対してレターボックスの設定が適用されます

         .. figure:: ../../_images/shelf_letter_renderoverride_comb.png
            :alt: LetterboxSettings_RenderOverrrideCombobox

    6. **Set the camera's Overscan attribute to 1.0**

       * カメラの ``Overscan`` アトリビュートを ``1.0`` に設定する場合は、チェックを入れてください

    7. **Camera**

       * ``Set the camera's Overscan attribute to 1.0`` を適用させるカメラを選択します

    8. **Apply**

       * 各種設定で指定した値を適用します

    9. **Refresh**

       * Maya®のシーンをリフレッシュし、UIを最新の状態に更新します

    10. **Close**

        * ウィンドウを閉じます


3. Refresh
==========

.. figure:: ../../_images/shelf_refresh_icon.png
    :alt: ShelfRefreshIcon

* ビューをリフレッシュします

  * RenderOverrideノードのアトリビュートを変更しても表示が更新されない場合は、このボタンをクリックし、画面をリフレッシュしてください

4. Help
=======

.. figure:: ../../_images/shelf_help_icon.png
    :alt: ShelfRefreshIcon

* Webブラウザで、オンラインドキュメントを開きます
