# TitanicSurvivalPrediction_NAIVEBAYES
Based upon NAIVEBAYES algorithm I have predicted whether the person has survived the Titanic incident or not
Check Python File And .ipynb File

Description
**Domain**
**Titanic Survival Data Analysis
**

 **Problem**
**Titanic Survival Prediction based on Some Parameters**
We have to predict whether a person survived the Titanic Survival or not using parameters(age,gender,health report) and its a classification

**Collecting Data**
Input :- Age,Pclass,Sex & Fare
Output :- Survived or Not
Based on Age,Pclass,Sex & Fare,we gonna predict whether the person might survived or not.

**Load & Summarize Datase**
Load Dataset from the Directory &
Summarize the details such as no.of Rows and Columns & Content
Datase.shape() -Function to get No. of Rows & Columns
Dataset.head(5)  - Funtion to Display 1st  5 rows of Dataset

**Mapping Gender Text Data to Binary Numbers**
If the data is male then it it gonna be mapped to 1,
Female to 0

**Segregating Dataset into X & Y**
Dataset  
X = dataset.drop('Survived' , axis ='columns')  -  dataset.drop-To remove column
Y = dataset.Survived	-Pick the certian Column

**Splitting Dataset to train & Test** 
Useful For Validation
train_test_spilt(X, Y ,test_size=0.25 ,random_state=0)

**Identify & Replacing NaN values in dataset**
X.isna().any()  - Checking for Nan 
X.Age.fillna(X.Age.mean())  - Replacing NaN values with Mean of that certain feature


**Algorithm**
naive_bayes - bases on bayes Theorem
Main Factor about this Theorem we are going to find out the probibility of event occuring from the event occured on the past

**Training**  
Training our Model for Pre-Processing Dataset
Model.fit(X_train, y_train)

**Validation**
Obtaining the accuracy of the model
Accuracy Score

**Prediction**   
Observing how our model is classifying our new data
result = model.predict(preson(Data))


**Note**:-As data is already loaded and mapping is done so avoid mapping again and again as female is not present so it will give error so better to start from load if any condition occured


  



