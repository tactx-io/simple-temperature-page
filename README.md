# simple-temperature-page 


This is the most simplistic way to register topics at a local broker and render the values on a web page. 

It is supposed to run fullscreen in a chromium browser on the Rasbperry PI. 
In this case the websites registers for temperature values measured by an array of ds19b20 temperature sensors. The tty-mqtt-bridge forwards the measured values in JSON format to the local broker.
The project can run stand-alone and does not require internet connection. 
## Precondition
*Mosquitto up and running on the local host
*Measure the real temperature values eg. Arduino or ESP8266

## Run
Simply opent the index.html in your web browser. In order to set the MQTT broker address commend/uncommend line 96 and line 97 in index.html.
* If the client is instantiated as in line 96 the website registers at the public broker of iot.eclipse.orgon port 80
* line 96 connects the client to a MQTT broker hosted on the localhost (Mosquitto)

Tested with Chrome (Windows) and Chromium (Raspbian)
