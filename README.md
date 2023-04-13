# Dcard_Intern_Homework
This is my implementation of Dcard Machine Learning Internship Homework.
## About the Project
In this work, I will predict the like count 24 hours after the post is created on Dcard.
The following shows the example of the training data.

|<nobr> title </nobr> |created_at |like_count_1h | like_count_2h | like_count_3h|like_count_4h|like_count_5h|like_count_6h|comment_count_1h|comment_count_2h|comment_count_3h|comment_count_4h|comment_count_5h|comment_count_6h|forum_id|author_id|forum_stats|like_count_24h|
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
|<nobr>分開是為了更好的相遇</nobr>|2022-12-10 12:14:06 UTC|2|7|7|12|13|14|0|1|1|1|2|2|399368|298421|48.6|16|

### Built with
[![](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)](https://www.python.org)
[![](https://img.shields.io/badge/VSCode-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com)
[![](https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/stable/)
[![](https://img.shields.io/badge/Keras-FF0000?style=for-the-badge&logo=keras&logoColor=white)](http://keras.io)

## Getting Started
Built with Python 3.9.16
### Prerequisites

#### For Windows or Linux
Use pip to install the required packages.
```
pip install tensorflow keras scikit-learn numpy pandas matplotlib seaborn xgboost
```
#### For Apple Chips
Since TensorFlow is not available on the Mac, we have to install miniforge.
Tutorial for installing tensorflow with Apple Chips: [Link](https://caffeinedev.medium.com/how-to-install-tensorflow-on-m1-mac-8e9b91d93706)

Build with conda `environment.yml`
```
conda env create -f environment.yml
```

### Installation
Clone the project repository
```sh
git clone git@github.com:Mao-Siang/Dcard_Intern_Homework.git
```

First, run all blocks in `RNN.ipynb` to generate the hidden layer output of RNN for later use in the regression model. The outputs will be stored in `train_rnn.csv`, `valid_rnn.csv`, and `test_rnn.csv` under the `ML Intern Homework` directory. (The output might be different)

Second, run all blocks in `main.ipynb`, and the results will be stored in `results.csv`.

### Directory structure
```
.
├── ML Intern Homework
│   ├── intern_homework_private_test_dataset.csv
│   ├── intern_homework_public_test_dataset.csv
│   ├── intern_homework_train_dataset.csv
│   ├── test_rnn.csv
│   ├── train_rnn.csv
│   └── valid_rnn.csv
├── README.md
├── RNN.ipynb
├── environment.yml
├── main.ipynb
├── report.pdf
└── results.csv
```
## Results
- Stored in `results.csv`
- Target Metric: MAPE (Mean Absolute Percentage Error)
- Current Results: MAPE 13.1%

## Acknowledgments
- [Comprehensive data exploration with Python](https://www.kaggle.com/code/pmarcelino/comprehensive-data-exploration-with-python/notebook#1.-So...-What-can-we-expect?)

## Other Links
- [Github Repository](https://github.com/Mao-Siang/Dcard_Intern_Homework)