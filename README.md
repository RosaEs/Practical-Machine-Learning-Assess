# Practical-Machine-Learning-Assess
Peer Assessments /Prediction Assignment Writeup

Background
Using devices such as Jawbone Up, Nike FuelBand, and Fitbit it is now possible to collect a large amount of data about personal activity relatively inexpensively. These type of devices are part of the quantified self movement – a group of enthusiasts who take measurements about themselves regularly to improve their health, to find patterns in their behavior, or because they are tech geeks. One thing that people regularly do is quantify how much of a particular activity they do, but they rarely quantify how well they do it. In this project, your goal will be to use data from accelerometers on the belt, forearm, arm, and dumbell of 6 participants. They were asked to perform barbell lifts correctly and incorrectly in 5 different ways. More information is available from the website here: http://groupware.les.inf.puc-rio.br/har (see the section on the Weight Lifting Exercise Dataset). 

Data 
The training data for this project are available here: 
https://d396qusza40orc.cloudfront.net/predmachlearn/pml-training.csv
The test data are available here: 
https://d396qusza40orc.cloudfront.net/predmachlearn/pml-testing.csv
The data for this project come from this source: http://groupware.les.inf.puc-rio.br/har. If you use the document you create for this class for any purpose please cite them as they have been very generous in allowing their data to be used for this kind of assignment. 

The goal of this project is to predict the manner in which they did the exercise. This is the "classe" variable in the training set. You may use any of the other variables to predict with.

> We have a dataset with to many columns and we need make a class prediction.
Firstly we prepare the dataset removing all columns with NA’s or with empty values. We also remove the columns that clearly aren't predictor variables.

> Secondly We split training data into 60% training and 40% validating dataset.
After that, we try some transformations into training, like Preprocess by centering and scaling but we compared results and noticed that it´s no necessary.

> We  decide implement a random forests model, when we evaluate the model we get an Accuracy of 99% over Validation dataset.
We use the model to predict on the testing data set. 

> Finally we submit our predictions to the Assignment that return us that all of them are correct.


