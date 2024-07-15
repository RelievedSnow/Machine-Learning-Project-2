# Machine-Learning-Project-2
# Project 2: Diabetes Prediction.
Dataset Link: https://www.dropbox.com/scl/fi/0uiujtei423te1q4kvrny/diabetes.csv?rlkey=20xvytca6xbio4vsowi2hdj8e&e=4&dl=0 

# Step 1: Importing Dependencies
* importing numpy for converting the 'input_data' into numpy array.
* importing pandas to read the '.csv' file.
* importing accuracy from sklearn.metrics libraby.
* importing'Support Vetor Model' from sklearn library.
* inporting 'test_train_split' from sklearn.model_selection.

# Step 2: Data Collection And Pre-Processing.
* Using the pandas library to read from the .csv file and storing it into a 'pd' variable.
* Using the .head() function to read the 1st five values from the Dateset.
* Using the .shape method to check the No. of Rows and Columns in the Dataset.
* Using the .describe() function for checking the statistical measures of the Dataset.
* Using the .value_counts() function to Count the No. of 0's and 1's in the labelled ['Outcome'] Data(0 = Non-Diabetic, 1= Diabetic).
* Using groupby() function on the ['Outcome'] labelled Data to find the mean of each Feature Depending on 0's and 1's.
* We now Seperate the labelled Data from Numerical Data using the drop function and storing the remaining features into the 'X' variable and only the labelled Data into the 'Y' variable.

# Step 3: Data Standardization.
* We store all the method/function from StandaredScaler() library.
* We now Fit the Numerical Dta('X') into the 'Scaler' Variable.
* After fitting it into the Scaler Variable we Transform it and store it into another variable 'standardized_data'.
* We store the 'standardized_data' back into the 'X' variable.

# Step 4: Train Test Split.
* We split the Data into Training Data and Testing Data using the train_test_split.

# Step 5: Training the Model.
* We store all the Model funtioncs into the 'classifier' variable.
* We fit the train_data and test_data into the classifier variable to insert it into the model.

# Step 6: Model Evaluation.
* We evaluate the 'accuracy_score' of the 'training data' and 'test data'.

# Step 7: Making Predictive System.
* We create a variable 'input_data' to enter the input values as list.
* We reshape the input data from 1-D to 2-D as we are providing it in 1-D form.
* We convert the 'input_data_reshaped' value into standardized data as we have provided the model with 'standardized_data'. So if we provide raw values it will fail to predict.
* Now we make predictions.
