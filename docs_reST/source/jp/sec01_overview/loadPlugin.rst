プラグインのロード
##################

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

* Mayaを起動する前に、プラグインのインストールを完了させてください

  * (:ref:`how-to-plugin-install_jp`)

* インストールができたら、Mayaを起動します


プラグインのロード方法
**********************

1. Mayaのメニューから ``Windows > Settings/Preferences > Plug-in Manager`` と辿ります
2. Plug-in Managerのダイアログの ``RenderOverrideNode.py`` と ``RenderOverride.py`` の **load** もしくは **Auto load** にチェックを入れます

.. figure:: ../../_images/_tmp_img.png
   :scale: 100%
   :alt: PluginManager
   :align: left


Shelf
*****

* RenderOverrideが正常にロードされると、"RenderOverride"のShelfが自動的に読み込まれます
* 下図のようなShelfが読み込まれていることを確認してください
* RenderOverrideノードの作成や、アクティブなノードの切り替えなどで使います

  .. figure:: ../../_images/shelf_all.png
     :scale: 100%
     :alt: Shelf

  .. seealso::
     Shelfの各機能の説明はこちら >  :ref:`shelf_jp`