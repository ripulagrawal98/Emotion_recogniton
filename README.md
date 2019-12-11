# Face To Text (Emotion Recognition)
The main objective of this project is to build a system that will recognize the emotions of person in the frame i.e. either image or video using his/her facial expressions.So basically the system will accept the input inthe form of image or video of the person and then using <b>Deep learning</b> model i.e. <b>Convolutional Neural Network</b> itwill output the emotion of person out of 7 classes of emotions including :
* 0- neutral
* 1- angry
* 2- disgust
* 3- fear
* 4- happy
* 5- sad
* 6- surprise

### Dataset
The dataset used is opensource dataset i.e. FER2013 challenge on Kaggle.Distribution of dataset looks like ![dataset](Data_set.JPG)

### Technologies Used:
* Python3
### Tools & Libraries used:
*  [Google Collaboratory](https://colab.research.google.com/notebooks/welcome.ipynb)
* [Keras](https://keras.io/) 
* [tensorflow](https://www.tensorflow.org/)
* Augmentor
* Open CV

### Step by Step Approach
#### Step1- Data Augmentation
* first the dataset will be loaded into the system and split the dataset according to different classes of emotions as dataset is mixed collection of all emotions
* Then apply data augmentation tothe dataset so as to increase the images for particulars emotions
<br>Run the<u> data_augmentation.ipynb</u> notebook for this step</b>

#### Step2- Data Preprocessing
In this step, convert images into numpy array,create the labels for the newly created images by data augmentation and other require processing. <br>
<b> Run the <u>data_preprocessing_step2.ipynb</u> notebook for this step</b>

#### Step3- Training model
This is the final step of our project.
* Use Keras to build the CNN architecture.
* After training of model on training set, evaluate the model on test set to check for its accuracy on the unknown dataset.

<b> Run the <u> model_.ipynb</u> notebook for the final step </b>
