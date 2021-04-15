# fifa-struong
Final Project


# Exploratory Data Analysis of FIFA21 using Voila deployed on Heroku

The dashboard site is: https://fifa-struong.herokuapp.com/

This project contains several data analysis about football player and team based on FIFA21 dataset.The contents of this project are:

1. Data statistic that can be filtered and sorted by some categories

The data is cleaned first because there are some players who do not have a club and some missing values related to league name. Some csv files are obtained from https://github.com/batuhan-demirci/fifa21_dataset/tree/master/data. 

Those csv files need to be concatenate as one dataframe. Age category is not available, the age should be obtained by calculate the difference between today and the player birth date. 

The list of country and team have to be obtained to create the combobox.

2. Histogram showing the distribution of each category.
This shows the distribution of nation, team, age, overall, wage and position.

3. A statistics comparing the average of age, overall and wage of each country
This part creates a new dataframe that is grouped by the nation and the user can sort the table according to the average of age, overall or wage.

4. Best starting lineup based on country, formation and age
This is useful for a manager/game player to decide what formation that creates best starting lineup. It returns the average overall. Even, the manager can choose the youngster to create U-18 or U-21 national team.

5. Correlation between Age or Wage with player overall
This plot shows how old is the player tend to decrease football ability and how is the correlation between the wage and the overall.

6. Classifier comparison to predict the best position according to the abilities.
In this part, seven csv files are read and concatenated with prior dataframe. Four classifier are used to predict the best position from the player abilities. The data is randomly splitted to 20% testing data and 80% training data. Before creating the classification model, some category that are not corellated are dropped and then normalized.
