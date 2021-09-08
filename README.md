# Hand Gesture Volume Controller
![image](https://user-images.githubusercontent.com/86593289/128878239-67a81275-d3b9-44cd-8ccf-64d75eb5fa89.png)

Using this you can control your PC/Laptop volume by Hand Gestures (pinch-in, pinch-out).
# Code
Firstly I have created a Module "HandTrackingModule.py", this file contains the code which detects our hand, in this file I have created functions for specific tasks in a "class handDetector()". 
Short description of functions are - 
* findHands() - This function detect hands and show landmarks of your hand and it return image in RGB.
* findPosition() - This function finds the position of particular landmark of your hand and it returns a list containing *id_of_that_landmark, x_position_of_that_landmark, y_position_of_that_landmark*.
* fingersUp() - This function check wheather your particular finger is up or not and it return a list containing values 0 (if finger is down) ans 1 (if finger is up). i.e. \[0,0,0,0,0] if all the 5 fingers are down and \[1,1,1,1,1] if all the fingers are up.


Then another file is "GestureVolumeController", this file uses that HandTrackingModule and contains the code which calculate distance between thumb and first-finger and by pinching-in(decrease distance) and pinching-out(increase distance) you can decrease and increase volume of your PC/Laptop. 


This project is created in Python-3 language using OpenCV, Mediapipe and Pycaw libraries.

# Installation
To run this file you need to install some PYTHON modules, open your CMD and type following commands-

* pip install mediapipe
* pip install opencv-python
* pip install numpy
* pip install pycaw

