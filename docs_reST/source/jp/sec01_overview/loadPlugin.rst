プラグインのロード
##################

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

* Maya®を起動する前に、プラグインのインストールを完了させてください

  * (:ref:`how-to-plugin-download_jp`, :ref:`how-to-plugin-install_jp`)

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

  .. warning::
     * Trial版のページからダウンロードされたソフトウェアは、有償版のライセンスを支払っていても、ライセンス認証されずに試用版として起動されます。
     * 有償版のライセンスを支払った場合は、Trial版をアンインストールし、有償版のソフトウェアをダウンロード・インストールしてください。

* ScriptEditorに認証の履歴が出力されます

  .. figure:: ../../_images/licenseAuthScriptEditor.png
     :alt: licenseAuthFlowJP

     (有償版のライセンスが有効な場合、図のような履歴が表示されます)

* ライセンス認証時に、次のようなダイアログが表示された場合は、新しいバージョンにアップデートをお願いします。

  * 新しい機能の追加と安定性の増したバージョンをお使いいただけるよう、このようなダイアログが表示されます。
  * また、セキュリティ上の問題回避のために、定期的にアップデートをお願いしております。

  .. figure:: ../../_images/licenseAuth_newRelease1.png
     :alt: licenseAuth_newRelease

     (この表示が出た場合、1か月以内にアップデートをお願いします)

  .. figure:: ../../_images/licenseAuth_newRelease2.png
     :alt: licenseAuth_newRelease

     (この表示が出た場合は、すぐにアップデートをお願いします。商用利用できなくなり、ウォーターマークが表示されます)

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
