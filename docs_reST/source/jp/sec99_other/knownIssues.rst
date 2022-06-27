.. _knownIssues_jp:

既知の問題
###########

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

.. _knownIssues_colorAttr_jp:

Colorアトリビュートの色を変更しても、ビューに直ぐに反映されない
***************************************************************

* これはアトリビュートエディタの仕様で、画面が直ぐにリフレッシュされないのが原因です

.. sep

* 解決方法

  * カラー以外のアトリビュートを変更する
  * Shelfの ``Refresh`` ボタンをクリックする

    .. figure:: ../../_images/shelf_refresh_icon.png
       :alt: shelf_editor_icon

  * NodeEditorの「 **Refresh the scene and UI** 」ボタンをクリックする

    .. figure:: ../../_images/NodeEditor_refresh.png
       :alt: NodeEditor_refesh

++++

.. _knownIssues_fgBgImg_jp:

foregroundやbackgroundの画像をfileノードで設定しても表示されない
****************************************************************

* この症状は、 **Maya®2023** で確認されています
* 画像の読み込みが遅く、表示されるまでに時間がかかる場合があります

.. sep

* 解決方法

  * カラー以外のアトリビュートを変更する
  * Shelfの ``Refresh`` ボタンをクリックする

    .. figure:: ../../_images/shelf_refresh_icon.png
       :alt: shelf_editor_icon

  * NodeEditorの「 **Refresh the scene and UI** 」ボタンをクリックする

    .. figure:: ../../_images/NodeEditor_refresh.png
       :alt: NodeEditor_refesh

++++

Gridを複数設定すると、表示されないものがある
********************************************

* 次の2つのGridは、先頭で指定しないと描画されません

  * ``Golden Spiral(A)``
  * ``Golden Spiral(B)`` (Mirror)

    .. figure:: ../../_images/gridTroubleA.png
       :alt: gridTroubleA

       (``Golden Spiral(A)`` が2番目に設定されているので、ビューに表示されません)


* 原因は、他のGridと描画処理が違う為です
* Gridの描画の順番を変えて対応をお願いします

    .. figure:: ../../_images/gridTroubleB.png
       :alt: gridTroubleB

       (``Golden Spiral(A)`` を先頭で指定すると、ビューに表示されます)

++++

.. note::
   * ここに書かれていない、バグ・トラブルがありましたら、「:ref:`bugReport_jp`」からご報告をお願いします。
   * 報告いただいたバグやトラブルなどの対応状況は `Issues`_ にて確認することができます。

.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues
