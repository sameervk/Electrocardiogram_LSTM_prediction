# Electrocardiogram_LSTM_prediction
Anomaly Detection in Electrocardiograms using LSTMs


* ECG data from http://www.cs.ucr.edu/~eamonn/discords/
* 2 inputs and multi-output model
* 2 LSTMs layers with accompanying batch normalization layers for each input
* Tensorflow version: 2.0.0-beta1
    

    
## Differencing

* Differencing implemented upto the first order trends. The data also seems to have long-range trends which could not be differenced out from the data.
* Signal analysis using Empirical Mode Decomposition and Autocorrelation plots
* Training with LSTMs shows good predictions and the ability to detect anomalies. With more data, the training can be improved to also model the higher order trends in the data.
* For anomaly warning, a mean absolute/squared error metric between the real and predicted data can be defined with a certain threshold above which an anomaly warning can be sounded.

