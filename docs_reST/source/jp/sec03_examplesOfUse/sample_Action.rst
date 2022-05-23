.. _sample_Action_jp:

作例: Actions (外部Pythonファイルの利用)
########################################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

概要
*****

* Pythonスクリプトを使うことで、状況に合わせたテキストを生成し、表示させることができます

  * Mayaシーンの情報の取得はもちろん、Webからの情報の取得や、データベースから情報を取り出すこともできます
* この作例では、RenderOverrideノードの ``Actions`` アトリビュートと組み合わせ、アクションの情報を出力する方法を紹介します

++++

手順
*****

1. Actionsアトリビュートの設定
==============================

* ``Actions`` アトリビュートに情報を加えてください


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

   * (テキストボックス上で右クリックすると、テンプレートを選択することができます( ``Python: Actions`` を選択してください))

   .. code-block:: python

      import renderoverride_actions;renderoverride_actions.actions_text()

4. 表示の確認
=============

* タイムラインを再生させ、添付動画のように表示が切り替われば成功です

++++

Pythonスクリプトの注意事項
**************************

:ref:`こちら<notes_python_jp>` を参照してください


