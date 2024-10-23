# Multi-Button-WS2812-RGB-esp8266-Decora
Multi Button WS2812 RGB esp8266 Decora <br>
![GitHub Logo](https://github.com/logichousepcb/Multi-Button-WS2812-RGB-esp8266-Decora/blob/main/3btn-pic-mounted.PNG)<br>
This project is a multi button RGB scene cotroller that fits a decora faceplate.  This initial project built on previous projects after digiblur suggested some ideas.  Using my already built template for creating devices that fit into a decora faceplate I set out to create thiis open hardware.  I have plans to create a few different version but I figure I would start with this 3 button version to prove the concept and built off of.

Thanks to digiblur and all the members of the projects-and-shares channel on his discord server for suggestions, help and inspiration. <br>

<br>
For a prebuilt controller or just the bare circuit board, visit my store at https://logixdiy.com/ and select board only for a bare board.<br>
<br>
I have included some basic esphome yaml for this switch. <br>
<br>
Tasmota Template and instructions <br>

For the ESP-12F version here is the template<br>

{"NAME":"Logix3","GPIO":[1,1,1,1,32,33,1,1,1376,34,1312,1,1,1],"FLAG":0,"BASE":18} <br>

For the ESP-C3-12F version use the one bellow as the pinout are different <br>

{"NAME":"Logix3-C3","GPIO":[1,1,1,1312,1376,32,0,1,1,1,1,0,0,0,0,0,0,0,34,33,1,1],"FLAG":0,"BASE":1} <br>
<br>
For the ESP-C3-12F 6 Button version with PIR and Temperature use the one bellow as the pinout are different <br>
{"NAME":"Logix6-C3","GPIO":[1,1,35,1376,32,166,34,33,1,1,36,0,0,0,0,0,0,0,1312,37,1,1],"FLAG":0,"BASE":1}
<br>
Here is a list of options I have configured on my device<br>
<br>
Led<x>	#RRGGBB = set hex color value where <x> is the pixel number of the LED. A blank-delimited list of colors sets multiple successive pixels. <br>
<br>
SetOption1 1 - turn off multi press to prevent accidental long press reset<br>
<br>
SetOption8 1 -	Show temperature in (0= Celsius (default) 1 = Fahrenheit)<br>
 <br>
SetOption73	1 - Detach buttons from relays and send multi-press and hold MQTT messages instead (0 = disable (default) 1 = enable) <br>
<br>
SetOption65	1 - Device recovery using fast power cycle detection (0 = enabled (default) 1 = disabled)<br>
<br>
TempOffset XX - where XX is a number from -12.6..12.6 as these dallas temp sensors aren't known for their accuracy<br>
 3D Printing<br>
 <br>
 <a href="https://www.buymeacoffee.com/logixpcbM" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a> <br>
 
 Print the back cover in the color of your choice<br>
 Print 3 buttons in clear PLA (white works in a pinch)<br>
 Print the Decora face in white (or whatever you like)<br>
 Print the Light Blocker in black or a dark color<br>
 <br>
 ![GitHub Logo](https://github.com/logichousepcb/Multi-Button-WS2812-RGB-esp8266-Decora/blob/main/3button_model.PNG)<br>
 
 <br>

 

 
 
