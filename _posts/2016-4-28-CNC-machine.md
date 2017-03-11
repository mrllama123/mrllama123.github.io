---
layout: post
title: CNC machine part 1
tag: [projects, CNC]
---
So i finally  decided to use my ardino for something useful and i knew i had some
old cd drives around the place so i decided to build an cnc machine, which is
something i have wanted to do for ages. this guide [here](http://www.instructables.com/id/Mini-CNC-Machine-Arduino-Based-Adafruit-Driver-Mot/) is what gave me the inspiration

So far i have token apart the cd drives which i will use the stepper motors (which control
  the movement of the lazer) to control the x and y axis i am still not sure what i will  
do for the z axis. I could either use an lazer of use an servo motor and place an pen
on the servo.
(sorry the crappy quality)

![cnc1](/images/cnc/IMG_20160427_202729.jpg)

![cnc2](/images/cnc/IMG_20160427_203727.jpg)

I also have done the soldering aspect of it as well, so creating the wires for the stepper
motors and soldering them to the motor pins, which was terrible soldering but hey it does the job.    
Then i had to buy an stepper motor controller so i could actually controll the motors which i works really well
using an old adafruit [motor driver libary](https://github.com/adafruit/Adafruit-Motor-Shield-library/) the only problem is that one of the axis is bigger than the other and is slower that the other which makes it intersting...
and my wonderfull soldering skills (to be fair there were some triky things to solder like the motor pins). So the
next stage is to put evrything together and figure out how i am going to code it.    

![cnc2](/images/cnc/IMG_20160427_224451.jpg)
