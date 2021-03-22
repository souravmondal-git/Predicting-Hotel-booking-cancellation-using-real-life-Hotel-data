# Predicting-Hotel-booking-cancellation-using-real-life-Hotel-data

Predicting hotel booking cancellations is an interesting problem in the hospitality industry. Recent advancements in computational power and algorithmic research made it possible to build Machine Learning models that can predict the booking cancellations efficiently. 

![hotelsashkinsstock](https://user-images.githubusercontent.com/70813394/111965184-78ae5180-8b1b-11eb-923d-a52996fd1fed.png)

In this problem I had booking cancellations data which consists of 119390 samples for 31 input features from different 'City Hotels' and 'Resorts'. Depending on the input features and the labeled output variable feature 'is_canceled' one can buid supervised models which can predict the output label of the unseen data. Before starting to build the model I needed to clean, analyse and the data. At the very behinning of this project I randomly sampled out a portion of the data, which I could use as unseen data to test my model. For the rest data I cleaned it using standard imputation techniques for the missing values and removed some fetures having considerably large number of missing values. (for example the feature 'company' having 94.29% of the data were missing. That feature indivcates the ID of the company/entity that made the booking or responsible for paying the booking.) Detailed study of the data shows there are some samples for which number of adults, childs and babies are zero at the same time which is suspicious. So I removed those features. Using Plotly I visualised the country of origin of the guests.

![Screen Shot 2021-03-22 at 2 59 55 PM](https://user-images.githubusercontent.com/70813394/111969196-fb391000-8b1f-11eb-8425-7b05747f994f.png)

After the data cleaning and analysis of numerical features I have used Bayesian Target encoding for the categorical features as they had high cardinality.

