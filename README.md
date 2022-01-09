# Analyze-classify-and-predict-three-different-data-using-machine-learning

# 1-  OnlineNewsPopularity dataset: 
I selected this dataset because it does not have a (NaN) and do not need a lot of preprocessing. OnlineNewsPopalurity is a dataset contain details about online news journals and articles and the target value is shares. I used the linear regression model to predict the number of shares of newspapers using many features like, Number of tokens content and average token length to predict number of shares. And this dataset also have no missing values and I checked that there is not a NaN values in the dataset. The outliers of this dataset are the number of shares that is bigger than 9000 shares so I removed it because it is disturbed the whole learning process. There are many columns in this dataset with many rows that I make it not easy in feature selection. The target class of this dataset is the shares. It's the class that describe the popularity of the news. 

# 2- Voice dataset: 
This dataset is for voice recognition. It is containing information about the tone of the voice. So, I selected this dataset because it is simple, do not have (NaN) and easy to understand. The features type to identify the label (“Male” or “female”) is the meanfrequncies, median, centroid, dfrange is the meanfrequncies, median, I used feature reduction method to identify the most important features that help the learning method to classify the label. There are no missing values in this dataset. There are no outliers in this dataset. The target class is the label and to classify the Male or female. 

# 3- abalone: 
this data set is used for predicting the number of layers or the number of rings in the abalone. And this dataset is interesting because by using it I can predict the number of rings of the abalone. So, I used a logistic regression model to predict the number of rings using many features provided by the dataset like the hieght,diameter and the gender of the abalone, and this data was good for us because it has no null values and no outliers. So, the target class of our dataset or the one to be predicted is the number of rings. I reduced the amount of data by selected only two classes to make a binary.

# Visualization Conclusion

![download](https://user-images.githubusercontent.com/96385070/148695429-afec148d-889f-4116-bbc1-c38c7d6702df.png)

I conclude from this visualization that the shares increases when the tokens content be less than 2000 and when token content increase the shares decrease. The best average for token length is between 4 to 6. after that when token length increase the shares decrease.

# Views

![download (1)](https://user-images.githubusercontent.com/96385070/148695480-6669f1e5-6d15-4b82-a685-805cba1eb537.png)

I concluded from this visualization that the meanfrequency of the male is more than female so the when the frequencies is high the probability that he’s male increase and the same in the median.

# Abalone

![download (2)](https://user-images.githubusercontent.com/96385070/148695518-37866b76-15b1-4df8-8a88-24cd6ccd2eca.png)


![download (3)](https://user-images.githubusercontent.com/96385070/148695536-3e674d25-c6b3-461e-ba84-9de2b9de0a51.png)

It's obvious from the first figure that the sex 0 (which is the female) and 2 (which is the male) is close to each other in terms of number of rings but, the sex 1(which is the infant) seems to be a little bit smaller than male and female. So, we can conclude that the small age abalone have number of rings less than the oldest abalone.
I Used 4 different models.  3 classsification model and 1 regression model.  

The classification models are: Logistic regression, Support vector machine and decision tree 

The regression model is linear regression. 

In linear regression model I used Root mean square error to measure the performance of the model and it was 9899. These a very high error and I used the r2 score function from sklearn library to measure the accuracy and it’s 0.17. that was too small.  

Conclusion is that the linear regression model was too bad, overfitted and failed to predict the target class with high accuracy because dataset was a sparse dataset. 

In Logistic regression model I measured the accuracy using accuracy measure in sklearn library and it was 0.62 and it was reasonable accuracy. Then I use the confusion matrix as measure for performance. Conclusion the logistic regression model was good and have reasonable accuracy. 

In Support Vector Machine I used the accuracy major and confusion matrix to measure the performance and it was 0.92. This was a good accuracy. 

In Decision Tree I used metrices accuracy score function to measure the accuracy of the decision tree. It was 0.97. It’s was a high accuracy and successes to predict. 

From comparing the 3 classification model with each other I conclude that the decision tree was the highest accuracy then support vector machine and at last the logistic regression model. 
