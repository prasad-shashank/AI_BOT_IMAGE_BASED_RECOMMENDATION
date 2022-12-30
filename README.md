

AI BOT FOR IMAGE-BASED PRODUCT RECOMMENDATION

SHASHANK PRASAD

*STUDENT ID- 1030468*

MS. ARTIFICIAL INTELLIGENCE AND MACHINE LEARNING

DECEMBER 2022





Introduction | Background

• We have seen how ecommerce market is

growing.

• Trends suggests that ecommerce industry will

surpass $20 trillion dollars by 2025.

• Resulting in increase of E-Commerce

application.

• Making inconvenient for user to download

multiple application and apply filters to find

right product.

• Filtering in these application is limited to

content based and very difficult to for user to

find product what they is looking for.





Introduction | Aim and Objective

• Other application apart from ecommerce app have

shown growth is of instant messaging app.

• Trend suggests there are more 3 billion monthly

active user across different instant messaging app.

Aim and Objective

q Build recommendation system which recommend product based on visual/ features and similarity.

q Identify best model to achieve high accuracy with less loss.

q Integrate image based recommendation system with instant messaging application via bot to

recommend product based on user interest.





Literature Review

2012

Modeling the Visual

2015

Evolution of Fashion

Trends with One-

Class Collaborative

Filtering

Image-based Product

Recommendation

System with

Convolutional Neural

Networks

2020

Image-Based Service

Recommendation

System: A JPEG-

Coefficient RFs

Approach

(Stewart, 2012)

2020

(Chen et al., 2015)

Product Based

Recommendation

System On Amazon

Data

2020

(Ullah et al., 2020)

Improvising the

performance of

image-based

(Dwivedi et al., 2020)

2022

End-to-End Image-

Based Fashion

Recommendation

(Elsayed et al., 2022)

recommendation

system using CNN

and DL

(Sulthana et al., 2020)





Literature Review | Research gaps

§ All the research done till date just aim to find the right model for image recommendation, and non

of the research consider user experience while building the model. In other words non of the

research work done is end to end.

§ In all most all the research done till date, the images used for testing is from the same dataset and

random image captured by user was not considered.

§ Some crucial models like GoogLeNet, Xception were missing in some research work.

§ Previous research solely rely on visual content of the image and contextual information of product

like product rating, cost, brand is not considered in the recommendation.





Problem Statement

• How can we effectively use visual information from images to make personalized

recommendations to users?

• Explore ways to use visual information from images to make more accurate and relevant

recommendations to users, with the goal of improving the overall user experience.

• Identify the best model for building the image based recommendation system.





Methodology

This research involved end to end implementation

in three phases :

\1. Develop bot for end user where user can upload

image of the product which will connect to

recommendation system.

\2. Identify the best model with high accuracy and low loss which can be used to build recommendation system

\3. Build recommendation system using identified model which takes input from the user and recommend N

products to the user.





Methodology | Bot

• In this research we have consider telegram bot for development.

• Search for “BotFather” and create new bot by “/newbot” command in telegram from

“BotFather” chat.

• “BotFather” will return token on successful creation of bot, use this token to communicate

with the bot.

• Remove the background of image uploaded by user using the telegram bot.

• Extract the features from the image and compare with the feature extracted from images

present in dataset and recommend N product with the closest feature to the user





Methodology | Approach

• Collected the Amazon product data across different category and store it in CSV file. The data

extracted is can be found in: [Amazon](https://drive.google.com/file/d/1rxzWS7pqG_WloSQHJKvuLwe7MbB8whrI/view)[ ](https://drive.google.com/file/d/1rxzWS7pqG_WloSQHJKvuLwe7MbB8whrI/view)[Dataset](https://drive.google.com/file/d/1rxzWS7pqG_WloSQHJKvuLwe7MbB8whrI/view).

• Load the data in categories and perform data cleaning where by remove duplicates, fill empty cell and

preform feature selection and data transformation.

• Perform exploratory analysis to explore the trend in the data.

• Create image classification model with aim to categories the random image using CNN model.

• Compare different model for accuracy and loss

• On best model extract feature and compute cosine similarity or nearest neighbour distance of the

product and give recommendation.





Methodology | Experiments on Models

• After creating data set and downloading all the image. We will first split the data in train and test.

• Load below module to train on train dataset.

o CNN –SVM

o ResNet50

o GoogLeNet

o VGG16

o Xception

• Evaluate the model on train, validation and test data to find the accuracy, loss of the models.





Results & Discussion | CNN Model

• As a part of implementation, first we build image classification model with aim to categories the random

image using CNN model.

• But we saw the result was not

accurate.

• Mainly because of low accuracy

and high loss.

• Conclusion – CNN model

developed is not accurate and

we need to look for model with

high accuracy and low loss.





Results & Discussion | Experiments on Models

• After evaluating models like CNN, ResNet-50, GoogLeNet, VGG16 and Xception on training and

test data, we found that VGG16 model with high accuracy and low loss across train, validation

and test data.





Results & Discussion | Image Recommendation

Model

Compute

nearest

neighbours

Extract image

features of data

set using

VGG16 (pre-

trained model)

Extract image

features of data

provided by

user using

VGG16 model

Recommend N

product based

on high score /

distance

distance of any

image features





Conclusion

• In this research we have build

recommendation system which recommend

product based on visual/ features and

similarity and integrated it with telegram bot.

• The research found the VGG16 as best mode

on given dataset with accuracy of 85.41% and

loss of 0.48.

• The research demonstrated the potential of

image-based recommendation systems to

enhance the user experience and engagement

on online platforms, and to support businesses

and organizations in their marketing and sales

efforts





Future works

\- Incorporate user feedback: Another way to improve image-based recommendation systems is to

incorporate user feedback into the recommendation process and use this feedback to improve

the accuracy of the system over time.

\- Increase scalability: As the dataset increases, increasing the scalability of system using

distributed computing techniques, such as parallel processing, to enable the systems to handle

larger datasets and serve more users.

\- Multi-model implementation: Combine image classification model, title and brand

recommendation model and image recommendation model to recommend product.

\- Explore GoogLeNet model by training the dataset on more epochs.





Demo

\1. To access image based recommendation bot open telegram and

search for @ml\_product\_recommendation\_bot or click on below link.

Link - <http://t.me/ml_product_recommendation_bot>

\2. Click on Start or type /start to start the application.

\3. Upload or click product image to find the similar product.





**THANK YOU !**

