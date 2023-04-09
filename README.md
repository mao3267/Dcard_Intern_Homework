# Dcard_Intern_Homework
This is my implementation of Dcard Machine Learning Internship Homework.
## About the Project
In this work, I will predict the like count 24 hours after the post is created on Dcard.
The following shows the example of the training data.

<style>
table th:first-of-type {
    width: 80px;
}
</style>

| title &nbsp; &nbsp; &nbsp; |created_at |like_count_1h | like_count_2h | like_count_3h|like_count_4h|like_count_5h|like_count_6h|comment_count_1h|comment_count_2h|comment_count_3h|comment_count_4h|comment_count_5h|comment_count_6h|forum_id|author_id|forum_stats|like_count_24h|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|分開是為了更好的相遇|2022-12-10 12:14:06 UTC|2|7|7|12|13|14|0|1|1|1|2|2|399368|298421|48.6|16|

### Built with
[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org)
[![](https://img.shields.io/badge/VSCode-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com)
[![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white)](http://keras.io)

## Getting Started
Built with Python 3.9.16
### Prerequisites
Use pip to install the required packages.
```
pip install keras, scikit-learn, numpy, pandas, matplotlib, seaborn, xgboost
```
### Installation
Clone the project repository
```sh
git clone git@github.com:Mao-Siang/Dcard_Intern_Homework.git
```

First, run all blocks in `RNN.ipynb` to generate the hidden layer output of RNN for later use in the regression model. The outputs will be stored in `train_rnn.csv`, `valid_rnn.csv`, and `test_rnn.csv` under the `ML Intern Homework` directory.

Second, run all blocks in `main.ipynb`, and the results will be stored in `results.csv`.

## Results
- Stored in `results.csv`
- Target Metric: MAPE (Mean Absolute Percentage Error)
- Current Results: MAPE 13.1%

## Acknowledgments
- [Comprehensive data exploration with Python](https://www.kaggle.com/code/pmarcelino/comprehensive-data-exploration-with-python/notebook#1.-So...-What-can-we-expect?)