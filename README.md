# Hand Gesture Volume Controller
Using this you can control your PC/Laptop volume by Hand Gestures (pinch-in, pinch-out) created with Open-CV (Python).
# Code
Firstly I have created a Module "HandTrackingModule.py" , this file contains the code which detects our hand, in this file I have created functions for specific tasks in a "class handDetector()". 
Short description of functions are -
* findHands() - This function detect hands and show landmarks of your hand and it return image in RGB.
* findPosition() - This function finds the position of particular landmark of your hand and it returns a list containing *id_of_that_landmark, x_position_of_that_landmark, y_position_of_that_landmark*.
* fingersUp() - This function check wheather your particular finger is up or not and it return a list containing values 0 (if finger is down) ans 1 (if finger is up). i.e. \[0,0,0,0,0] if all the 5 fingers are down and \[1,1,1,1,1] if all the fingers are up.
