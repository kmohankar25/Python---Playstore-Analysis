Google Playstore Data Analysis - Python Project

![logo](https://github.com/kmohankar25/Python---Playstore-Analysis/assets/102423663/1c36e16d-99e6-4d0b-a182-3e4f8997b634)






➤ Objective :-

The objective of this project is to gain insights into the applications hosted on Google Playstore and the sentiment of their user reviews and present these insights in the form of visualisation which can be used to improve the overall experience and optimise the application development processes.

➤ Data Source : Kaggle
playstore_apps.csv - It contains the basic details of the app like number of user reviews, ratings, etc.

App: It contains the name of the app with a short description (optional).
Category: This section gives the category to which an app belongs. In this dataset, the apps are divided among 33 categories.
Size: The disk space required to install the respective app.
Rating: The average rating given by the users for the respective app. It can be in between 1 and 5.
Reviews: The number of users that have dropped a review for the respective app.
Installs: The approximate number of times the respective app was installed.
Type: It states whether an app is free to use or paid.
Price: It gives the price payable to install the app. For free type apps, the price is zero.
Content rating: It states which age group is suitable to consume the content of the respective app.
Genres: It gives the genre(s) to which the respective app belongs.
Last updated: It gives the day in which the latest update for the respective app was released.
Current Ver: It gives the current version of the respective app.
Android Ver: It gives the android version of the respective app.

➤ Steps Involved

Data Cleaning and Transforming :


To prepare the data for analysis, we performed several data cleaning steps. First, we checked for null values to ensure that there were no missing pieces of data. We also identified and removed outliers, especially in cases where ratings had a specific range. If null values existed and needed to be replaced with some value, we inserted values using the modeValue method. We modified data values, for size column we removed symbols like K and M and replaced them with their respective values, as well as removed unwanted characters like "+" and ",". We changed data types of columns to ensure that the data was in a format that was easy to analyze. Finally, we dropped duplicates and checked unique values to ensure the integrity of the data and that it was compliant with the intended datatype. A new column 'Revenue' was added by multiplying the prices and installs value for each record.
