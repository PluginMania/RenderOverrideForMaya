新バージョンのモニター
######################

.. contents:: このページの目次:
   :depth: 2
   :local:

++++

モニターについて
****************

* 本ソフトウェアの新バージョンのリリースを前に、モニターを募集しています
* 実際にツールを使用していただき、使用感のフィードバックやバグの報告をお願いしております
* モニターの方には、開発者より新バージョンのプログラムファイルとライセンスをお送りします

  * ライセンスが有効な間、商用利用することができます
  * 既にサブスクリプション契約をされている方は、モニター期間中は契約を一時中断して頂いて構いません

    * 中断の設定を行わないと、使用料が引き続き引き落とされるのでご注意ください
    * モニター期間終了後に引き続き商用利用される場合は、再度サブスクリプションのご契約をお願いします

  * 有効期間については、ライセンス受取り時に開発者に確認するか、ライセンスファイルの中身から確認することができます

    .. figure:: ../../_images/sp_licenseDate.png
       :alt: LicenseDate

       ライセンスファイルは、 ``C:/ProgramData/Autodesk/ApplicationPlugins/RenderOverride/Contents`` 内にあります

++++

条件など
********

+--------+------------------------------------+
| 対象者 | 開発者が認めた者(自薦、他薦問わず) |
+--------+------------------------------------+
| 報酬   | 開発者から、モニターへの謝礼はなし |
+--------+------------------------------------+
| 報告   | 使用感のフィードバック、バグの報告 |
+--------+------------------------------------+
| 期間   | 1-3ヵ月程度 (延長あり)             |
+--------+------------------------------------+

* 謝礼はありませんが、最新のバージョンをいち早く、無料で使えるというメリットがあります

++++

新しいバージョンのインストール/ 削除方法
****************************************

インストール
============

* 既にRenderOverrideを使用しており、 **Plug-in Manager** の ``Auto Load`` にチェックが入っている場合は、チェックを外してください

  * 既にインストールされている実行ファイルと、新しいバージョン(テスト用プログラム)の実行ファイルの衝突を防ぐために、予めチェックを外しておきます
  * 既にインストールされている、正規版のアプリはアンインストールする必要はありません

    .. figure:: ../../_images/sp_loadOff.png
       :alt: PluginManager

* 新しいバージョンのプログラムファイルは、zip圧縮したものを個別に共有します

  * 配布されたzipファイルを解凍してください

  .. figure:: ../../_images/sp_zipExtract.png
     :alt: zipFile

* 解凍されたフォルダの中に、 ``RenderOverrideNewFeature_[VERSION]`` という名前のフォルダが入っています。(AutodeskAppStoreからインストールしたフォルダと被らないような名前になっています)

  .. figure:: ../../_images/sp_rootFolder.png
     :alt: RootFolder

* ``RenderOverrideNewFeature_[VERSION]`` フォルダを、 ``C:/ProgramData/Autodesk/ApplicationPlugins/`` にコピーしてください

  .. figure:: ../../_images/sp_copyRootFolder.png
     :alt: CopyRootFolder

* コピー後にMayaを起動し、 **Plug-in Manager** を確認すると、 ``RenderOverrideNewFeature_[VERSION]`` の項目がありますので、ロードしてください

  * 正常にロードされると、通常の製品版と同じように使用することができます

  .. figure:: ../../_images/sp_loadOn.png
     :alt: PluginManager


削除方法
========

1. Mayaを落とします
2. ``RenderOverrideNewFeature_[VERSION]`` フォルダをDeleteしてください

   * (``C:/ProgramData/Autodesk/ApplicationPlugins/`` 内)

   .. note::
      モニター期間終了後は、削除するようにしてください。

++++

フィードバック
**************

* フィードバックは、下記の [GoogleForm] に報告をお願いします

  * 報告は何回でも可
  * 1つの事象につき、1回ずつ分けて回答してください

.. raw:: html

   <iframe src="https://docs.google.com/forms/d/e/1FAIpQLScRNiGF8OeBPQQ3PdV2iaIjc74r59tac3zuEOoFzk5ei5_uhA/viewform?embedded=true" width="640" height="1521" frameborder="0" marginheight="0" marginwidth="0">読み込んでいます…</iframe>

