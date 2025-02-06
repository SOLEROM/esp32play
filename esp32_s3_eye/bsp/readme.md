# esp BSP


A BSP typically supports all of the hardware components provided on development board. Apart from the pinout definition and initialization functions, a BSP ships with drivers for the external components such as sensors, displays, audio codecs etc.

The BSPs are distributed via IDF Component Manager, so they can be found in ESP Component Registry.

* https://github.com/espressif/esp-bsp


Packages from this repository are uploaded to the IDF component registry. You can add them to your project via idf.py add-dependency, e.g.

    idf.py add-dependency esp_wrover_kit==1.0.0

    idf.py add-dependency --component=my_component example/cmp<=3.3.3

    idf.py add-dependency --path="../../my_component" example/cmp^3.3.3

