.. _notes_python_jp:

Pythonスクリプトの注意事項
##########################

.. contents:: このページの目次:
   :depth: 3
   :local:

++++

Text Stringの記述
*****************

* Pythonスクリプトを直接実行させる時は、次のように書きます(ログインユーザー名を取得するスクリプト)

  .. code-block:: python

     import getpass;getpass.getuser()

  * セミコロン(``;``)を使うことで、複数行のスクリプトを1行で記述することができます


* 外部のPythonコードを実行させたい時は、先に ``PYTHONPATH`` などを使用して、パスを通しておくとよいでしょう

  * モジュールの読み込みと関数を実行させるコードを1行で記述します

  .. code-block:: python

     import actions;actions.actions_text()

  .. seealso::
     :ref:`sample_Action_jp`


スクリプトの返り値
******************

* 返り値の型は、 ``list[str]`` もしくは ``str`` のみ受け付けます

.. sep

* ``list[str]`` は、1行ずつ要素に分けて文字列を格納してください

  .. code-block:: python

     def get_text() -> list[str]:
         text_lines = [
            'Line 1',
            'Line 2',
            'Line 3'
         ]
         return text_line


* 文字列を改行させたい場合は、改行コード ``\n`` を挿入してください

  .. code-block:: python

     def get_text() -> str:
         text_lines = 'Line 1\nLine 2\nLine 3'
         return text_line


* ``list[str]`` や ``str`` の形で値を返してくる ``maya.cmds`` コマンドであれば、直接実行させることもできます

  .. code-block:: python

     import maya.cmds;maya.cmds.ls(sl=True)

  .. warning::
     * 返り値の型を保証するのは、開発者の責任です。Noneや他の型が返されないように注意してください。
     * 返す文字が何もないときは、空文字( ``''`` )を返してください。

