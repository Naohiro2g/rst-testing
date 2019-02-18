Read the great document at https://ssd1306.readthedocs.io/en/latest/

Installation
^^^^^^^^^^^^

..

sudo apt-get install libjpeg62-turbo-dev libjpeg-dev
sudo -H pip3 install --upgrade luma.oled




## SPI connection of my display module (VCC and GND was reversed !)

========== ====== ============ ====================
OLED Pin   Name   Remarks      RPi Function
========== ====== ============ ====================
1 Brown    GND    Ground       GND
2 Red      VCC    +3.3V Power  3V3
3 Orange   D0     Clock        GPIO 11 (SCLK)
4 Yellow   D1     MOSI         GPIO 10 (MOSI)
5 Green    RST    Reset        GPIO 25 (*)
6 Blue     DC     Data/Command GPIO 24 (*)
7 Purple   CS     Chip Select  GPIO 8 (CE0)
========== ====== ============ ====================
