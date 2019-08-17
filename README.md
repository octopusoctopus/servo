# servo
빙글빙글
```cpp
#include<Servo.h>
Servo myservo;

void setup() {
  // put your setup code here, to run once:

myservo.attach(9);

}

void loop() {
 int angle;
 for(angle=0 ; angle<180; angle=angle+10){
  myservo.write(angle);
  delay(30);
 }
 for(angle=180 ; angle>0; angle=angle-10){
  myservo.write(angle);
  delay(30);
 }
}
