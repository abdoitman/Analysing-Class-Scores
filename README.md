# **Analysing Class Scores**
## Overview
Analysing a whole class' CGPA and registered credit hours in college. The data was origanally collected from real college students scores and obtained credit hours in a text form containing the IDs, registered credit hours and the CGPA of the students. Then it was converted into excel using a simple python script, after that, it was further organized into an excel workbook adding the name and the gender for each students using another sheet.

## The Data
The Data used in this project is found in the excel woorkbook named **class_data.xlsx** which contain **2** sheets.<br>
The main sheet contains **248** enteries each represent a student with the following columns:
1) **ID**: Unique college ID.
2) **Hours_Taken**: Total credit hours each student has completed up to senior year.
3) **CGPA**: Cumulative GPA of the student at senior year.
5) **Gender**: Gender of the student, M for male, F for female
6) **Name**: Name of the student.

The second sheet contains **ID**, **Gender** and **Name** columns. This sheet is the look up table for the main sheet.<br>

### Basic Statistics of The Data
At first before we get into the details, a quick analysis of the data will get us the following information:
1) **Average (Mean) CGPA** of the class = **2.973**
2) **Maximum** CGPA of the class = **3.76**
3) **Minimum** CGPA of the class = **1.98**
4) **Average (Mean) completed credit hours** = **130**
5) **Maximum completed credit hours** = **135**
6) **Minimum completed credit hours** = **115**

## Analysing Class CGPA
We Notice that the distibution of the class' CGPA is as following<br>
![image](https://user-images.githubusercontent.com/77892920/215297427-23ab11c4-e707-4762-b18b-00bc2e60a0c6.png)
As seen above most students lie around 3 CGPA with around **third of students** lie between **2.9** and **3.2**<br><br>

Now we are interested in categorizing the students into 4 tiers:
1) **Tier 1 (Excellent)** : Students who got a CGPA equal to 3.3 or more
2) **Tier 2 (Very Good)** : Students who got a CGPA between 3.3 and 2.7
3) **Tier 3 (Good)** : Students who got a CGPA between 2.7 and 2.3
4) **Tier 4 (Ok)** : Students who got a CGPA between 2.3 and 1.7
![image](https://user-images.githubusercontent.com/77892920/215297913-483ed1e4-e64d-4f9e-9be5-0f07adaa4239.png)<br>
As shown above, we conclude that two thirds of students lie in tier 2.

## Analysing Number of Completed Credit Hours Among The Class

First we get the distribution among the class<br>
![image](https://user-images.githubusercontent.com/77892920/215299013-4e6e4178-8e63-47ac-aa59-5e7e0e7c5eef.png)<br>
We notice that most of the students **(around 67%)** completed 133 credit hours up to senior year.<br>

## Correlation between CGPA and completed credit hours
![image](https://user-images.githubusercontent.com/77892920/215299436-19b92fbe-fccf-4b3d-9c70-afc665ed38db.png)<br>
Here we notice that students who completed less than average (130) credit hours have a lower average CGPA than students who completed 130 credit hours or more. We also notice one outlier who completed less than average credit hours, yet scored an excellent CGPA.<br>
This might have happened due to many reasons such as scoring a GPA less 2 in any semester will lead to the student registering less credit credit hours the following semester, *but determining whether that's the case or not will require more data such previous semesters GPA*<br>
### A more detailed look on CGPA vs completed credit hours
![image](https://user-images.githubusercontent.com/77892920/215299882-0c226052-77a9-4ac5-a00b-ee472cf98d12.png)<br>

## Male Students vs. Female Students
The count of genders in the class is as follows:<br>
█████████████ - **160 (64.52%) Males**<br>
███████ - **88 (35.48%) Females**<br>

### Male students' CGPA vs Female students' CGPA
**Mean CGPA for male studens = 2.987**<br>
**Mean CGPA for female studens = 2.949**<br>
![image](https://user-images.githubusercontent.com/77892920/215300733-f1468a34-7544-44f2-8fe8-3da956648b4f.png)<br>
Looking at the above violin plot, we notice that male students' CGPA are more condensed around 3, while the female students' CGPA are more spread out having more range.<br>
### Males vs Females in Different Tiers
![image](https://user-images.githubusercontent.com/77892920/215301296-7d837cf0-ec8a-4578-bade-38788d847365.png)
### Males' vs Females' Completed Credit Hours
![image](https://user-images.githubusercontent.com/77892920/215301319-f4373c9a-b769-46f2-b0f1-7493969721e9.png)<br>
We conclude that roughly the distribution of male students and female students doesn't change much in both CGPA Ties and completed credit hours.<br>
### CGPA vs Completed Credit Hours for Males and Females
To get a more detailed look at male students data and female students data we plot a scatter graph for CGPA and completed credit hours for both male and female studetns.
![image](https://user-images.githubusercontent.com/77892920/215302160-fa8bdd99-5d1b-4969-8e09-1d7e87eb4dc2.png)
