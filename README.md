# Seattle-Boston-Airbnb-Data-Analysis


## CRISP-DM

* ### Business Understanding

    The key idea of Business Understanding is to understand the problem and find questions that you are interested in answering.
    There are two strategies for arriving at the questions of interest.
    You might not have any data, but you might have questions that are interesting. In this case, collect the necessary data in order to answer those questions.
    You have the data and you get familiar with the data to come up with questions of interest.

    **The questions of interest for the Seattle/Boston datasets are as follows:**
 
    * Anticipated visitors to Seattle/Boston over time 
    (based on non availability of listings)?

    * Areas that are more likely to be crowded/ areas that are more likely to be 
      preferred by people (based on the number of bookings)?
     
    * The busiest time to visit Seattle/Boston?

    * Compare the average daily price of listings for a month over time (between the two cities).

    * Predict the price of listings for Seattle/Boston.
 
    
* ### Data Understanding

    Now we have the question, we need to move the question into the data. Find the columns from the datasets that would answer these questions.
    
    **The columns identified to answer the necessary questions are as below:**

   * Anticipated visitors to Seattle/Boston over time 
   (based on non availability of listings)?
     - date, accommodates (columns)
   * Areas that are more likely to be crowded/ areas that are more likely to be 
     preferred by people (based on the number of bookings)?
     - neighbourhood, zipcode (columns)
   * The busiest time to visit Seattle/Boston?
     - date, accommodates (columns) : Seattle-July, Boston-March.
   * Compare the average daily price of listings for a month over time (between the two cities).
     - price, date, weekly_price, monthly_price (columns) from calendar.csv
   * Predict the price of listings for Seattle/Boston.
     - property_type, room_type, neighbourhood, zipcode, accommodates, 
      bathrooms, bedrooms, beds, cleaning fee, instant_bookable, 
      cancellation_policy (columns or more) 


* ### Data Preparation

    [Data Preparation](https://github.com/jyothishkjames/Seattle-Boston-Airbnb-Data-Analysis/blob/master/data_prepration_modeling_evaluation.ipynb)
    
    The data preparation has various rigorous steps including the following:
    * Filling missing data
    * Removing data
    * Transforming data
* ### Modeling

    [Modelling](https://github.com/jyothishkjames/Seattle-Boston-Airbnb-Data-Analysis/blob/master/data_prepration_modeling_evaluation.ipynb)
    
    For predicting the price of listings, we split the prepared data into train and test data. The training data is then used to fit the linear model. Thereafter, the test data is used to test the linear model.

* ### Evaluation

    [Evaluation](https://github.com/jyothishkjames/Seattle-Boston-Airbnb-Data-Analysis/blob/master/data_prepration_modeling_evaluation.ipynb)
    
    For the evaluation, we use the r-square score to get an understanding of how well our model works. The price prediction for Seattle has an r-square score of .528 on test data, which is higher as compared to Boston which an r-square score of .206. The closer the score is to 1, the better your model fits the data.
* ### Deployment

    Deployment is the stage where we applying the conclusion to our Business.  To recap, the conclusions are based on the statistical inference and the model prediction.