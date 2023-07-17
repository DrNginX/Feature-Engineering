# Analysis of Transformation
Basically, The project is based on feature transformation which is a subpart of the feature Engineering. In this project I have perform multiple feature Transformation techniques inside the dataset to get more accurate model prediction. So for that we use Linear Regression as model and cross validate it to get the almost exact accuracy. Then after we apply the transformation and try to get difference between with transformation and without transformation accuracy rate and both have to validate with Cross validation techniques. In the project we use population dataset which is downloaded from kaggle dataset collection. The main moto of this project is to check which tranformation ehance more accuracy of model.

## Feature-Engineering
Feature engineering is the process of creating new features or transforming existing features in a dataset to improve the performance of machine learning models. It involves selecting, extracting, or deriving relevant information from the raw data that can enhance the model's ability to learn and make accurate predictions. Feature engineering often requires domain knowledge and creativity to identify meaningful patterns, relationships, or representations in the data. This can involve various techniques such as encoding categorical variables, handling missing values, scaling, normalizing, binning, creating interaction or polynomial features, applying mathematical transformations, and more.

## Feature Transformation
Feature transformation is a fundamental technique used in various fields, such as machine learning and data analysis, to enhance the performance and interpretability of models. It involves applying mathematical operations or functions to the existing features of a dataset to create new representations that capture more meaningful or informative aspects of the data. Feature transformation can encompass a wide range of methods, including scaling, normalization, logarithmic or exponential transformations, polynomial expansions.

By transforming features, we can uncover hidden patterns, reduce dimensionality, improve data distribution, and enable models to better capture complex relationships. This process plays a crucial role in preprocessing data and optimizing model performance, ultimately contributing to more accurate predictions and insightful data analysis.

In this repository I am just trying to enhance the accuracy of model by putting all type of transformation techniques such as power transformation and function transformation inside the dataset.

# Table of Content
1. Power Transformatio

  a. Box-Cox Tranformation

  b. Yeo-johnson Tranformation

2. Function Transformation

  a. Log Tranformation

  b. Square Transformation

# Power Transformation
Power transformation, also known as a power function or power law transformation, is a type of mathematical transformation applied to a variable in order to change its distribution or reduce skewness. It involves raising the variable to a power or applying a logarithmic function.

The power transformation can be expressed as:

Y = X^λ

where X is the original variable, Y is the transformed variable, and λ is the power parameter. The value of λ determines the type and direction of the transformation.

## Box-Cox Tranformation
The Box-Cox transformation is a family of power transformations that includes both square root and logarithmic transformations as special cases. It introduces an additional parameter, λ, which is estimated from the data to find the best transformation for normalizing the distribution

## Yeo Johnson Tranformation
The Yeo-Johnson transformation is a power transformation method that extends the Box-Cox transformation to handle both positive and negative values, including zero. It is particularly useful when dealing with data that may exhibit skewness or heteroscedasticity.

The Yeo-Johnson transformation is defined as follows:

For y ≥ 0:
Y = [(y + 1)^λ - 1] / λ if λ ≠ 0
log(y + 1) if λ = 0

For y < 0:
Y = -[(|y| + 1)^(-λ) - 1] / λ if λ ≠ 0
-log(|y| + 1) if λ = 0

Here, y represents the original variable, Y represents the transformed variable, and λ is the power parameter estimated from the data.

The Yeo-Johnson transformation handles a wider range of data distributions compared to the Box-Cox transformation, making it more versatile in practice. It can accommodate both positively and negatively skewed data, handle zero values, and offer flexibility in choosing the appropriate power parameter. 

# Fuctional Tranformation
Function transformation refers to the process of applying mathematical operations or functions to a function's equation or graph to alter its shape, position, or characteristics. By manipulating the equation or graph of a function, we can create new functions with different properties or modify existing functions to suit specific needs.

## Log Transformation
Log transformation is a common type of mathematical function transformation that involves taking the logarithm of a variable. It is particularly useful when dealing with skewed or exponentially distributed data, as it can help normalize the data and make it more suitable for analysis or modeling purposes.

The logarithm function used in log transformation is typically the natural logarithm (base e) or the common logarithm (base 10). The logarithm of a positive number x is denoted as log(x).

The log transformation is applied by taking the logarithm of each value of the variable. This has the effect of compressing the range of values, reducing the impact of extreme values, and making the data distribution more symmetric. The transformation can also help linearize exponential relationships, making them more amenable to linear modeling techniques.

## Square Transformation
The square transformation is a mathematical function transformation that involves squaring the values of a variable. It is a simple and commonly used transformation technique that can be applied to a variety of data types and distributions.

To perform a square transformation, each value of the variable is multiplied by itself (raised to the power of 2). This has the effect of amplifying the differences between values and can often emphasize patterns or relationships in the data.

# Installation and Use
In this project We use Power Transformation and function transformation both where in fuction transformation we only applied log transformation inside the dataset coz data is right skewed.

## Installed Libraries

1. Scikit Learn
2. Scipy
3. Pandas
4. Numpy
5. Matplotlib
6. Seaborn

with the help of these libraries I perform all the operation inside the dataset and get insight.

# Feature Transformation Life-cycle model
The procedure of Data transformation is simple :-

step 1:- Extract the dataset

step 2:- Select the correlated features

step 3:- Split the data into train and test set.

step 4:- Apply the transformation into X train set and X test 

but thing is that if direct start doing the feature transformation you have not get anything so, before start doing the feature transformation first of all check the accuracy rate with Linear Regression or else other model then cross validate it. Cross validation help to get more accurate insight of accuracy of model prediction. After then if you get low accuracy rate then check the skewness of the data with the help of Visualization techniques. In this project I use the scipy probplot, matplotlib and seaborn libraries.
Analyse the graph and the regression line so that it will help to take appropriate decison that this transformation is suitable for this feature or may be it will improve the accuracy rate. Then you can apply the transformation inside the data and proceed further.

## Acknowledgment
I would like to thanks kaggle.com for providing me the valuable dataset which is used inside the project. Without the assistance and contributions of these individuals and organizations, this project would not have been possible. I am truly grateful for their involvement and for making this journey a rewarding and enriching experience.

Hence Project is END

# Thanking You
