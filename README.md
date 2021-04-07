# int-247-km007-ca-2-praveenkumar

## DATA OVERVIEW 

Elevation - Elevation in meters

Aspect - Aspect in degrees azimuth

Slope - Slope in degrees

Horizontal_Distance_To_Hydrology ** - Horz Dist to nearest surface water features**

Vertical_Distance_To_Hydrology - Vert Dist to nearest surface water features

Horizontal_Distance_To_Roadways - Horz Dist to nearest roadway

Hillshade_9am (0 to 255 index) - Hillshade index at 9am, summer solstice

Hillshade_Noon (0 to 255 index) - Hillshade index at noon, summer solstice

Hillshade_3pm (0 to 255 index) - Hillshade index at 3pm, summer solstice

Horizontal_Distance_To_Fire_Points - Horz Dist to nearest wildfire ignition points

Wilderness_Area (4 binary columns, 0 = absence or 1 = presence) - Wilderness area designation

Soil_Type (40 binary columns, 0 = absence or 1 = presence) - Soil Type designation

Cover_Type (7 types, integers 1 to 7) - Forest Cover Type designation

## Dataset Source

Link for dataset can be found in https://archive.ics.uci.edu/ml/datasets/covertype

## Preprocessing
###### Standard Scaler
Datas are Standard scaled because distace based machine learning algorithms are used
###### Principle Component Analysis
Used PCA for dimentionality reduction to make use of important feature selection for the model.


## Models
###### Random Forest Classifier with Hyperparameter Tuning
In the case of a random forest, hyperparameters include the number of decision trees in the forest and the number of features considered by each tree when splitting a node. (The parameters of a random forest are the variables and thresholds used to split each node learned during training). Scikit-Learn implements a set of sensible default hyperparameters for all models, but these are not guaranteed to be optimal for a problem. The best hyperparameters are usually impossible to determine ahead of time, and tuning a model is where machine learning turns from a science into trial-and-error based engineering.

###### KNearest Neighbors with Hyperparameter Tuning
In case of KNearest Neighbors the hyperprameter includes the value of K which determines the nearest point with them

###### Support Vector Machine with Hyperparameter Tuning
SVM creates a decision boundary which makes the distinction between two or more classes. How to draw or determine the decision boundary is the most critical part in SVM algorithms. When the data points in different classes are linearly separable, it is an easy task to draw a decision boundary.

## Metrics
###### Confusion matrix
confusion matrix is a tabular way of visualizing the performance of your prediction model. Each entry in a confusion matrix denotes the number of predictions made by the model where it classified the classes correctly or incorrectly.

## Exploratory Data Analysis



