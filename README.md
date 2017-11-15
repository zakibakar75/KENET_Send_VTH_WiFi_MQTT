MQTT connection using ESP8266 Cytron WiFi Shield to Dioty MQTT broker 

This is not a library. This is my code to publish on-board voltage, DHT22 sensor reading to Dioty MQTT broker.

The hardware used here are :
1) Arduino UNO clone.
2) Cytron Technologies WiFi ESP8266 shield.
3) DHT22 Temperature & Humidity Sensor

Libraries used :
1) PubSubClient : https://github.com/knolleary/pubsubclient
2) WiFiESP : https://github.com/bportaluri/WiFiEsp

Don't use Cytron ESP8266 library (https://github.com/CytronTechnologies/CytronWiFiShield) because it won't work on MQTT connection.
Took me some time to try different libraries to make MQTT to work.

As far as the MQTT broker is concerned, initially, i used HiveMQ MQTT public broker, but since it always up and down, i decided to change to another MQTT public broker, ie Dioty.
You just need to register an account there (http://www.dioty.co) and follow my example for topic creation.
