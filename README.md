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
     * Venue(Ground)
     * Result
     * Date
    
* Data Preprocessing: To ensure the quality and preparation of the input data, We preprocessed every dataset used in our model as per the requirements.
    1. Data Cleaning: Cleaned the data scrapped as per the requirements. handled missing values by removing rows or replacing it with 0/mean and removing the duplicate values.
    2. Data Integration: Data files coming from different sources and in different formats, we need to merge them appropriately.
    3. Encoding Categorical data: Machine learning works on numeric data hence categorical data which are not of the type float/int has to be converted into numeric values. We done it by LabelEncoding/OnehotEncoding.
    4. Splitting the Dataset into the Training set and Test set: Splitted the data into training set and testing set as per the standard ratios.
    5. Feature Scaling: It helps ensure that all features contribute equally to the model training process. We used StandardScaler class of sklearn.preprocessing
   
* Feature Selection: Used EDA stats, correlations to extract the necessary features and removed redundant, noisy and irrelevant features. it plays crucial role on optimizing and enhancing model performance and reducing computational complexity.

* Model Training:
  1. Performed Deep neural network model considering activation function, class weight, batch normalization, kernel initializer, kernel regularizer, batch size and early stopping. We tried out many different configurations of the network architecture and settled on the one which gave us better accuracy and less overfitting.
  2. We also used RandomForestClassifier and RandomForestRegressor and tried different hyperparamer values - especially max_depth which affected the extent of overfitting. We observed that this model was giving pretty good results on almost all the datasets.
  3. We tried out XGB as well, as expected it was performing good on the datasets with small number of instances.
 

* Model Evaluation:
 1. In the multi-class classification problems, the loss function used is categoriacal cross-entropy. We had to use different nomenclatures according to the specific model that we are using. For example - XGB class reffered to the same loss as 'mlogloss'. The models were judged based on accuracy and the loss functions were used to train the models.
 2. For regression problems, the usual mean square error was used as the loss function and the models were trained and judged based on the same.
  
* Prediction
  Finally, the input data for which we wanted to predict was fed to the trained classifiers/regressors and the desired predictions were obtained.

* Deployment
     
  
