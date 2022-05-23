.. _attr_Letterbox_jp:

レターボックス
######################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++


概要
*****

* 上下左右にレターボックスを表示させることができます
* 枠を表示する基準は、ResolutionGateになります
* レターボックスの幅は、ResolutionGateの幅/高さの比率で指定します

  * 例えば、Topの値に ``10`` を入力すると、ResolutionGateの高さの10%の厚みで表示されます

.. figure:: ../../_gif/_tmp_gif.gif
   :alt: letterbox


++++

アトリビュート
**********************

.. figure:: ../../_images/letterboxAttr.png
   :alt: letterbox

Color
=====

* レターボックスのカラー

Opacity
=======

* レターボックスの不透明度

Top (%)
=======

* 上部に表示させる、レターボックスの高さ指定
* ResolutionGateの高さに対する割合で指定します

Left (%)
========

* 左側に表示させる、レターボックスの幅指定
* ResolutionGateの幅に対する割合で指定します

Right (%)
=========

* 右側に表示させる、レターボックスの幅指定
* ResolutionGateの幅に対する割合で指定します

Bottom (%)
==========

* 下部に表示させる、レターボックスの高さ指定
* ResolutionGateの高さに対する割合で指定します
