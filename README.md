# RealEngFinalProject




## Robot Arm Planning

## Design Goal

The goal of our robot arm is to be able to pick up an object and place it in a diffrent location based on the person controlling it. We plan to make our robot arm open and close with a screw like sytem powered by dc motors and double A batteries. We plan to 3D print our robot arm and make the wiring out of the materials provided by the engineering lab, which include 3 DC motors, male jumper cabels, Ardiuno, breadboard, other wiring related objects and 3d printed part's. The design is relativily simple with the main motion of the arm opening and closing and going up and down working on the screw sytem, and the arm moving right to left on a pully sytem connected to a frame. The code will make it so we have buttons that will control open close, up down, and side to side. Our goal is to make it work like a arcade claw machine but with buttons.


## Scope

Step 1 - TOP DOWN DESIGN METHOD
• All of the Parts are modeled in the same
Part Studio
• Geometric and dimensional data is shared
between parts
• Design intent is consistent across multiple
parts
• Multiple parts can be edited at the same
time

Step 2 - Create the Sketch of the Base

Step 3 - Create the Sketch of the Gripper
Extrude the Base and the Gripper
Create Actuator Hole in the Base

Step 4 - Create the Swing Arm

Step 5 - Create the Actuator

Step 6 - Create the Control Arm

Step 7 - Assemble the Gripper Parts
Using Mates

Step 8 - Animate the Gripper Action

This design is robot arm the goal of our project we are working on pick and- place robbitic arm picking up objects from one location and placing them in another.




## Schedule
Week 1 (January 2-5)------------: Continue designs, drawings, initial CAD design .

Week 2 (January 8-12)-----------: Design and CAD ,code for motor.

Week 3 (January 15-19)----------: Continue CAD , Continue code for motor.

Week 4 (January 22-26)----------: Start assembly for onshape parts, motor, Continue coding for motor.

Week 5 (January 29-February 2)--: Continue  for preject, Continue coding.

Week 6 (February 5-9)-----------: Continue assembly for preject, Continue code for motor (work on notebook).

Week 7 (February 12-16)---------: Continue assembly for preject, Continue code for motor (work on notebook).

Week 8 (February 19-23)---------: Continue assembly for preject, Continue code for motor (drwaings of preject).

Week 9 (February 26-March 1)----: Continue assembly for preject, Continue code for motor (drwaings of preject).

Week 10 (March 4-8)-------------: Improve design for motors, strengthen weak points. Add walls and exit point if possible.

Week 11 (March 11-15)-----------: Improve design for motors, strengthen weak points. Add walls and exit point if possible.

Week 12 (March 18-22)-----------: If walls and exit point not added already, add. Perform kinetics tests for the pico, improve cushioning and structure.

Week 13 (March 25-29)-----------: Improve design for motors, strengthen weak points. Add walls and exit point if possible.

Week 15 (April 8-12)------------: Improve drawing and others.

Week 16 (April 15-19)-----------: work on issues for onshape and code.

Week 17 (April 22-26)-----------: Finish with Onshape and code .

Week 18 (April 29-May 3)--------: Finish printing get videos and photos .

week 19 ( May 3, 18)---------: Finish code and onshape and print also assembly.

Week 20 (May 20-30)--------------: Finish documentation.

Week 21 (May 29-31)-------------: Finish documentation.

## Sketches
![317787767-896c4c5b-4e64-4d1d-b46a-123b3a68b62f](https://github.com/IANDORA87/engineer3/assets/143534987/b466ac69-1554-4689-bd5f-14cb3b67ba49)
![317787933-18be97c7-8c6a-47fe-aa0d-1148cbb50759](https://github.com/IANDORA87/engineer3/assets/143534987/ddc19f84-b8ef-4aa5-ac76-42600269a7d9)

## Pseudocode

```
python
import time
import board
from analogio import AnalogIn
import pwmio
from digitalio import DigitalInOut

#pins
potentiometerpin = AnalogIn(board.A0)
motorpin = pwmio.PWMOut(board.D7)

while True:
    print(button.value)
    if button.value:  # Button is pressed (remember, we're assuming it's pull-down)
        print("btn1 pressed \t")
        print(current_angle)
        current_angle = current_angle + 10
        current_angle = max(0, min(360, current_angle))
    time.sleep(0.05)  # Small delay to avoid excessive checking

    print(button2.value)
    if button2.value:  # Button is pressed (remember, we're assuming it's pull-down)
        print("btn2 pressed \t")
        print(current_angle)
        current_angle = current_angle - 10
        current_angle = max(0, min(360, current_angle))
        print(potentiometerpin.value)
    time.sleep(0.1)
    motorpin.duty_cycle = potentiometerpin.value

    time.sleep(0.05)  # Small delay to avoid excessive checking
```



## Evidence
<img width="807" alt="MotorControlWiring" src="https://github.com/JoshBricker30/RealEngFinalProject/assets/143528213/792b9a85-455a-4456-ade9-b6b7b5da4822">
    ![pic 1](https://github.com/JoshBricker30/RealEngFinalProject/assets/143528213/f8d4a1ed-c115-43d5-a261-8eea060b5e3d)
    ![pic 3](https://github.com/JoshBricker30/RealEngFinalProject/assets/143528213/ac3477c1-2166-4b6e-8332-4088ab2970cf)
    ![pic 4](https://github.com/JoshBricker30/RealEngFinalProject/assets/143528213/69f4798e-6c1a-48cb-b1ea-607969eaf213)
    ![pic2](https://github.com/JoshBricker30/RealEngFinalProject/assets/143528213/3e35c57a-1387-4556-b868-c1df632bbc28)


## Links

https://docs.google.com/spreadsheets/d/137HGSNZTTR_IkVGg8gcBn5OXVTHr438-3fES2nv-ZDA/edit#gid=0
[https://cvilleschools.onshape.com/documents/45a013841ca662a47591e1ff/w/3954e8a8cc011ba53df39d5e/e/5a5578e3d4a967c2c8b67bae?renderMode=0&uiState=66589d360f48217e21d14c89
](https://cvilleschools.onshape.com/documents/45a013841ca662a47591e1ff/w/3954e8a8cc011ba53df39d5e/e/5a5578e3d4a967c2c8b67bae?renderMode=0&uiState=6658b26a1f003d73b38d4b02)
## Bill of materials

![image](https://github.com/IANDORA87/engineer3/assets/143534987/e02d3528-53e1-48ed-b444-978b54b90621)


## Risk Mitigation

First risk mitigation that i face with with


## Reflection

What went wrong / was challenging, how'd you figure it out, and what did you learn from that experience? Your goal for the reflection is to pass on knowledge that will make this assignment better or easier for the next person. Think about your audience for this one, which may be "future you" (when you realize you need some of this code in three months), me, or your college admission committee!



On Thu, May 30, 2024 at 11:40 AM Josh Bricker <jbricke30@charlottesvilleschools.org> wrote:
image.png
