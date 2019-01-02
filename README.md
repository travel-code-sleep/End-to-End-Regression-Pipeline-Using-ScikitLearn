# Prediction of Burn Area using Meteorological Data

* **Link - ** http://www.kaggle.com/travelcodesleep/end-to-end-regression-pipeline-using-scikitlearn

#### My goal with this kernel is to provide a reusable end-to-end Regression framework that is deployable in real world. It is imperative that the users adapt it to the dataset in hand and make small necessary changes, but the overall process and class-objects given can adapt to any regression system.

#### Also, this kernel showcases how Scikit-Learn library can simplify and automate data preprocessing, model building and predicting for practical deployment.

#### I chose this dataset because this problem showcases several fundamental challenges in data science, that are not always easy to overcome: - such as highly left-right skewed data, extreme outliers, underfitting, overfitting, lack of enough examples etc. Many of these problems can be dealt with by collecting more data, meaningful feature engineering, and may be removing rare cases or modelling with different techniques that can handle outliers much better, but that is not the motivation behind this kernel.

#### This dataset covers meteorological and spatiotemporal data for forest fires (between 2000 and 2003) in Portugal’s Montesinho Natural Park, with 13 attributes each for 517 such incidents. Our target attribute from these 13 is ‘area’ - total burned area in hectares (ha). The corresponding weather data is that which is registered by sensors when the fire was detected (or first broke out). We have: temp, RH (relative humidity), wind (speed), rain (accumulated precipitation over the last 30 minutes).

#### We also have DMC, DC, ISI and FFMC are components of the Canadian Forest Fire Weather Index (FWI) System, which measures the effects of fuel moisture and wind on fire behavior. These have been calculated using consecutive daily observations of temperature, relative humidity, wind speed, and 24-hour rainfall - i.e. these are time-lagged and not instantaneous values, unlike the four weather variables. Roughly, the higher these components, the more the expected severity of the fire.

#### Spatiotemporal data includes the month and day of the week that the incident occurred, and X and Y co-ordinates of the incident with respect to the park. Smaller fires are much more frequent. This is the case in this dataset, as well as with incidences of wildfires around the world, making this a difficult regression problem.
