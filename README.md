# ICC_World_Cup_2023_Prediction🏏
## Course Project 3 of Data Mining Course

* This Project aims to predict:
  1. Predicting the batsman who will score most runs/ hit most sixes/ make most centuries in the tournament.
  2. Predicting the target run scored by the team bats first in semi finals.
  3. Predicting the Finalist Teams and Players
  4. Predict the Winner of ICC Cricket World Cup 2023

## Basic Flow of the Event:
* Data Scraping/ Collection: We collected the data required in all the predictions. We considered the ODI data ranging from past 1 year to 50 years.
  1. Major data columns used:
     * Team1 Name
     * Team2 Name
     * Score
     * Batsman information
     * Baller information
     * Venue
     * Result
     * Date
    
* Data Preprocessing: To ensure the quality and preparation of the input data, We preprocessed every dataset used in our model as per the requirements.
    1. Data Cleaning: Cleaned the data scrapped as per the requirements. handled missing values by removing rows or replacing it with 0/mean and removing the duplicate values.
    2. Encoding Categorical data: Machine learning works on numeric data hence categorical data which are not of the type float/int has to be converted into numeric values. We done it by LabelEncoding/OnehotEncoding.
    3. Splitting the Dataset into the Training set and Test set: Splitted the data into training set and testing set as per the standard ratios.
    4. Feature Scaling: It helps ensure that all features contribute equally to the model training process. We used StandardScaler class of sklearn.preprocessing
   
* Feature Selection: Used EDA stats, correlations to extract the necessary features and removed redundant, noisy and irrelevant features. it plays crucial role on optimizing and enhancing model performance and reducing computational complexity.

* Model Training:
  1. Performed Deep neural network model considering activation function, class weight, batch normalization, kernel initializer, kernel regularizer, batch size and early stopping.
 

* Model Evaluation

* Prediction

* Deployment
     
  
