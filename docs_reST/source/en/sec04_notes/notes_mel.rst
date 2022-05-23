.. _notes_mel_en:

MEL Scripting Notes
###################

.. contents:: Contents of this page:
   :depth: 3
   :local:

++++

How to write "Text String"
**************************

* To run the MEL script directly, write the following (script to get the name of the selected object)

  .. code-block:: c

     ls -sl

* If you want to run an external MEL file (.mel), you can make Maya recognize the procedure (``global proc``) first


Return value
************

* Only ``string[]`` or ``string`` is accepted as the return type.

.. sep

* ``string[]`` should contain strings, one element per line

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


* If you want to break a string, insert a newline code ``\n``.

  .. code-block:: c

     global proc string getText()
     {
         string $textLines = "Line 1\nLine 2\nLine 3";
         return $textLines;
     }

  .. warning::
     * It is the developer's responsibility to guarantee the return type.
     * If there are no characters to return, return an empty string (``""``).


