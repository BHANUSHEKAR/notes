========================================
Firefox 設定
========================================


.. contents:: 目錄


基本
========================================

* 如果有效能變差的問題記得先清 Cache 和歷史試試： ``Control + Shift + Delete``



相關頁面
========================================

* ``about:support`` 檢查目前的一些狀態
* ``about:config`` 更改細部設定



只使用記憶體當 Cache
========================================

+-------------------------------+-------+----------+
| 名稱                          | 值    | 其他     |
+===============================+=======+==========+
| browser.cache.disk.enable     | false |          |
+-------------------------------+-------+----------+
| browser.cache.memory.enable   | true  |          |
+-------------------------------+-------+----------+
| browser.cache.memory.capacity | -1    | 需要新增 |
+-------------------------------+-------+----------+



更改 Session 儲存間隔
========================================

+-------------------------------+--------+------------------------------------------+
| 名稱                          | 值     | 其他                                     |
+===============================+========+==========================================+
| browser.sessionstore.interval | 150000 | 分頁儲存時間，單位毫秒，1000 毫秒 = 1 秒 |
+-------------------------------+--------+------------------------------------------+



開啟追蹤保護
========================================

+------------------------------------+------+------+
| 名稱                               | 值   | 其他 |
+====================================+======+======+
| privacy.trackingprotection.enabled | true |      |
+------------------------------------+------+------+



關閉贊助內容
========================================

+-------------------------------------+------+------+
| 名稱                                | 值   | 其他 |
+=====================================+======+======+
| browser.newtabpage.directory.source | 空白 |      |
+-------------------------------------+------+------+
| browser.newtabpage.directory.ping   | 空白 |      |
+-------------------------------------+------+------+



開啟多 Process 支援（Electrolysis）
========================================

+-------------------------------+------+------+
| 名稱                          | 值   | 其他 |
+===============================+======+======+
| browser.tabs.remote.autostart | true |      |
+-------------------------------+------+------+



把整個 Profile 放在記憶體內（使用 tmpfs）
=========================================

可以直接使用現有的 script 處理，
目前有個叫 ``Profile-sync-daemon`` 的 script 就是負責把瀏覽器的 Profile 放在記憶體內，
並且定時寫回硬碟。

從 AUR 裝玩 ``profile-sync-daemon`` 後，
先執行指令一次以產生預設的設定檔：

.. code-block:: sh

    $ psd

接著到 ``$XDG_CONFIG_HOME/psd/psd.conf`` 更改設定檔，
打開需要支援的瀏覽器（可用空白分隔），
例如：

::

    BROWSERS="firefox"

另外還可以打開 OverlayFS 支援以減少記憶體使用量、增加同步速度。


接者可以打開 daemon ：

.. code-block:: sh

    systemctl --user start psd.service


最後查看狀態：

.. code-block:: sh

    $ psd p
    Profile-sync-daemon v6.25 on Arch Linux.

     Systemd service is currently active.
     Systemd resync service is currently active.
     Overlayfs v23 is currently active.

    ...



參考
========================================

* `ArchWiki - Firefox tweaks <https://wiki.archlinux.org/index.php/firefox_tweaks>`_
* `ArchWiki - Firefox on RAM <https://wiki.archlinux.org/index.php/Firefox_on_RAM>`_
* `ArchWiki - Profile-sync-daemon <https://wiki.archlinux.org/index.php/Profile-sync-daemon>`_
