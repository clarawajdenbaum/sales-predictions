# Sales Predictions
## Predicting the sales of various objects 

**Clara Wajdenbaum**

### Business problem:

The goal is to make predictions about future sales based on the data provided.

### Data:
Sales predictions

### Methods:

In the feature column 'Item Weight', I have replaced the missing values with the mean weight. I couldn't delete rows with missing values as the percentage was too high.
In the feature column 'Outlet Size', I have replaced the missing values with 'missing'. I have decided to add a new category 'Missing' so it doesn't affect our data.
I have scaled the integer and float columns and I have OneHotEncode the object columns.

### Results:

**Item Outlet Sales via Item Types**

![Item Outlet Sales via Item Types](https://user-images.githubusercontent.com/101348370/167168745-d752ab72-81aa-48c9-8d20-1a47f48c3194.png)

**Frequency of Item Outlet Sales**

![Frequency of Item Outlet Sales](https://user-images.githubusercontent.com/101348370/167168891-04c7d262-adc3-4f42-af61-632e7500fd03.png)

### Modeling Results

The Linear Regression Model is absolutely not a model that fits our data. 
The Regression Tree Model with a max depth of 7 has a score on the testing set of 59%.

### Summary

The Linear Regression model doesn't work at all on our dataset as we have a negative r^2 score on the testing sets. 

I would recommend a Regression Tree Model with a max_depth of 7.
This model has a low variance and a moderate r^2 score. 
The RMSE of this model on the testing set is of 0.11 which is very low. The lowest it is, the best, as it means that we have a small margin of errors.

### For further information:

For any additional questions, please contact **clara.wajdenbaum@icloud.com**
