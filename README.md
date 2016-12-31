# My Home Assistant Config
Example [Home Assistant](https://home-assistant.io) Configs

My HA installation runs on a Pi 3 with the following:

Software
--------
* [Plex Media Server](https://plex.tv)
* [Homebridge](https://github.com/nfarina/homebridge) *for Apple HomeKit Support*

Hardware
--------
* 1 x [Foscam FI8918W](https://www.amazon.co.uk/gp/product/B0046710G6) for a PTZ camera in my toddler's room which I've then configured using HA scripts to allow me to point at three different locations in the room
* 2 x [Foscam FI9800P](https://www.amazon.co.uk/gp/product/B015STDPJ0) - one for the front of the house, one for the back
* 1 x [Foscam C1 Lite](https://www.amazon.co.uk/gp/product/B0196AN3IU) for the hallway
* 2 x [Fibaro FGMS-001 Motion Sensor](https://www.amazon.co.uk/gp/product/B00JHHNUPY/) for motion and temperature (it does brightness too but I'm not making use of that yet)
* 1 x [Aeotec USB Z-Stick S5](https://www.amazon.co.uk/gp/product/B00YETCNOE/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1) plugged into the Pi to interface with the z-wave devices

Automation
--------
I use the iCloud component for presence, which when combined with the Fibaro sensor gives me alerts when motion is detected and both my wife and I are out of the house. This then triggers some automations;

* If we haven't enabled motion detection it sends a pushbullet notification to remind us
* If notifications _are_ on, and motion gets detected, send a pushbullet notification

![UI](http://i.imgur.com/3KEEfmj.png)