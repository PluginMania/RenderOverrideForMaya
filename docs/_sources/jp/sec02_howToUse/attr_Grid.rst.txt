.. _attr_Grid_jp:

グリッド
######################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++


概要
*****

* ResolutionGate内(レターボックスが表示されている時は、レターボックスの枠内)に、グリッドを表示させます
* ファイ・グリッド(Phi Grid)など、よく使われているグリッドのプリセットが用意されています
* 複数のグリッドを組み合わせて表示することもできます

  .. figure:: ../../_gif/renderoverride_gridTop.gif
     :scale: 70%
     :alt: gridOverview

++++


アトリビュート
**********************

.. figure:: ../../_images/gridAttr1.png
   :alt: gridAttr1

Enable
======

* Grid全体のon/offを制御します


[Add New Item] ボタン
=====================

* グリッドのアイテムを追加します

++++


アトリビュート(Grids[*]枠内)
****************************

.. figure:: ../../_images/gridAttr2.png
   :alt: gridAttr2

Enable
======

* 各Gridのon/off
* 個別に無効にすることができます

Grid Type
=========

* 下図のグリッドが用意されています
* ``Mirror`` アトリビュートで反転させる事ができます

  .. figure:: ../../_images/grid_list_v002.svg
     :alt: gridList
     :scale: 100%

     (図の青い破線は補助線です(ラインの頂点の場所を示したもので、描画されません)。画像をクリックすると大きな画面でご覧いただけます)

Mirror
======

* グリッドを反転させます
* (殆どのグリッドが左右反転ですが、一部のグリッドでは上下に反転します)

Color
=====

* グリッドのカラー
* (テクスチャを接続しても、単色で表示されます)

Opacity
=======

* グリッドの不透明度
* (テクスチャを接続しても、均一に不透明度が適用されます)

Line Width
==========

* グリッドの太さ
* (テクスチャを接続しても、均一に太さが適用されます)

"ゴミ箱"アイコン
================

* グリッドを削除します
* 一時的に非表示にしたい場合は、 ``Enable`` アトリビュートを使用してください


++++


注意事項 (既知の問題)
*********************

Gridを複数設定すると、表示されないものがある
================================================

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

