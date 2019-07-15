# Description
Computer animated agents and robots bring new dimension in human computer interaction which makes it vital as how computers can affect our social life in day-to-day activities. Face to face communication is a real-time process operating at a a time scale in the order of milliseconds. The level of uncertainty at this time scale is considerable, making it necessary for humans and machines to rely on sensory rich perceptual primitives rather than slow symbolic inference processes.

In this project we are presenting the real time facial expression recognition of seven most basic human expressions: ANGER, DISGUST, FEAR, HAPPY, NEUTRAL SAD, SURPRISE.

This model can be used for prediction of expressions of both still images and real time video. However, in both the cases we have to provide image to the model. In case of real time video the image should be taken at any point in time and feed it to the model for prediction of expression. The system automatically detects face using HAAR cascade then its crops it and resize the image to a specific size and give it to the model for prediction. The model will generate seven probability values corresponding to seven expressions. The highest probability value to the corresponding expression will be the predicted expression for that image.

# Business Problem
However, our goal here is to predict the human expressions, but we have trained our model on both human and animated images. Since, we had only approx 1500 human images which are very less to make a good model, so we took approximately 9000 animated images and leverage those animated images for training the model and ultimately do the prediction of expressions on human images.

For better prediction we have decided to keep the size of each image 350*350.

For any image our goal is to predict the expression of the face in that image out of seven basic human expression

# Problem Statement
CLASSIFY THE EXPRESSION OF FACE IN IMAGE OUT OF SEVEN BASIC HUMAN EXPRESSION

# Source Data
We have downloaded data from 4 different sources.

 - Human Images Source-1: http://www.consortium.ri.cmu.edu/ckagree/
 - Human Images Source-2: http://app.visgraf.impa.br/database/faces/
 - Human Images Source-3: http://www.kasrl.org/jaffe.html
 - Animated Images Source: https://grail.cs.washington.edu/projects/deepexpr/ferg-db.html

# Real-World Business Objective & Constraints
Low-latency is required.
Interpretability is important for still images but not in real time. For still images, probability of predicted expressions can be given.
Errors are not costly.

# How to Run the Model
After downloading data from the aforementioned sources you have to structure the data into separate folders corresponding to the seven class labels. Then you can use the code in the file "FacialExpressionRecognition.ipynb" to train the model. You can add or delete layers in MLP part of the model based on your data and results. Don't forget to save your model after each epoch. Then for real time prediction you can run the file "Real_Time_Prediction.ipynb".

# Prerequisites
You need to have installed following softwares and libraries in your machine before running this project.

 - Python 3
 - Anaconda: It will install ipython notebook and most of the libraries which are needed like sklearn, pandas, seaborn, matplotlib, numpy, PIL.
 - OpenCV
 - keras
# Installing
 - Python 3: https://www.python.org/downloads/
 - Anaconda: https://www.anaconda.com/download/
 - OpenCV: pip install opencv-python
 - Keras: pip install keras
 # Built With
 - ipython-notebook - Python Text Editor
 - OpenCV - It is used for processing images
 - Keras - Deep Learning Library
 - Sklearn: It is a Machine Learning library but here it is used just to calculate accuracy and confusion matrix.
