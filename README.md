# COVID-19-Detector
Detecting COVID-19 with the help of X-RAY Images (#Convolutional Neural Network #Deep Learning)

#AIM : Rapid Evalution of Covid Samples                                                                                                                                                                   
In the recent times COVID-19 has become a burning topic all over the world. It had affected all of us in many aspects of our lives.
Due to it's rigorous spread ,many of us are afraid of it, that whether they are attacked by it or not , so we go for testing but it takes certain time to get the result .
so , here comes the importance of this COVID-19 Detector since rapid evalution is very important to stop spread of the virus.

So, I had built a Deeping Learning Model with help of Convolutional Neural Network

Coming to the details of the project:
I have a attached a file named as : COVID-19 Detector - Colaboratory ,(I had built this model on Googl colab ,so attached the same file here)
It consists of
 * URL for the dataset (run it and download the dataset ,then unzip it)
 * complete code for building the model along with the comments for explaination
 * training of my model on the specified dataset
 * also included the confusion matrix for better analysis of the model

About the Model:                                                                                                                                                                      
Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 222, 222, 32)      896       
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 220, 220, 64)      18496     
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 110, 110, 64)      0         
_________________________________________________________________
dropout (Dropout)            (None, 110, 110, 64)      0         
_________________________________________________________________
conv2d_2 (Conv2D)            (None, 108, 108, 64)      36928     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 54, 54, 64)        0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 54, 54, 64)        0         
_________________________________________________________________
conv2d_3 (Conv2D)            (None, 52, 52, 128)       73856     
_________________________________________________________________
max_pooling2d_2 (MaxPooling2 (None, 26, 26, 128)       0         
_________________________________________________________________
dropout_2 (Dropout)          (None, 26, 26, 128)       0         
_________________________________________________________________
flatten (Flatten)            (None, 86528)             0         
_________________________________________________________________
dense (Dense)                (None, 64)                5537856   
_________________________________________________________________
dropout_3 (Dropout)          (None, 64)                0         
_________________________________________________________________
dense_1 (Dense)              (None, 1)                 65        
=================================================================
Total params: 5,668,097
Trainable params: 5,668,097
Non-trainable params: 0


CONCLUSION :                                                                                                                                                                      
Though it is not 100% correct predictor but with help of rigorous training of the model on large dataset and also with the help of CT scan images we could certainly reach to some optimal level of prediction.

