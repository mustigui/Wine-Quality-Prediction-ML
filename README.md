<p align="center">
  <a href="" rel="noopener">
 <img width=200px height=200px src="https://theecologist.org/sites/default/files/styles/inline_l/public/NG_media/77780.jpg?itok=xaoab9x-" alt="Project logo"></a>
</p>

<h3 align="center">Red Wine Quality Prediction with ML</h3>

<div align="center">

</div>

---

<p align="center"> Apply Random forest, SVM, and Deep Learning, and hyper-parameter tuning to predict wine quality
    <br> 
</p>

## 📝 Table of Contents

- [About](#about)
- [Prerequisites](#reqs)
- [Data Source](#datasource)

## 🧐 About <a name = "about"></a>

Red Wine Quality Dataset

The two datasets are related to red and white variants of the Portuguese "Vinho Verde" wine. For more details, consult the reference [Cortez et al., 2009]. Due to privacy and logistic issues, only physicochemical (inputs) and sensory (the output) variables are available (e.g. there is no data about grape types, wine brand, wine selling price, etc.).

These datasets can be viewed as classification or regression tasks. The classes are ordered and not balanced (e.g. there are much more normal wines than excellent or poor ones).

```
For more information, read [Cortez et al., 2009].
Input variables (based on physicochemical tests):
1 - fixed acidity
2 - volatile acidity
3 - citric acid
4 - residual sugar
5 - chlorides
6 - free sulfur dioxide
7 - total sulfur dioxide
8 - density
9 - pH
10 - sulphates
11 - alcohol
Output variable (based on sensory data):
12 - quality (score between 0 and 10)

```
## 📝 Prerequisites / Python packages <a name = "reqs"></a>
```
#Importing required packages.
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
from sklearn.ensemble import RandomForestClassifier
from sklearn.svm import SVC
from sklearn.linear_model import SGDClassifier
from sklearn.metrics import confusion_matrix, classification_report
from sklearn.preprocessing import StandardScaler, LabelEncoder
from sklearn.model_selection import train_test_split, GridSearchCV, cross_val_score
%matplotlib inline
from sklearn.neural_network import MLPClassifier, MLPRegressor
from sklearn.metrics import accuracy_score, mean_squared_error, r2_score
```
## 🎉 Data Source <a name = "datasource"></a>

https://www.kaggle.com/datasets/uciml/red-wine-quality-cortez-et-al-2009