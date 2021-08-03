# Girier JR-DS10 data dump

Girier JR-DS10 is a smart switch, controllable via WiFi using Tuya.

![Overview](http://ipic.su/img/img7/fs/kiss_245kb.1627998700.png)

![Internals](http://ipic.su/img/img7/fs/kiss_475kb.1627998721.png)

## Datasheet

* `VCC` — 3v
* `GND` — ground
* `K1` — ???, works fine without it
* `LED` — Built-in LED
* `PLY/PIAY` — Relay
* `S1` — Switch

![Pins](http://ipic.su/img/img7/fs/kiss_233kb.1627998777.png)

![Pins on chip connector](http://ipic.su/img/img7/fs/kiss_250kb.1627999496.png)

## Tasmota convertion

You can desolder TW-02 chip from the board and solder on ESP8266 and flash it with Tasmota.

For example, I used Wemos D1 mini and I've soldered `PLY/PIAY` to `D7` and `S1` to `D3`.
In Tasmota, I've selected `Generic (18)` preset and used this configuration:

* `PLY/PIAY` — Relay
* `S1` — Switch

![Tasmota configuration](http://ipic.su/img/img7/fs/kiss_16kb.1627999503.png)
