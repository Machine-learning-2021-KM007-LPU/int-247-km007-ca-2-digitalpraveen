# int-247-km007-ca-2-praveenkumar

# Forest Cover Type
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
![standardization](https://user-images.githubusercontent.com/54984891/113806375-ca8fe200-977f-11eb-92ff-99afde238409.png)

###### Principle Component Analysis
Used PCA for dimentionality reduction to make use of important feature selection for the model.
![PCA](https://user-images.githubusercontent.com/54984891/113806399-d67ba400-977f-11eb-9d3d-acecc557333e.png)



## Models
###### Random Forest Classifier with Hyperparameter Tuning
In the case of a random forest, hyperparameters include the number of decision trees in the forest and the number of features considered by each tree when splitting a node. (The parameters of a random forest are the variables and thresholds used to split each node learned during training). Scikit-Learn implements a set of sensible default hyperparameters for all models, but these are not guaranteed to be optimal for a problem. The best hyperparameters are usually impossible to determine ahead of time, and tuning a model is where machine learning turns from a science into trial-and-error based engineering.

![RF](https://user-images.githubusercontent.com/54984891/113806416-e0050c00-977f-11eb-906e-78c3f8b79fdb.png)


###### KNearest Neighbors with Hyperparameter Tuning
In case of KNearest Neighbors the hyperprameter includes the value of K which determines the nearest point with them

![KNN](https://user-images.githubusercontent.com/54984891/113806455-ef845500-977f-11eb-867c-3cdaa38c34c6.png)

###### Support Vector Machine with Hyperparameter Tuning
SVM creates a decision boundary which makes the distinction between two or more classes. How to draw or determine the decision boundary is the most critical part in SVM algorithms. When the data points in different classes are linearly separable, it is an easy task to draw a decision boundary.

![SVM](https://user-images.githubusercontent.com/54984891/113806488-fc08ad80-977f-11eb-9b25-0ccb37993ba9.png)


## Metrics
###### Confusion matrix
confusion matrix is a tabular way of visualizing the performance of your prediction model. Each entry in a confusion matrix denotes the number of predictions made by the model where it classified the classes correctly or incorrectly.
###### Random Forest Confusion Matrix
![RFCM](https://user-images.githubusercontent.com/54984891/113806215-8a306400-977f-11eb-829b-35fdc9bf8814.png)

###### KNearest Neighbors Confusion Matrix
![KNNCM](https://user-images.githubusercontent.com/54984891/113806266-9c120700-977f-11eb-81b8-28d685efd5da.png)

###### Support Vector Machine confusion Matrix
![SVMCM](https://user-images.githubusercontent.com/54984891/113806315-b1873100-977f-11eb-8281-070223d3c21f.png)



## Exploratory Data Analysis
###### Count plot for analysing Target feature
![countplot](https://user-images.githubusercontent.com/54984891/113806040-3e7dba80-977f-11eb-903c-544ef7066163.png)

###### Heatmap for checking corelation
![Heatmap](https://user-images.githubusercontent.com/54984891/113806153-7258e000-977f-11eb-8d9f-63c800e93d17.png)







