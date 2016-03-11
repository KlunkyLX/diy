---
layout: post
title:  "Experiences with Cheap MMS Spy Camera"
date:   2016-03-10 20:00:0
thumbnail: images/2016-03-09-mms-spy-camera/03.jpg
tags:
- camera
- mms
- outdoor
- spy
---

In the past few years I created and tested several web--cams for outdoor use. [Here is summary of all my experiments (in Slovak)](https://www.nabezky.sk/node/15989).

Recently I discovered on eBay a very cheap device named [GPRS Positioning MMS Video Taking Locator Video band GSM spy camera](http://www.ebay.com/itm/262112627110). In terms of features the device is similar to trail hunting cameras, but the price is awesome, just 24 USD (shipment included). Regarding the price there are some drawbacks too -- the camera resolution is `640 x 480 px`, the user manual seems to be machine translated from Chinese and thus hard to understand, and the device is barebone, just a circuit lacking any waterproof case.

![MMS Spy Camera]({{site.baseurl}}/images/2016-03-09-mms-spy-camera/03.jpg "MMS Spy Camera")

The device is shipped with `400mAh` lipol battery. According to specification, standby time should be 12 days and working time 4--6 days. Unfortunately user manual provides no information on what is the difference between standby time and working time and there does not seem to be an option to switch the device from one mode to the other.

The device is managed solely via SMS/MMS messages. You send the device a SMS message with a text code (e.g. `111` means take photo) and device will send you back an MMS with photo.

I needed the device to operate for cca 2 months, so I abandoned the default `400 mAh` battery and connected ten times larger battery instead (i.e. `4.000 mAh`). My expectation was that if the minimal working time with `400 mAh` battery is 4 days, then `4.000 mAh` battery will allow me to use the device for at least 40 days.

Camera with large `4.000 mAh` battery:

![MMS Spy Camera with 4.000mAh battery]({{site.baseurl}}/images/2016-03-09-mms-spy-camera/02.jpg "MMS Spy Camera")

I put the device in a plastic box and placed it outdoors in a place with good GPRS signal. The air temperature was between 0&deg;C (night) to 10&deg;C (day). Each day I took one or two photos with the device. 

Here is sample photo:

![MMS Spy Camera Sample Photo]({{site.baseurl}}/images/2016-03-09-mms-spy-camera/01.jpg "MMS Spy Camera")

Sometimes the device sent no response after first `make photo` message. In such case it was sufficient to send another `make photo` SMS 5 minutes later and the second SMS was processed successfully.

After 5 days the device sent me an SMS with text `Device battery is low`. According to user manual, such a message is sent by the device when the battery is left with `10%` of its capacity. I was surprised by this behavior as I expected that I will receive such a message no sooner than after cca 35 days of usage.

When I started the experiment battery voltage was `4.17V`, which means fully charged. When I tested the battery voltage after receiving `Device battery is low`, the battery voltage was `3.90V`.
`3.90V` means that li-pol battery has cca `60%` of its capacity. It seems MMS spy camera device is unable to properly measure battery voltage.
 Nevertheless, the device is depleting the battery much faster than expected.
 
### Other Remarks
 
* User manual states that after you start the device, `the product will automatically switch on the red light with shining four times`. 
  * This is not true. The LED will shine for cca 4 seconds steadily, but no blinking happens.
* According to user manual the device has following feature: `Binding the master number: Use the mobile phone to send the text message 000 to the alarm locator, the machine will reply a text message; Set; Binding + the master number`. 
  * The device provides no response (though my SMS is flagged as received). However the master phone number seems to be bind properly -- low battery warnings were sent properly to my phone number. 
* Rebooting the device with SMS works fine.
* The device has a microphone. You can call the device and you will hear in your phone the microphone's input.
* The device sent me no response to GPS position requests.
* I have not tried the other features (e.g., video).
* User manual provided with the device seems to be from some other model (`GF-08`) which features [a box with android logo](http://topcctvdvr.com/product.php?id_product=585). Here is first page of the user manual:

![MMS Spy Camera Manual]({{site.baseurl}}/images/2016-03-09-mms-spy-camera/04.jpg "MMS Spy Camera Manual")
 
### Conclusion
 
Despite very low price (24 USD, shipment included) the device is somehow operational (actually I expected that it won't work at all). From my point of view the biggest drawback is very poor battery life -- when taking one photo per day and using `4.000mAh` battery, the device will consume 40% of the battery in 5 days.
 
 










