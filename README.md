# dnn
Boston House prices Predictions using Deep Neural Network
This program code is written in python  for building and training a neural network to predict house prices using the Boston Housing data-set.  Following are the steps for implementation:
1.Data Preprocessing
2.Model Architecture
3.Compilation and Training
4.Evaluation
5.Predictions.
1.Data Preprocessing:
The dataset is split into training and testing sets , 80% & 20& respectively: X_train, y_train, X_test, y_test.
The feature data is scaled using Standard Scaler to normalize the features, which typically improves neural network performance.
2.Model Architecture:
A Sequential model is defined with three layers:
A dense layer with 64 neurons and ReLU activation.
A Dropout layer to prevent overfitting (drop 20% of the neurons randomly).
A second dense layer with 32 neurons and ReLU activation.
A final dense layer with a single output unit (for regression).
3.Compilation and Training:
The model is compiled with the Adam optimizer and Mean Squared Error (MSE) loss. The Mean Absolute Error (MAE) is also tracked as a metric during training.
The model is trained for 100 epochs with a batch size of 32, and the validation split is set to 0.2.
4.Evaluation:
After training, the model is evaluated on the test set.
The MAE is calculated again using mean_absolute_error from sklearn.metrics.
5.Predictions:
Predictions are made on the test set, and the Mean Absolute Error (MAE) between the predicted values and the true values is printed.
MAE measures the average absolute difference between the predicted prices and the actual prices. A lower MAE indicates better model performance. This approach to understand how well the model is predicting the house prices.
