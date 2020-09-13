![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Housing stats analysis

Housing in Ames, Ohio USA analyzed
<br>Ironhack Berlin week 5 project
<br>Rinze Douma
<br>13/09/2020

## Content
- [Project description](#Project-description)
- [Workflow](#Workflow)
- [Organization](#Organization)
- [Links](#Links)

## Project description

This is a project as part of the Ironhack Data Analytics course. The goal is to get familiar with doing statistical tests in Python. A public dataset concerning house sales in Ames, Ohio USA over the years 2006-2010was analyzed to check what factors heavily influence the sale price.

## Workflow
- After importing the dataset I first explored the shape and general characteristics of the dataset. Columns with a high percentage of null values were dropped. 
- Then some general characteristics of the data was investigated, such as the change of sale price over time.
- Also I had a look at the distribution of sale price
- Then I checked the distribution of the number of houses built over time
- A check was done for low variance
- Then I proceeded to check which numerical columns showed a high correlation with sale price. As a cut off point I choose an Pearson coefficient of .6 or higher.
- The resulting factors (Overall quality, ground living area, and different area sizes) were analyzed a little further, the different area's combined into one. 
- After this I started to check categorical columns. Using dummy columns I had a look at the neighborhood, which appeared fairly correlated to sale price. 
- A similar process was done for the type of dwelling, but this showed less significance.
- I also attemped to use time series regression for year built vs sale price, but this didn't work correctly.

## Organization

#### Data
The directory 'data' contains the original data is in a file named train.csv. Also there are two text files with descriptions of the columns. 

#### Notebooks
For this project I used one notebook, named housing.ipynb in the 'notebooks' directory.


## Links
- [Repository](https://github.com/therinz/housing_stats)
- [Kaggle dataset](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data)

