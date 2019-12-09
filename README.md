# US-Accident-Risk-Prediction
Machine Learning algorithms are utilized for accident risk prediction

##### Team Members:
1. Nagajanaki Dwadasi (013853034)
2. Rama Tejaswini Thotapalli (013785681)
3. Priyanka Kumar (013749866)
4. Vaidehi Naik (012560938)


### Dataset: https://www.kaggle.com/sobhanmoosavi/us-accidents

#### Abstract:

Given the challenges of public safety today, research and analysis of real-time traffic and accident data to predict the risk of accidents is ubiquitous. Accident risk prediction can significantly improve public safety by warning the public. In this paper, the probability of accident risk for a given case with selected conditions is predicted. Features like weather, traffic volume, road conditions, time of the day, description of previous accidents are utilized from the dataset. Machine learning algorithms like Logistic Regression, Support Vector Machines (SVM), Decision Tree, Neural Networks are used and their results are compared to provide the best prediction.

#### Data Preprocessing:

##### Feature Selection: 
Features are selected based on their importance and correlation observed in the visualizations from exploratory data analysis. Selected features majorly contribute to determine the effect of road conditions and a few weather conditions to predict accident risk. Features related to road conditions include Amenity, Bump, Crossing, GiveWay, Junction, NoExit, Railway, Roundabout, Station, Stop, TrafficCalming, TrafficSignal, TurningLoop. Features related to weather conditions include Temperature(F), WindChill(F), Humidity, Pressure(in), Visibility(mi), WindDirection, WindSpeed(mph), Precipitation(in), WeatherCondition, SunriseSunset.

##### Data Pre-processing: 
In the Data Preprocessing step, data cleaning techniques like removing null valued rows and columns, filling the null values with median and mode are performed. Data scaling using standard scaler on train data and normalization are performed. Data transformation using Label encoder, One Hot encoder are performed. As the label of the dataset is very skewed, the label of the data contains very few elements of the 0 class and very high elements of 4 class. So, the data of 0 class is skewed and need to do sampling of the dataset. We performed under sampling of the data by combining both classes of 0 and 1 to 8Dimensionality reduction is performed using Principal Component Analysis (PCA). Parameter tuning using Grid Search CV is performed.
 
##### Model Implementation: 
In this step, several models are implemented on the preprocessed dataset. The models implemented include the following

1. Logistic Regression
2. K Nearest Neighbors (KNN)
3. MLP Classifier
4. Decision Tree
5. Random Forest Classifier
6. Ensemble Modeling

##### Evaluation methods:

1. Accuracy Score
2. Confusion matrix
3. Cross validation score
