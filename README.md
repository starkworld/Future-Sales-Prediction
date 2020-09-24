# Future-Sales-Prediction
* Predicting the future sales of 1C Russian company based on given 34months of sales data
* This is one of the active problem in kaggle which is prediciting future sales of the 1C Russiun company. They have given past 34 months of data by using that we have to predict next month sales of each item in that company.
Here we are using simple LSTM netwrok model to train our data. Before that we have lot of work to do.
* Lets go and explore data.
* At first we have to see the outliers in our dataset which means values which are distributed away from cluster of values. For our dataset we have seen plotted a boxplot to display it. Here is the Image of outliers.
![Alt text](https://github.com/starkworld/Future-Sales-Prediction/blob/master/Screen%20Shot%202020-09-24%20at%201.13.10%20AM.png)

* after seeing the image we have a feeling that both item price and item cnt day columns have some outliers, so we will filter out them now. This image shows data without outliers.
![Alt text](https://github.com/starkworld/Future-Sales-Prediction/blob/master/Screen%20Shot%202020-09-24%20at%201.13.27%20AM.png)

* After this step we have to see the correlation between each columns with dependent variable so we can know which independent factor effecting the dependent factor most. So we can see it below
![Alt text](https://github.com/starkworld/Future-Sales-Prediction/blob/master/Screen%20Shot%202020-09-24%20at%201.13.35%20AM.png)

* After this step I remove all the unnecassary columns and cleaned data its now ready for splitting train and test sets.
Here I used train set for model training and test set for predicting model accuracy.
* After this step I fed data into LSTM model and it trained on our training data with loss- 4.395
And it pretty well performed on test set to predict future sale!!
