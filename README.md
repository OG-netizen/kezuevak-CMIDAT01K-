# Measure Humidity and Temperature with Raspberry Pi 3A and DHT22 sensor
Frequently, a lot of data is generated in projects that run around the clock. One way to store them permanently is to store the data in a local database. However, there are also some reasons that speak against it. In order to keep the measured data (for example, from a weather station) available in the future, it is also possible to avoid various online services. One of these providers is ThingSpeak. In this project we're gonna measure the humidity and temprature then log it in a cloud via an API.

## Setting up thingspeak account
Before we start, you need an account at ThingSpeak. Create an account on this link https://thingspeak.com/login if you do not have one yet. Then, create a new channel at https://thingspeak.com/channels.
![This is an image](https://thingspeak.com/assets/Signup_TSP_ML_image-3d581d644f5eb1ff9f4999fc55ad04e2530ee7f54be98323d7bb453032353750.svg)

## Setting up rasberry pi 
First you have to flash your SD card. To download the rasbian OS visit this link https://www.raspberrypi.com/software/ 
After flashing the SD card, make two new files SSH and wpa_supplicant.config , in the wpa_supplicant.config file it should be filled with this:
```
country=US # Your 2-digit country code
ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
network={
    ssid="YOUR_NETWORK_NAME"
    psk="YOUR_PASSWORD"
    key_mgmt=WPA-PSK
}


```

