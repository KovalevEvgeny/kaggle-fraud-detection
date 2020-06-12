# IEEE-CIS Fraud Detection
https://www.kaggle.com/c/ieee-fraud-detection

**Team:** [ods.ai] No Fosters for Fraudsters

**Private results:** 76/6381, top 2%, silver medal

KUDOS to my teammates:
  - https://www.kaggle.com/dvorobiev
  - https://www.kaggle.com/kirill702b
  - https://www.kaggle.com/leensman500
  - https://www.kaggle.com/mishanyap

## Model description

Throughout the competition, we created various models which used different data preprocessing techniques, sets of hyperparameters and random seeds. For the final solution, we selected 21 LightGBM models and 4 Catboost models. Using LightGBM, we stacked them. Finally, we postprocessed the result.

Model scheme:

https://drive.google.com/file/d/1EQWsDyP7V6K2XOeDGuOhdNIidHqrHC35/view?usp=sharing

![](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/FraudDetection_Solution_Scheme.png?raw=true)

## First-layer model aliases

- Models 1-4: [`fraud-lgb-kfold-newfeatures`](https://github.com/blacKitten13/kaggle-fraud-detection/blob/master/ligthgbm_models/fraud-lgb-kfold-newfeatures.ipynb), `fraud-lgb-kfold-newfeatures-seed-44`, `fraud-lgb-kfold-newfeatures-seed-111`, `fraud-lgb-kfold-newfeatures-seed-122`
- Models 5-9: `fraud-dima-940490`, `fraud-dima-942747`, `fraud-dima-943304`, `fraud-dima-943354`, `fraud-dima-944193`
- Models 10-11: `fraud-artem-new-val-no-day`, `fraud-artem-new-val-seed-99-no-day`
- Model 12: `fraud-misha-9436`
- Models 13-14: `fraud-kirill-predictions-9438`, `fraud-kirill-predictions-9459`
- Models 15-16: `fraud-mix-lgbm-no-day`, `fraud-mix-lgbm-seed-101-no-day`
- Models 17-20: `fraud-fs-fe9477-no-day`, `fraud-fs-fe9477-no-day-seed-88`, `fraud-fs-fe9477-no-day-seed-133`, `fraud-fs-fe9477-no-day-seed-144`
- Model 21: `fraud-fs-fe9477-catboost-no-cat`
- Models 22-23: `fraud-dima-cb-hope-v1-944414`, `fraud-dima-cb-hope-v2-943496`
- Models 24-25: `fraud-catboost-dima-943978`, `fraud-dima-944053`

## Task description
Imagine standing at the check-out counter at the grocery store with a long line behind you and the cashier not-so-quietly announces that your card has been declined. In this moment, you probably aren’t thinking about the data science that determined your fate.

Embarrassed, and certain you have the funds to cover everything needed for an epic nacho party for 50 of your closest friends, you try your card again. Same result. As you step aside and allow the cashier to tend to the next customer, you receive a text message from your bank. “Press 1 if you really tried to spend $500 on cheddar cheese.”

While perhaps cumbersome (and often embarrassing) in the moment, this fraud prevention system is actually saving consumers millions of dollars per year. Researchers from the IEEE Computational Intelligence Society (IEEE-CIS) want to improve this figure, while also improving the customer experience. With higher accuracy fraud detection, you can get on with your chips without the hassle.

IEEE-CIS works across a variety of AI and machine learning areas, including deep neural networks, fuzzy systems, evolutionary computation, and swarm intelligence. Today they’re partnering with the world’s leading payment service company, Vesta Corporation, seeking the best solutions for fraud prevention industry, and now you are invited to join the challenge.

In this competition, you’ll benchmark machine learning models on a challenging large-scale dataset. The data comes from Vesta's real-world e-commerce transactions and contains a wide range of features from device type to product features. You also have the opportunity to create new features to improve your results.

If successful, you’ll improve the efficacy of fraudulent transaction alerts for millions of people around the world, helping hundreds of thousands of businesses reduce their fraud loss and increase their revenue. And of course, you will save party people just like you the hassle of false positives.
