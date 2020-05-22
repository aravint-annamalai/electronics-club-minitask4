# DEBUGGING CONTACTLESS HANDWASH TIMER

The project can be divided into two cmponents for debugging - the sensor part and the motor part. 

We are going to use an ultrasonic sensor to detect the presence of the hand so that the washing begins. To make sure that the sensor works properly, we have to test the sensor, using the method usually used(which is, connecting it to an Arduino and running a code so that the value detected by the sensor is displayed on the serial monitor). If it works, then there won't be any problem as far as the sensor is concerned.

Then the most important part is the motor part. A servo motor is used here, which turns 180 degrees every 20sec, the ending of which will stop the water pipe. For that, the motor turns 1 degree every 111.1 millisecond. If the timing is not maintained properly, then we have to check the code, whether the instructions for the rotation of the motor is correct. 

So the debugging of this project can be done by splitting the project into two, analysing the possible bugs in each component, and integrating them back together.
