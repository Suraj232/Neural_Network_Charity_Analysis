# Neural_Network_Charity_Analysis
## ANalysis Overview

The major purpose of this analysis is to use deep-learning neural network by using TensorFlow platform in GoogleColab.
The steps included througout the process are as follows:
- Preprocessing the data and spliting it accordingly
- Complie, train and evaluate the model
- Optimize the model

## Results
### Data Processing

- "EIN" and "Name" columns are dropped from the data which are basically distinct from eachother.
- The data is futher analyzed. The data has a unique value more than 10 in Application type and Classification. The binning process is carried out where the data with low value is grouped together to a category called others.
- The OneHotEncoder method is used to value the data. Encoding of the categorical variables, spliting into training and testing datasets and standardization have been applied to the features.
- The data is split by taking Is_Successful column which contains binary data refering to, if the charity donation was used effectively. 

### Compiling, Training, and Evaluate the Model
- The deep-learning nueral network model is made of two hidden layer. The activation model used here is ReLU for hidden layers. As our output is a binary classification, Sigmoid is used on the output layer.
- During compile, the loss function used is binary_crossentropy, metrics used is Accuracy and optimiazer is adam.
- The model accuracy is under 75%. This is below satisfying performance to predict the outcome of the charity donation.
- To increase the performanec of the model, we applied and organized the different values. The  number of neurons were changed.
- The activation function for all the optimizitions try were used different (tanh, sigmoid), but none of the changes helped improve the models accuracy.

## Summary

The model did not reach above 75 % of accuracy. Eventhough the accuracy seems to be avarage, the model is not outperforming.
As ita a binary classification situation, we could only use a supervised machine learning model such as the Random Foredst Classifier to combine a decision tress to generate a classified output and evaluate its performance against the neural network model.
