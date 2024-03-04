# Module_13_Challenge

## Deep Learning Models

### Data Preparation

The objective of this challenge is to prepare the data for analysis using neural network models and develop deep learning models for predictive success of venture funding investments. The Data pertains to a Alphabet Soup's ,a hypothetical firm, venture funding investments. 

The first step was to prepare the data to be used on neural network model. Here, using pandas functions like shape, info and drop, the data structure is analysed to understand the features and target variable. Those data points which do not have predictive relevance like Employer ID and Name were dropped. Then, using OneHotEncoder the categorical data is transformed to numerical type.  

The dataframe is split into X(predictors) and y(target) data. Further, using scikit learn's train and test split function, the entire data is randomly divided into training and testing samples for using in the ML model. The train data is next normalized using StandardScaler to reduce th impact of large numbers.


### Model Building

Now, using Tensorflow Keras library, neural network model is initialized to predict the binary classification problem. The first model uses 2 hidden layers with 10 nodes each and ReLU activation function, with sigmoid function for output layer. To compile the model, adam optimizer and binary crossentropy as loss function is used with accuracy metric for output display. The model is then fit to the train data with test data as validation set and 50 epochs. The result is a model with Loss: 0.5557 and Accuracy: 0.7280.

Next, two alternate models with chnages in number of nodes in hidden layer, adding a dropout layer and changing activation function to tanh are used to redevlop models to check for improved accuracy.  

