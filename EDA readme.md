# Exploratory Data Analysis (EDA) of Waze App Data

This project uses a dataset called waze_app_dataset.csv. It contains synthetic data created for this project in partnership with Waze. Data analyze, clean, process, data analysis by using Python and its Library **pandas, numpy, matplotlib.pyplot, seaborn** with presentation in Jupyter Notebook.


![waze logo](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/waze%20logo.png)



## Project Overview

**"The Waze data team is currently developing a data analytics project aimed at increasing overall growth by preventing monthly user churn on the Waze app. Thorough exploratory data analysis (EDA) enables Waze to make better decisions about how to proactively target users likely to churn, thereby improving retention and overall customer satisfaction. This report offers details and key insights from Milestone 3, which impact the future development of the overall project."**


## Project Background

- Waze’s data team is working on the churn project. 

- EDA and cleaning

- Select and build visualization(s) type

- Create plots to visualize variables and relationships between variables

- Share your results with the data team

[Waze Dataset](https://github.com/nihalshaikh-analyst/Waze-Churn-Data-Understanding-and-Analysis/blob/main/waze_app_dataset.csv)





## Jupyter Notebook

[Notebook](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/EDA%20of%20Waze%20app.ipynb)

**"EDA is important because ... EDA helps a data professional to get to know the data, understand its outliers, clean its missing values, and prepare it for future modeling. Visualizations helped me understand .. That this dataset has some outliers that we will need to make decisions on prior to designing a model."**


## Storytelling and Problem Solveing

### The Waze data team is currently developing a data analytics project aimed at increasing overall growth by preventing monthly user churn on the Waze app. Thorough exploratory data analysis (EDA) enables Waze to make better decisions about how to proactively target users likely to churn, thereby improving retention and overall customer satisfaction. This report offers details and key insights from Milestone 3, which impact the future development of the overall project. 


[Presentations](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Waze%20EDA%20Findings.pptx)


![Presentations](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Waze%20EDA%20presentataion.png)

<img width="629" height="297" alt="image" src="https://github.com/user-attachments/assets/e691d982-6081-4ed9-8e98-166af4d232b9" />

**The churn rate is highest for people who didn't use Waze much during the last month.**


<img width="376" height="314" alt="image" src="https://github.com/user-attachments/assets/61ab80d3-835d-45cc-af93-58fe2035e370" />

**The proportion of churned users to retained users is consistent between device types.**


## Key Insights

### 1. The more times users used the app, the less likely they were to churn. While 40% of the users who didn't use the app at all last month churned, nobody who used the app 30 days churned.

### 2. Distance driven per driving day had a positive correlation with user churn. The farther a user drove on each driving day, the more likely they were to churn.

### 3. Number of driving days had a negative correlation with churn. Users who drove more days of the last month were less likely to churn.

### 4. Users of all tenures from brand new to ~10 years were relatively evenly represented in the data.

### 5. Nearly all the variables were either very right-skewed or uniformly distributed. 

### 6. For the right-skewed distributions, this means that most users had values in the lower end of the range for that variable. 

### 7. For the uniform distributions, this means that users were generally equally likely to have values anywhere within the range for that variable.

### 8. Several variables had highly improbable or perhaps even impossible outlying values, such as: driven_km_drives, activity_days and driving_days.



## Next Step

**Investigate the erroneous or problematic discrepancies between number of sessions, driving_days, and activity_days.**

**Continue to explore user profiles with the greater Waze team; this may glean insights on the reason for the long distance drivers’ churn rate.**

**Plan to run deeper statistical analyses on the variables in the data to determine their impact on user churn.**








## Step by Step EDA Process

- Imports, links, and loading

- Data Exploration

- Data cleaning

- Building visualizations

- Evaluating and sharing results

- For EDA of the data, import the data and packages that will be most helpful, such as pandas, numpy, and matplotlib.

- Read in the data and store it as a dataframe object called df.

- Data overview and summary statistics

head()

size()

describe()

info()

- Generate summary statistics using the describe() method.

- And summary information using the info() method.

- Visualizations

- Now that you know which data columns you’ll use, it is time to decide which data visualization makes the most sense for EDA of the Waze    dataset
 
Line graph

Bar chart

Box plot

Histogram

Heat map

Scatter plot

A geographic map

- Box plots will be helpful to determine outliers and where the bulk of the data points reside in terms of drives, sessions and all other    continuous numeric variables

- Histograms are essential to understand the distribution of variables

- Scatter plots will be helpful to visualize relationships between variables

- Bar charts are useful for communicating levels and quantities, especially for categorical information

- Begin by examining the spread and distribution of important variables using box plots and histograms.

- The number of occurrences of a user opening the app during the month

- The sessions variable is a right-skewed distribution with half of the observations having 56 or fewer sessions. However, as indicated by   the boxplot, some users have more than 700.

- An occurrence of driving at least 1 km during the month

- The drives information follows a distribution similar to the sessions variable. It is right-skewed, approximately log-normal, with a       median of 48. However, some drivers had over 400 drives in the last month.

- A model estimate of the total number of sessions since a user has onboarded

- The `total_sessions` is a right-skewed distribution. The median total number of sessions is 159.6. This is interesting information because, if the median number of sessions in the last month was 56 and the median total sessions was ~160, then it seems that a large proportion of a user's (estimated) total drives might have taken place in the last month. This is something you can examine more closely later.

- The number of days since a user signed up for the app

- The total user tenure (i.e., number of days sinceonboarding) is a uniform distribution with values ranging from near-zero to \~3,500 (\~9.5 years).

- Total kilometers driven during the month

- The number of drives driven in the last month per user is a right-skewed distribution with half the users driving under 3,495 kilometers. As you discovered in the analysis from the previous course, the users in this dataset drive a lot. The longest distance driven in the month was over half the circumferene of the earth.

- Total duration driven in minutes during the month

- The duration_minutes_drives variable has a heavily skewed right tail. Half of the users drove less than ~1,478 minutes (~25 hours), but some users clocked over 250 hours over the month.

- Number of days the user opens the app during the month

- Within the last month, users opened the app a median of 16 times. The box plot reveals a centered distribution. The histogram shows a nearly uniform distribution of ~500 people opening the app on each count of days. However, there are ~250 people who didn't open the app at all and ~250 people who opened the app every day of the month.

- Number of days the user drives (at least 1 km) during the month

- The number of days users drove each month is almost uniform, and it largely correlates with the number of days they opened the app that month, except the driving_days distribution tails off on the right.

- However, there were almost twice as many users (~1,000 vs. ~550) who did not drive at all during the month. This might seem counterintuitive when considered together with the information from activity_days. That variable had ~500 users opening the app on each of most of the day counts, but there were only ~250 users who did not open the app at all during the month and ~250 users who opened the app every day. Flag this for further investigation later.

- The type of device a user starts a session with

- There are nearly twice as many iPhone users as Android users represented in this data.

- Binary target variable (“retained” vs “churned”) for if a user has churned anytime during the course of the month

- Less than 18% of the users churned

- Because both driving_days and activity_days represent counts of days over a month and they're also closely related, you can plot them together on a single histogram. This will help to better understand how they relate to each other without having to scroll back and forth comparing histograms in two different places.

- Confirm the maximum number of days for each variable&mdash;`driving_days` and `activity_days`.

- It's true. Although it's possible that not a single user drove all 31 days of the month, it's highly unlikely, considering there are 15,000 people represented in the dataset.

- One other way to check the validity of these variables is to plot a simple scatter plot with the x-axis representing one variable and the y-axis representing the other.

- Notice that there is a theoretical limit. If you use the app to drive, then by definition it must count as a day-use as well. In other words, you cannot have more drive-days than activity-days. None of the samples in this data violate this rule, which is good.

- Plot a histogram that has four bars—one for each device-label combination—to show how many iPhone users were retained/churned and how many Android users were retained/churned.

- The proportion of churned users to retained users is consistent between device types.

- Retention by kilometers driven per driving day

- Create a new column in df called km_per_driving_day, which represents the mean distance driven per driving day for each user.

- Call the describe() method on the new column.

- This is the result of there being values of zero in the driving_days column. Pandas imputes a value of infinity in the corresponding rows of the new column because division by zero is undefined.

- Convert these values from infinity to zero. You can use np.inf to refer to a value of infinity.

- Call describe() on the km_per_driving_day column to verify that it worked.

- The maximum value is 15,420 kilometers per drive day. This is physically impossible. Driving 100 km/hour for 12 hours is 1,200 km. It's unlikely many people averaged more than this each day they drove, so, for now, disregard rows where the distance in this column is greater than 1,200 km.

- Plot a histogram of the new km_per_driving_day column, disregarding those users with values greater than 1,200 km. Each bar should be the same length and have two colors, one color representing the percent of the users in that bar that churned and the other representing the percent that were retained. This can be done by setting the multiple parameter of seaborn's histplot() function to fill.

- The churn rate tends to increase as the mean daily distance driven increases, confirming what was found in the previous course. It would be worth investigating further the reasons for long-distance users to discontinue using the app.

- Create another histogram just like the previous one, only this time it should represent the churn rate for each number of driving days.

- The churn rate is highest for people who didn't use Waze much during the last month. The more times they used the app, the less likely they were to churn. While 40% of the users who didn't use the app at all last month churned, nobody who used the app 30 days churned.

- This isn't surprising. If people who used the app a lot churned, it would likely indicate dissatisfaction. When people who don't use the app churn, it might be the result of dissatisfaction in the past, or it might be indicative of a lesser need for a navigational app. Maybe they moved to a city with good public transportation and don't need to drive anymore.

- Create a new column percent_sessions_in_last_month that represents the percentage of each user's total sessions that were logged in their last month of use

- Now, create a histogram depicting the distribution of values in this new column.

- Check the median value of the `n_days_after_onboarding` variable.

- Half of the people in the dataset had 40% or more of their sessions in just the last month, yet the overall median time since onboarding is almost five years.

- Make a histogram of n_days_after_onboarding for just the people who had 40% or more of their total sessions in the last month.

- The number of days since onboarding for users with 40% or more of their total sessions occurring in just the last month is a uniform distribution. This is very strange. It's worth asking Waze why so many long-time users suddenly used the app so much in the last month.

- The box plots from the previous section indicated that many of these variables have outliers. These outliers do not seem to be data entry errors; they are present because of the right-skewed distributions.

Depending on what you'll be doing with this data, it may be useful to impute outlying data with more reasonable values. One way of performing this imputation is to set a threshold based on a percentile of the distribution.

To practice this technique, write a function that calculates the 95th percentile of a given column, then imputes values > the 95th percentile with the value at the 95th percentile. such as the 95th percentile of the distribution.

Next, apply that function to the following columns:

sessions

drives

total_sessions

driven_km_drives

duration_minutes_drives

- Call describe() to see if your change worked.


#### Conclusion

**Analysis revealed that the overall churn rate is \~17%, and that this rate is consistent between iPhone users and Android users.**

**Perhaps you feel that the more deeply you explore the data, the more questions arise. This is not uncommon! In this case, it's worth asking the Waze data team why so many users used the app so much in just the last month.**

**Also, EDA has revealed that users who drive very long distances on their driving days are _more_ likely to churn, but users who drive more often are _less_ likely to churn. The reason for this discrepancy is an opportunity for further investigation, and it would be something else to ask the Waze data team about.**





Any query connect nihalshaikh.analyst@gmail.com

----------Thank you.............

  
