# DSProject2-PredictingAirbnbPrice

This Capstone project aims to develop a machine learning model that predicts the price of an Airbnb rental unit given the features of the property. The goal is to provide pricing strategies and informed decision-making in the Airbnb marketplace. 

I decided to narrow the focus of my project to Toronto, the city I was raised and currently live in. This made it interesting to explore the differnet locations within the city that I recognized and explore various trends among them. The data is taken directly from Airbnb and had a lot of work to do in preparation for the analysis. 

**Data Wrangling & Exploratory Analysis** 

The raw dataset was taken from the official Airbnb website for the city of Toronto, which featured 75 columns and 17,997 unique rows. There was a breadth of data available to work with, however, it required ample cleaning and reduction in order to draw quality insights from it. I also imported a dataset that contained neighbourhood and borough information in Toronto to create more specific features for analysis. 

The Wrangling and EDA portion of the project served to clean the dataset of inconsistencies, explore the data and find feature correlations to our price target. One such tool of course was a heatmap:
![heatmap](https://github.com/user-attachments/assets/f15fe559-e547-4405-8bb6-ca2287298849)

**Modeling**

The models used to predict the price of listings were the following:
1. Linear Regression
2. Ridge and Lasso Regression
3. Random Forest Regressor

The Random Forest Model performed the best. Furthermore I also ran a RF model with a max depth of 2 to simulate an investor's best estimaation of price given that they are not utilizing any form of ML model to make decisions. 

<img width="537" alt="Screen Shot 2024-09-30 at 10 32 21 AM" src="https://github.com/user-attachments/assets/6846d514-4cd3-4756-b87b-ace921df91be">

Model 1 outperforms the latter by 25% in explaining the variance in the dependent variable. Similarly, it also shows better accuracy in its predictions with a lower MAE of 39.84, a difference of 13.22. For context, stakeholders leveraging the model could optimize their pricing strategy more effectively compared to those neglecting the model. This discrepancy in application could translate into a $13.22 variation in unit price per night. Such a disparity holds substantial ramifications for return on investment (ROI) over the long term, potentially accumulating to thousands of dollars across multiple years.

<img width="726" alt="Screen Shot 2024-09-30 at 10 33 09 AM" src="https://github.com/user-attachments/assets/34e4ecad-89f7-4693-9dab-dfd3673b54cf">
