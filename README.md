# Smart Home
Graduation Project using Arduino

Controlling multiple appliances through Google assistant from anywhere in the world

Monitoring sensor's data from anywhere in the world

Automating home appliances(lights,fans,etc) whenever we enter into the room using motion sensor

Getting notifications on our phone whenever anyone secretly enters in our room or lab.

IoT based Air quality monitoring device by attaching dust sensor,Co2 sensor,Temperature,humidity etc

# Items which are used: 
1. ESP8266 12e (NODEMCU)

2. 5V Relay

3. 1n4007 Diode

4. BC547 transistor

5. 330ohm resistors

6. 16 channel analog multiplexer module

7. PIR motion sensor 

8. MQ35  sensor

9. Sound Sensor

10. Light Sensor

11. DHT11 Temperature and Humidity sensor

12. 9V Power supply

# Description:
First some things need to be clear:

IFTTT: IFTTT stands for "if this then that", it is platform to merge to services by making an applet. basically IFTTT needs to have one condition as "input" and one action as "output" so if the condition is satisfies then the action will be performed...

for example: If google assistant listens to "turn on fan" it will perform an action to send data 1 to fan feed of Adafruit MQTT broker

MQTT : MQTT stands for "Message Queue Telemetry Transport" which is two magor components: broker and client, broker is regarded as a server and a clinet is nothing but micro-controller port

for example: Let's have 3 clients A,B and C, client B and C are subscribed to topic "temperature" on the MQTT broker so now the client A publishes the data on the temperature for example 20 so the same data is sent to everyone who is subscribed to temperature topic, the broker can be a local broker works in the range of WiFi router or can be cloud base broker that can work anywhere in the world, in this case the broker works as a cloud.

The Esp8266 works as client in the MQTT so any change in the data will be recived by the board 

AdaFruit : it is the MQTT dashboard 
