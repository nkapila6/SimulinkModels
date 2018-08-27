# Pendulum Model  
The problem that arises here is, how we’re going to design & control the motion of the pendulum. For control, obviously we use a motor but we also refer to the motor here with a general term known as actuation.
Let us start with the designing process, there are 3 questions to ask yourself before any complex Simulink design. This will help you process and ease the confusion of implementation.
1.	The first question for any designing process is, what do we require? Asking yourself this will help you in choosing the blocks easily without any confusion.

2.	The second question would be: How will we fix the blocks? A better framed question would be: How are we going to implement the blocks chosen and in what way? What will be it’s (x,y,z) position? What will be its orientation? (mainly being the rigid transform blocks)

3.	The third question is how we are going to control the motion? Are we going to use a motor or are we going to give it some specific equation of motion or are we going to let it move freely within the space.

We have to answer the following questions (in detail compared to above)
1.	We obviously require 2 solid blocks which will make the ball and the cylindrical rod.
2.	We also require a rigid transform block to translate the ball to the end of the cylinder.
3.	The most important block which will create the motion of the rod is the revolute joint block.
4.	For motion control of the aforementioned block, we can possibly implement 2 options to choose from:
•	Actuation through the general equation of a single pendulum.
•	Actuation using a sine wave.

5.	The implementation of a control system.


