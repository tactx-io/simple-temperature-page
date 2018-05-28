# simple-temperature-page 


This is the most simplistic way to register topics at a local broker and render the values on a web page. 

It is supposed to run fullscreen in a chromium browser on the Rasbperry PI. 
In this case the websites registers for temperature values measured by an array of ds19b20 temperature sensors. The tty-mqtt-bridge forwards the measured values in JSON format to the local broker.
The project can run stand-alone and does not require internet connection. 
## Precondition
*Mosquitto up and running on the local host
*Measure the real temperature values eg. Arduino or ESP8266
