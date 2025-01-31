************
Get Started
************

Introduction
=============

This driver is based on `esp_lcd`_.

Currently only some basic functions are supported.It will be compatible with `st7789_mpy`_ in the future.

.. _esp_lcd: https://docs.espressif.com/projects/esp-idf/en/latest/esp32/api-reference/peripherals/lcd.html
.. _st7789_mpy: https://github.com/russhughes/st7789_mpy

Supported LCD Types
====================

- Intel 8080 parallel LCD
- DPI(RGB) LCD
- SPI LCD
- QSPI LCD

Supported driver ICs
=====================

- ST7789
- ST7701s
- ST7735
- ILI9488
- RM67162

Compiling guide
================

Get the source code
--------------------

.. code-block:: shell

    cd micropython
    git clone https://github.com/lbuque/lcd_binding_micropython.git extmod/lcd_binding_micropython

esp32
------

.. note::

    Please prepare `esp-idf release/v4.4 <https://github.com/espressif/esp-idf/tree/release/v4.4>`_ before compiling

    For more detailed compilation of esp32, please refer to https://github.com/micropython/micropython/tree/master/ports/esp32

.. code-block:: shell

    cd ports/esp32/
    make USER_C_MODULES=../../../extmod/lcd_binding_micropython/lcd/micropython.cmake

.. toctree::
    :maxdepth: 1
    :hidden:

    self
    API Reference <api-reference/lcd>
    LCD WiKi <screen/index>
    Copyrights <COPYRIGHT>
