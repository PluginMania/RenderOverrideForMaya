.. _sample_Action_jp:

Actions (外部Pythonファイルの利用)
##################################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

概要
*****

* Pythonスクリプトを使うことで、状況に合わせたテキストを生成し、表示させることができます
* この作例では、RenderOverrideノードの ``Actions`` アトリビュートと組み合わせ、アクションの情報を出力する方法を紹介します

  .. figure:: ../../_gif/renderoverride_actionsSampleResult.gif
     :scale: 70%
     :alt: ActionsResult

     テキストの表示を、右上のように切り替えることができます

++++

サンプル プロジェクト
*********************

* このプロジェクトの完成シーンです (Maya2022で保存されています)

  * :download:`MayaScene(2022) <../../_download/cube_animation_sample_actions_maya2022_v001.zip>`

++++

手順
*****

1. Actionsアトリビュートの設定
==============================

* ``Actions`` アトリビュートに情報を加えてください

  .. figure:: ../../_images/sample_actions_attrs.png
     :alt: ActionsAttr

     アクション名/ 開始フレーム/ 終了フレームを入力します

2. Pythonスクリプトの準備
=========================

* 今回は、プラグインで用意されている ``renderoverride_actions.py`` を使用します

  * Pythonファイルは ``C:/ProgramData/Autodesk/ApplicationPlugins/RenderOverride/Contents/plug-ins/[OS-MAYA VERSION]/python/`` にインストールされています
  * RenderOverrideをロードした段階で ``PYTHONPATH`` が通っているので、すぐに使うことができます

    * (自分で作ったPythonコードを実行させたい時は、 ``PYTHONPATH`` などを使用し、パスを通しておくことを推奨します)


3. Textアトリビュートの設定
===========================

1. Textの ``Enable`` にチェックを入れます
2. Textの ``Generate Type`` を **Python** に設定します
3. ``Text String`` アトリビュートに、次のコードを入力します

   .. code-block:: python

      import renderoverride_actions;renderoverride_actions.actions_text()

   .. figure:: ../../_images/sample_actions_textAttrs.png
      :alt: TextAttr

   * テキストボックス上で右クリックし、 ``Python: Actions`` を選択すると、コードが入力されます

     .. figure:: ../../_images/sample_actions_textRightClicked.png
        :alt: TextRightClicked

4. 表示の確認
=============

* タイムラインを再生させ、次の動画の、右上のテキストのように表示が切り替われば成功です

  .. figure:: ../../_gif/renderoverride_actionsSampleResult.gif
     :scale: 70%
     :alt: ActionsResult

++++

.. seealso::
   :ref:`notes_python_jp`
