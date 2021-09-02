# Covid19_week5_predictions
Training and test data was taken from kaggle. The link for training and test data is (https://www.kaggle.com/c/covid19-global-forecasting-week-5/data). Training data consisits the past day cases of 187 countries and predictions are made according to that for the next 45 days.
</br>
I have use four LSTM layers with 16 units in each layer. Dropout of 0.3 was also added to prevent the model from overfitting and timestep of 40 gave the best results. A dense layer was also added after LSTM layers to predict the output. 
</br>
The regressor predicts the confirmed cases and fatalities for upcoming days with some avoidable error. Two regressors are used, one predicts the confirmed cases after observing the past trends and the other one predicts the fatalities. 
