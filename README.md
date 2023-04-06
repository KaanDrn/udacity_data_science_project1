
# udacity_data_science_project1

# Motivation
This repsotory shows the analysis of the Boston AirBnB Dataset provided by [Kaggle](https://www.kaggle.com/datasets/airbnb/boston). The focus of this analysis is to determine the value of the assets, listed in the dataset and to provide additional information to the hosts about what makes their asset valuable and how can they enhance the value of their assets.
In addition this analysis provides information to the customers on which time they can stay in Boston the cheapest.
In short, the following three questions have been answered in this anlysis:
1. What makes an asset valuable (high price)?
2. How can hosts enhance their prices for their assets?
3. What is the best time to book an apartment?

# Libraries
The analysis makes use of the most known python libraries, namely:
- pandas
- numpy
- matplotlib
- sklearn
- seaborn
- datetime

# Files
The repo contains three directories, namely: `./code`, `./data` and  `./blogpost`.
The `./repo` directory contains a jupyter notebook (`Boston_data.ipynb`), describing the analysis in depth. This is also where all the visualization is made.
The data used in this analysis can be found in the `./data` directory.
A shorter and more general description of the analysis and the results can be found in the `./blogpost` directory, where a Gitlab Blogpost describes the analysis.

# Results
For the three questions stated previously we can conclude the following:

__Question 1__: What determines the price of an asset the most is:
1.  The proprty and room type
2.  The number of rooms (bathrooms, bedrooms, and beds)
3.  And the place, your apartment is at.

Therefore a host can not easily enhance his apartment, since the host can not add any more rooms, change the location, etc. Hence an alternative way to enhance the value had to be found, which lead us to the second question.

__Question 2__: A Host can enhance the price for his asset depending on the asset type.
For smaller apartments, the price increases, if basic needs are fulfilled (e.g.: TV, Hairdryer, etc.). For owner of bigger apartments, people are looking for indoor fireplace or want to take their pets to their apartment as well. If hosts allow animals or already have animals on the property, this increases the value as well.

__Question 3__: Now its time to change the view and provide information about the best time to rent an apartment in Boston for the lowest price. During the analysis it was found that the best time to rent an apartment was from January until April.

# Acknowledgments
Thanks to AirBnB and Kaggle for making the data available for the public without any restrictions.