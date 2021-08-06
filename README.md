# Seattle Police - Terry Stops Analysis

## Overview

This project analyses Terry Stops recorded by officers of the Seattle Police Department and see which key features of a terry stop lead to an arrest.

## Business Problem


### Data

This project uses [public data](https://data.seattle.gov/Public-Safety/Terry-Stops/28ny-9ts8) from the Seattle Police Department and represents records of police reported stops under [Terry v. Ohio, 392 U.S. 1 (1968)](https://www.oyez.org/cases/1967/67). Each row represents a unique Terry Stop. Each record contains perceived demographics of the subject, as reported by the officer making the stop and officer demographics as reported to the Seattle Police Department, for employment purposes.


### Method



### Results

The final model that produced the best results for the analysis was the Random Forest Classifier model.

![best_model_train](./Images/best_model_train_scores.PNG)


![best_model_test](./Images/best_model_test_scores.PNG)

## Recommendations

Three key features that the model highlighted as important in being able to predict if a terry stop would lead to an arrest are:

1 - Officer's and Subject's Race
2 - Time of the Year
3 - Officer's Age
 
While more research will need to be invested, a few preliminary solutions towards each recommednation include 1) trying to match an officer's race with the race of neighborhood they patrol whenever possible 2) coordinating a communication push during morning briefs on how police officers can manage or be aware of their own biases and 3) having training requirements for officer's who reach a certain age or time as an officer with an emphasis on diveristy and inclusiveness and community building skills.


### Future Analysis

Future analysis of a few key areas of the dataset would be beneficial to the model. The first area would be looking at the geographical data and seeing how the data breaks down by precint or sector. It would also be interesting to import latitude and longitude data of where the terry stop occured and see if there are any trends there. The second area would be the day of the week and time of day and seeing if the weekends or weekdays or a specific day or morning, afternoon, night could be anothe key feature. The third area would be to compare Seattle's performance to other cities of similar size and make up and see how they rank. 

Lastly, strategizing on how we can implement these changes into the department with stakeholder buy-in will be key in order to ensure these changes are interweaved into the structure of the police department.

### Repository Structure

├── images
├── 01_data_cleaning.ipynb
├── 02_predictive_modelling.ipynb
├── 03_data_visualizations.ipynb
├── README.md # Tools and utilities
├── Terry_Stops.csv
└── Terry_stops_cleaned.csv