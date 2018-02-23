
IoT using KENET WiFi 

1) Protocol used : MQTT
2) Data Format used : JSON

This is my code to publish on-board voltage, DHT22 sensor reading to Dioty MQTT broker.  Main thing when use MQTT protocol is to make sure you are able to establish MQTT connection using your KENET WiFi (contains ESP8266 Cytron WiFi Shield) to Dioty MQTT broker.  

As far as the MQTT broker is concerned, initially, i used HiveMQ MQTT public broker, but since it always up and down, i decided to change to another MQTT public broker, ie Dioty.
You just need to register an account there (http://www.dioty.co) and follow my example for topic creation.

The hardware used here are :
1) Arduino UNO clone.
2) Cytron Technologies WiFi ESP8266 shield.
3) DHT22 Temperature & Humidity Sensor (optional)

Libraries used :
1) PubSubClient : https://github.com/knolleary/pubsubclient
2) WiFiESP : https://github.com/bportaluri/WiFiEsp
3) DHT library : https://drive.google.com/file/d/0B1paTI5fzcHodno5azFOSVVDT0E/view?usp=sharing (optional)

Please don't use Cytron ESP8266 library (https://github.com/CytronTechnologies/CytronWiFiShield) because it won't work on MQTT connection.
Took me some time to try different libraries to make MQTT to work.


