# Facial-Keypoints-Detection
**The task:** The objective of this task is to predict keypoint positions on face images. Detecing facial key points is a very challenging problem.
An Example: 

<img src="https://github.com/loveleen-amar/Mini_Project-Facial_Keypoints_Detection/blob/main/1.png" width="250">  


**What type of problem:** 
This keypoint detection problem is a regression problem since we are predicting the coordinates for the landmarks on the face which are real numbers. Detection of facial keypoints is very useful for a number of tasks like facial recognition, detection etc. The keypoints selected in this code uses 15 keypoints representing the various coordinates on the human face. 

**Dataset:** 
The dataset for this problem was downloaded from Kaggle. In the space of pixel indices, each anticipated keypoint is defined as a (x,y) real-valued pair. The following components of the face are represented by 15 keypoints. The input picture is a list of pixels (sorted by row) stored as numbers in the final field of the data files (0,255). The pictures have a resolution of 96x96 pixels.

**Model:** 
I used Convolutional Neural Network for this problem. The model was trained on a set of approx 1700 images and around 300 images were taken for validation purposes. 
The images were grayscale and had the shape 96 X 96.The images were grayscale and had the shape 96 X 96. The network architecture is shown below.


<img src="https://github.com/loveleen-amar/Mini_Project-Facial_Keypoints_Detection/blob/main/2.JPG" width="450">  

**Hyperparameter:**
Epochs= 60
batchsize= 32
**Optimizer=** ADAM
**loss=** Mean squared error
**Eval metrics=** Accuracy

**Reason for using this algorithm:**
Convolutional Neural Networks (CNN) are used in a variety of applications. It is, without a doubt, the most widely used deep learning architecture. CNN has become the go-to model for every image-related issue. They outperform the competitors in terms of accuracy. The major benefit of CNN over its predecessors is that it identifies important features without the need for human intervention.CNN is computationally efficient. It performs parameter sharing and employs specific convolution and pooling methods. Thus I chose CNN baseline architecture to solve this problem of Facial keypoints detection.

**Results:** 
85% train accuracy, 77% validation accuracy & 2.9% loss. (Score on Kaggle- 2.5 RMSE)


