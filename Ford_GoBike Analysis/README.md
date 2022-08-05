# Ford GoBike Data
## Elemide Sofiyah


# Table of contents
1. [Introduction](#introduction)
    1. [Description](#description)
    
2. [Software and Libraries](#libraries)

3. [Project Walkthrough](#walk)
    1. [Gathering and Assessing](#sub1)
    2. [Cleaning, Storing and Visualization](#sub2)
        
4. [Conclusion and Limitations](#conclusion)

5. [Summary and Insights](#summary)

6. [References](#references)

## 1. Introduction <a name="introduction"></a>
- This project gathers, cleans and analyzes data from Ford GoBike System. The [dataset]([https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd1c4c_tmdb-movies/tmdb-movies.csv.](https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1659713813739392&usg=AOvVaw3FJndwEO6Sb_bQq5a7W6mb) collected from the database contains records of bike ride trips with features of each trip that makes up the columns in the dataset.
### 1.1. Description <a name="description"></a>
- This data set includes information about individual rides made in a bike-sharing system covering the greater San Francisco Bay area. The data set contains information about **183412** ride details that occured in 2019, collected from Ford GoBike System. The dataset contains **16 columns** with gives the details about each ride. Each column is described below:
1. duration_sec: Trip duration in seconds
2. start_time: Time the trip started
3. end_time: Time the trip ended
4. start_station_id: Unique number assigned to the start station
5. start_station_name: Name of the start station
6. start_station_latitude: Latitude of start station
7. start_station_longitude: Longitude of start station
8. end_station_id: Unique number assigned to the end station
9. end_station_name: Name of the end station
10. end_station_latitude: Latitude of end station
11. end_station_longitude: Longitude of end station
12. bike_id: Unique number asigned to the bike used
13. user_type: Whether user is a one off customer or a subscriber
14. member_birth_year: User year of birth
15. member_gender: User gender
16. bike_share_for_all_trip

    
## 2. Software and Libraries <a name="libraries"></a>
- Python
- Prefarred IDLE: VS Code, Jupyter Notebook etc.
- Numpy
- Pandas
- Matplotlib

## 3. Project Walkthrough <a name="walk"></a>
### 3.1. Gathering and Assessing <a name="sub1"></a>
The [data set]([https://d17h27t6h515a5.cloudfront.net/topher/2017/October/59dd1c4c_tmdb-movies/tmdb-movies.csv.](https://www.google.com/url?q=https://video.udacity-data.com/topher/2020/October/5f91cf38_201902-fordgobike-tripdata/201902-fordgobike-tripdata.csv&sa=D&source=editors&ust=1659713813739392&usg=AOvVaw3FJndwEO6Sb_bQq5a7W6mb) is provided by Udacity and readily available for analysis. 
The data is loaded into a dataframe and assessed for quality and tidines issues which are documented cleaned after detection. Most frequent issues are wrong datatypes and missing values.

### 3.2. Cleaning, Storing and Visualization <a name="sub2"></a>
After cleaning the dataset, store the cleaned dataset for later use, mainly for visualization or model building. Summaries of findings are communicated through exploratory and explanatory visualizations.

## 4. Conclusion and Limitations <a name="conclusion"></a>
The most important variable of interest in this dataset is the trip duration. 
Throughot this document, I explored the other features that can be usedas a predictor for the trip duration. 
The feature that is most likely to correctly predict the trip duration are the member's age and user_type. 
I created univariate, bivariate and multivariate charts to get an insight on how features like age, user type, gender and days of weeks can be a factor to predict the trip duration.

### Limitations
We would have a great model precision and recall if we had a better predicting feature like distance between the start trip and end trip. 
There were missing values in the age variable that would affect the precision of a model if one were to be built. 

## 5. Summary and Insights <a name="summary"></a>
1. Some Trips are taken over night and usually completed on the following day. There are total of 320 trips that were taken overnight.
2. The most popular combination of start and end stations are Berry St at 4th St. and San Francisco Ferry Building respectively with the total trip of 337.
3. Customer user type has an higher average trip duration than Subscriber despite the fact that there are higher number of Subscribers than Customers.
4. Also Other gender has the highest average trip duration, despite being the least count of user.
5. Most popular times of the day trips are started and ended are 8am and 5pm. Those time corresponds with a workplace's opening and closing time.

## 6. References <a name="references"></a>
- [1]  Description of GoBike System
 https://github.com/BetaNYC/Bike-Share-Data-Best-Practices/wiki/Bike-Share-Data-Systems.


- [2] matplotlib: Python plotting library
https://matplotlib.org/

- [3] Pandas: Chart Viualization
https://pandas.pydata.org/docs/user_guide/visualization.html

- [4] How to Choose a Chart Type
https://towardsdatascience.com/data-visualization-101-how-to-choose-a-chart-type-9b8830e558d6
