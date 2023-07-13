# Approch towards the problem statement to predict the product length :

### 1) Importing necessary libraries:
The code starts by importing several libraries such as Pandas, xgboost, Seaborn, Scikit-learn, NumPy, Matplotlib, and others. These libraries are essential for data analysis and machine             learning tasks

### 2) Reading the data:
The code reads the training and test data from two CSV files using the read_csv() function from Pandas. The training data is stored in a DataFrame named 'train_data' and the test data is stored in a DataFrame named 'test_data

### 3) Printing summary of the training data:
The describe() function from Pandas is used to print a summary of the training data which includes statistical information such as mean, standard deviation, minimum, maximum, etc. for each numerical feature. This helps to understand the distribution of data and detect outliers or missing values

### 4) Encoding categorical features:
The code then encodes categorical features using LabelEncoder from Scikit-learn. The 'DESCRIPTION', 'BULLET_POINTS', and 'TITLE' columns are encoded and converted from strings to floats using the fit_transform() and astype() functions. This is necessary as most machine learning models only work with numerical data

### 5) Preparing the data for the model:
After encoding the categorical features, the code prepares the data for the model by dropping the 'TITLE' column from the training and test data sets and setting 'PRODUCT_LENGTH' as the target variable for the model. The drop() function is used to remove the 'TITLE' column from the data sets and the values attribute is used to extract the values from the data sets

### 6) Initializing and training the model:
The code initializes an XGBRegressor model with default parameters and fits it on the training data using the fit() function from XGBoost. The model is trained to predict the 'PRODUCT_LENGTH' based on other features in the training data

### 7) Evaluating the model:
The code does not explicitly evaluate the performance of the model on the training or test data. However, this is an essential step in any machine learning task to ensure that the model is not overfitting or underfitting the data

Overall, the given code performs several data preprocessing tasks and fits an XGBRegressor model on the training data to predict the target variable 'PRODUCT_LENGTH'. The code can be further optimized and improved by fine-tuning the parameters of the model, performing feature engineering, and evaluating the performance of the model on the test data

~ The online evaluation score we recieved using this model is = 31.20856 ~
