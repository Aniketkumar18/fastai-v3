# Sports Image Classifier

The aim of this project is to classify the image into "Cricket", "Football", "Golf" or "Tennis" using Convolution Nueral Network. In this image classification project I have used the transfer learning from the imagenet data.

After creating and training my model, I have deployed it as a web application on render.

Please visit the below url to test

URL: https://sports-image-classifier.onrender.com/

Built a Sports Image Classifier.

Data Collection:-
Built my own labelled data by running java script in browser to download a csv file with the image url's and then store each category of images in different folders. Each category had 400 images

Processing:-
All the images were in different shape and size transformed the image to same size, also normalized the image and data augmentation was also done to rotate images, cropped the image from center and converted the shape to a square box of equal dimensions.

Model Building:-
Built various models 
1. leveraging the practical library such as fast.ai
2. Used Amazon SageMaker in built image classification algorithm
3. Built image classification model using fully connected neural network (MLP)
4. Built image classification model using sparsely connected using CNN in PyTorch

After training the model fast.ai provided best results however CNN was better to incorporate different layer settings, convolution layer configuration or adding pooling layer even adding dropouts and back propagation to update the weights and bias.

Quality Checking:-
This is supervised learning with multi class classification thus I have used CrossEntropyLoss to calculate the model performance with validation set. Since the model accuracy was around 77%, performed transfer learning using RESNET50 architecture which is pre-trained on IMAGENET data with 1000 classifications and more than million images. This helped a lot improving the performance to 94% and then used the hyperparameter tuning to enhance the performance to 97%.


 
