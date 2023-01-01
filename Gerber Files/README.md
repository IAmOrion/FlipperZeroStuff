# FlipperZeroStuff

Important note: As of the date of uploading these (Jan 1st 2023 @ 01:43am) - I have not had received my boards from JLCPCB yet so have not physically tested and of these boards. In theory they should be fine, but I will update this readme after testing.  Obviously, during the design phase, I tested the individual components connected and the design via breadboards

# Flipper Zero Rear Mount PCB

Simple PCB to allow other add-on boards to be mounted behind the flipper zero

LEDs / Resistors are all SMD 1206 package size

![alt text](/images/Flipper Zero Rear Mount PCB TOP.png)

![alt text](/images/Flipper Zero Rear Mount PCB BOTTOM.png)

# Flipper Zero ProtoType PCB

Simple prototyping board with the same PCB outline footprint/size of the Official WiFi Dev Board

LEDs / Resistors are all SMD 1206 package size

# Flipper Zero NRF24L01 PCB

Simple NRF24L01 board to allow the use of numerous NRF24 modules with the Flipper Zero.  Make sure you pay attention to the pinout used with the actual NRF24 board you are using with it.

LEDs / Resistors / Capacitors are all SMD 1206 package size

1 x 10uF 
1 x 100nF (aka 0.1uF)
1 x NRF24L01+

# Flipper Zero Multi Board PCB

This is mostly designed as an "off the shelf plugin parts" board.  It's a messy multi board that covers multiple options.
The ESP32 can be used "Stand-alone" with a 2.8" TFT Touch Screen so you can run Marurder standalone (doesn't need the flipper companion app).  You can obv opt to not use the tft, enable the TX/RX pins via DIP switches and use the flipper companion app.  There's also connections for an HC-SR04, I2C (3.3v, GND, SCL, SDA) Breakout, Adafruit GPS, Wemos D1 + Micro SD Card, ESP32S (30 Pin) + Micro SD Card, NRF24

Apps tested: Flashlight, NMEW GPS, HC-SR Dist Sensor, ESP32 Marurder, ESP8266 Deauther

LEDs / Resistors / Capacitors are all SMD 1206 package size

2 x SD Card: https://www.sparkfun.com/products/544
1 x Wemos D1 Mini
1 x ESP32S 30-Pin (ESP32-WROOM-32D)
1 x NRF24L01+
1 x Adafruit GPS (#746)
1 x HC-SR04

*IMPORTANT* -- During testing, I found that some ESP8266 boards had their RX/TX mislabled (Specifically marked Wemos but could be bad clones).  Meaning that connections are TX -> TX, RX -> RX and *NOT* the normal RX -> TX, TX -> RX! This was annoying, so trying and cover all bases with the ESP8266 so there are tiny jumper pads to set the appropriate TX/RX pins correctly.

# Some Notes

All these boards are realistically V1's.  Tested on breadboards, probably (likely) could be improved, but here they are, as they stand, gerbers provided, for all download and use freely for personal use

I am based in the UK and personally use https://jlcpcb.com for all my PCBs.  Not affiliated or sponsored in anyway, they're just who I preferred after giving a few companies a try.
