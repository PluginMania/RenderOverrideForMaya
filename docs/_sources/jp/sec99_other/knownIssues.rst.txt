.. _knownIssues_jp:

既知の問題
###########

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

Colorアトリビュートの色を変更しても、ビューに直ぐに反映されない
***************************************************************

* これはアトリビュートエディタの仕様で、画面が直ぐにリフレッシュされないのが原因です
* Shelfの ``Refresh`` ボタンをクリックするか、カラー以外のアトリビュートを変更し、画面をリフレッシュさせてください

  .. figure:: ../../_images/shelf_refresh_icon.png
     :alt: shelf_editor_icon


++++

foregroundやbackgroundの画像をfileノードで設定しても表示されない
****************************************************************

* この症状は、 **Maya2023** で確認されています
* Shelfの ``Refresh`` ボタンをクリックし、画面をリフレッシュさせてください

  .. figure:: ../../_images/shelf_refresh_icon.png
     :alt: shelf_editor_icon


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
   ここに書かれていない、バグ・トラブルがありましたら、「 :ref:`bugReport_jp` 」からご報告をお願いします。

