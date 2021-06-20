# task-one-
in this project we Motor drive design and implementation for robot arm
the project was implemented by Tinkercad program
equipments is: Arduino uno R3 , Breadboard small , and 5 Micro servo
the point is Design the electronic circuit to control 5 servo motors
first, Connect a wire frome Micro servo ground to negative point of the board
second, Connect a wire frome Micro servo power to 5V in the Arduino
Third, Connect a wire frome Micro servo signle to Digtal( PMW ) of the Arduino
Fourthly, Connect a wire frome Arduino GND to negative point of the board
fifth, We programmed a code to make all movements at (90) degrees
this code for the project
// C++ code
//
#include <Servo.h>

int poistion = 0;

int i = 0;

int j = 0;

int k = 0;

int m = 0;

int n = 0;

int o = 0;

Servo servo_9;

Servo servo_7;

Servo servo_5;

Servo servo_3;

Servo servo_1;

void setup()
{
  servo_9.attach(9, 500, 2500);

  servo_7.attach(7, 500, 2500);

  servo_5.attach(5, 500, 2500);

  servo_3.attach(3, 500, 2500);

  servo_1.attach(1, 500, 2500);

}

void loop()
{
  poistion = 1;
  for (poistion = 1; poistion <= 90; poistion += 1) {
    servo_9.write(poistion);
    delay(30); // Wait for 30 millisecond(s)
  }
  poistion = 1;
  for (poistion = 1; poistion <= 90; poistion += 1) {
    servo_7.write(poistion);
    delay(30); // Wait for 30 millisecond(s)
  }
  poistion = 1;
  for (poistion = 1; poistion <= 90; poistion += 1) {
    servo_5.write(poistion);
    delay(30); // Wait for 30 millisecond(s)
  }
  poistion = 1;
  for (poistion = 1; poistion <= 90; poistion += 1) {
    servo_3.write(poistion);
    delay(30); // Wait for 30 millisecond(s)
  }
  poistion = 1;
  for (poistion = 90; poistion <= 1; poistion += 1) {
    servo_1.write(poistion);
    delay(30); // Wait for 30 millisecond(s)
  }
}
