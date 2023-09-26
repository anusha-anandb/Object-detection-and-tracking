# Object-detection-and-tracking
# MainProject


## Contributors:<br/>
Anusha Anand B<br/>
Hamsa R D<br/>
Adiba Thereen<br/>
# Project
"Real time object detection and tracking with low
compute robot using ESP32 CAM module and ESP32"

## Project Introduction
 Real-time object detection and tracking is a vast, vibrant yet inconclusive and complex
area of computer vision. Due to its increased utilization in surveillance, tracking system
used in security and many others applications have propelled researchers to continuously
devise more efficient and competitive algorithms. The ESP32 camera module was used
which can be programmed through FTDI Module. It is required to set up the arduino
IDE for the ESP32 camera module. The ESP32 camera takes sends the picture to a
remote device that is connected to the internet and analyzes the object and determines
the class of the object. The applications of real time object detection include tracking
objects, video surveillance, people counting, self-driving cars, face detection, ball tracking
in sports and many more.<br/>

-Object Detection is the process of finding and recognizing real-world object instances such as car, bike, TV, flowers, and humans out of videos.
The ESP32 CAM would stream images to system via web socket packages and then receive the image and do object detection.<br/>
-Object Tracking is to track an object over a sequence of images.
The most popular application in this area is video surveillance, to help understand the movement patterns of people with suspicious actions.<br/>
## Systems design
   
Systems design is the process of defining the architecture, modules, interfaces, and data
for a system to satisfy specified requirements. Systems design could be seen as the
application of systems theory to product development. There is some overlap with the
disciplines of systems analysis, systems architecture and systems engineering.<br/>
BLOCK DIAGRAM<br/>
![image](https://github.com/anusha-anandb/Object-detection-and-tracking/assets/145751154/1534910f-65d7-4803-9daa-857b7ec34c84)
## Hardware Requirements<br/>
1.ESP32 Camera Module<br/>
2.L298N Motor Driver Module<br/>
3.DC Motor<br/>
4.Servo motor<br/>
5.Portable Battery<br/>
6.Wheels<br/>
## Software Requirements<br/>
ESP32 AI CAMERA ON ANDROID
The ESP32 AI camera app is a software application designed to run on the ESP32 microcontroller. 
It is designed to capture and process images and video using advanced artificial intelligence techniques. 
The app is designed for use in a variety of applications, including surveillance, robotics, and drones.
![image](https://github.com/anusha-anandb/Object-detection-and-tracking/assets/145751154/619d917c-9493-497f-8611-943c1121b5c1)
## Flow of the project
-ESP32-CAM and Android Phone connect to the same wifi network. <br/>

-ESP32-CAM act as a UDP server listens on port 6868, Android Phone sends a broadcast message to address 255.255.255.255:6868 to acquire the address of the ESP32-CAM, then create a WebSocket connection to that address port 86.<br/>

-After connection is established, ESP32-CAM will stream images to Android phone, then the image processing is done there.<br/>

##  Proposed system of model
![image](https://github.com/anusha-anandb/Object-detection-and-tracking/assets/145751154/ccc5c863-d7ad-4bb2-be8b-f1448775cfd9)

## Result
Our project showed that the ESP32CAM can reliably detect and track objects in different
scenarios, such as indoor and outdoor environments, with various lighting conditions and
object sizes. We tested the system with several objects, such as laptop, cars, and pets,
and obtained high detection rates and low false positives.<br/>
To showcase our results, we captured several snapshots of the ESP32CAM’s output
when detecting and tracking objects. These snapshots show the original image with a
bounding box around the detected object and its label, as well as the corresponding
confidence score, which indicates how confident the model is in its prediction.<br/>
![image](https://github.com/anusha-anandb/Object-detection-and-tracking/assets/145751154/2e4e2c70-3896-4784-9c40-93b6f438acc5)

![image](https://github.com/anusha-anandb/Object-detection-and-tracking/assets/145751154/b3e53fc6-612c-4846-91f8-11f9d8d0f3fd)



## Literature/Industry research review
-"ESP32-CAM Based Low-Cost Real-Time Object Detection and Tracking System"
by N. N. Ali, M. A. Hossain, M. T. Islam, and M. A. R. Bhuiyan (2021). This paper
proposes a low-cost real-time object detection and tracking system based on the
ESP32-CAM module and ESP32 microcontroller. The system uses the YOLOv3
object detection algorithm and a Kalman filter-based object tracking algorithm.
The proposed system achieves real-time performance and high accuracy in object
detection and tracking tasks.<br/>
- "Object Detection and Tracking with the ESP32-CAM: A Low-Cost Solution for
Vision-Based Robotics" by Daniel Mateo, David Mayoral, and Víctor Mayoral
Vilches (2020). This paper presents a low-cost solution for object detection and
tracking in vision-based robotics using the ESP32-CAM module and ESP32 microcontroller. The system uses the Haar Cascade Classifier for object detection
and a Kalman filter-based object tracking algorithm. The proposed system achieves
good performance in object detection and tracking tasks while requiring low computational resources.<br/>


## Importance:
Tracking objects.<br/>
CCTV surveillance.<br/>
Self driving vehicles.<br/>
Face detection and face recognition.<br/>
Activity recognition.<br/>
Ball tracking.<br/>
Object recognition as image search.<br/>



## Future Study  
-To make the system fully automatic and also to overcome the above limitations,
in future, multi-view tracking can be implemented using multiple cameras. Multi
view tracking has the obvious advantage over single view tracking because of wide
coverage range with different viewing angles for the objects to be tracked.<br/>
-Object identification task with motion estimation needs to be fast enough to be
implemented for the real time system.<br/>
-Geometric properties of the image can be included in the feature and can increase
the efficiency of the object recognition system.<br/>


## References
-R. Kirpan , Pooja I. Baviskar, Shivani D. Khawase, AnjaliS. Mankar, Karishma A.Ramteke, “Object detection inrasberry pi” International Journal of Engineering Science and Computing, Volume 7, issue 3, March 2017.<br/>
- Prof. Poonam Khare, “Literature survey of various methods of object detection” International Journal of Engineering and Technology (IRJET) Volume 3, Issue 12 December 2016.<br/>
-Wei Liu , Dragomir Anguelov, Dumitru Erhan, ChristianSzegedy, Scott Reed, Cheng-Yang Fu, Alexander C. Berg “SSD: Single Shot Multi Box Detector” December 2016.<br/>
-Shaoqing Ren, Kaiming He, Ross Girshick, and Jian Sun “Faster R-CNN: Towards Real-Time Object Detection with Region Proposal Networks” January 2016.<br/>

