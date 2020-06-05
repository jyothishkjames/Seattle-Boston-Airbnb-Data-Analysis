# Seattle-Boston-Airbnb-Data-Analysis

The motivation of this project is to get as much as insights from the Seattle/Boston datasets 
to answers our questions of interest, which are crucial for business decision-making.

Data analysis is the process of cleaning, transforming, and modelling data to find useful insights that are beneficial for business decision-making. CRISP-DM is a structured approach that makes the life of a data scientist easier.

Prerequisites
-------------
The following libraries are used for the project:

        numpy
        pandas
        matplotlib
        seaborn
        sklearn



## CRISP-DM

* ### Business Understanding

    The key idea of Business Understanding is to understand the problem and find questions that you are interested in answering.
    
    There are two strategies for arriving at the questions of interest:
    
    * You might not have any data, but you might have questions that are interesting. In this case, collect the necessary data in order to answer those questions.
    
    * You have the data and you get familiar with the data to come up with questions of interest.

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
     - date, accommodates (columns) 
   * Compare the average daily price of listings for a month over time (between the two cities).
     - price, date (columns) from calendar.csv
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
    
    For the evaluation, we use the r-squared score to get an understanding of how well our model works. The price prediction for Seattle has an r-squared score of .517 on test data, which is higher as compared to Boston which has an r-squared score of .313. The closer the score is to 1, the better your model fits the data.
* ### Deployment

    Deployment is the stage where we applying the conclusion to our Business.  To recap, the conclusions are based on the statistical inference and the model prediction.
    
 ## Summary of Data Analysis
 
 Form the statistical analysis, it was found that the busiest time to visit Seattle is in January and for Boston is in September. It was also inferred that the
 neighbourhood Capitol Hill was most likely to be preferred by visitors to Seattle. For Boston, the visitors preferred the neighbourhood Allston-Brighton. 
 
 ## Link to the Blog
  
 [Link to the Blog](https://medium.com/@jyothishlp/crisp-dm-approach-for-data-analysis-468ec2d5b2dd)  