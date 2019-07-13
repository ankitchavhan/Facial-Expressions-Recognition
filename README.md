# Facial-Expressions-Recognition

Basically, this is the high level view of what i am going to do in making this recognition task.

        Input Image ----> Face Detection ----> Feature Extraction ----> Classification ----> Output

So, in the first step i am going to take the input image using webcam and detect the face using opencv in python and try to get the features from the obtained face image using CNN concept of deep learning and for classification task, the extracted features are given to the classifier like Logistic Regression, SVM etc and classifier predicts the recognized expression as output.


## Getting Started

  To solve this problem, we need a large database of different faces depicting different emotions. For that, you can download the CK+ database (http://www.consortium.ri.cmu.edu/ckagree/) or you can make your own but make sure that dataset is big or diverse so you can also take help of your friends in making it diverse ….;-) or u can find another one.
  
Here, i am using my own database with thousand of images and organized them in a folder named dataset within there are 7 different subfolders (that are going to be your 7 classes) named anger, disgust, fear, happy, neutral, sad, surprise which contains the images of particular expression.
To do this task, we need to find the face on each image, convert it to grayscale, crop it and save the image to the dataset. We can use a HAAR filter from OpenCV to automate face finding.
 Ref:- [http://opencv-python-tutroals.readthedocs.io/en/latest/py_tutorials/py_objdetect/py_face_detection/py_face_detection.html]
