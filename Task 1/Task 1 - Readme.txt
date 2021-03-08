
Loading the dataset using pandas
Splitting the data into dependent and independent variables
Splitting the data into training and test

Feature scaling the training and testing data



Calculate the entropy of the total dataset
Calculate the values and the corresponding counts for the split attribute 
Calculate the weighted entropy
Calculate the information gain


If the dataset is empty, return the mode target feature value in the original dataset
If the feature space is empty, return the mode target feature value of the direct parent node
the direct parent node is that node which has called the current run of the ID3 algorithm and hence
the mode target feature value is stored in the parent_node_class variable.
If none of the above holds true, grow the tree!

Select the feature which best splits the dataset
Create the tree structure. The root gets the name of the feature (best_feature) with the maximum information
gain in the first run
Remove the feature with the best inforamtion gain from the feature space
Grow a branch under the root node for each possible value of the root node feature
Split the dataset along the value of the feature with the largest information gain and there with create sub_datasets
Call the ID3 algorithm for each of those sub_datasets with the new parameters(recursion)
Add the sub tree, grown from the sub_dataset to the tree under the root node
We drop the index respectively relabel the index
starting form 0, because we do not want to run into errors regarding the row labels / indexes
Train the Random Forest model
Create a list in which the single forests are stored
Create a number of n models
Grow a tree model for each of the training data
We implement the subspace sampling in the ID3 algorithm itself. Hence take a look at the ID3 algorithm above!
Predict a new query instance

Using RandomForestClassifier to fit the model from sklearn 
Using  Matplotlib to plot the test data Age in x-axis and Estimated Salary in y-axis