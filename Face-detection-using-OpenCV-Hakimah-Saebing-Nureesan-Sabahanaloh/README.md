# FACE DETECTION
# Introduction :
 	Face detection is a computer technology being used in a variety of applications that identifies human faces in digital images. Face detection can be regarded as a specific case of object-class detection. In object-class detection, the task is to find the locations and sizes of all objects in an image that belong to a given class. Examples include upper torsos, pedestrians, and cars.
           	Face-detection algorithms focus on the detection of frontal human faces. It is analogous to image detection in which the image of a person is matched bit by bit. Image matches with the image stores in the database. 
# Before     
<p align="center">
  (https://user-images.githubusercontent.com/96815665/162872601-c1c0d806-a99b-4606-b91c-0d04842921a8.jpg)
</p>

# After
<p align="center">
(https://user-images.githubusercontent.com/96815665/162872744-a608aed3-a1cd-4889-94fe-b800e40646a6.png)
 </p>
 
# How face detection works : 
        Face detection applications use algorithms and ML to find human faces within larger images, which often incorporate other non-face objects such as landscapes, buildings and other human body parts like feet or hands. Face detection algorithms typically start by searching for human eyes -- one of the easiest features to detect. The algorithm might then attempt to detect eyebrows, the mouth, nose, nostrils and the iris. Once the algorithm concludes that it has found a facial region, it applies additional tests to confirm that it has, in fact, detected a face.
        
 # Design Solution : 
 (https://user-images.githubusercontent.com/96815665/162873171-6245372c-82fd-4b03-b802-fb20b4c70ee8.png)
 
  # Problem Statement :
           	Many parts of a certain image may not contain the useful information we need, so the goal of face detection is to display an image that can be identified as human faces and can be analyzed more easily. 

# Requirements :
OpenCV
Importing the Libraries :
CV2
Haar  Cascade
 
# Algorithm :
	Steps in Face detection :-

Importing the libraries

#Importing the picture
import cv2 as cv

Building the model
#Read the image
 img = cv.imread('smile.jpg')
 
#Haar cascade model
Face_model = cv.CascadeClassifier(face-detect-model)
 
#Change color BGR to GRAY
gray_scale = cv.cvtColor(img, cv.COLOR_BGR2GRAY)
 
#Draw a square
cv.rectangle(img, (200,200), (400,400), (255,255,0), 2) 	#RGB to BGR

https://user-images.githubusercontent.com/96815665/162874808-890ad474-6b1e-4cd0-ae69-3f0a464b192f.png

for (x,y,w,h) in faces:
#Draw a square like in the beginning.
cv.rectangle(img, (x,w), (y,h),(x+w,y+h), (255,255,0), 2) 	#RGB to BGR

(https://user-images.githubusercontent.com/96815665/162872744-a608aed3-a1cd-4889-94fe-b800e40646a6.png)

#Window at will be pop up
cv.imshow('image', img)
 
#Exit and turn off window
 cv.waitkey(0)
cv.destroyAllWindows()

# Conclusion :
Face detection is a type of computer technology used in various applications to accurately identify faces in images and in specific cases of face detection Its task is to find the location and all objects in a given class image and will focus on detecting human faces.





