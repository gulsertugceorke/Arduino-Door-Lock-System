# Arduino-Door-Lock-System
In this project, we open the door by entering the password 4567 into the system via the keyped. 
Then the system counts from 5 backwards using the buzzer. After this countdown,
the door closes back and the system locks. If the wrong password is entered, the red led turns on and the buzzer sounds.
The keypad.h library has been used for keypad usage. LiquidCrystal.h is used for lcd screen usage. 
Servo.h library is used for servo motor.
int pos=0 used for LCD Connections.
myservo.attach(9) in this part servo attached.
for(pos = 180; pos>=0; pos-=5) servo motor rotates 180 degrees.
myservo.write(pos); tell servo to go to position in variable 'pos'.
delay(5); waits 15ms for the servo to reach the position.
for(pos = 0; pos <= 180; pos +=5) goes from 0 degrees to 180 degrees.
myservo.write(pos) tell servo to go to position in variable 'pos'.
