# Pr_1_PD_RafaelEMoncayo

## Codigo de la práctica:

#include <Arduino.h>
#define LED 18

void setup() {

    Serial.begin(115200);
    pinMode(LED,OUTPUT);
    
}

void loop() {

    delay(500);
    Serial.println("ON");
    digitalWrite(LED,HIGH);
    delay(500);
    Serial.println("OFF");
    digitalWrite(LED,LOW);
    
}

## Diagrama de flujos:

```mermaid
graph LR
  Inicio-->Delay500ms;
  Delay500ms-->LED_ON;
  LED_ON-->Delay500ms_2;
  Delay500ms_2-->LED_off;
  LED_off-->Delay500ms;
```
  
 
  
