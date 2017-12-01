# DetectHeadMovement

Detect head movement in top-down or left-right direction.

##Description

Initially user's face region is detected. Points on face are tracked on the user's facial region to track the user's head movement. 
If the user moves the head in top-down direction, 
the tool displays the message on the top left corner of the windown about the gesture that is detected.

Tracking Mechanism:
```
Initially the facial region is identified with the help of Intel distributed fa. Once the facial region is identified. 
The sysmtem uses Lucas-Kanade algorithm to track the spacial feature point on the face.
Program currently tracking only one single feature point. That is the center of the facial region.

```

In order to execute the program kindly enter the following command from console:
>python path_to_DeatectHeadMovement/headNodDetection.py

## Dependencies:
1. Python 2.7
2. OpenCV 3.0
3. Face Dectection Using haarcascade_frontalface_default.xml. _File is distributed from Intel, kindly follow the license agreement before using and redistributing the file._