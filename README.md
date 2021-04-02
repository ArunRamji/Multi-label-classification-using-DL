# Multi-label classification using Deep Learning 
Demo of how to implement multi-label classification using Deep learning , explained how to implement using real time banking data to predict next best product for customer based on their past behaviour . 

## Objective
Illustrate how to implement multilabel classification using Deep Learning using Keras framework 

## What is multi-lable classification, how it is differnce from multiclass classification ?
The difference is that in multi-class problems the classes are mutually exclusive, 
whereas for multi-label problems each label represents a different classification task, 
but the tasks are somehow related (so there is a benefit in tackling them together rather than separately). 
For example, in the famous leptograspus crabs dataset there are examples of males and females of two colour forms of crab. 
You could approach this as a multi-class problem with four classes (male-blue, female-blue, male-orange, female-orange) or as a multi-label problem, 
where one label would be male/female and the other blue/orange. 
Essentially in multi-label problems a pattern can belong to more than one class.

## Example used : 
ML model to predict , what will be the next best product for bank customer that bank can offer , Based on the past behaviour of similar customer 
we are going to predict for new/target customer 


## Problem Definition :
* To predict which products Bank's existing customers will use in the next month based on their past behavior and that of similar customers. With a more effective recommendation system in place, Santander can better meet the individual needs of all customers and ensure their satisfaction no matter where they are in life.

* you are provided with 1.5 years of customers behavior data from Santander bank to predict what new products customers will purchase. The data starts at 2015-01-28 and has monthly records of products a customer has, such as "credit card", "savings account", etc. You will predict what additional products a customer will get in the last month, 2016-06-28, in addition to what they already have at 2016-05-28. These products are the columns named: ind_(xyz)_ult1, which are the columns #25 - #48 in the training data. You will predict what a customer will buy in addition to what they already had at 2016-05-28. 

## Data Source :
https://www.kaggle.com/c/santander-product-recommendation/data?select=train_ver2.csv.zip 

## Model detail 
* Library   : Keras 
* Algorithm : Standard Neural Network 
* Regularization : Dropout
* Classification : binary (Multi-label)
* Regularization : Dropout
* Hyper parm tuning : No

![image](https://user-images.githubusercontent.com/40143199/113405576-b0dd4c00-93c7-11eb-8f9b-9d86656e67c1.png)

**Overall Accuracy on test(Out of sample)** : 57%

**How to increase the model performance further**
* Balancing class distribution of some samples 
* Sourcing the right lables (In our example there are lables with only positive or negative class which affects the peformance )
* Trying out different neural network structure 
* Applying hyper param tuning (like learning rate , number of nodes, optimizer , batch size ..etc)


## Conclusion :
Based on the above example and model performance , it is evident that Deep learning can be used eaily and efficiently for any multi-label classifcation 
moedl
