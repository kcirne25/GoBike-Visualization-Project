# GoBike: Data Visualization Project

This project was created to analyze the [Ford GoBike Dataset from Bay Wheels](https://www.lyft.com/bikes/bay-wheels/system-data) to extract insights and behaviours about individual bike rides made in a bike-sharing system covering the greater San Francisco Bay area.

The visual analysis of the dataframe will focus in analyze and provide insights to 3 questions :

* What is the average duration of bike rides?
* Does people prefer to ride bikes in some specific months?
* Is there a difference in the duration of bike rides from subscribers or a customers? 

## Datasets

The dataset used in the project was from Ford GoBike System Data. It was extracted from GoBike System Data 12 csv files, from July 2019 to June 2020. During the exploratory analysis, it was seen that data from April 2020 to June 2020 had a different syntax construction from other files. Because of this issue, these csv files were excluded from the analysis, so data from 9 months was analyzed.

## Packages

The project requires the installation of the following packages: `Pandas`, `Numpy`, `Matplotlib`, `Seaborn` `Glob` and the magic function `%Matplotlib inline`.

## Structure

It is possible to verify the following sections in the project:

* Part I - Data Wrangling
* Part II - Visual Data Analysis
* Part III- Conclusions
* Part IV - References

## Exploratory Analysis

Analyzing the dataset, it was possible to observe that 3 main features: Duration of a bike ride, Months were a bike was rented and type of user. It was also possible to visualyze that months could easilly be extracted and ''transfered'' to a new column and to turn the analysis more 'human friendly', a new Duration of Rides in Minutes column was created.

 ### Summary Of Findings

- Dataset has more than 2 million observations and 10 columns;
- Most of the duplicated rows are related to NaN values;
- user_type column has just 2 variables: Subscribers and Costumers;
- There is a total of 1490110 subscribers and 669531 customers;
- San Francisco Caltrain (with 30813 entries) is the most common start station to rent a bike, followed by Berry St (28649 entries) and Market St (28174 entries);
- The log plot turns it easier to analyze the distribution of bike rides;
- Customers spend on average 17.5 minutes in rides, while subscribers spend almost 12.5 minutes;
- With this heatmap it was possible to verify that subscribers possibly use this rent system to daily tasks like going to work, supermarket or school, for example.   

 ### Key insights

* Average duration of bike rides are between 5 to 20 minutes;
* As data is from San Francisco (North Hemisphere), winter takes place in the months of November-January, resulting in bike rides with a shorter duration. The months from July to October shows more bike rides with 200 or more;
* Most subscribers prefer to take bike rides and spend up to 400 minutes. Rides that last longer than 400 minutes usually are performed by Customers.

## Conclusions

The analysis through this project provided insights and answered the questions about the behaviour of people who ride bike using the GoBike system.

A log plot turned it easier to analyze the distribution from bike rides, which usually take from 5 to 20 minutes.

Bike rides had shorter duration during colder months of the year. Warmer months (July to October) showed more bike rides with 200 or more minutes.

The Multivariate Exploration shows valuable insights when it is needed to analyze a third variable. It was possible to verify that most subscribers prefer to take bike rides and spend up to 400 minutes. These rides last longer during the warmer months of the year.

Rides that last longer than 400 minutes usually are performed by Customers.

## References

* [Glob function to merge csv files](https://docs.python.org/3/library/glob.html)
* [Extracting month from a column](https://stackoverflow.com/questions/25146121/extracting-just-month-and-year-separately-from-pandas-datetime-column)
* [Error tokening - bad_lines](https://github.com/kaushaltrivedi/fast-bert/issues/96)
* [Rename Function](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.rename.html)

