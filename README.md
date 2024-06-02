                                                                ![image](https://github.com/rabhaembarak/Time_Series/assets/161968874/d24498e2-c4b4-453f-85dc-73283da66cdf)


# Time Series Season Classification Based on Energy Consumption

## Introduction
This project focuses on classifying seasons based on energy consumption using time series data. The dataset consists of hourly time series data sourced from the ENTSO-E Transparency platform, consisiting of years from 2015 to mid-2020. It includes variables such as electricity consumption, generation capacity, and prices. The classification is done for four seasons: winter, spring, summer, and autumn.

## Data
The dataset (`time_series_60min_singleindex.csv`) is preprocessed to extract relevant features, including electricity consumption, wind generation, and solar generation. Data preprocessing steps include extracting country-specific data (UK and Belgium), converting hourly data to daily data, and handling missing values.

## Preprocessing
The data is preprocessed using Python and the library pandas. It involves extracting country-specific data (the project is applied on UK and Belgium), transforming the dataframe, handling missing values, and converting hourly data to daily data.

## Time Series Classification
The dataset is divided into four seasons: winter, spring, summer, and autumn. Each season is represented by 24-hour segments of hourly consumption data. Various classification algorithms are applied, including Random Forest, K-Nearest Neighbors, and MUSE (MUltivariate Symbolic Extension), to classify the seasons.

## Deep Learning Models
Deep learning models, including ResNet, LSTM, and RNN, are implemented to classify the seasons based on energy consumption. Pretrained ResNet architecture is used, and optimal learning rates are determined for better accuracy. LSTM and RNN models are trained and evaluated on the dataset, and their performance is compared with other classification algorithms.

## Results
The classification results for UK are summarized below:

- RandomForestClassifier: 0.958
- KNeighborsClassifier: 0.980
- MUSE: 0.980
- ResNet: 0.994
- RNN: 0.894
- LSTM: 0.932

## Conclusion
The project demonstrates the effectiveness of various classification algorithms and deep learning models in classifying seasons based on energy consumption for both UK and Belgium data. The results provide valuable insights into seasonal energy consumption patterns in both countries.
