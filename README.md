# arduino3controlledLEDs
arduino code controlling 3 LEDs 

using 3 buttons(input) to switch on/off 3 LED light(output)
![3input3output](https://github.com/user-attachments/assets/8b2209ce-a80f-4731-b0ce-2595d5e591a1)

```cpp
// C++ code
//
int buttonState1 = 0;

int buttonState2 = 0;

int buttonState3 = 0;

void setup()
{
  pinMode(2, INPUT);
  pinMode(3, INPUT);
  pinMode(4, INPUT);
  pinMode(11, OUTPUT);
  pinMode(12, OUTPUT);
  pinMode(13, OUTPUT);
}

void loop()
{
  buttonState1 = digitalRead(2);
  buttonState2 = digitalRead(3);
  buttonState3 = digitalRead(4);
  if (buttonState1 == HIGH) {
    digitalWrite(11, HIGH);
    
  } else {
    digitalWrite(11, LOW);
     
   
  }
  if (buttonState2 == HIGH) {
    digitalWrite(12, HIGH);
    
  } else {
    digitalWrite(12, LOW);
     
   
  }
  if (buttonState3 == HIGH) {
    digitalWrite(13, HIGH);
    
  } else {
    digitalWrite(13, LOW);
     
   
  }
  delay(5); // Delay a little bit to improve simulation performance
}
```
