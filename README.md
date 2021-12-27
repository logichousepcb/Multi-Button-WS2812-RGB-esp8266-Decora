# Multi-Button-WS2812-RGB-esp8266-Decora
Multi Button WS2812 RGB esp8266 Decora <br>
![GitHub Logo](https://github.com/logichousepcb/Logix_Multifunction/blob/main/LH2_0_Rack_Mount.PNG)<br>
This project is a multi button RGB scene cotroller that fits a decora faceplate.  This initial project built on previous projects after digiblur suggested some ideas.  Using my already built template for creating devices that fit into a decora faceplate I set out to create thiis open hardware.  I have plans to create a few different version but I figure I would start with this 3 button version to prove the concept and built off of.

Thanks to digiblur and all the members of the projects-and-shares channel on his discord server for suggestions, help and inspiration. <br>
<br>
Find the schematic and pcb at https://oshwlab.com/mdegenaa <br>
<br>

I have included some basic esphome yaml for this switch. <br>
<br>
Tasmota Template and instructions <br>

{"NAME":"Logix3","GPIO":[1,1,1,1,34,33,1,1,1376,32,1312,1,1,1],"FLAG":0,"BASE":18} <br>
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


 

 
 
