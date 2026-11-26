# EXP-4-Interfacing-Analog-Output-With-Development-Board-And-Servo-Motor

## Aim:

To interface a servo motor with an Arduino Uno development board and control its angular position using analog output signals.

## Algorithm:

1. Start the program and include the Servo library.
2. Create a servo motor object and attach it to digital pin 9.
3. Set the servo motor angle to 45° and wait for 1 second.
4. Change the servo angle to 90°, 135°, and 180° with a 1-second delay at each position.
5. Repeat the process continuously to rotate the servo motor between different angles.
6. Observe the servo motor movement and verify the angular positions.

## Procedure:

1. Open Tinkercad Circuits and create a new circuit.
2. Place an Arduino Uno and a servo motor in the workspace.
3. Connect the servo motor's signal wire to digital pin 9 of the Arduino.
4. Connect the power wire (VCC) to the 5V pin and the ground wire (GND) to the GND pin.
5. Include the Servo library and write the Arduino program to control the motor angles.
6. Upload the code and start the simulation.
7. Observe the servo motor rotating to 45°, 90°, 135°, and 180° with a 1-second delay at each position.

## Code:

~~~C++
#include <Servo.h>

Servo myservo; 
               

void setup()
{
  myservo.attach(9);
}

void loop()
{
  myservo.write(45);
  delay(1000); 
  myservo.write(90);
  delay(1000);
  myservo.write(135);
  delay(1000);
  myservo.write(180); 
  delay(1000);
}
~~~

## Output:

<img width="1107" height="695" alt="WhatsApp Image 2026-11-20 at 8 51 27 AM" src="https://github.com/user-attachments/assets/f035ff63-ecab-46ec-a895-9d19fd3b0687" />

<img width="1918" height="823" alt="image" src="https://github.com/user-attachments/assets/69a96f23-feea-4bc5-8ef9-3df9eef92887" />

## Result:

Thus, the servo motor was successfully interfaced with the Arduino Uno development board, and its angular position was controlled at 45°, 90°, 135°, and 180° using the Servo library.
