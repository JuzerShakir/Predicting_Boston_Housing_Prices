# My Fourth Project in Machine Learning Foundations Nanodegree
# Model Evaluation and Validation
## Project: Predicting Boston Housing Prices

<br>
<p align = 'center'><img src = 'boston_houses.png'></p>

----

### Table Of Contents:
- [Description](#description)<br>
    - [About the project](#about-the-project)<br>
    - [What needs to be done](#what-needs-to-be-done)<br>
    - [Why this project](#why-this-project)<br>
- [Data](#data)<br>
    - [Files](#files)<br>
    - [Dataset file](#dataset-file)<br>
- [Loading Project](#loading-project)<br>
    - [Requirements](#requirements)<br>
    - [Execution](#execution)<br>
- [Conclusion](#conclusion)<br>
    - [What I learned](#what-i-learned)<br>
    - [Evaluation](#evaluation)
    - [Results](#results)

----

### Description

#### About the project

The Boston housing market is highly competitive, and I want to be the best real estate agent in the area. To compete with my peers, I decide to leverage a few basic machine learning concepts to assist myself and my client with finding the best selling price for their home. Luckily, I've come across the Boston Housing dataset which contains aggregated data on various features for houses in Greater Boston communities, including the median value of homes for each of those areas.My task is to build an optimal model based on a statistical analysis with the tools available. This model will then be used to estimate the best selling price for my client's homes.

#### What needs to be done

In this project, I will apply basic machine learning concepts on data collected for housing prices in the Boston, Massachusetts area to predict the selling price of a new home. I will first explore the data to obtain important features and descriptive statistics about the dataset. Next, I will properly split the data into testing and training subsets, and determine a suitable performance metric for this problem. I will then analyze performance graphs for a learning algorithm with varying parameters and training set sizes. This will enable me to pick the optimal model that best generalizes for unseen data. Finally, I will test this optimal model on a new sample and compare the predicted selling price to your statistics.

#### Why this project

This project is designed to get us acquainted to working with datasets in Python and applying basic machine learning techniques using NumPy and Scikit-Learn. Before being expected to use many of the available algorithms in the sklearn library, it will be helpful to first practice analyzing and interpreting the performance of our model.

-----

### Data

#### Files

This project contains three files:

- `report.ipynb`: This is the main file where I have performed my work on the project.
- `housing.csv`: The project dataset. I'll load this data in the notebook.
- `visuals.py`: This Python script provides supplementary visualizations for the project.
- `export/` : Folder containing HTML and PDF version file of notebook.

Template code is provided in the `report.ipynb` notebook file. I will be required to use the included `visuals.py` Python file and the `housing.csv` dataset file to complete my work. While some code has already been implemented to get me started, I'll need to implement additional functionality when requested to successfully complete the project. 

> **Note that the code included in `visuals.py` is meant to be used out-of-the-box and not intended to manipulate.** If you are interested in how the visualizations are created in the notebook, please feel free to explore this Python file.

#### Dataset file

The dataset for this project originates from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Housing). The Boston housing data was collected in 1978 and each of the 506 entries represent aggregated data about 14 features for homes from various suburbs in Boston, Massachusetts.

For the purposes of this project, the following preprocessing steps have been made to the dataset:

- 16 data points have an `'MEDV'` value of 50.0. These data points likely contain **missing or censored values** and have been removed.
- 1 data point has an `'RM'` value of 8.78. This data point can be considered an **outlier** and has been removed.
- The features `'RM'`, `'LSTAT'`, `'PTRATIO'`, and `'MEDV'` are essential. The remaining **non-relevant features** have been excluded.
- The feature `'MEDV'` has been **multiplicatively scaled** to account for 35 years of market inflation.

**Features**
1.  `RM`: average number of rooms per dwelling
2. `LSTAT`: percentage of population considered lower status
3. `PTRATIO`: pupil-teacher ratio by town

**Target Variable**

4. `MEDV`: median value of owner-occupied homes

----

### Loading Project

#### Requirements

This project requires **Python 3.6.5** and the following Python libraries installed:

- [Python 3.6.5](https://www.python.org/downloads/release/python-365/)
- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://jupyter.org/install)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](https://www.anaconda.com/download/) distribution of Python, which already has the above packages and more included.

#### Execution

In a terminal or command window, navigate to the top-level project directory `Predicting_Boston_housing_prices/` (that contains this README) and run one of the following commands:

```bash
ipython notebook report.ipynb
```  
or
```bash
jupyter notebook report.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

----

### Conclusion

#### What I learned

Things I've learned by completing this project:

- How to use NumPy to investigate the latent features of a dataset.
- How to analyze various learning performance plots for variance and bias.
- How to determine the best-guess model for predictions from unseen data.
- How to evaluate a model's performance on unseen data using previous data.

#### Evaluation
My project was reviewed by a Udacity reviewer against the **<a href="https://review.udacity.com/#!/rubrics/103/view" target="_blank">Predicting Boston Housing Prices project rubric</a>**. All criteria found in the rubric must be *meeting specifications* for me to pass.

#### Results
[My Project Review by an Udacity Reviewer](https://review.udacity.com/#!/reviews/1003487)

----