# Hotel Booking Prediction

### Problem Statement:

When we plan a business trip or a family trip the first thing, we think about is where do we stay? It is quite normal that we might make a booking at a hotel for a few days and at the last minute due to sudden change in plans, we may cancel the booking. Hotels generally come across this behavior and quite a times they must drop a customer due to
the existing booking due to which their revenue is highly affected. Therefore, using classification models, we are trying to leverage the guest dataset and perform an analysis of the Room Booking Behavior Pattern and then devise a strategy for the Hotel Revenue Management.

---
### Dataset Description:

The Dataset set contains 1.1 million observations and 33 Columns. 
https://www.kaggle.com/code/sanjana08/hotel-booking-cancellation-prediction/data

---
### Methodology:

1. We obtained the dataset from Kaggle.
2. We extracted dataset into SQL lite database, removed and modified the incomplete, null, and duplicate data.
3. Normalized the database and imported the data into the Jupyter notebook for the analysis.
4. Performed Bi-variate analysis and created derived variables and then created a new table with updated columns.
5. Bi-variate analysis is performed by generating various bar plots to understand the trend between features and the target variable.
6. Then we split the dataset to the Training set (70%) and testing set (30%).
7. Applied machine learning classification models to the dataset. Machine learning models used for the training were: Logistic regression, Decision Tree Classifier, andRandom Forest Classification.
8. Constructed a dashboard with insights into the data.

---
### Analysis:

The features are compared with the target in order to find the best features that maintain a trend with the target variable, this comparison is called Bi-variate analysis.
The following bar graphs plotted are used to compare features with the target variable ‘is_cancelled’:
1. Is_canceled vs meal
2. Is_canceled vs is_reapeated guest
3. Is_canceled vs market_segment
4. Is_canceled vs arrival_date_month
5. Is_canceled vs stay_in_weekend_nights
6. Is_canceled vs stay_in_week_nights
7. Is_canceled vs previous_cancellation

On comparing the features with the target variable we see a change of trend between the 3,4,5,6 and 7 from which we can deduce that the above features will be a good fit for our model.

---
### Result:

Classification models are applied to the dataset with new filtered features, and we generated a confusion matrix and a classification report which are the metrics used to test the classification models.
1. Accuracy of logistic regression on test set: 0.62
2. Accuracy of Decision Tree on test set: 0.84
3. Accuracy of Random Forest on test set: 0.82

The decision tree gave us the best accuracy for the dataset compared to the Logistic Regression and Random Forest models.
Comparing the models, it can be said that Random Forest has made the best prediction as it tends to prevent overfitting.
The Receiver Operating Characteristics graph is plotted to compare the number of False Positive rates and True Positive rates of all three models.

---
### Conclusion:

The main objective of the project was to generate a report for the Hotel Revenue Management team and to understand the trend in the cancellations done by the various customers over the period of time. This will help the hotel revenue team analyze and make sure that the customer who has currently made a reservation will be staying in the hotel or not, or is he/she likely to cancel the reservation. This way the hotel can take up reservations from other customers and keep the business running.










