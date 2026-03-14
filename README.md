# Basic ESP beginner project

Test your ESP by connecting it to your home modem/router and controlling it using your smart devices such as phone or PC, that are also connected to your modem. Here the ESP acts as a station node connecting to your modem i.e. access point (ESP >> Router/Modem  << Laptop/Phone). ESP chips provide a low-cost, low-power System-on-a-Chip (SoC) solution for wireless connectivity in Internet of Things (IoT) applications. 

# Key Functions of ESP:

Wireless Communication:
They provide integrated Wi-Fi and often Bluetooth (Classic and Low Energy) to allow devices to connect to local networks, smartphones, or the cloud.

Embedded Control: 
They function as microcontrollers that can read data from sensors (like temperature or motion) and control hardware (like motors, lights, or displays) via numerous GPIO pins.

Standalone or Slave Operation: 
They can run as a complete, independent system or serve as a communication bridge for another "host" processor (like an Arduino).

Edge Computing: 
Modern variants like the ESP32-S3 include hardware acceleration for AI and Machine Learning, allowing for local voice recognition or image processing. 

# ESP can act as a WiFi access point or as a station Node
ESP >> ESP  << Laptop/Phone  (Diagram attached)

ESP >> Router/Modem  << Laptop/Phone  (Diagram attached) 

# Datasheets and documentation on ESP chips:

https://www.espressif.com/en/support/documents/technical-documents

# Please Note the following:
In this project ESP8266MOD is used, therfore the required Board Managers are installed and additional board manger URL is updatd on the Arduino IDE (screenshorts attached). Please install the Board Manager according to the ESP chip you are working with.

# Requirments
-PC / mobile with an interner browser app

-Arduino IDE to programm on the PC

-ESP32 / ESP8266 (all have WiFi module)

-Data cable for ESP

-WiFi

# Code  
Code file: ESP8266WiFiConnectNControl.ino

Changes the following in code: SSID of your router(Cell:13), Password of router(cell:14)

Set the right port and select the appropriate board in the Arduino IDE. Verify and uploading the code to the board.

Next check the serial port(115200 baud) of Arduino IDE for the IP assigned to ESP by the router to connect your phone and PC(some ESPs you need to hit the reset button to start the connection with WiFi).  

Now copy the IP address from the serial port and open it in browser or search engine of your PC or phone which is also connected to the same WiFi. Now you must notice that the webpage loads, and displays the following two line:


-GPIO is now high/low

-Click here to switch LED GPIO on, or here to switch LED GPIO off.



Now you can trigger the light on the ESP to On and OFF from the browser of your device through your WiFi. 


More beginner codes with simple examples on ESP functionallity can be found on Arduino IDE>> Files>> Examples.   


