# Measure Humidity and Temperature with Raspberry Pi 3A and DHT22 sensor
Frequently, a lot of data is generated in projects that run around the clock. One way to store them permanently is to store the data in a local database. However, there are also some reasons that speak against it. In order to keep the measured data (for example, from a weather station) available in the future, it is also possible to avoid various online services. One of these providers is ThingSpeak. In this project we're gonna measure the humidity and temprature then log it in a cloud via an API.

## Setting up thingspeak account
Before we start, you need an account at ThingSpeak. Create an account on this link https://thingspeak.com/login if you do not have one yet. Then, create a new channel at https://thingspeak.com/channels.
