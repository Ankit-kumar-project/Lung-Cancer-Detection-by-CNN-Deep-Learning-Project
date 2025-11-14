<pre>
# Topic : Lung Cancer detection model using CNN 

# Description:
Lung-Cancer-Detection-by-CNN-Deep-Learning-Project
Computer Vision is one of the applications of deep neural networks and one such use case is in predicting the presence of cancerous cells, to build a classifier using Convolution Neural Network which can classify normal lung tissues from cancerous tissues.

# Folder Structure
|
|-LungCancerByCNN.ipynb
|-CNN_Project.pptx
|-README.md

## API Dataset from kaggle

"https://www.kaggle.com/datasets/hamdallak/the-iqothnccd-lung-cancer-dataset/data"

Dataset/
├── Benign cases/
├── Malignant cases/
└── Normal cases/

Each directory consist of CT images belong to there respective classes

## Workflow

### 1. Preprocessing
- Read images from each folder  
- Resize them to a fixed size(128*128) and convert into numpy array
- Normalize pixel values  
- Convert image into Grey scale for better performance.
- Encode labels and split into train and test sets  

### 2. CNN Model
A standard CNN architecture is used with:
- Convolution layers  
- MaxPooling layers  
- Flatten layer  
- Dense layers  
- Relu function use as internal activation function
- Softmax output layer  

Model compiled with:
- Loss: sparse_categorical_crossentropy  
- Optimizer: adam  
- Metric: accuracy  

### 3. Training
The model is trained for 30 epochs. Training and validation accuracy is monitored to track learning progress.
It's Accuracy score is 0.9994 with 0.0027 loss function


### 5. Saving the Model
After training, the model is saved for future deployment.



</pre>