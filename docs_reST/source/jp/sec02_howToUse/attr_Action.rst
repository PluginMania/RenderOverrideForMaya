.. _attr_Action_jp:

Action List
###########


.. contents:: このページの目次:
   :depth: 3
   :local:

++++


概要
*****

* このアトリビュートは、直接ビューに影響を与えることはありません
* PythonやMELのスクリプトと組み合わせ、表示をカスタマイズすることができます

  * ゲームのアニメーション作成時に使われることが多いアトリビュートです
  * 具体的な使い方は、[:ref:`sample_Action_jp`]を参照してください


++++


アトリビュート
**************

.. figure:: ../../_images/actionAttr1.png
   :alt: actionAttr1


Add New Item ボタン
===================

* Actionのアイテムを追加します

++++


アトリビュート(Actions[*]枠内)
******************************

.. figure:: ../../_images/actionAttr2.png
   :alt: actionAttr2


Action Name
===========

* アクション名を入力します

  * ``Walk`` ``Jump`` など

Start Frame
===========

* アクションのスタートフレームを入力します

  .. note::
     * ``End Frame`` アトリビュートが必要であれば、 `Issues`_ に報告をお願いします
     * (著者は、スクリプトで制御できると考えています ( :ref:`sample_Action_jp` ))

       .. code-block:: python

          # basic
          cur_actions_end_frame = next_actions_start_frame - 1

          # has margin frame? (各アクションの間にマージンが入りますか?)
          cur_actions_end_frame = next_actions_start_frame - margin_time - 1



"ゴミ箱"アイコン
================

* Actionを削除します


.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues

