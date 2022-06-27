プラグインのロード
##################

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

* Maya®を起動する前に、プラグインのインストールを完了させてください

  * (:ref:`how-to-plugin-install_jp`)

* インストールができたら、Maya®を起動します


プラグインのロード方法
**********************

1. **Plug-in Manager** を立ち上げます (``Windows > Settings/Preferences > Plug-in Manager``)
2. Plug-in Managerのダイアログの ``RenderOverride.py`` と ``RenderOverrideNode.py`` の **Loaded** もしくは **Auto load** にチェックを入れます

   .. figure:: ../../_images/pluginManager.png
      :alt: PluginManager


++++

ライセンス認証
**************

* プラグインのロード時に、ライセンス認証が行われます
* 認証の手順は次の通りです

  1. LICENSEファイルのチェック

     * LICENSEファイルが存在する場合は、ライセンスが有効かどうかを確認します
     * 有効な場合は、商用版として使うことができます
     * LICENSEファイルが有効であれば、(2.)のAutodesk App Storeへの認証プロセスはスキップされます

  2. Autodesk App Storeへ、商用ライセンスの有無を確認する

     * ネットワーク経由でAutodesk社のサーバーへアクセスし、ライセンスが有効かどうかを確認します
     * 必ずネットワークに繋がっていることを確認してください
     * 下図のようなダイアログが表示されますので、AutodeskユーザーID(メールアドレス)を入力し、OKボタンを押してください

       .. figure:: ../../_images/licenseAuthUserIdDialog.png
          :alt: AutodeskUserID

     * 認証されると商用利用が可能になります
     * 認証されなかった場合は、試用利用になります(ウォーターマークが表示されます)

* 図で表すと次の通りです

  .. figure:: ../../_images/licenseAuthFlowJP.PNG
     :alt: licenseAuthFlowJP

* プラグインがロードされる際、ScriptEditorに認証の履歴が出力されます

  .. figure:: ../../_images/licenseAuthScriptEditor.png
     :alt: licenseAuthFlowJP

  .. note::
     * ライセンスのトラブルが発生した時は「 :ref:`bugReport_jp` 」からご報告をお願いします。
     * その際、ScriptEditorのスナップショットを添付していただけると、対応しやすくなります。

++++

Shelf
*****

* RenderOverrideが正常にロードされると、"RenderOverride" Shelfが自動的に読み込まれます

  * (プラグインのインストール後、Maya®起動時に自動的に読み込まれている可能性があります)

* 下図のようなShelfが読み込まれていることを確認してください
* RenderOverrideノードの作成や、アクティブなノードの切り替えを行うときに使います

  .. figure:: ../../_images/shelf_all.png
     :alt: Shelf

  .. seealso::
     Shelfの各機能の説明はこちら >  :ref:`shelf_jp`



.. _Issues: https://github.com/PluginMania/RenderOverrideForMaya/issues
