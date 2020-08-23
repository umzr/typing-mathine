
this is a last year project
F6 

```Material: 
arduino Pro micro HKD$35
plastic button HKD$9
plastic box: HKD15

1)
![image](https://na.cx/i/KYJBqgm.jpg)

2)
![image](https://na.cx/i/MOWfFQP.jpg)

3) CODE
https://www.arduino.cc/reference/en/language/functions/usb/keyboard/

#include "Keyboard.h"

const int Pin = 4;

int b = HIGH;   
int counter = 0;                  

void setup() {
  
  pinMode(Pin, INPUT);
  
  Keyboard.begin();
}

void loop() {
 
  int a = digitalRead(Pin);
  
  if ((a != b)
      
      && (a == HIGH)) {
    Keyboard.println("I go to school by bus "); // 你想輸入乜嘢潮文就打入去
  }

b = a;
```}

