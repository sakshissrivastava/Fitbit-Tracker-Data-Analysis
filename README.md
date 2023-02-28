# Fitbit Tracker DataSet Analysis

The data set used for this analysis is available on [Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit)

### Task: 
Analyze FitBit fitness tracker data to gain insights into how consumers are using the FitBit app and discover trends for marketing strategy.

### About the Dataset:
1) Data is publicly available on Kaggle: FitBit Fitness Tracker Data and stored in 18 csv files.
2) Generated by respondents from a survey via Amazon Mechanical Turk between 12 March 2016 to 12 May 2016.
3) 30 FitBit users consented to the submission of personal tracker data.
4) Data collected includes physical activity recorded in minutes, heart rate, sleep monitoring, daily activity, steps and calories.

### Limitations:
A good dataset must ROCCC or in other words must be Reliable, Original, Comprehensive, Current, Cited. 

1) Reliable: LOW - Not reliable as it only has 30 respondents
2) Original: LOW - Generated by Third Party (Amazon Mechanical Turk)
3) Comprehensive: MED - Data minute-level output for physical activity, heart rate, and sleep monitoring. While the data tracks many factors in the user activity and sleep, but the sample size is small and most data is recorded during certain days of the week.
4) Current: LOW - Dataset is almost 7 years old and might not be relevant
5) Cited: LOW - Data collected from third party, hence unknown

Hence this dataset is considered bad quality and must not be used of making any business decisions.

### Tools:
Python is used for data cleaning, transformation and visulization

### CSV file used:
1) dailyActivity_merged.csv
2) sleepDay_merged.csv
3) hourlyIntensities_merged.csv

### Findings:
##### dailyActivity_merged.csv & sleepDay_merged ->
 There are 33 unique Ids avaialable in the csv file.
 NO NULL values
 
#### Statistical Observation:
1) On average, users logged 7,637 steps or 5.4km which is not adequate. As recommended by CDC, an adult female has to aim at least 10,000 steps or 8km per day to benefit from general health, weight loss and fitness improvement.
2) Average sedentary time is 991 minutes or 16 hours which is a lot!
3) Average calories burned is 2,303 calories equivalent to 0.6 pound. Details cannot be adeuqately interpreted as calories burned depend on several factors such as the age, weight, daily tasks, exercise, hormones and daily calorie intake.

#### Visulization Interpretations:

<img src="https://user-images.githubusercontent.com/123297799/221629654-353c6422-c3ec-4146-b43c-71683fc096ec.png" width="250" height="250">

1) From the Histogram above is is discovered that users prefer or remember to track their activity on the app during midweek from Tuesday to Friday.
2) The frequency dropped on Friday and continue on weekends and Monday.

![image](https://user-images.githubusercontent.com/123297799/221651980-abaac333-de3d-403b-98c6-691797f3b540.png)

1) There is a positive correlation seen in the calories vs steps taken visulization above. 
2) The intensity of calories burnt is more between 0 to 15,000 steps taken as compared to higher value of steps

![image](https://user-images.githubusercontent.com/123297799/221652988-6659cf06-23dd-4a8c-bdb1-4725e982f99f.png)  ![image](https://user-images.githubusercontent.com/123297799/221653046-039e442c-bea1-414a-8d09-0c0c2ea32545.png)

Calories burnt every hours logged weak positive relationship, this maybe be due to higher sedentary hours. According to the pie chart sedentary times accounts for 81% of the total time logged. 
**This could highly be because the users might be utilizing the fitness band for daily commute, inactive movements (moving from one spot to another) or running errands and lesser for tracking their fitness.**

![image](https://user-images.githubusercontent.com/123297799/221653609-8098798a-9f16-444f-9f9f-8cbbcf14b24a.png)  ![image](https://user-images.githubusercontent.com/123297799/221658042-63773f0d-c75c-4e89-bcde-fab942ce154f.png)

Sedentary time also shows the negative linear correlation with total minutes asleep. This shows that higher sedentary minutes accounts for lesser sleep.

##### hourlyIntensities_merged.csv
![image](https://user-images.githubusercontent.com/123297799/221654056-9a76d6a8-2d28-4fe2-801a-080f79fd1bbf.png)

After visualizing Total Intensity hourly, it is found out that people are more active between 5 am and 10pm.


### Recommendations:

As per the analysis, the markteing team of any other fitness brands which have the similar devices can benefit from these findings:
1) The marketing team can encourage users by enlightening and empowering them with knowledge about the advantages of fitness, suggesting various forms of exercise (for example, a straightforward 10 minute exercise on weekdays and a more intense exercise on weekends), and providing information on calorie intake and burn rate on the thier respective app.
2) The company's app can also send out notifications on the weekends to motivate users to work out.
3) If the users wants to improve their sleep they can consider reducing the sedenatary hours and increase in time on bed hours. The company app can send notifications to go to sleep earlier.
4) Since most activity happens between 5 pm and 7 pm it is safe to assume that people go to a gym or for a walk after finishing work. This time frame can be utilized by the companies to remind and motivate users to go for a run or walk.

