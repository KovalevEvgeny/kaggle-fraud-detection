# IEEE-CIS Fraud Detection
https://www.kaggle.com/c/ieee-fraud-detection

**Team:** [ods.ai] No Fosters for Fraudsters

**Private results:** 76/6381, top 2%, silver medal

Kudos to my teammates:
  - https://www.kaggle.com/dvorobiev
  - https://www.kaggle.com/kirill702b
  - https://www.kaggle.com/leensman500
  - https://www.kaggle.com/mishanyap

## Model description

Throughout the competition, we created various models which used different data preprocessing techniques, sets of hyperparameters and random seeds. For the final solution, we selected 20 LightGBM models and 5 Catboost models. Using LightGBM, we stacked them all. Finally, we postprocessed the result.

Model scheme:

https://drive.google.com/file/d/1EQWsDyP7V6K2XOeDGuOhdNIidHqrHC35/view?usp=sharing

![](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/FraudDetection_Solution_Scheme.png?raw=true)

## Links

**First-layer models:**

- Models 1-4: [`fraud-lgb-kfold-newfeatures`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-lgb-kfold-newfeatures.ipynb), [`fraud-lgb-kfold-newfeatures-seed-44`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-lgb-kfold-newfeatures-seed-44.ipynb), [`fraud-lgb-kfold-newfeatures-seed-111`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-lgb-kfold-newfeatures-seed-111.ipynb), [`fraud-lgb-kfold-newfeatures-seed-122`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-lgb-kfold-newfeatures-seed-122.ipynb)
- Models 5-9: [`fraud-dima-940490`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-dima-940490.ipynb), [`fraud-dima-942747`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-dima-942747.ipynb), [`fraud-dima-943304`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-dima-943304.ipynb), [`fraud-dima-943354`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-dima-943354.ipynb), [`fraud-dima-944193`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-dima-944193.ipynb)
- Models 10-11: [`fraud-artem-new-val-no-day`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-artem-new-val-no-day.ipynb), [`fraud-artem-new-val-seed-99-no-day`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-artem-new-val-seed-99-no-day.ipynb)
- Model 12: [`fraud-misha-9436`](https://www.kaggle.com/blackitten13/fraud-misha-9436)
- Models 13-14: [`fraud-kirill-predictions-9438`](https://www.kaggle.com/blackitten13/fraud-kirill-yakovlev-9438), [`fraud-kirill-predictions-9459`](https://www.kaggle.com/blackitten13/kirill-best-9459)
- Models 15-16: [`fraud-mix-lgbm-no-day`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-mix-lgbm-no-day.ipynb), [`fraud-mix-lgbm-seed-101-no-day`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-mix-lgbm-seed-101-no-day.ipynb)
- Models 17-20: [`fraud-fs-fe9477-no-day`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-fs-fe9477-no-day.ipynb), [`fraud-fs-fe9477-no-day-seed-88`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-fs-fe9477-no-day-seed-88.ipynb), [`fraud-fs-fe9477-no-day-seed-133`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-fs-fe9477-no-day-seed-133.ipynb), [`fraud-fs-fe9477-no-day-seed-144`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-fs-fe9477-no-day-seed-144.ipynb)
- Model 21: [`fraud-fs-fe9477-catboost-no-cat`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/catboost_models/fraud-fs-fe9477-catboost-no-cat.ipynb)
- Models 22-23: [`fraud-dima-cb-hope-v1-944414`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/catboost_models/fraud-dima-cb-hope-v1-944414.ipynb), [`fraud-dima-cb-hope-v2-943496`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/catboost_models/fraud-dima-cb-hope-v2-943496.ipynb)
- Models 24-25: [`fraud-catboost-dima-943978`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/catboost_models/fraud-catboost-dima-943978.ipynb), [`fraud-dima-944053`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/catboost_models/fraud-dima-944053.ipynb)

**Preprocessing:**

- for models 1-4: https://www.kaggle.com/kyakovlev/ieee-fe-with-some-eda
- for models 17-21: `[fraud-messing-v31`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/preprocessing/fraud-messing-v31.ipynb)
- additional for model 21: `[fraud-fs-fe9477-no-day-data-preparation`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/preprocessing/fraud-fs-fe9477-no-day-data-preparation.ipynb)
- for models 24-25: [`fraud-data-for-catboost`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/preprocessing/fraud-data-for-catboost.ipynb)


## Task description
Imagine standing at the check-out counter at the grocery store with a long line behind you and the cashier not-so-quietly announces that your card has been declined. In this moment, you probably aren’t thinking about the data science that determined your fate.

Embarrassed, and certain you have the funds to cover everything needed for an epic nacho party for 50 of your closest friends, you try your card again. Same result. As you step aside and allow the cashier to tend to the next customer, you receive a text message from your bank. “Press 1 if you really tried to spend $500 on cheddar cheese.”

While perhaps cumbersome (and often embarrassing) in the moment, this fraud prevention system is actually saving consumers millions of dollars per year. Researchers from the IEEE Computational Intelligence Society (IEEE-CIS) want to improve this figure, while also improving the customer experience. With higher accuracy fraud detection, you can get on with your chips without the hassle.

IEEE-CIS works across a variety of AI and machine learning areas, including deep neural networks, fuzzy systems, evolutionary computation, and swarm intelligence. Today they’re partnering with the world’s leading payment service company, Vesta Corporation, seeking the best solutions for fraud prevention industry, and now you are invited to join the challenge.

In this competition, you’ll benchmark machine learning models on a challenging large-scale dataset. The data comes from Vesta's real-world e-commerce transactions and contains a wide range of features from device type to product features. You also have the opportunity to create new features to improve your results.

If successful, you’ll improve the efficacy of fraudulent transaction alerts for millions of people around the world, helping hundreds of thousands of businesses reduce their fraud loss and increase their revenue. And of course, you will save party people just like you the hassle of false positives.
