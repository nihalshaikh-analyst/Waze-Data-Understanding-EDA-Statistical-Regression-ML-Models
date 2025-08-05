# Waze-Churn-Data-Understanding-and-Analysis
This project uses a dataset called waze_app_dataset.csv. It contains synthetic data created for this project in partnership with Waze.  Data analyze, clean, process, data analysis by using Python and its Library pandas and numpy with presentation in Jupyter Notebook.

![waze logo](https://github.com/nihalshaikh-analyst/Waze-Churn-Data-Understanding-and-Analysis/blob/main/waze%20logo.png)


## The Waze data team is currently developing a data analytics project aimed at increasing overall growth by preventing monthly user churn on the Waze app. For the purposes of this project, churn quantifies the number of users who have uninstalled the Waze app or stopped using the app. This report offers a preliminary data summary, information on the project status and key insights of Milestone 2, which impact the future development of the overall project.


## Background on the Waze scenario.

Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go. Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Waze partners with cities, transportation authorities, broadcasters, businesses, and first responders to help as many people as possible travel more efficiently and safely. 

You’ll collaborate with your Waze teammates to analyze and interpret data, generate valuable insights, and help leadership make informed business decisions. Your team is about to start a new project to help prevent user churn on the Waze app. Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app. This project focuses on monthly user churn. 

This project is part of a larger effort at Waze to increase growth. Typically, high retention rates indicate satisfied users who repeatedly use the Waze app over time. Developing a churn prediction model will help prevent churn, improve user retention, and grow Waze’s business. 


[Waze Dataset](https://github.com/nihalshaikh-analyst/Waze-Churn-Data-Understanding-and-Analysis/blob/main/waze_app_dataset.csv)

- Who are the users most likely to churn?

- Why do users churn? 

- When do users churn?



## Team members at Waze

**Data team roles**

- Harriet Hadzic - Director of Data Analysis 

- May Santner - Data Analysis Manager 

- Chidi Ga - Senior Data Analyst 

- Sylvester Esperanza - Senior Project Manager 

Data team members have technical experience with data analysis and data science. However, you should always be sure to keep summaries and messages to these team members concise and to the point. 

## Cross-functional team members

- Emrick Larson - Finance and Administration Department Head 

- Ursula Sayo - Operations Manager

Note: The story, all names, characters, and incidents portrayed in this project are fictitious. No identification with actual persons (living or deceased) is intended or should be inferred. And, the data shared in this project has been created for pedagogical purposes. 


![waze](https://github.com/nihalshaikh-analyst/Waze-Churn-Data-Understanding-and-Analysis/blob/main/waze.png)


## Data dictionary

**This project uses a dataset called waze_dataset.csv. It contains synthetic data created for this project in partnership with Waze.**

The dataset contains:

14,999 rows – each row represents one unique user 

13 columns


## Project background

Waze’s data team is in the earliest stages of the churn project. The following tasks are needed before the team can begin the data analysis process:

- Build a dataframe for the churn dataset

- Examine data type of each column

- Gather descriptive statistics

- Assignment


## Specific project deliverables

- Complete the questions in the Course 2 PACE strategy document

- Answer the questions in the Jupyter notebook project file

- Complete coding prep work on project’s Jupyter notebook

- Summarize the column Dtypes

- Communicate important findings in the form of an executive summary

- creative work and approach problem-solving!






## Project Status

🎯 **Target Goal:**

- Inspect user data to learn important relationships between variables.
  

  
🎯 **Methods:**

- Built a dataframe
  
- Each row represents a single observation, and each column represents a single variable

- Collected preliminary statistics
  
- Analyzed user behavior
  

  
🎯 **Impact:**

- Our team determined important relationships between variables that will guide further analysis of user data


## Storytelling Finding and Persentation

[Presentation](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Waze%20Churn%20Data%20Understsnding%20Findings.pptx)


![Presentations and Key Insight](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Waze%20data%20understanding%20presentation.png)


## Insights

**1. This dataset contains 82% retained users and 18% churned users.**

**2. The dataset contains 12 unique variables with types including objects, floats, and integers; the label column is missing 700 values with no indication that the omissions are non-random.**

**3. Churned users averaged ~3 more drives in the last month than retained users.**

**4. Retained users used the app on over twice as many days as churned users in the last month.**

**5. The median churned user drove ~200 more kilometers and 2.5 more hours during the last month than the median retained user.**

**6. Churned users had more drives in fewer days, and their trips were farther and longer in duration. Perhaps this is suggestive of a user profile; our team will have to continue exploring!**

**7. The median user who churned drove 698 kilometers each day they drove last month, which is about 240% the per-drive-day distance of retained users.**

**8. Regardless of user churn, the users represented in this data drive a lot! It is probably safe to assume that this data does not represent typical drivers at large.**


## Next Step

**"Our team recommends gathering more data on the super-drivers. It's possible that the reason they’re driving so much is also the reason why the Waze app does not meet their specific set of needs, which may differ from the typical driver."**

**"The immediate next step is to conduct thorough EDA and develop data visualizations to illustrate the narrative behind the data and guide future project decisions."**


## Step by Step Process

**1. Understand the situation**

**2. Understand the data**

**3. Understand the variables**

- Prepare by reading in the data, viewing the data dictionary, and exploring the dataset to identify key variables for the stakeholder.

- Start by importing the packages that you will need to load and explore the dataset. Make sure to use the following import statements:

import pandas as pd

import numpy as np

- Then, load the dataset into a dataframe. Creating a dataframe will help you conduct data manipulation, exploratory data analysis (EDA), and statistical activities.

- View and inspect summary information about the dataframe by coding the following:

df.head(10)

df.info()

**1. None of the variables in the first 10 observations have missing values. Note that this does not imply the whole dataset does not have any missing values.**

**2. The variables label and device are of type object; total_sessions, driven_km_drives, and duration_minutes_drives are of type float64; the rest of the variables are of type int64. There are 14,999 rows and 13 columns.**

**3. The dataset has 700 missing values in the label column.**


- Compare the summary statistics of the 700 rows that are missing labels with summary statistics of the rows that are not missing any values.

- Comparing summary statistics of the observations with missing retention labels with those that aren't missing any values reveals nothing remarkable. The means and standard deviations are fairly consistent between the two groups.

- Next, check the two populations with respect to the device variable.

- Of the 700 rows with null values, 447 were iPhone users and 253 were Android users.

- Now, of the rows with null values, calculate the percentage with each device—Android and iPhone. You can do this directly with the value_counts() function.

- The percentage of missing values by each device is consistent with their representation in the data overall.

- There is nothing to suggest a non-random cause of the missing data.

- This dataset contains 82% retained users and 18% churned users.

Next, compare the medians of each variable for churned and retained users. The reason for calculating the median and not the mean is that you don't want outliers to unduly affect the portrayal of a typical user. Notice, for example, that the maximum value in the driven_km_drives column is 21,183 km. That's more than half the circumference of the earth!

- Users who churned averaged ~3 more drives in the last month than retained users, but retained users used the app on over twice as many days as churned users in the same time period.

- The median churned user drove ~200 more kilometers and 2.5 more hours during the last month than the median retained user.

- It seems that churned users had more drives in fewer days, and their trips were farther and longer in duration. Perhaps this is suggestive of a user profile. Continue exploring!

- Calculate the median kilometers per drive in the last month for both retained and churned users.

- Begin by dividing the driven_km_drives column by the drives column. Then, group the results by churned/retained and calculate the median km/drive of each group.

- To calculate this statistic, repeat the steps above using driving_days instead of drives.

- Now calculate the median number of drives per driving day for each group.

- The median user who churned drove 698 kilometers each day they drove last month, which is ~240% the per-drive-day distance of retained users. The median churned user had a similarly disproporionate number of drives per drive day compared to retained users.

- It is clear from these figures that, regardless of whether a user churned or not, the users represented in this data are serious drivers! It would probably be safe to assume that this data does not represent typical drivers at large. Perhaps the data—and in particular the sample of churned users—contains a high proportion of long-haul truckers.

- In consideration of how much these users drive, it would be worthwhile to recommend to Waze that they gather more data on these super-drivers. It's possible that the reason for their driving so much is also the reason why the Waze app does not meet their specific set of needs, which may differ from the needs of a more typical driver, such as a commuter.

- Finally, examine whether there is an imbalance in how many users churned by device type.

- Begin by getting the overall counts of each device type for each group, churned and retained.

- Now, within each group, churned and retained, calculate what percent was Android and what percent was iPhone.

- The ratio of iPhone users and Android users is consistent between the churned group and the retained group, and those ratios are both consistent with the ratio found in the overall dataset.



## Conclusion

**"Recall that your supervisor, May Santer, asked you to share your findings with the data team in an executive summary. Consider the following questions as you prepare to write your summary. Think about key points you may want to share with the team, and what information is most relevant to the user churn project."**

- The dataset has 700 missing values in the label column. There was no obvious pattern to the missing values.

- Mean is subject to the influence of outliers, while the median represents the middle value of the distribution regardless of any outlying values.

- the median user who churned drove 698 kilometers each day they drove last month, which is about 240% the per-drive-day distance of retained users. It would be helpful to know how this data was collected and if it represents a non-random sample of users.

- Android users comprised approximately 36% of the sample, while iPhone users made up about 64%

- Generally, users who churned drove farther and longer in fewer days than retained users. They also used the app about half as many times as retained users over the same period.

- No. The churn rate for both iPhone and Android users was within one percentage point of each other. There is nothing suggestive of churn being correlated with device.




Any concerns contact to us nihalshaikh.analyst@gmail.com


-------Thank you........
