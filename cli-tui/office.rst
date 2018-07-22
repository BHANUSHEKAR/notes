========================================
Office
========================================

現在如果提到開源的辦公軟體，
最大宗的應該就是 LibreOffice 了。
（在 LibreOffice 從 OpenOffice fork 出去前，
最多人用的應該是 OpenOffice）

歷史發展：

.. image:: https://upload.wikimedia.org/wikipedia/commons/f/fb/StarOffice_major_derivatives.svg



.. contents:: 目錄




LibreOffice
========================================


OpenCL
------------------------------

Extension
------------------------------


常用指令
------------------------------

轉成 PDF
++++++++++++++++++++

作法一：

.. code-block:: sh

    libreoffice --headless --convert-to pdf *.doc *.docx *.ppt *.pptx


作法二：使用 ``unoconv`` （仍然依賴 LibreOffice）

.. code-block:: sh

    unoconv *.doc *.docx *.ppt *.pptx


參考
========================================

* `Wikipedia - LibreOffice <https://en.wikipedia.org/wiki/LibreOffice>`_
* `ArchWiki - LibreOffice <https://wiki.archlinux.org/index.php/LibreOffice>`_
* `Gentoo Wiki - LibreOffice <https://wiki.gentoo.org/wiki/LibreOffice>`_
* `Collabora Office - LibreOffice in the Cloud <https://www.collaboraoffice.com/>`_
* `LibreOffice online <https://cgit.freedesktop.org/libreoffice/online/>`_
