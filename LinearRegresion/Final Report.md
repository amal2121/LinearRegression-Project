## Introduction :

The nutrition industry is currently experiencing huge growth. Increasing awareness of how diet affects health.
 Set against a backdrop of busy lifestyles and global health concerns, the nutrition market looks set to skyrocket as people look for quick and easy solutions.
From this point we get inspiration to talk about nutrition and health grocery market and predict price of it.
By doing web scrubbing from IHERB.com

## Data Description:

A model performance depends heavily on the data it was trained on . To acquire the data, we used web scraping on iHerb website.
 The features of the products dataset are the following:
 
* Name: the name of the product.

* Class_info: the name of the category the product belongs to (Sports-Nutrition, Grocery)

* Weight: the size measurement of the products

* Ratings: the average rate of the product.

* Reviews: the number of customers reviews on the product.

## The target is :

Price: product cost

## workflow:

After getting the data we start to clean them remove nulls values, weight conversion . After that we started to explore the dataset and split the data into %60 train/%20validation, and %20 for the test.
Finally we tried two types of models:

* First one is linear regression :

The R square (Train) = 0.682

The R square(validation) = 0.679

The testing R square = 0.684

* Second is Polynomial Regression :

The R square (Train) = 0.707

The R square(validation) = 0.67

The testing R square = 0.667

#### As we see here we pick linear regression depends on the minimum difference between R square and testing R square which mean the model learn from linear regression better than polynomial regression and fit the data.
Then we combine train and validation data then test it and the testing R square was equal 0.7033
