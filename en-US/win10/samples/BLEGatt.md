---
layout: default
title: BLE GATT Sample - Overview
permalink: /en-US/win10/samples/BLEGatt.htm
lang: en-US
---

## Bluetooth Low Energy (BLE) Generic Attribute Profile (GATT) Sample Overview
In this sample we will discover how to work with Bluetooth Low Energy devices using the GATT profile and a TI CC2541 SensorTag. You can find the source code for this sample by downloading a zip of all of our samples [here](https://github.com/ms-iot/samples/archive/develop.zip){:target="_blank"}, and navigating to the [`BluetoothGATT/CS`](https://github.com/ms-iot/samples/tree/develop/BluetoothGATT/CS){:target="_blank"} folder.

### What is Bluetooth Low Energy & GATT?
Bluetooth Low Energy (BLE), or Bluetooth Smart, is a wireless protocol that is part of the Bluetooth 4.0 core specification. The key feature of BLE is its low power consumption, leading to its widespread adoption by IoT and wearable devices. 

Generic Attribute Profile (GATT) is the Bluetooth Profile that BLE devices will use to communicate with each other. Data is organized into nested objects called Profiles, Services, and Characteristics, as illustrated in the diagram below:

![Gatt Structure Diagram]({{site.baseurl}}/images/BLEGatt/GattDiagram.png)

It is strongly suggested to have a good grasp on these concepts before continuing. Adafruit has a great overview of how Bluetooth Low Energy (BLE) & the GATT profile work [here](https://learn.adafruit.com/introduction-to-bluetooth-low-energy/introduction){:target="_blank"}.

### The TI CC2541 SensorTag

![SensorTag Picture]({{site.baseurl}}/images/BLEGatt/SensorTag_with_iPad.jpg)
<sub>*[Image from Texas Instruments](http://processors.wiki.ti.com/index.php/File:SensorTag_with_iPad.jpg){:target="_blank"}*</sub>

In this sample we will be connecting a Windows IoT Core device with the [Texas Instruments CC2541 SensorTag Development Kit](http://www.ti.com/tool/cc2541dk-sensor){:target="_blank"} via BLE. The SensorTag is a BLE device powered with the TI CC2541 chip, which features a programmable Bluetooth 4.0 stack. On the device are also the following 6 sensors, which are exposing data through the GATT profile:

1. Contactless IR temperature sensor (Texas Instruments TMP006)

2. Humidity Sensor (Sensirion SHT21)

3. Gyroscope (Invensense IMU-3000)

4. Accelerometer (Kionix KXTJ9)

5. Magnetometer (Freescale MAG3110)

6. Barometric pressure sensor (Epcos T5400)

For the sample, we are running firmware version 1.4.1 on the SensorTag. More detailed information about the SensorTag can be found [here](http://processors.wiki.ti.com/index.php/SensorTag_User_Guide){:target="_blank"}.

### Hardware Support
We are currently supporting the [Orico Model A Bluetooth dongle](http://www.amazon.com/ORICO-BTA-403-Bluetooth-Adapter-Compatible/dp/B00ESBRTMO/ref=sr_1_7?ie=UTF8&qid=1436917745&sr=8-7&keywords=bluetooth+4.0+orico){:target="_blank"}.

### What's Next?
1. [Pairing a BLE Device and GATT Attribute Table Dump Tool]({{site.baseurl}}/{{page.lang}}/win10/samples/BLEGatt1.htm) --- Learn how to pair the SensorTag with a Windows IoT Core device, and how to retrieve a GATT Attribute Table in Windows.

2. [Using and Dissecting the Code]({{site.baseurl}}/{{page.lang}}/win10/samples/BLEGatt2.htm) --- Learn how to use the sample along with a walkthrough of the code.