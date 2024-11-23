## Flowchart IoT wireless devices with various connections

``` mermaid
flowchart LR;
 Sensor-->Gateway;
  Sensor-->Actuator;
  Gateway-->Cloud;
  Actuator-->Cloud;
  Cloud-->MobileApp;
  MobileApp-->Sensor;
  Cloud-->Actuator;
  Cloud-->Gateway;
  MobileApp-->Gateway;
  Sensor-->MobileApp;
  Gateway-->Sensor;
  Gateway-->MobileApp;
```