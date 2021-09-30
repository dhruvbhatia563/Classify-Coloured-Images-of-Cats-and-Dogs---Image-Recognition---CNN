# Classify-Coloured-Images-of-Cats-and-Dogs---Image-Recognition---CNN
-----------------------------------------------------------------------
To build a model to classify 1000 images of cats and dogs. Dataset containing 4000 pictures of cats and dogs (2000 cats, 2000 dogs). We will use 2000 pictures for training, 1000 for validation, and finally 1000 for testing
-----------------------------------------------------------------------
-----------------------------------------------------------------------
Deatails of project:
------------------------------------------------------------------------
     - Binary Classification Problem. Either image is of Cat or of a Dog. Hence 2 classes.
     - Colored Images. Hence 3 channels --> RGB
     - No standard dimension of all the images
     - Dataset of 4000 images:
         - Train: 2000 images
         - Validation: 1000 images
         - Test: 1000 images
 -----------------------------------------------------------------------
Process of the project:
 -----------------------------------------------------------------------
     - CNN Model with 4 convolutional layers, paid with pooling layers
     - Introducing data augmentation, a process of creating artifical images using the original dataset. Using various transformation techniques: Linear, Rotations, Shear, 
       Zooming In and Out etc...
     - Use pre-learned architectures to classify images, Transfer Learning
-----------------------------------------------------------------------
-----------------------------------------------------------------------
![image](https://user-images.githubusercontent.com/68370376/135506132-2ad45d54-4ecf-458b-90d4-aa63b9b1dee6.png)

![image](https://user-images.githubusercontent.com/68370376/135506164-f60099a1-8043-4fa7-a96e-a7cacd58dd29.png)

![image](https://user-images.githubusercontent.com/68370376/135506209-205575ea-58b1-4ba2-b4e1-3288fc6c1252.png)
-----------------------------------------------------------------------
Simple CNN Structure
-----------------------------------------------------------------------
![image](https://user-images.githubusercontent.com/68370376/135506324-4644c3b0-2280-43b7-8e60-4a80862d475e.png)
![image](https://user-images.githubusercontent.com/68370376/135506365-59d7ebcb-2245-479b-bc49-6988e9223fcc.png)

Observation : there is a large difference between training_acc and validation_acc, val_acc oscilating around 73-74%, train_acc oscilating around 92-93% and increasing with each epoch, graph shows there is an Overfitting in the model becuase with each epoch train_Acc is increasing but not able to increase the val_acc. To overcome overfitting --> will be creating dummy data, will modify exsisting data into different forms by applying zoom,shear,rotation etc. Aim know to increase validation accuracy and reduce overfitting.

Data Augmentation :

![image](https://user-images.githubusercontent.com/68370376/135506701-db5b96b2-ed22-4289-b48c-635cb8a9e588.png)
![image](https://user-images.githubusercontent.com/68370376/135506769-8f62ea65-b3d1-4450-aefd-c0894a9ac9ac.png)

Transfer Learning : VGG16Net

![image](https://user-images.githubusercontent.com/68370376/135506824-a50f3414-8f61-43a5-b65d-6be6f0939ba6.png)
![image](https://user-images.githubusercontent.com/68370376/135506951-76ce8b76-f6a4-48bf-8524-ebc27e35fa08.png)
![image](https://user-images.githubusercontent.com/68370376/135506981-b1fd5735-ad65-4a8c-bfa8-b9ca7aa82256.png)

After testing on test dataset :

![image](https://user-images.githubusercontent.com/68370376/135507063-f2df8c18-84d4-4302-9b90-b3940a054839.png)

Transfer Learning : InceptionResNetV2

![image](https://user-images.githubusercontent.com/68370376/135507292-f1a4febf-f1c2-4ba9-8fe0-9e187d51312d.png)

After testing on test dataset :

![image](https://user-images.githubusercontent.com/68370376/135507344-f6f0bb84-6e70-4444-807a-d45419025511.png)


