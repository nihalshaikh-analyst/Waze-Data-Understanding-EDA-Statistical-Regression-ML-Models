# Statistical Analysis of Waze app

This project uses a dataset called waze_app_dataset.csv. It contains synthetic data created for this project in partnership with Waze. Data analyze, clean, process, data analysis by using Python and its Library **pandas, numpy, matplotlib.pyplot, seaborn** and **Statistical anaysis, A/B testing, Hypothesis testing** with presentation in Jupyter Notebook.

![waze logo](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/waze%20logo.png)


## Project Overview

#### "The Waze data team is currently developing a data analytics project aimed at increasing overall growth by preventing monthly user churn on the Waze app. As part of the effort to improve retention, Waze wants to learn more about users’ behavior. This report offers information on the project status and results of Milestone 4, which impact the future development of the overall project."  


## Project background

- Explore the project data

- Implement a hypothesis test

- Communicate insights with stakeholders within Waze

[Waze Dataset](https://github.com/nihalshaikh-analyst/Waze-Churn-Data-Understanding-and-Analysis/blob/main/waze_app_dataset.csv)


## Specific project deliverables

- Complete the questions in the Course 4 PACE strategy document

- Answer the questions in the Jupyter notebook project file

- Conduct a two-sample hypothesis test

- Create an executive summary to share your results


## Jupyter Notebook

[Notebook](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Statistical%20Analysis%20of%20Waze.ipynb)


## Storytelling and Problem Solveing

### Objective

🎯 Target Goal: Develop a two-sample hypothesis test to analyze and determine whether there is a statistically significant difference between mean number of rides and device type – Android vs. iPhone.
🎯 Impact: Statistical tests, such as the one conducted for Milestone 4, enable the Waze data team to make inferences about the populations from which the data was drawn and help them learn more about their user base.

[Presentations](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Statistics%20of%20Waze%20Findings.pptx)


![presentations](https://github.com/nihalshaikh-analyst/Waze-Data-Understanding-EDA-Statistical-Regression-ML-Models/blob/main/Statistics%20of%20Waze%20Presentation.png)


## Result

##### "Based on the calculations, drivers who use an iPhone to interact with the application have a higher number of drives on average." 

##### "The t-test results concluded there is not a statistically significant difference in mean number of rides between iPhone users and Android users."


<img width="431" height="425" alt="image" src="https://github.com/user-attachments/assets/d188d15e-c6f3-4dc9-adc0-918a10eb9c64" />



## Next Step

##### Due to the results rendered from this specific hypothesis test, the Waze data team recommends running additional t-tests on other variables to learn more about user behavior.

##### Additionally, since the user experience is the same, temporary changes in marketing or user interface may be impactful rendering more data to investigate user churn behavior. 


## Step by Step Process

- The purpose of this project is to demostrate knowledge of how to conduct a two-sample hypothesis test.

- The goal is to apply descriptive statistics and hypothesis testing in Python.

-  Imports and data loading

-  Conduct hypothesis testing

-  Communicate insights with stakeholders

-  Data exploration and hypothesis testing

-  Imports and data loading¶
Import packages and libraries needed to compute descriptive statistics and conduct a hypothesis test.

- Import the dataset.

- In general, descriptive statistics are useful because they let you quickly explore and understand large amounts of data. In this case, computing descriptive statistics helps you quickly compare the average amount of drives by device type.

- Data exploration
Use descriptive statistics to conduct exploratory eata analysis (EDA).

- In the dataset, device is a categorical variable with the labels iPhone and Android.

- Creating a new variable is ideal so that you don't overwrite original data.

- Hypothesis testing¶
State the null hypothesis and the alternative hypothesis
Choose a signficance level
Find the p-value
Reject or fail to reject the null hypothesis

- This is a t-test for two independent samples. This is the appropriate test since the two groups are independent (Android users vs. iPhone users).

- Hypotheses:

𝐻0
 : There is no difference in average number of drives between drivers who use iPhone devices and drivers who use Androids.

𝐻𝐴
 : There is a difference in average number of drives between drivers who use iPhone devices and drivers who use Androids.
  

- Next, choose 5% as the significance level and proceed with a two-sample t-test.

- Isolate the drives column for iPhone users.

- Isolate the drives column for Android users.

- Perform the t-test

## Conclusion

**Since the p-value is larger than the chosen significance level (5%), you fail to reject the null hypothesis. You conclude that there is not a statistically significant difference in the average number of drives between drivers who use iPhones and drivers who use Androids.**

**The key business insight is that drivers who use iPhone devices on average have a similar number of drives as those who use Androids.**

**One potential next step is to explore what other factors influence the variation in the number of drives, and run additonal hypothesis tests to learn more about user behavior. Further, temporary changes in marketing or user interface for the Waze app may provide more data to investigate churn.**


Any concern please contatct to us nihalshaikh.analyst@gmail.com


-------------------Thank you.........................
