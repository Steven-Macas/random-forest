<div align="center">

# Random Forest & AdaBoost

**Hyper-parameter tuning with GridSearchCV on regression and classification problems**

<img src="https://img.shields.io/badge/Python-3-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python: 3" /> <img src="https://img.shields.io/badge/Pandas-data-150458?style=flat-square&logo=pandas&logoColor=white" alt="Pandas: data" /> <img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" alt="scikit-learn: ML" /> <img src="https://img.shields.io/badge/Seaborn-charts-4C72B0?style=flat-square" alt="Seaborn: charts" />

</div>

## Overview

Supervised learning with **Random Forest** on two datasets: preprocessing, training and prediction,
evaluation, hyper-parameter optimisation with `GridSearchCV` and an attempt to improve the best model with **AdaBoost**.

| Notebook | Problem | Dataset |
| --- | --- | --- |
| [`randomForest_bike.ipynb`](https://colab.research.google.com/github/Steven-Macas/random-forest/blob/main/randomForest_bike.ipynb) | Regression – bikes rented per day | Bike Sharing (`day.csv`) |
| [`randomForest_vino.ipynb`](https://colab.research.google.com/github/Steven-Macas/random-forest/blob/main/randomForest_vino.ipynb) | Classification – wine quality | Wine Quality (`WineQT.csv`) |

## Results

| Dataset | Model | Metric | Value |
| --- | --- | --- | --- |
| Bike Sharing | Random Forest + GridSearchCV | MAE | 75.0 |
| Bike Sharing | AdaBoost (Random Forest base) | MAE | **68.4** |
| Wine Quality | Random Forest + GridSearchCV | Accuracy | **67.2 %** |
| Wine Quality | AdaBoost (Random Forest base) | Accuracy | 65.5 % |

AdaBoost improves the regression error on the bike data, but not the wine classification.

<table>
  <tr><td align="center" valign="top"><img src="images/bike-predictions.png" alt="Bike Sharing – real vs predicted" width="380" /><br /><sub>Bike Sharing – real vs predicted</sub></td><td align="center" valign="top"><img src="images/wine-confusion-matrix.png" alt="Wine Quality – confusion matrix" width="380" /><br /><sub>Wine Quality – confusion matrix</sub></td></tr>
</table>

*The notebooks are written in Spanish.*

---

<sub>Made by <b>Steven Macas</b> — Data Engineer &amp; Data Analyst · <a href="https://gointy.com">gointy.com</a> · <a href="https://www.linkedin.com/in/steven-macas">LinkedIn</a> · <a href="https://github.com/Steven-Macas">GitHub</a></sub>
