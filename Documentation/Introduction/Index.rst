﻿.. ==================================================
.. FOR YOUR INFORMATION
.. --------------------------------------------------
.. -*- coding: utf-8 -*- with BOM.

.. include:: ../Includes.txt


.. _introduction:

Introduction
------------

.. _about-tsref:

About this document
^^^^^^^^^^^^^^^^^^^

This document is a complete reference to all objects and properties of
TypoScript as used in TYPO3 TypoScript templates (and not in TSconfig).

For explanations about the syntax of TypoScript itself, please refer
to the :ref:`"TypoScript Syntax and In-Depth Study" <t3tssyntax:start>` manual.

This version is updated for TYPO3 CMS version 7.1.


.. _what-s-new:

What's new
^^^^^^^^^^

During the development of TYPO3 7, a lot of properties have been added,
changed, deprecated or removed.

Additionally various descriptions were improved and many smaller
mistakes were fixed.

For a list of all changes see the `commit log on GitHub
<https://github.com/TYPO3-Documentation/TYPO3CMS-Reference-Typoscript/commits/latest>`_.


For more details about changes in the various TYPO3 versions please
refer to the links below.

.. tip::

   **More information about changed properties**

   You can find a list of changes for more recent TYPO3 versions here:

   TYPO3 4.2: `http://wiki.typo3.org/Documentation\_changes\_in\_4.2
   <http://wiki.typo3.org/Documentation_changes_in_4.2>`_

   TYPO3 4.3: `http://wiki.typo3.org/Documentation\_changes\_in\_4.3
   <http://wiki.typo3.org/Documentation_changes_in_4.3>`_

   TYPO3 4.4 and 4.5:
   `http://wiki.typo3.org/Documentation\_changes\_in\_4.4\_and\_4.5
   <http://wiki.typo3.org/Documentation_changes_in_4.4_and_4.5>`_

   TYPO3 4.6: `http://wiki.typo3.org/Documentation\_changes\_in\_4.6
   <http://wiki.typo3.org/Documentation_changes_in_4.6>`_

   TYPO3 4.7: `https://forge.typo3.org/versions/1454 <https://forge.typo3.org/versions/1454>`_

   TYPO3 6.0: `https://forge.typo3.org/versions/1623 <https://forge.typo3.org/versions/1623>`_

   TYPO3 6.1: `https://forge.typo3.org/versions/1960 <https://forge.typo3.org/versions/1960>`_

   TYPO3 6.2: `https://forge.typo3.org/versions/1968 <https://forge.typo3.org/versions/1968>`_


.. _credits:

Credits
^^^^^^^

The manual was originally written by Kasper Skårhøj. Over the years it
has been maintained and updated successively by Michael Stucki,
François Suter and Christopher Stelmaszyk.


.. _feedback:

Feedback
^^^^^^^^

For general questions about the documentation get in touch by writing
to `documentation@typo3.org <mailto:documentation@typo3.org>`_ .

If you find a bug in this manual, please be so kind as to check the
online version on http://docs.typo3.org/typo3cms/TyposcriptReference/.
From there you can hit the "Edit me on GitHub" button in the top right corner
and submit a pull request via GitHub. Alternatively you can just file an issue
using the bug tracker: https://github.com/TYPO3-Documentation/TYPO3CMS-Reference-Typoscript/issues.

Maintaining high quality documentation requires time and effort
and the TYPO3 Documentation Team always appreciates support.
If you want to support us, please join the documentation
mailing list/forum (http://forum.typo3.org/index.php/f/44/).


.. _general-information:

General information
^^^^^^^^^^^^^^^^^^^

.. _case-sensitivity:

Case sensitivity
""""""""""""""""

All names and references in TypoScript are **case sensitive!** This
is very important to notice. For example watch the words "TEXT" and "value"
in this TypoScript code::

   myObject = TEXT
   myObject.value = <strong>Some HTML code</strong>

This is not the same as ::

   myObject = text
   myObject.Value = <strong>Some HTML code</strong>

While the first will be recognized as the content object "TEXT" and
will produce the desired output, the latter will not be recognized and
will not output anything. Even if you wrote **"TEXT"** in uppercase in the
second example, it would still not work, because the property **"value"**
is misspelled.

Always remember: In this manual the case of objects **is** important.


.. _version-numbers:

Version numbers
"""""""""""""""

For new features TSref includes a note in which TYPO3 version the
feature was added. If such a note is missing, the feature is part of
TYPO3 since version 6.2 at least.

