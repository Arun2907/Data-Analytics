# CALORIES-BURN-PREDICTION
The fast food consumption rate is high nowadays and has led to the intake of unhealthy food. This leads to various heath issues such as obesity, diabetes , an increase in blood pressure etc. This project focuses on the calories burned in accordance with the duration provided and heart rate during the exercise period. This research helps in providing the benefits of a machine learning algorithm over predicting the calories burned.
# libraries
<ul>
<li>Numpy
<li>Pandas
<li>Matplotlib
<li>Plotly
<li>Seaborn
<li>Scikit learn
</ul>

# Dataset
<ul>
<li>Exercise.csv - we have 15000 rows and 8 columns
<li>calories.csv - we have 15000 rows and 2 columns
</ul>

1.User_ID : The ID of the person which is unique.\ 
2.Gender : Gender of the person.\ 
3.Age : Age of the person.\ 
4.Height : Height of the person in cm .\ 
5.Weight : Weight of the person in kg .\ 
6.Duration : Duration of the person's exercise/activity in min.\ 
7.Heart_Rate : Heart rate per min of the person.\ 
8.Body_Temp : Body temperature of the person in celsius .\ 
9.Calories : Calories burned in kilo calories.

# Handling outliers
<ul>
<li>For detecting Outliers - IQR Method
<li>For Removing Outliers  - Quantile based Flooring and capping
</ul>
  
# Data Visualization

Here we have visualize the charts based on some categories.Here by some samples

First we are going to find correlation between the dependent and independent variables.
![Screenshot (246)](https://user-images.githubusercontent.com/94120618/156772364-1b77774b-7259-4277-981a-da101a91684e.png)

As we can observe, old individuals have burned more kilocalories in compare of two other age groups.And the young persons are the least in burning kilocalories which is a surprise!
Another interesting thing is, females in all age ranges performed very similar.In other words, they burned same amount of kilocalories in average.But for males, old group outperformed and the youth have the weakest performance.
![Screenshot (248)](https://user-images.githubusercontent.com/94120618/156773195-22e4d838-1157-4860-9418-60dd3dd314e0.png)

As we can see , the exercise duration of each group is pretty identical.Every group have the same interquartile range , median and so on.
In addition, the duration is very similar for males and females in old and middle-aged groups.But in youth, males outperformed.
Another tip is, the median exercise duration of this dataset is about 15 minutes
![Screenshot (249)](https://user-images.githubusercontent.com/94120618/156773440-aab3da1d-7b33-4a3f-89c3-d39a0dce5867.png)

As we can see the Categorized_BMI is identically distributed between age groups(the sequence is identical, for example in both Normal and Overweight ; Young comes first , 'Middle-Aged` comes second , etc.)
An interesting thing is , about 50% of old individuals have Normal weight and another 50% are Overweight.
![Screenshot (254)](https://user-images.githubusercontent.com/94120618/156773599-21a50668-2477-48c9-b085-24c442a8684e.png)

we plotted the scatter plot for the duration of exercise and heart rate on size of calories.From that when the people do more exercises more heart rate and theor
calories also burning high.
![Screenshot (255)](https://user-images.githubusercontent.com/94120618/156773983-a9007d10-bf03-4545-9ad6-764de43b4bf6.png)

# Building Regression Model
Since it is a Regression Dataset we are going to use different algorithms
<ul>
<li>Linear Regression
<li>RandomForest Regressor
<li>AdaBoost Regressor
<li>Decision Tree Regressor
<li>Ridge Regression
<li>XGBoost Regression
</ul>

# Regression Evaluation Metrics

we use diffrent evaluation metrics to Evaluate our model
<ul>
<li>MAE
<li>MSE
<li>RMSE
</ul>

![Screenshot (261)](https://user-images.githubusercontent.com/94120618/157043801-2985753b-95cd-44ec-ac3c-8a67567a34f9.png)


By plotting the Mean Absolute Error value it shows that XGBoost Regressor giving better results when comparing with other algorithms be the better for MAE.


![Screenshot (262)](https://user-images.githubusercontent.com/94120618/157043875-a8b41cc4-627d-409f-9202-fa6aa7cdd9e5.png)


By considering the Mean squared Error values it shows that XGBoost Regressor giving better result for MSE values.


![Screenshot (263)](https://user-images.githubusercontent.com/94120618/157044463-04b5ae04-5ff5-44f3-8bf7-7411f81cbde1.png)


By consideration of Root Mean Squared Error XGBoost Regression giving better prediction for RMSE.

By comparing MAE, MSE, RMSE of all algorithms XGBoost Regressor will make the better prediction when compared to other algorithms.
