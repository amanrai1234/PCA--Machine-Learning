# Project-4--PCA-using-Scikit-learn


In this segment we are training a Random forest classifier 
using sklearn.

## DATASET:( Briefly analyse and discuss the dataset.)

The dataset has two componenents and they are X and y variable and they are separate compressed components and I extracted them using numpy Npz load. And the shape of X is 10000,
1000 and the shape of y is 10000,1 and y is the target variable 
of the dataset and X is the data for the model. Here this data was compressed as it was high dimensional and training on this 
data would take a lot of time and resources.

Step 1:

Converting the values from NumPy to pandas

Step 2:

Visualizing the head of the table using pandas .head()

Step 3:

Splitting the dataset(here scaling the dataset does not make a
lot of difference but anyway scaling is always preferred)

Step 4:

Training the data into random forest classifier using scikit-lear
n and then fitting the data and then calculating the performanc
e of this task using metrics (confusion matrix)

Step 5:

Measuring the time taken to do PCA using time.time in pytho
n

Step 6:

Performing PCA using Scikit-learn and reducing the number o
f dimensions using the number of components or directly the 
variance (0.95)

Step 7:

Fit the data in the random forest again and this time we use th
e PCA data and here we have reduced the dimensionality of th
e data.

Step 8:

Here we time the model and compare the time of both the PC
A vs non-PCA models.

Step 9:

Here we also calculate the accuracy of the model and print the 
tree depth.



discuss the classification performance of Random Forest u
sing an appropriate metric?

• The accuracy I have received after performing the rando
m forest algorithm is 0.9990909090909091

• And the training time of the data is (Training time: 4.2787089
347839355)

Whereas the other metrics of the data are:

True Positives: 1667
True Negatives: 1630
False Positives: 2
False Negatives: 1
Precision: 0.9988016776512882
Recall: 0.999400479616307

# The time required to reduce the data by using PCA

• Training time: 2.064049243927002s for PCA

• Each instance has 5 features after fitting the model with vari
ance of 95%.

• The training time for the Random forest is Training time: 0.41
64729118347168s

• Yes the training time of the model(random forest) drasticall
y reduces after training.

# The metrics if the model are:
Random forest

True Positives: 1667

True Negatives: 1628

False Positives: 4

False Negatives: 1

Precision: 0.997606223818073

Recall: 0.999400479616307

Accuracy: 0.9984848484848485

The things that we can observe are the difference between trainin
g time of the two classifiers, as the dataset is less in the second par
t the training part of the requires less time (4 seconds less than the 
first part) and the accuracy of the algorithm has also been increas
ed by very less amount. This is very important detail as we have s
een, this signifies that the we have data which has highly correlate
to each other
