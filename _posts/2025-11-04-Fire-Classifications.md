---
layout:     post
title:      "Fire Classifiction: Arson or Accidental?"
published:  true
---


# Can fire cause be determined from images from the scene?

I'm an avid true crime watcher and a tester who works hard trying to notice the unnoticeable. I experimented with Jupyter notebooks in uni but haven't attempted anything in this area for a long time. 

I decided I wanted to attempt to classify images based on existing image models and a custom data set, set it up, gather data and develop this skill set more. The subject I settled on was fires - I wanted something niche that way the possibility of stumbling onto something useful could be greater. 


# Fires
## Accidental or Arson? 

I wanted to try and determine if there were any differences that could be detected of property on fire or fire damaged that would indicate the cause of the fire. I focused on mostly exterior photos, photos of damaged properties trying to get as many photos of the subject actively on fire as I could to try to enable analysis of the smoke and flame colour. 

Some patterns between arson vs accidental fire cause include multiple points of extreme damage, hints of multiple points of origin, unusual spread distribution. Darker smoke may suggest accelerants. 

I searched through news websites, google to find images where it was reported that the cause was suspected arson or accidental. It was harder than I thought to gather images I wanted to build a large dataset whilst also having the information available on whether the cause was arson or accidental. 

In the end I gathered initially 80 images and then grew this to a still very small 157 images in total but the classification may be subject to human error or misreporting on the sources. Disclaimer any marked as arson also include being described suspected arson there may be some small inaccuracies. 

I used the 70:15:15 ratio to distribute test, train and validation data over my classified dataset. I set up a Google Colab notebook.
The first step was to install libraries required such as split-folders, numpy, tensorflow, and Keras. Keras's ImageDataGenerator was used. The images I gathered were all different sizes and file formats, an Extract, Transform, and Load (ETL) process resized the images, converted them all to the same format (even though they could likely be handled this was to rule out discrepancies). 

ResNet50 was the base model used for this project. I set the base_model.trainable to false to "freeze" the main layers. GlobalAveragePooling2D was used for classification and condensing. 2 classification categories were specified: {'accidental': 0, 'arson': 1}. 

A 0.5 dropout was set to prevent overfitting due to having a smaller dataset to try to prevent over reliance. Predictions are created converting the output to probability distribution giving the probability of being either accidental or arson. I started training on a small number of epochs at 15.. The results were plotted using matplotlib. 

Here are some example results: 
![ModelResults](/assets/modelResults.png)

As we can see the results are not very reliable. The data set is quite small. I undertook this project to start learning principles and to learn the process so getting high and accurate results are not the goal here. 

After the initial training stage, I wanted to be able to pass in single unclassified images to test the results using the .predict() model to see how the results would fare given my setup is very prone to overfitting. 

I would then classify the images properly after and tweak to check for improvements. As the dataset grows I can rerun and monitor the results. 

On top of increasing the amount of images in the data set, other things could be looked at such as combining with metadata such as was there forced entry detected, time of day, weather etc. 

It's hard to say how much can be inferred from exterior photos alone. The results were inaccurate, when 6 new images were fed into predict classification, 4 were wrong and 2 were right. It predicted accidental every time so it is hard to know if it got the 2 right or it was a matter of change picking accidental each time. 

So can fire cause be determined from images from the scene? 
Potentially but not from this model as it is too unreliable. Something like this should only be used a supplementary aid should a dataset large enough garner more accurate and reliable results. Additional sources of investigation will always be needed such as checking the scene for accelerants, signs of forced entry and other indicators. 

