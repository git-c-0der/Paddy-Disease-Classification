# Paddy-Disease-Classification
### Classifying the diseases in the paddy crop by using Artificial Intelligence.

In this project, we have been provided with 11,000 paddy image crop which were divided into 10 different classes 1 was normal and rest were showing 9 different types of disease commonly find in the paddy crops. Our task was to build a machine learning model which can predict on a new test image whether there is some disease in the paddy crop or it is healthy/normal.

I used transfer learning technique by using MobileNetV2 architecture model which is a 155 layers deep CNN trained on imagenet dataset. But why only MobileNetV2 not VGG16 or may be InceptionV3? Answer lies in the implementational details of the MobileNetV2 architecture this model was designed to perform on a low compute devices and less memory resources. And at last we would like to build an app out of it and provide it to the farmers so, that they can just click a picture can diagnose the conditions of their crop.

![image](https://user-images.githubusercontent.com/77848178/164979677-365ec5bd-2acf-432b-bf3f-641f259491dd.png)


The secret of of giving high accuracy even on the low compute devices lies depend upon the two things:
1. Depthwise Seperable Concolutions - To extract features with as less computations as possible.
2. Skip Connections - To restore the lost information in the above step.

![image](https://user-images.githubusercontent.com/77848178/164979645-52f8a4f5-d8de-4b2e-a918-4f6810c6aec7.png)

After this I had tried to fine tune some of the deeper layers of the network to make the model more customized for the task at hand. And this had certainly helped in improving the performance of the model.

This was a very fun and learning project for me as this was the first time I used MobileNetV2 architecture and fine tuning. Here is the [link](https://www.kaggle.com/competitions/paddy-disease-classification) for the Kaggle competion and my [notebook](https://www.kaggle.com/code/abhishek123maurya/mobilenetv2-paddy-disease-classifier). Above images are taken from google and are not mine.

Thank you! for Reading.
