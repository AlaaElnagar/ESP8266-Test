# ESP32-Test
![Alt text](https://images.squarespace-cdn.com/content/v1/59b037304c0dbfb092fbe894/1573230009361-8KRM4G2CWI9FS4AQPL2J/nodemcu_front_side.JPG)
### Note: This is a demonestraion repo about how we will organise the pdf materias 

<details>
           <summary>To  :Mr.Ahmed Alsaleh</summary>
           <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
         
<details>
           <summary>By :Eng.Alaa Elnaggar</summary>
           <p>Content 1 Content 1 Content 1 Content 1 Content 1</p>
</details>
         
## Introduction about ESP
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

![Alt text](https://i.pinimg.com/736x/9d/16/7b/9d167b9e4f50215c42ef883817e997ce.jpg)

* Internet Enabled Smoke alarm

![Alt text](https://iotdesignpro.com/sites/default/files/main-image/IoT-based-Fire-Alarm-System-using-NodeMCU-ESP8266_0.jpg)

## Technical Features
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

# ESP Code

```
/*
 * Created by esp32io.com
 *
 * This example code is in the public domain
 *
 * Tutorial page: https://esp32io.com/tutorials/esp32-button-led
 */

// constants won't change. They're used here to set pin numbers:
const int BUTTON_PIN = 7;  // the number of the pushbutton pin
const int LED_PIN =  3;   // the number of the LED pin

// variables will change:
int buttonState = 0;   // variable for reading the pushbutton status

void setup() {
  // initialize the LED pin as an output:
  pinMode(LED_PIN, OUTPUT);
  // initialize the pushbutton pin as an pull-up input:
  // the pull-up input pin will be HIGH when the switch is open and LOW when the switch is closed.
  pinMode(BUTTON_PIN, INPUT_PULLUP);
}

void loop() {
  // read the state of the pushbutton value:
  buttonState = digitalRead(BUTTON_PIN);

  // control LED according to the state of button
  if(buttonState == LOW)         // If button is pressing
    digitalWrite(LED_PIN, HIGH); // turn on LED
  else                           // otherwise, button is not pressing
    digitalWrite(LED_PIN, LOW);  // turn off LED
}


```

