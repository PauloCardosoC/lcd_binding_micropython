*********
快速开始
*********

概况
====

此驱动程序基于 `esp_lcd`_。

目前只支持部分基本功能，未来会兼容 `st7789_mpy`_。

.. _esp_lcd: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/peripherals/lcd.html
.. _st7789_mpy: https://github.com/russhughes/st7789_mpy

已支持的LCD类型
===============

- Intel 8080并行LCD
- DPI(RGB) LCD
- SPI LCD
- QSPI LCD

已支持的驱动IC
==============

- ST7789
- ST7701s
- ST7735
- ILI9488
- RM67162

编译指南
========

获取源码
---------

.. code-block:: shell

    cd micropython
    git clone https://github.com/lbuque/lcd_binding_micropython.git extmod/lcd_binding_micropython

esp32
------

.. note::

    编译前请准备好`esp-idf release/v4.4 <https://github.com/espressif/esp-idf/tree/release/v4.4>`_

    关于esp32更详细的编译说明，请参考 https://github.com/micropython/micropython/tree/master/ports/esp32

.. code-block:: shell

    cd ports/esp32/
    make USER_C_MODULES=../../../extmod/lcd_binding_micropython/lcd/micropython.cmake

.. toctree::
    :maxdepth: 1
    :hidden:

    self
    API 参考 <api-reference/lcd>
    屏幕 WiKi <screen/index>
    版权 <COPYRIGHT>
