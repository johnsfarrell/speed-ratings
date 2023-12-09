# Speed Ratings

The goal of this project is to create an accurate machine learning model to
predict the [speed rating](https://tullyrunners.com/Data/Articles/SpeedRatingInfo.htm) of all finishers in any given race in New York State. The model will be trained, valuated, and tested on speed ratings from [2014 to 2019](https://tullyrunners.com/database.htm) along with weather data from the [National Centers for Environmental Information](https://www.ncdc.noaa.gov/cdo-web/search?datasetid=GHCND) and course specific information from [Tully Runner's](https://tullyrunners.com/) and [Milesplit](https://www.milesplit.com/). The hope is that this model can be applied to future high school cross country races and produce a higher quantity of accurate speed ratings.

The repository is organized as follows:

- `data/` contains all of the raw and preprocessed data used in the project
- `figures/` contains all of the figures generated in the project
- `report/` contains reports on the development and results of the project
- `results/` contains all of the results generated in the project (including the final trained models)
- `src/` contains all the code. The code is organized as follows:
  - `compile.ipynb` contains code for compiling the raw data
  - `preprocessing.ipynb` contains code for preprocessing the compiled raw data
  - `eda.ipynb` contains code for exploratory data analysis
  - `elasticnet_ml.ipynb` contains code for training and testing the elastic net model
  - `randomforest_ml.ipynb` contains code for training and testing the random forest model
  - `xgb_ml.ipynb` contains code for training and testing the xgboost model
  - `knn_ml.ipynb` contains code for training and testing the k-nearest neighbors model
  - `evaluation.ipynb` contains code for evaluating the final models

This project is built in Python 3.11.4 and uses the following key packages:

- joblib 1.3.2
- matplotlib 3.7.2
- numpy 1.24.4
- pandas 2.0.3
- scikit-learn 1.3.0
- scipy 1.11.3
- seaborn 0.12.2
- shap 0.42.1
- xgboost 1.7.6

The `environment.yml` file contains a full list of the packages for this project.
