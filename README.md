# ESP32-Test
![Alt text](https://images.squarespace-cdn.com/content/v1/59b037304c0dbfb092fbe894/1573230009361-8KRM4G2CWI9FS4AQPL2J/nodemcu_front_side.JPG)
### Note: This is a demonestraion repo about how we will we organise the pdf materias 

<details>
           <summary>To  :Mr.Ahmed Alsaleh</summary>
           <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
         
<details>
           <summary>By :Eng.Alaa Elnaggar</summary>
           <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
         
## Introduction
![Alt text](https://openthread.google.cn/images/ot-contrib-espressif.png?authuser=2)

wifi SOC (system on a chip) produced by Espressif Systems . It is an highly integrated chip designed to provide full internet connectivity in a small package.

## What is it good for?
![Alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/WiFi_Logo.svg/1200px-WiFi_Logo.svg.png)

ESP8266 can be used as an external Wifi module, using the standard AT Command set Firmware by connecting it to any microcontroller using the serial UART, or directly serve as a Wifi-enabled micro controller, by programming a new firmware using the provided SDK.

![Alt text](https://i1.wp.com/randomnerdtutorials.com/wp-content/uploads/2018/08/ESP32-DOIT-DEVKIT-V1-Board-Pinout-30-GPIOs-Copy.png?w=966&ssl=1)

The GPIO pins allow Analog and Digital IO, plus PWM, SPI, I2C, etc.

This board has been around for almost a year now, and has been used mostly in IoT contexts, where we want to add connectivity for example to an Arduino project. A wide adoption has been facilitated by the very modest price, ranging from 2.50 to 10 USD depending on the features offered by the manufacturers.

## Some example projects:

* Temperature logging and Web UI
![Alt text](https://i.pinimg.com/736x/bf/2a/2a/bf2a2a2b3260f1bd94e9c85ea9f65752.jpg)

* Retro Web Browser
* Internet Enabled Smoke alarm
* Technical Features
* Wi-Fi Direct (P2P), soft-AP
* Built-in TCP / IP protocol stack
* Built-in TR switch, balun, LNA, power amplifier and matching network
* Built-in PLL, voltage regulator and power management components
* Built-in temperature sensor
* Support antenna diversity
* off leakage current is less than 10uA
* Built-in low-power 32-bit CPU: can double as an application processor
* SDIO 2.0, SPI, UART
* STBC, 1×1 MIMO, 2×1 MIMO
* A-MPDU, A-MSDU aggregation and the 0.4 Within wake
* connect and transfer data packets
* standby power consumption of less than 1.0mW (DTIM3)
Variants
ESP8266-based boards are available from several vendors and with different breakout boards. Most of the boards differ in the number of pins made available, the amount of Flash memory for storing program and data, and the shielding on the SOC for certified boards.

Some boards also support an external uFL antenna connector as well as the buil-in on-chip antenna.

The most common variants are:

ESP-01
ESP-01

This is the first and simplest board using the ESP8266. It allows to attach serial lines, and only breaks out two GPIO pins for native usage. This is also the cheapest and can be purchased from many chinese suppliers at 2.5 dollars.

ESP-03
ESP-03

This is the second generation board, breaking out more GPIO pins, and using a different antenna, plus an external antenna connector.

Olimex ESP8266 Eval Board
Olimex

This board, produced by Olimex, breaks out all the ESP8266 pins in breadboard headers, but can also be soldered as a module.
It contains 2Mb of flash memory, four times that available on the ESP-01 and ESP-03, for larger firmware and space for files useful to make a webserver.

Using the ESP8266 with Arduino
Several Libraries have been developed to use ESP8266 as a module for Arduinos.

Also there is a port of the Arduino IDE for programming the ESP Directly, see below.

Using the ESP8266 via Serial port
You can interact with the ESP8266 sending AT Commands via the provided TX and RX pins by using another microcontroller.

Pay attention to the voltage of your signal lines, as the ESP8266 only works with 3.3v and pins are not 5V tolerant.

I.e. if you want to attach it to an Arduino clone you must use a logic level converter such as this .

An alternative to the logic level converter is to build a voltage divider circuit for each
signal line.

Programming the ESP8266 Directly
In order to program the ESP directly you need to install a toolchain and firmware upload utility.

The ESP8266 Wiki explains the process in detail.

You should use the ESP Open SDK to build your toolchain.

Espressif also provides an SDK containing the AT Firmware and the proprietary libraries.

Finally a ready to use VirtualBox virtual machine is available here

As an alternative you might want to program the ESP using the Arduino libraries. A port of the Arduino IDE 1.6.x is available here .

Documentation
English Datasheet
Resources
NURDSpace ESP8266
Community Wiki
Vendor Wiki
Peter Scargill Blog
