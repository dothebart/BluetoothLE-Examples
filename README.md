# working my way into Bluetooth LE

Having purchased a [Genuino 101](https://www.arduino.cc/en/Main/ArduinoBoard101) I wanted to do some hacking with it.
Most of the easy examples I found focused on getting stuff visible on a mobile, which I didn't care for.

Deciding that I shouldn't have unknown factors on both sides, I purchased the TI sensor tag, a BLE USB stick for my Odroid C1.

After first trying with python I found [bleno](https://github.com/sandeepmistry/bleno) and [noble](https://github.com/sandeepmistry/noble) by [Sandeep Mistry](https://twitter.com/sandeepmistry) which seems to give a better start. After some fiddling with the build and stracing I got it working on the Odroid via some symlinks.

Since all these verbs around bluetooth tend to become tricky, I purchased some books, [Getting Started with Bluetooth Low Energy](https://www.amazon.de/Getting-Started-Bluetooth-Low-Energy/dp/1491949511/ref=sr_1_23?ie=UTF8&qid=1464447774&sr=8-23) gives a fair overview of all the termina around bluetooth (Central, Peripherial, GATT, device profile, ...). 

A bit more about getting some examples implemented is 
[Make: Bluetooth: Bluetooth LE Projects with Arduino, Raspberry Pi, and Smartphones](https://www.amazon.de/Make-Bluetooth-Raspberry-Smartphones-2015-12-21/dp/B01A68PHR6/ref=sr_1_16?ie=UTF8&qid=1464447747&sr=8-16) which features some tiny projects with noble, bleno and the sensor tag.

#My first own hacks
## sensorTag/sensorTagExample/sensortagAccellmouse.js
Couples the sensor tag, and uses [robotjs](https://github.com/octalmage/robotjs) to move the mouse cursor.

Stay tuned and expect to find more.

Derived from the clone: ;-)


# BluetoothLE-Examples

This repository contains examples for Bluetooth LE in node.js, Arduino, and Apache cordova. These were written for classes at [ITP](http://itp.nyu.edu) by Tom Igoe, Maria Paula Saba, with contributions by Don Coleman, Sandeep Mistry and Shawn Van Every.

## Software You'll Need

To run these examples, you'll need to [node.js](http://www.nodejs.org), [Arduino 1.6.0](http://arduino.cc/en/Main/Software) or later, and [Cordova 4.0](https://cordova.apache.org/) or later. We've tested the Cordova examples on iOS and Android.

The node.js examples are all written using [Sandeep Mistry](https://github.com/sandeepmistry)'s Bluetooth LE libraries for node.js, specifically [noble](https://github.com/sandeepmistry/noble), [bleno](https://github.com/sandeepmistry/bleno), and various libraries he's made deriving from those. The cordova libraries are written using [Don Coleman](https://github.com/don)'s [BLE Central plugin for Cordova](https://github.com/don/cordova-plugin-ble-central). The Arduino examples are mostly intended for use with Nordic NRF8001 and NRF51822 radios, using Sandeep's [Arduino BLE Peripheral library](https://github.com/sandeepmistry/arduino-BLEPeripheral). These examples were written using RedBear Labs' [BLE Nano](http://redbearlab.com/blenano/) boards and [RFDuino](http://www.rfduino.com/)'s boards. There are also some examples for Punchthrough's [LightBlue Bean](https://punchthrough.com/bean/) modules.

For Windows users, Don Coleman's done a nice [video explaining how to set up Windows for Bluetooth LE and Node Development](https://www.youtube.com/watch?v=mL9B8wuEdms) using noble. 
