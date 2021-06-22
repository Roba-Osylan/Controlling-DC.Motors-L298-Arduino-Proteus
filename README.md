# Controlling-DC.Motors-L298-Arduino-Proteus
Through this project, two DC motors are controlled using arduino and drived using H-Bridge L298 Motor Driver. Motor drivers are widely used in robotica and they are able to control both the direction and the speed of the motor (maximum speed of 255 for the L298). The simulation tool that will be used is Proteus 8, however, TINKERCAD may be used as well. In the following section we will see how to add the Arduino and L298 libraries to Proteus.

# Adding Arduino and L298 Libraries and Models 
Please follow the instructions explained on the links
Arduino Library: https://www.youtube.com/watch?v=cJpJagAsjUE
L298 Library: https://www.youtube.com/watch?v=SmHCOFh87ok
** Note: there are many other libraries and models that you can download. **

# Circuit Implementation
1- Components
The components used are: 
-Arduino Uno.
-L298 Motor Driver.
-2xDC Motors.
-1x12V and 2x5V batteries.

2- Circuit Connection
See the figure or follow the instructions below.
![DC-Motors Circuit](https://user-images.githubusercontent.com/85955049/122925331-6688bd00-d36f-11eb-98a6-77cc3da85c1e.png)

-Connect ENA, IN1, IN2, IN3 IN4, ENB pins of the L298 with the pins 12, 9, 6, 5, 3, 2 of the Arduino respectively. 
-Connect the 12V battery to the 12V input of the L298, one 5V battery to the 5V input of the L298 and the other to the 5V pin on the Arduino. 
-Connecto one motor to the ports OUT1&OUT2, and the other to OUT3&OUT4 of the L298.
-Ground the GND input of L298 and the GROUND pin of the Arduino and the two pins under OUT2 of the L298.

#Code 
After writing the code on Arduino, export the code to a compiled binary file (HEX extention) or simply download the code uploaded in the repository with the name "DC-Motors.ino.standard.hex". Next, upload the code file to the Arduino model on Proteus.

The code is written to rotate the motors on all directions forward, backward, right and left. Finally, the motors stop and reapate the program all over again.
