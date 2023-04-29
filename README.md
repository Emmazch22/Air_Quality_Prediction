# Machine Learning Model for Air Quality Prediction

By: Emmanuel Zúñiga Chaves
Contact: emanuel2202zch@gmail.com

## Description
This work is implementation a machine learning model based on a neural network LSTM for the prediction of the concentration of pm 2.5 in the air according to certain dates.

## Dataset
For this purpose, a dataset containing information on the concentration of particulate matter in the surroundings of the [U.S. Embassy in San Jose, Costa Rica is used](https://aqicn.org/city/costa-rica/san-jose/us-embassy/); this dataset collects data for the last 41 weeks (as of April 29, 2023), and the concentration of pm 2.5 on that date [1].

## Results
To predict the concentration of pm 2.5, the date must be changed in the date variable (follow the specified format), then the model will show the prediction made for that date.
```
# Change this variable to predict the pm 2.5
date = '2023-04-30' # follow the format Y-M-D
datetime = dt.datetime.strptime(date, '%Y-%m-%d')
prediction_date = pd.Timestamp(datetime).timestamp()
```

Once the model has performed the prediction, the following output will be obtained:

```
Prediction for 2023-04-30:
pm 2.5 Concentration: [[35.991245]]
```

## References

[1] aqicn.org, “San Jose US Embassy Air Pollution: Real-time Air Quality Index (AQI)”, [Online]. Available: https://aqicn.org/city/costa-rica/san-jose/us-embassy/. [Accesed at: 29-apr-2023].