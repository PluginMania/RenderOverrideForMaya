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

* RenderOverrideノードの作成や、アクティブなノードの切り替えなどでこのShelfを使います

++++

各ツールの説明
**************

1. Node Editor
==============

  .. figure:: ../../_images/shelf_editor_icon.png
     :alt: ShelfNodeEditorIcon

  * アイコンをクリックすると、次のようなウィンドウが開きます

    .. figure:: ../../_images/NodeEditorAll_JP.png
       :alt: NodeEditorAll

    * **ノードのリスト**

      * Mayaシーンに存在するRenderOverrideノードのリストが表示されます
      * 各項目のチェックボックスは、 ``Enable`` アトリビュートの **on** / **off** を表しています
      * リストをクリックすると、そのノードが選択され、アクティブになります

        * (選択したノードの ``Enable`` アトリビュートが **on** になり、その他のノードは **off** になります)

    * **Create RenderOverride Node**

      * RenderOverrideノードを作成します
      * 作成されたノードがアクティブになります

    * **Refresh UI**

      * UIを最新の状態に更新します

    * **Close**

      * ウィンドウを閉じます

2. Refresh
==========

  .. figure:: ../../_images/shelf_refresh_icon.png
     :alt: ShelfRefreshIcon

  * アイコンをクリックすると、ビューがリフレッシュされます
  * RenderOverrideノードのアトリビュートを変更しても表示が更新されない場合は、このボタンをクリックし、画面をリフレッシュしてください

