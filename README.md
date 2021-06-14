# Restaurant-Segmentation-And-Prediction-System
A system that recommends whether a customer will order from a vendor or not!
The aspiration of this case study is to develop a prediction cum recommendation system to predict the vendors from which customers are most expected to order. These customers can have varied locations, various orders and distinctive vendors as well. Hence, we have to predict utilising addressed customer location, restaurant information, and customer order history.
This business answer will provide Akeed, an app-based food delivery service in Oman, to customise restaurant recommendations for each of their customers and guarantee a more convincing overall user familiarity with more reliable classifications.
Akeed's concept is to be the delivery and discovery platform for everything people demand spontaneously. Akeed resembles the dimensions of food delivery by taking the order, routing it to a restaurant, picking up the order and delivering it to the customer.
Constraints:
No low-latency requirement.
Submitted code must run on the original train, test, and other datasets provided.

A. DATA FORMATS:
There are 10,000 customers in the test set. These are the customers you will need to recommend a vendor to. Each customer can order from multiple locations (LOC_NUM). There are 35,000 customers in the train set. Some of these customers have made orders to at least one of 100 vendors.
There are the following datasets that are available to us in this case study.
1.test_customers.csv - customer id's in the test set.
2.test_locations.csv - latitude and longitude for the different locations of each customer for the test data.
3.train_locations.csv - customer locations details in the training dataset.
4.train_customers.csv - latitude and longitude for the different locations of each customer for the train data.
5.orders.csv - orders that the customers train_customers.csv from made.
6.vendors.csv - vendors that customers can order from and their respective details.
7.VariableDefinitions.txt - Variable definitions for the datasets
B. STRUCTURE OF FINAL SUBMISSION:
The competition demanded the final structure of the predicted file.
SampleSubmission.csv - is an example of what our submission file should look like. The order of the rows does not matter, but the names of CID X LOC_NUM X VENDOR must be correct. The column "target" is our prediction. Target 1 means The customer CID will have the highest chance of taking orders from vendor VENDOR, and 0 means, CID will not order at all from the vendor.
C. PERFORMANCE METRICS
The error metric for this competition is the F1 score, which ranges from 0 (total failure) to 1 (perfect score). Hence, the closer your score is to 1, the better your model.
1. Precision :
This is an indicator of the number of items correctly identified as positive out of the total items identified as positive. The formula is given as TP/(TP+FP)
2. Recall / Sensitivity / True Positive Rate (TPR)
: This is an indicator of the number of items correctly identified as positive out of total actual positives. The formula is given as TP/(TP+FN)
3. F1 Score:
A performance score that combines both precision and recall. It is a harmonic mean of these two variables. The formula is given as 2*Recall/(Precision + Recall)
TP=True Positive, FP=False Positive, TN=True Negative, FN=False Negative
