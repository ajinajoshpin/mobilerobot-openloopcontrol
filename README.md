# MobileRobot-Openloopcontrol
## Aim:

To develop a python control code to move the mobilerobot along the predefined path.

## Equipments Required:
1. RoboMaster EP core
2. Python 3.7

## Procedure

## Step1:

use from robomaster import robot

## Step2:

choose the x,y,z - axis movement distance(meters)


## Step3:

choose ep_chassis.move to move straight.

## Step4:

give time.sleep() for a break.

## Step5:

give ep_chassis.drive_speed to have a circular movement

## Program
```python
from robomaster import robot
import time
from robomaster import camera

if _name_ == '_main_':
    ep_robot = robot.Robot()
    ep_robot.initialize(conn_type="ap")

    ep_chassis = ep_robot.chassis
    ep_led = ep_robot.led
    ep_camera = ep_robot.camera

    print("Video streaming started.....")
    ep_camera.start_video_stream(display=True, resolution = camera.STREAM_360P)

    ep_chassis.move(x=2.55, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=0,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=80, xy_speed=0).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=255,b=0,effect="on")

    ep_chassis.move(x=1, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=153,b=225,effect="on")

    ep_chassis.move(x=0, y=-1.4, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=60, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=192,g=192,b=192,effect="on")

    ep_chassis.move(x=1.5, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=45, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=225,g=225,b=0,effect="on")

    ep_chassis.move(x=1.45, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=225,b=225,effect="on")

    ep_chassis.move(x=0, y=0, z=3, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=153,g=153,b=225,effect="on")

    ep_chassis.move(x=0, y=-2.1, z=0, xy_speed=1.2).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=0,b=128,effect="on")

    ep_chassis.move(x=0, y=0, z=170, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=0,g=225,b=0,effect="on")

    ep_chassis.move(x=0.6, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=255,g=255,b=0,effect="on")

    ep_chassis.move(x=0, y=0, z=0, xy_speed=1.5).wait_for_completed()
    ep_led.set_led(comp = "all",r=51,g=51,b=51,effect="on")

    time.sleep(4)
    ep_camera.stop_video_stream()
    print("Stopped video streaming.....")

    ep_robot.close()
```

## MobileRobot Movement Image:

![WhatsApp Image 2023-12-28 at 10 28 48_845e1cfe](https://github.com/ajinajoshpin/mobilerobot-openloopcontrol/assets/148514578/6f05f4a2-aed8-414e-8e67-abed95c500c4)

![WhatsApp Image 2023-12-28 at 10 28 48_231f6301](https://github.com/ajinajoshpin/mobilerobot-openloopcontrol/assets/148514578/bcba45bd-48fe-4776-96cd-ae4acba78d0b)

![WhatsApp Image 2023-12-28 at 10 28 48_338be082](https://github.com/ajinajoshpin/mobilerobot-openloopcontrol/assets/148514578/a27c854b-0ec6-4c5a-a970-07a3045914ba)

![WhatsApp Image 2023-12-28 at 10 28 48_d078f926](https://github.com/ajinajoshpin/mobilerobot-openloopcontrol/assets/148514578/5cc724fc-9672-4630-9449-49b83be17f47)

![WhatsApp Image 2023-12-28 at 10 28 48_d2d2ccab](https://github.com/ajinajoshpin/mobilerobot-openloopcontrol/assets/148514578/43df762c-18f9-4f38-bc53-e01f73c2df60)


<br/>
<br/>
<br/>
<br/>

## MobileRobot Movement Video:


https://youtube.com/shorts/fH1QrrpZba4?feature=share

<br/>
<br/>
<br/>
<br/>

## Result:
Thus the python program code is developed to move the mobilerobot in the predefined path.


```
Mobile Robotics Laboratory
Department of Artificial Intelligence and Data Science/ Machine Learning
Saveetha Engineering College
```
