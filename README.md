# COVID-19-Rule-Checker


:file_folder: *PARTS(FOLDERS) OF THIS REPOSITORY*
---
* **app.py** is the root of the web application. This python script will link all the features of web-app.
* Code for hosting the full project as a web application is implemented in **WebServer** folder.
* Code for counting the number of people entered and exited the area has been added in **ENTRY_EXIT COUNT** folder.
* Code for detecting nose and mask i.e. mask has been worn, not worn and not properly worn has been added in **MASK AND NOSE DETECTION.**
* Code for measuring the distance between 2 people is implemented which keeps a check on the social distancing rules and had been added in **distance** folder.
* **requirements.txt** contains every installed dependency of our porject.
---

## :star: *app.py*
* This is the root of our web application.This is where all the Flask application goodness will go.It contains routes of all the features along with the functionality to run them.

---
## :star: *WebServer folder*

* currently the work includes to run all the features of our project from a web application.
* static folder contains all the output gifs and images .
* templates folder contains all the html pages that are being loaded on the web application.
---

## :star: *ENTRY_EXIT COUNT folder*

* counter.py :- The file that contains the implementation logic of people counter
* people_capture.mp4 :- The input video file used to test the code 

## :hourglass: **Project Demo**

![counter](Webserver/static/counter.gif)
---
## :star: *MASK AND NOSE DETECTION*
* Initially the work includes to check whether the person is wearing the mask or not
> * So we have tried to include the other part as well in which even if the person is wearing the mask , our code will check whether the mask is worn properly or not by detecting the nose(nostrils) or if the person is using hands instead of mask.
* code_mask.py :-The file that contains the implementation logic of Mask Detection.
* haarcascade_frontalface_alt2.xml :- Pre-trained haarcascade model to detect face.
* haarcascade_mcs_nose.xml :- Pre-trained haarcascade model to detect nose.
* mask_v1.mp4 :- The input file used to check the code for the validity in the above 3 cases.
* mask_v2.mp4 :- The input file used to check the code by using hands instead of mask.
* model.h5 :- Pre-trained MobileNet-V2 model based on ImageNet Database
* Dataset Link:- [DATASET](https://drive.google.com/drive/folders/1XDte2DL2Mf_hw4NsmGst7QtYoU7sMBVG?usp=sharing)

## :hourglass: **Project Demo**

![mask](Webserver/static/mask.gif)
---
## :star: *distance folder*
* it is used to find the distance between 2 persons and generated an red alarm when the people are not following the social distancing rule 
* SocialDistancingDetector.py :- The file that contains the implementation logic of checking the social distance between people.
* vtest.avi :- The input file used to check the code.
* yolo
  * coco.names :- 80 names of objects (labels) that can be detected on the image.
  * yolov3.cfg :- Configuration file with complete information about number of nodes in layers .
  * yolov3.weights:- values of neurons i.e weights already trained are stored in this file.
    * Link to weights file :- [WEIGHTS](https://drive.google.com/drive/folders/1CSY9WrDhRpyUIhncNXftyaaHo7u1NNXM?usp=sharing)
 

## :hourglass: **Project Demo**

![social distancing](Webserver/static/social-dist.gif)

