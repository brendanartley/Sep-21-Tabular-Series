# Sep 2021 Tabular Series

Competed in the Tabular data series competition hosted on Kaggle. The goal of the competition was to predict whether a customer made a claim on an insurance policy based on unlabelled data.

<p align="center">
  <img src="https://github.com/brendanartley/Sep-21-Tabular-Series/blob/main/ic.jpeg" />
</p>

In this competition, we were given a tabular dataset with a range of discrete and continuous numerical variables. We were not given the feature names, so each user had to be very creative in their feature engineering approaches. Because nobody knew what the features were, a large amount of the work done on this competition was in the EDA (exploratory data analysis) stage.

Another competitor was kind enough to share that the number of missing values in a given row was very valuable in terms of predicting whether a user had made a claim or not. After hearing this information, I added this feature to the model. I also created some aggregated statistics by row ie "mean, std, max, skew, etc." These features also boosted the model performance. Feature engineering is so powerful, and I have found that what separates great models from good models is creatively feature engineered pipelines. This is why most time should be spent on this stage.

In the final 2 weeks of the competition, I decided to move on from finding "magical features" to testing different model structures, tuning hyperparameters, and applying cross-validation techniques. I tested CatBoost, XGBoost, and LGBM Decision Tree models and found that the LGBM model worked the best. I also tested 5-fold, 10-fold, 20-fold, and 30-fold cross-validation models. I saw marginal gains until 20-folds and then there was no difference in prediction accuracy.

The final notebook version is attached in this repo, but feel free to check the notebook versions on my Kaggle Profile here --> [brendanartley](https://www.kaggle.com/brendanartley)

Thank you to the Kaggle Team for hosting another great competition!
