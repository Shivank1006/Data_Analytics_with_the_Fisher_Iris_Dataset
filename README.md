# Data Analytics with the Fisher Iris Dataset


## Abstract


This document summarizes the results of data exploration and data classification per-
formed on the Fisher Iris Dataset. The Iris Dataset contains the samples of four different
features from three different species of Iris flower. The features include the length and
width of the sepals and petals measured in centimetres. Histogram, scatter plots and
box plot of the features are included for the exploration of data. Logistic Regression,
Gaussian Naive Bayes and K-Means algorithms are used to classify the data by using
the five-fold cross-validation technique. For each algorithm, the confusion matrix is 
tabulated and classification report is generated. The performance of each algorithm on the
given dataset is also compared.

## 1 Dataset


The Iris flower data set or Fisher’s Iris data set is a multivariate data set introduced by the
British statistician and biologist Ronald Fisher in his 1936 paper The use of multiple mea-
surements in taxonomic problems as an example of linear discriminant analysis. It is some-
times called Anderson’s Iris data set because Edgar Anderson collected the data to quantify
the morphological variation of Iris flowers of three related species. Two of the three species
were collected in the Gaspé Peninsula "all from the same pasture, and picked on the same
day and measured at the same time by the same person with the same apparatus".
The data set consists of 50 samples from each of three species of Iris (Iris setosa, Iris
virginica and Iris versicolor). Four features were measured from each sample: the length
and the width of the sepals and petals, in centimeters. Based on the combination of these
four features, Fisher developed a linear discriminant model to distinguish the species from
each other.

## 2 Data Exploration


Used various methods to explore the data in Iris Dataset including the correlation heatmap,
histograms, scatter plot and box plot. Each of these has provided different insights into
the data. It is found that there are no null entries in the dataset which is good. The major
conclusions are given below along with the plots.


<p align="center">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/1.png?raw=true" width=224 align="middle">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/2.png?raw=true" width=224 align="middle">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/10.png?raw=true" width=224 align="middle">
</p>

Figure 1: (a)Correlation Heat map for different features. (b)Scatter plot with Petal Length(x)
and Petal Width(y) for all data points. (c)Distribution of Sepal Width(y) by grouping Sepal
Length(x) into 5 or 10 bins.

### 2.1 Description

<p align="center">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/7.png?raw=true" width=700 align="middle">
</p>


### 2.2 Correlation Heatmap

Plotted the heatmap to show the correlation between the features. It can be seen in figure
1(a) that there is a very high correlation between petal width and petal length with a corre-
lation coefficient of 0.96. The correlation of sepal length and petal length and also the sepal
length and petal width is found to be positive with a correlation coefficient of 0.87 and 0.
respectively. However, there is a negative correlation between sepal width and petal length
and sepal width and petal width with the correlation coefficient of -0.43 and -0.37.

### 2.3 Scatter Plot

Made a scatter plot with Petal Length (x) and Petal Width (y) for all the values in the dataset.
It was analysed that the points increased linearly. The overall petal length and petal width
were longer for the Virginica species whereas it was shorter for the Setosa species ( too short
in comparison ). However, for the Versicolor species, the lengths were closer to the Virginica
species. The scatter plot is given in the figure 1(b).

### 2.4 Box Plot

The median for the virginica species is always greater than the two other species but not in
the case of sepal width. Also in every boxplot the length of the box and whiskers show the
variation of values from average value. The variation is again high for virginica in the first

<p align="center">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/3.png?raw=true" width=300 align="middle">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/4.png?raw=true" width=300 align="middle">
 </p>
 <p align="center">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/5.png?raw=true" width=300 align="middle">
<img src="https://github.com/Shivank1006/Data_Analytics_with_the_Fisher_Iris_Dataset/blob/master/images/6.png?raw=true" width=300 align="middle">
</p>

Figure 2: (a)Box plot for petal length(cm) (b)Box plot for petal width(cm) (c)Box plot for
sepal length(cm) (d)Box plot for sepal length(cm)

three cases but for sepal width, it is less. The number of outliers is more virginica for sepal
width and for setosa in the case of petal length and petal width. However the average sepal
width is more for setosa than the other two species.

## 3 Logistic Regression

Fitted the Logistic Regressor on the dataset for five-fold cross-validation.
Hence the average accuracy for the model is 96%.
Also plotted the confusion matrix and tabulated the classification report for the model.

## 4 Gaussian Naive Bayes

Performed the five-fold cross-validation on the dataset for the Gaussian Naive Bayes too.
The average accuracy came out to be 95.33%
Also plotted the confusion matrix and tabulated the classification report for the Gaussian
Naive Bayes model.

## 5 K-Means

Used the complete dataset to train the KMeans model. Plotted the confusion matrix for the
model. Also performed PCA to plot the misclassified data points on a scatter plot.


## 6 Conclusion

The logistic regression and Gaussian Naive Bayes performed well on the dataset whereas
the performance of the KMeans classifier was satisfactory. Also the results for the KMeans
varied with multiple runs as it depends on the initial centroids chosesn randomly. Also there
were some outlier in the dataset which too affected the performance of the models. However
they can be removed from dataset to make it more clean and better for training.
The things that I learn are that K-Fold Cross-Validation significantly increase the perfor-
mance of a model and also aware us about the fitting of the model on the dataset and protect
it from overfitting on the data.


