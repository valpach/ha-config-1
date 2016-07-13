# My Home Assistant Config
Example [Home Assistant](https://home-assistant.io) Configs

My HA installation runs on a Pi 3 with the following devices:

* [Plex Media Server](https://plex.tv)
* [Homebridge](https://github.com/nfarina/homebridge) *for Apple HomeKit Support*
* [Foscam FI8918W](https://www.amazon.co.uk/gp/product/B0046710G6)
* [Fibaro FGMS-001 Motion Sensor](https://www.amazon.co.uk/gp/product/B00JHHNUPY/)
* [Aeotec USB Z-Stick S5](https://www.amazon.co.uk/gp/product/B00YETCNOE/ref=oh_aui_detailpage_o06_s00?ie=UTF8&psc=1)

I use the iCloud component for presence, which when combined with the Fibaro sensor gives me alerts when motion is detected and both my wife and I are out of the house. This then triggers some automations;

* If we haven't enabled motion detection it sends a pushbullet notification to remind us
* If notifications _are_ on, and motion gets detected, send a pushbullet notification

![UI](http://i.imgur.com/3KEEfmj.png)
