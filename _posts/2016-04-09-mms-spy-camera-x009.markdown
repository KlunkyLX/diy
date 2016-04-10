---
layout: post
title:  "Experiences with X009 Device (Cheap Spy SIM GPRS GPS Camera)"
date:   2016-04-09 20:00:0
thumbnail: images/2016-04-09-mms-spy-camera-x009/01.jpg
tags:
- camera
- mms
- outdoor
- spy
---

Previous month I played with unbranded Chinese [MMS spy camera](https://petervojtek.github.io/diy/2016/03/10/mms-spy-camera.html), this time I tested similar device branded as X009. The principle is the same for both devices -- you send SMS message to the device and receive photo in MMS message (and there are plenty other features like microphone and video).

The X009 device can be found on eBay as ["Mini SIM GPRS Tracker Locator SOS GSM DV Camera Monitor Recorder Device Callback"](http://www.ebay.com/itm/321967172495) and its price 16 USD (shipment to EU included) is so far lowest I have seen for such a device.

![MMS Spy Camera X009]({{site.baseurl}}/images/2016-04-09-mms-spy-camera-x009/01.jpg "MMS Spy Camera X009")

X009 is packed in a non-waterproof plastic case which contains also `450mAh` battery. Device is shipped with small paper manual book written in English and Chinese and is easy to follow.

X009 is also shipped with charging cable as the charging connector is not USB micro-B but some special one. This photo features USB micro-B connector on the top and the weird connector required to charge X009 is below:

![MMS Spy Camera X009]({{site.baseurl}}/images/2016-04-09-mms-spy-camera-x009/04.jpg "MMS Spy Camera X009")

Manual claims that X009 will provide 3 to 5 days of lifetime when in use, and 12 to 15 days of life when in standby mode. Because I needed to use the device for longer period of time, I disassembled it and attached larger `4.000 mAh` battery. Soldering is required for this step.

Here is X009 when original case and battery is removed. Camera si on the left side, SIM card and SD card holders are on top.

![MMS Spy Camera X009]({{site.baseurl}}/images/2016-04-09-mms-spy-camera-x009/03.jpg "MMS Spy Camera X009")

I inserted SIM card, freshly formatted SD card (FAT32), plugged in battery and pressed power button. The power LED blinked several times indicating device started working.

After then I send SMS with text `111` to the device and X009 replied with MMS with image attached. [Description on eBay](http://www.ebay.com/itm/321967172495) states that camera resolution is 2Mpx which is not true. Camera resolution is `640px x 480px`, here is sample photo:

![MMS Spy Camera X009]({{site.baseurl}}/images/2016-04-09-mms-spy-camera-x009/05.jpg "MMS Spy Camera X009")

After then I kept the device working to see for how long the large battery will last. As with the previous spy camera test I sent one or two `get photo SMS requests` per day.

On day three I received no response after repeated attempt to obtain photo.
On day four X009 replied successfully to my get photo request, but that was the last time I received any response from it.

In subsequent days I did not managed to receive response from the device. On day 6 I gave up, detached battery from the device and measured battery voltage. When experiment started the large `4.000 mAh` lipo battery was fully charged (`4.18V`). After 5 days its voltage dropped to `4.12V` which means battery still kept cca 85% of its capacity.

Apart from camera I tried few other X009 features:

* The device can receive phone calls -- I was able to call it and listened in my smartphone to input from X009's microphone.
* X009 is storing photos on SD card. The date and time set to photos does not seems to be correct (in my case year was 2013).
* I tried phone callback feature - when SMS with text `888` is sent to device it will reply with `Sound function is opened. Decibel is 60`. When noise above 60dB is made, X009 should call my phone number and I should be able to listen to its microphone.
Howeve no matter how much noise I made, the device made no phone call attempt.
* When X009 has low battery and you send it a request request, device will reply with `Tracker battery is low` SMS.
* I have not tried other features.

### Summary

Concerning the low price (16 USD with shipment) the X009 device is amazing piece of hardware. Camera and microphone work properly, thought their quality do match the price. Camera resolution is only 640x480 px and not 2MPx. Battery life seems to be fine however my main problem is that X009 is unable to operate reliably for more than few days without manual reboot (and the SMS API has no message to reboot the device remotely).
The non-standard charging connector is a fail but it is easy to dismantle the device and replace battery directly without charging it via board.