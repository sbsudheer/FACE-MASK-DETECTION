# FACE-MASK-DETECTION
checks whether people wear mask or not

INTRODUCTION

Face mask detection is the ability to quickly determine the presence of face masks in large groups of people, or inside buildings, has been an ongoing challenge. While an individual might be wearing a face mask upon entry, they might remove their mask at some point – violating a local, government or other policy.

MOTIVATION

In the present scenario due to Covid-19,Identifying those with and without a mask on can be tricky, especially as protecting the health and safety of the general public remains a concern. Human intervention alone is not able to handle this task, especially in situations like public transportation, where face masks are mandated on buses, trains and airplanes, or for college campuses which may require students and faculty wear a mask throughout campus.


The programming language used here is Python. For optimal operation, a high-processing equipment (GPU) is needed. Another of the essential requirements is to have the necessary databases in order to carry out the training and obtain the classification and recognition models. Taking into account that building the database of these databases requires a high investment of time when working with artificial intelligence and especially with convolutional neural networks.

It is proposed to design a system that is capable of identifying a person’s face, even if it is with or without a mask. For the system to work properly, it is necessary to use two databases: the first is for classifier training and consists of a large number of images of people who wear a face mask and others who do not. The second is used for training the facial recognition system, and here there are people with and without the biosafety material (face mask). The input data are obtained either from an image, or a video and the architecture used is MobileNet, with the aim of having a better precision and robustness. This project is divided into three stages

This stage focuses on finding the location and dimension of one or more faces, regardless of whether or not they wear a mask, within an image. For this, the OpenCV Deep Learning-based face detection model is used and, as a result, the region of interest (ROI) is obtained, which contains data such as the location, width, and height of the face.


This is where the classifier training is performed to detect faces with a mask and without a mask.
![image](https://user-images.githubusercontent.com/101164581/158309807-dcfe19a2-fc86-49fa-9372-b6aa921968a0.png)

For the classifier, MobileNet V2 architecture is used, as it uses smaller models with a low latency and low parameterization power. 
![image](https://user-images.githubusercontent.com/101164581/158310298-8103165e-def5-4fbd-b046-333b3b2774e1.png)

Once the face of the person has been identified, in the third stage, facial recognition is carried out, for which a set of own observations is used that is built based on the faces of various people. For the construction of the set of observations, a balance is sought in terms of gender, namely, five women and five men from whom the images are obtained
![image](https://user-images.githubusercontent.com/101164581/158310636-8c484cd1-e380-45d3-9d1e-c515f88412be.png)
Set of observations using a face mask
![image](https://user-images.githubusercontent.com/101164581/158310675-35d9bdd7-9f93-4269-9c58-b87e148ec9b5.png)
Set of observations without using a face mask.
