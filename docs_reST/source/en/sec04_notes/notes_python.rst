.. _notes_python_en:

Python Scripting Notes
##########################

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++

How to write "Text String"
**************************

* To run the Python script directly, write the following (script to get the login user name)

  .. code-block:: python

     import getpass;getpass.getuser()

  * A semicolon (``;``) allows you to write a multi-line script on a single line


* If you want to run external Python code, you can use ``PYTHONPATH`` or similar to pass it through

  * One line of code to load the module and execute the function

  .. code-block:: python

     import renderoverride_actions;renderoverride_actions.actions_text()

  .. seealso::
     :ref:`sample_Action_en`


Return value
************

* Only return types ``list[str]`` or ``str`` are accepted.

..  sep

* ``list[str]`` should contain strings, one element per line

  .. code-block:: python

     def get_text() -> list[str]:
         text_lines = [
            'Line 1',
            'Line 2',
            'Line 3'
         ]
         return text_line


* If you want to break a string, insert a newline code ``\n``.

  .. code-block:: python

     def get_text() -> str:
         text_lines = 'Line 1\nLine 2\nLine 3'
         return text_line


* If the ``maya.cmds`` command returns a value in the form of ``list[str]`` or ``str`` , it can be executed directly

  .. code-block:: python

     import maya.cmds;maya.cmds.ls(sl=True)

  .. warning::
     * It is the developer's responsibility to guarantee the return type.Make sure that None or any other type is not returned.
     * If there are no characters to return, return an empty string (``''``).


