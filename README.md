# Convolutional Neural Net 

I built a Convolutional Neural Net, CNN, image classifier for cats and dogs. This project was inspired by HotDog or NotHotDog from the HBO show Silicon Valley. While I very much intend to work on HotDog or NotHotDog, the first step in completing the project was to develop a firm grasp of CNN's.

## What You Need
* computer
* python
* tensorflow
* keras
* jupyter notebook 

## Step 1 - Gather Data
You'll first want to gather your data for this excercise. The data that went into training the model was collected from [Kaggle.com](https://www.kaggle.com/c/dogs-vs-cats). Additionally, the data collected in the sampling process to determine the best features was collected from different variations in the optimization technique and architecture.

## Step 2 - CNN Architecture
For this part, it may be best to reference the jupyter notebook while you read through this section. I define the model's sequential architecture below. First, you feed the data into the first convolutional layer then a pooling layer, then another convolutional layer and another pooling layer, then a final convolutional layer and a final pooling layer. The model was then compiled and connected to the fully connected layers resulting in a prediction for cat or dog.

#### CNN Architecture
![CNN Model](https://github.com/Life-According-to-Jordan/Cat_Dog/blob/master/CNN.png)

## Step 3 - Paramters
Once the model is built and it's able to run, you may want to adjust different parts of the model. You could adjust the size of the convolutional layers, pooling layers, or fully connected layers. Additionally, you could adjust the optimization technique and dropout layers of the model.

## Step 4 - Train Model
Once the model is built and you have your parameters set, you can train the model. You'll build a trainging generator and a testing generator. My CNN was trained on a MacBook Pro with an Intel core i5 processor and the final model took a whopping 36 hours to train.

## Final Model 
My CNN performs best with Adaptive Moment Estimation, Adam. Additionally, I found that 3 convolutional layers, each with a pooling layer, and 2 fully connected layers performed the best. More to it, data augmentation allows the model to learn by distorting the images when training the model. This process allows the model to increase its accuracy from 87.5% to 91%.

#### Accuracy Score - Final Model with Data Augmentation
![Augmented Findal Model](https://github.com/Life-According-to-Jordan/Cat_Dog/blob/master/Final_graph.png)

* After 30 epochs on 20,000 training images, the model's accuracy is near 87.5%.
* After 30 epochs on 20,000 training images, with data augmentation, the model's accuracy is near 91%.


Also, huge shoutout to Siraj Raval for always keeping Data Science and Computer Science interesting. Here is his [video](https://www.youtube.com/watch?v=cAICT4Al5Ow) covering CNN's! Siraj always has a way of capturing my attention and I hope he is able to capture yours as well! 

#### Additional Resources:
* [Keras](https://keras.io/)
* [Download Tensorflow](https://www.tensorflow.org/install/)
* [Literature On The Topic](http://papers.nips.cc/book/advances-in-neural-information-processing-systems-28-2015)
