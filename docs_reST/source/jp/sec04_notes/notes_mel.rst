.. _notes_mel_jp:

MELスクリプトの注意事項
##########################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

Text Stringの記述
*****************

* MELスクリプトを直接実行させる時は、次のように書きます(選択しているオブジェクト名を取得するスクリプト)

  .. code-block:: c

     ls -sl

* 外部のMELファイル(.mel)を実行させたい時は、先にプロシージャ(``global proc``)をMaya®に認識させておくとよいでしょう


スクリプトの返り値
******************

* 返り値の型は、 ``string[]`` もしくは ``string`` のみ受け付けます

.. sep

* ``string[]`` は、1行ずつ要素に分けて文字列を格納してください

  .. code-block:: c++

     global proc string[] getText()
     {
        string $textLines[] = {
           "Line 1",
           "Line 2",
           "Line 3"
        };
        return $textLines;
     }


* 文字列を改行させたい場合は、改行コード ``\n`` を挿入してください

  .. code-block:: c

     global proc string getText()
     {
         string $textLines = "Line 1\nLine 2\nLine 3";
         return $textLines;
     }

  .. warning::
     * 返り値の型を保証するのは、開発者の責任です。
     * 返す文字が何もないときは、空文字( ``""`` )を返してください。

