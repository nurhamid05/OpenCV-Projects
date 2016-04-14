# OpenCV-Projects has classification of Open/Closed eyes, based on OpenCV.

This work develop 3 stages in order to classify Open/Closed Eyes.

For each frame, let's say:

![](ScreeShots/org.png)

1. Face detection - LBP it is performed:

![](ScreeShots/face.png)

- Then changing ROI

![](ScreeShots/face_cropped.png)

- Then both eyes are located according to geometry of the face

![](ScreeShots/Eyes_Geometry.png)


- Now changing ROI for each eye
    Left Eye
![](ScreeShots/Left_Eye.png)

    Right Eye
![](ScreeShots/Right_Eye.png)

2. Eye detection - Haar it is performed (Different detector for each one), and we got:

    Left Eye
![](ScreeShots/Left_Eye_Haar.png)

    Right Eye
![](ScreeShots/Right_Eye_Haar.png)

3. Binary classification according to both eyes:

![](ScreeShots/open.png)

![](ScreeShots/closed.png)
