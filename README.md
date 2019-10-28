To be, or not to be
==============================

Classy Shakespeare plays and players

Author: Ruturaj Kiran Vaidya

Project Organization
------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
                              the creator's initials, and a short `-` delimited description, e.g.
                              `1.0-jqp-initial-data-exploration`.


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>

### Before Getting Stated

There may be notebook rendering problems with github ecosystem. Please use following link to see the notebook:

https://nbviewer.jupyter.org/github/Ruturaj4/to_be_or_not_to_be/blob/master/notebooks/1.0-rkv-to-be-or-not-to-be.ipynb

### Aim

The aim of this project is to obtain additional values using exploratory data analysis and to use classification algorithms to build models to determine "player" using other columns. Here, other columns are treated as features and player values are treated as labels. hence the input dataset contain features as well as labels (i.e input and output).

### Dataset used

Shakespeare Plays: https://www.kaggle.com/kingburrito666/shakespeare-plays

### Discussion

First, I imported the dataset in pandas dataframe. Second I cleaned up data, e.g. removed NAN values. Third, using feature engineering and data analysis, additional features are derived. I used one hot encoding on "Play" data, and split "ActSceneLine", to derive additional features. The idea is to convert categorial data into numerical data, to apply learning algorithms on it. Lastly, I applied two classification algorithms on the data and found their accuracy. Classification models used are:

* Decision Tree
* Random Forest

### Final Comments

Accuracy of Random Forest came as <b>0.7037230754600352</b> and Decision tree accuracy came as <b>0.6782844372592839</b>, with above configuration. Radom Forest was better than decision tree as expected. My assumption from the above tests is that, the random forest algorithm works better on this dataset (it has also be discussed in class slides). Also, I observed that the learning speed of decision tree model was better than random forest model (cosidering the above configuration).

### License

<b>MIT</b>
