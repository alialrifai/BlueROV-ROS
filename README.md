# BlueROV-ROS
Senior Desing Project BlueROV2

We plan to run the blueROV using ROS with mavros. The only thing is that we need direct control of the thrusters. Mavros and Ardusub do not allow for that. With mavros we can only send commands to the ROV with the rcin/override topic. mavros link: http://wiki.ros.org/mavros
However in ardusub rcin is linked to the pitch, roll, yaw, forward and lateral of the vehicle as seen here https://www.ardusub.com/operators-manual/rc-input-and-output.html
For the plan for Ardusub we are going to directly link rcin to rcout. rcout it the pwm signals to the thrusters. To be able to make changes to ardusub follow the direction on this link. https://www.ardusub.com/developers/developers.html
I was messing around a few weekends ago and I have made the changes in my repository https://github.com/dbrandonk/ardupilot/tree/feature/aqua_coog_mod
But I have not tested the changes yet so I do not think that they work and they are not complete.
When you make changes to your code you can test it with SITL (Software in the loop). Example Link but there are other ways (http://ardupilot.org/dev/docs/sitl-simulator-software-in-the-loop.html). Right now we dont have a working pixhawk because the one we have broke down. But we will be ordering two more so we will be able to have a test bed for you to test your code on real hardware soon.
Let me know if you have any questions.

Branch comments (((((((((((((((((((((((((

More edits9999999999999999999999999
======

Anohter update by Ali
