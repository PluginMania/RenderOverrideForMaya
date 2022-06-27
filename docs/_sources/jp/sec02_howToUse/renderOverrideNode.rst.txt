.. _RenderOverrideNode_jp:

Render Override Node
####################

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

概要
*****

RenderOverrideを起動すると基本的な情報(テキスト)が表示されますが、より詳細に制御したい場合は ``RenderOverrideノード`` を作成し、各種アトリビュートを設定します

.. figure:: ../../_images/outlinerFindNode.png
   :alt: outlinerFindNode

++++

RenderOverride ノードの作成
***************************

* **方法1**

  1. Shelfから、 **NodeEditor** アイコンをクリックし、エディタを立ち上げます

     .. figure:: ../../_images/shelf_editor_icon.png
        :alt: shelf_editor_icon

  2. ``Create RenderOverride Node`` ボタンをクリックすると、ノードが作成されます

     .. figure:: ../../_images/NodeEditor_create.png
        :alt: NodeEditorCreate

* **方法2**

  * 次のMELコマンドを実行します

    .. code-block:: c++

       createNode "renderOverride";

++++

ノードの確認方法
****************

* RenderOverrideノード(DGノード)が作成されたことを確認します

  * **Outliner で確認する**

    .. figure:: ../../_images/outlinerFindNode.png
       :alt: outlinerFindNode

    * Outlinerでは、メニューの ``Display > DAG Objects Only`` のチェックを外してください

      .. figure:: ../../_images/outlinerMenu.png
         :alt: outlinerMenu

  * **NodeEditor で確認する**

    .. figure:: ../../_images/NodeEditorList.png
       :alt: NodeEditorAll

       NodeEditorのノードのリストに、作成されたノードが表示されます。


.. important::

   * RenderOverrideノードは、Maya®シーンの中で複数作ることができますが、ビューに適用されるノード("アクティブなノード")は1つだけです。
   * ビューに適用されるノードは次のように決まります

     1. RenderOverrideノードを、名前順に ``Enable`` アトリビュートにチェックが入っているかどうかを確認します
     2. 最初に ``Enable`` アトリビュートにチェックが入っていたノードの情報が適用されます

        * ``Enable`` にチェックが入っているノードが1つも無ければ、デフォルトのテキストが表示されます。

   .. sep

   * NodeEditorを使用すれば、選択したノード以外の ``Enable`` アトリビュートは **off** になるので、アクティブなノードを1つに限定することができます
   * 「 **レイアウト用** 」, 「 **Playblast用** 」のように、複数のノードを目的に応じて使い分けることができます。

   .. `(文字のGrammerがバグったので、調整用コメント)

++++

プリセット
**********

  .. figure:: ../../_images/renderOverrideNode_AEPresets.png
     :alt: AEPresets

  * ノード作成後、アトリビュートエディタの **Presets** ボタンから、定義されたHUDの文字列などを流し込むことができます

++++

RenderOverrideノードのアトリビュート
************************************

Enable
======

  .. figure:: ../../_images/attrEnable.png
     :alt: outlinerFindNode

  * チェックが **on** の場合、各種設定がビューに反映されます

    * チェックが **off** の場合は無効になります
    * 複数のRenderOverrideノードがシーンに存在する場合は、 ``Enable`` が **on** のノードの中で、名前順で一番先頭のノードの情報が反映されます

++++

その他アトリビュート
====================

その他のアトリビュートの設定方法は、専用のページで紹介します(以下のリンク)


・ :ref:`attr_Text_jp`
----------------------

・ :ref:`attr_Letterbox_jp`
---------------------------

・ :ref:`attr_Grid_jp`
----------------------

・ :ref:`attr_Foreground_jp`
----------------------------

・ :ref:`attr_Background_jp`
----------------------------

・ :ref:`attr_Action_jp`
------------------------

