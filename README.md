## INTRODUCTION

In recent times, facial recognition has become the object of research worldwide. Furthermore, with the advancement of technology and the rapid development of artificial intelligence, very significant advances have been made in the field. As the Covid-19 virus spreads through physical contact, conventional recognition systems such as fingerprints or typing a password using a keyboard become hazardous. Hence, facial recognition systems are the best option at hand, as they do not require physical interaction like in the other cases. However, we lose several data points during facial recognition as in today’s times, half of people’s faces are covered with masks, which imposes a significant challenge to these systems. Therefore, there exists a need to create algorithms that recognize a person wearing a face mask and has made it necessary to implement new strategies to achieve robustness in the current systems.
 

## MATERIALS AND METHODS

### Description of the problem

Today, using a face mask is a mandatory preventive measure, and keeping the mouth, nose, and cheeks covered has now made people only recognizable by their eyes, eyebrows, and hair. This is a problem to the human eye, which tends to find similarities in several faces with similar features. This problem also affects artificial intelligence systems, as facial recognition systems are now widespread. They are used to unlock smartphones, laptops, access sensitive applications, and enter various workplaces. Current systems usually process information from the person's entire face, which is why technology must adapt to these new conditions. The same has been done to maintain the user's biosecurity and at the same time allow them to continue with the activities as naturally as possible.
The literature has shown that systems seek to identify whether people use it properly. These works have had excellent results. However, facial recognition using biosecurity material has not yet been explored. All of this motivated the present investigation, in which a detection system with an approach. A facial recognition algorithm in controlled environments, allowing personnel to be identified automatically without removing the face mask. This can be implemented as an access system to an institution or a home, but at a low cost. This is ensured by using open-source programming software and simple features that reduce computational expense. For this reason, the possibility of improving the adaptability of current facial recognition systems in the face of new circumstances has been established as a starting hypothesis.


### Data Collection

The data in this project has been collected from various sources including images found on Kaggle.

### System Development

The programming language in use is python, and the framework in use is Keras. The proposal is to design a system capable of identifying a person’s face, even if they are wearing a mask or not. The images are divided into training and testing sets with a test size of 0.20. The training data is obtained from images, while the model runs through simultaneous video input from the webcam of the user. A classification model based on the MobileNetV2 architecture and the OpenCv’s face detector is used with the aim of having a better precision and robustness, as it uses smaller models with a low latency and low parameterization power. This improves the performance of mobile models in multiple tasks and benchmarks, resulting in a better accuracy. It also retains the simplicity and does not require any special operator to classify multiple images and various detection tasks for mobile applications. Once the face of the person has been identified, in the third stage, facial recognition is carried out, for which a set of own observations is used that is built based on the faces of various people.

### Training of Facial Recognition Models

The training of the facial recognition model includes loading the face mask data set, then training the face mask classifier using Keras/Tensorflow and then serialize the face mask classifier to the disk. The data is split into testing and training sets using train_test_split from scikitlearn. This is the first stage of the project.

### Application of the Facial Recognition System

The application of the facial recognition system is the second stage of the project. It involves Loading the face mask classifier from the disk and and detecting faces from the image/video stream. From this stream, each face ROI is extracted  and the face mask classifies is apllied to each face mask ROI giving a positive (“Mask”) or negative (“No Mask”) result. This result is then shown on the screen to the user.
 

## RESULTS

![Training Loss and Accuracy Plot](https://github.com/yatin2901/facemask/blob/main/plot.png)

Figure above shows the training accuracy vs training loss graph.

![Project Implementation](https://github.com/yatin2901/facemask/blob/main/Model.png)

Image above shows the implementation of the model in real-life.
 

## FUTURE WORKS

1. This prototype system allows for the facial recognition of people with and without a mask and could be used as a low computational consumption proposal for personnel access control. 
2. It can be implemented on to a webpage or an application for publishing and public use.
3. It could also be worked upon to perform various other functions that require image processing and facial recognition, for example, it is possible to know their identity. This is if the face is within the selected database. 

## MEMBERS

1.	Yashowardhan Samdhani
2.	Daketi Yatin
3.	Harikrishnaa

## BIBLIOGRAPHY

1. https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/
2. https://www.mdpi.com/2071-1050/13/12/6900/htm
3. https://data-flair.training/blogs/face-mask-detection-with-python/
4. https://docs.opencv.org/3.4/db/d28/tutorial_cascade_classifier.html
5. https://docs.opencv.org/3.4/d5/de7/tutorial_dnn_googlenet.html

