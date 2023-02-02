# BlueBerryWinery

![wine](https://learn.wineenthusiast.com/wp-content/uploads/2019/09/HeaderImage.svg)


## Introduction 

The focus of the project is  to  build a Wine Quality Analytics System to determine the quality of the wines produced based on their composition.

## Data set overview

The dataset contains physicochemical and sensory variables:
* Fixed acidity: acids are major wine properties and contribute greatly to the wine’s taste. Usually, the total acidity is divided into two groups: the volatile acids and the nonvolatile or fixed acids. This variable is expressed in g(tartaricacid)/dm3 in the data sets.

* Volatile acidity: the volatile acidity is basically the process of wine turning into vinegar. In the U.S, the legal limits of Volatile Acidity are 1.2 g/L for red table wine and 1.1 g/L for white table wine. In these data sets, the volatile acidity is expressed in g(aceticacid)/dm3.

* Citric acid is one of the fixed acids that you’ll find in wines. It’s expressed in g/dm3 in the two data sets. Residual sugar typically refers to the sugar remaining after fermentation stops, or is stopped. It’s expressed in g/dm3 in the red and white data.

* Chlorides can be a significant contributor to saltiness in wine. Here, you’ll see that it’s expressed in g(sodiumchloride)/dm3.

* Free sulfur dioxide: the part of the sulfur dioxide that is added to a wine and that is lost into it is said to be bound, while the active part is said to be free. The winemaker will always try to get the highest proportion of free sulfur to bind. This variable is expressed in mg/dm3 in the data.

* Total sulfur dioxide is the sum of the bound and the free sulfur dioxide (SO2). Here, it’s expressed in mg/dm3. There are legal limits for sulfur levels in wines: in the EU, red wines can only have 160mg/L, while white and rose wines can have about 210mg/L. Sweet wines are allowed to have 400mg/L. For the US, the legal limits are set at 350mg/L, and for Australia, this is 250mg/L.

* Density is generally used as a measure of the conversion of sugar to alcohol. Here, it’s expressed in g/cm3.

* pH or the potential of hydrogen is a numeric scale to specify the acidity or basicity the wine. Most wines have a pH between 2.9 and 3.9 and are therefore acidic.

* Sulfates  are expressed in g(potassiumsulphate)/dm3.

* Alcohol: this variable is  expressed in % vol.

* Quality: wine experts graded the wine quality between 0 (very bad) and 10 (very excellent). The eventual number is the mean of at least three evaluations made by those same wine experts. 

According to the quality score  given by wine experts,the  wines were grouped  into 3 groups:
  * low quality   <= 5 
  * medium quality <=7
  * high quality >=8

## Modelling 

I used  a Supervised learning type of machine learning. My goal was to train a model that could in future  to apply the  quality labels (low,medium,high)  to new data. For this purpose I used the classification concept which basically categorizes a set of data into classes. 

Machine learning models:
* Naive Bayes model consists of two types of probabilities that can be calculated directly from  training data: 1) The probability of each class; and 2) The conditional probability for each class given each x value.

* Logistic Regression to find the best-fitting relationship between the dependent variable  and the set of independent variables.

* Random Forest conctruction of a multitude of decision trees at training time and output the class that is the mode of the classification.

Steps:
* Selection of the variables (incl.: Encoding and Noramalisation) 
* Fitting the model and prediction of the results.
* Model evaluation
* Model Improvement 


## Conclusions

[Presentation_Part1](https://www.canva.com/design/DAFO0A6yuTc/6e8ccHFxxY05sAaMm_2-9Q/view?utm_content=DAFO0A6yuTc&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)


[Presentation_Part2](https://www.canva.com/design/DAFQOLFU8Bc/zHNSTn49DqzBl5VyXdkLqg/view?utm_content=DAFQOLFU8Bc&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)

## Data source 

[Dataset](https://archive.ics.uci.edu/ml/datasets/wine+quality)

There are 3 data files:

the file named winequality-red.csv contains the dataset pertaining to 1599 records of red wine samples
the file named winequality-white.csv contains the dataset pertaining to 4898 records of white wine samples
the file named winequality.names consists of detailed information and the data dictionary pertaining to the datasets

[Wine_prices](https://drive.google.com/file/d/148ndWjamqPBlWsk5yofmmAB9XcikP0bJ/view)

the file contains the dataset pertaining to 65K records of information about: 
* wine quality score;
* country of production;
* description;
* price;
* province & region
* winery