# School_District_Analysis
#### Analyzing school district with Pandas


### Overview of the school district analysis: Explain the purpose of this analysis.
In PyCitySchools we're going to change the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once we change the math and reading scores, we would like you to repeat the school district analysis that we did in PyCitySchools module.
In this module we learn how to use *loc()* method with conditional statements and comparison and logical operators, we will select the ninth-grade reading and math scores for Thomas High School Then, use the Pandas NumPy module to change the reading and math scores to NaN.

### Results: Using bulleted lists and images of DataFrames as support, address the following questions.

before reviewing some questions let's go through important parts of the code to see how it works.
In this part of the code we're Cleaning Student Names.

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/clean.PNG)

and in Deliverable 1 we replace the 9th grade reading and math scores at Thomas High School with NaN. 

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/nan.PNG)

In Deliverable 2 we make different DataFrames to analyse the data from different aspects. and with added changes we make new DataFrames and compare it with the ones we had from PyCitySchools which is in the same file in PyCitySchools_challenge. we will see that Thomas High School rank will change from 2nd to 8th because of all the NaNs we added to data.

In school summary by using loc method we calculate new math, reading and overal passing and replacing it in the school summary dataframe.

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/overall.PNG)

now let's answer some questions compare the results.

## How is the district summary affected?

This is the result for district_summary_df in PyCitySchools before changes

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/district_summary_df1.PNG)

and this is the results after changes in PyCitySchools_challenge

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/district_summary_df2.PNG)

> we can see the difference in the results after changing the 9th grade in Thomas High School, it's affecting all the Average Math Score, % Passing Math,% Passing Reading, % Overall Passing.

## How is the school summary affected?

this is Thomas High School before chane in PyCitySchools
![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/per_school_summary_df1.PNG)

and this is the results after changes in PyCitySchools_challenge 

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/per_school_summary_df2.PNG)

> we can see the change in % Overall Passing, first it was 91 and then after change in PyCitySchools_challenge it goes down to 65, which we can realize after adding NaNs, it's dropping down all the results.

## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

let's take a look at the code these two pictures, before and after change

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/top5_1.PNG)


![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/top5_2.PNG)

> in the first picture Thomas High School in PyCitySchools is the 2nd top school and in the second picture after the change it's in 8th place.

## How does replacing the ninth-grade scores affect the following:

#### - Math and reading scores by grade

this is the picture for PyCitySchools

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/math_grade1.PNG)

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/reading_grade1.PNG)

and this the picture for PyCitySchools_challenge

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/math_grade2.PNG)

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/reading_grade2.PNG)

> we compare 9th grade which we changed the vlues, in grade DataFrame we don't see much difference in both pictures. the ninth grade for math and reading classes are NAN and it's not giving us any mean for ninth grade Thomas High School.

#### - Scores by school spending

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/spending1.PNG)

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/spending2.PNG)

> in spending DataFrame we can see slight different in $630-644 bin, if we compare overal passing in PyCitySchools is 62.85 and in PyCitySchools_challenge is 62.77 .

#### - Scores by school size

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/size1.PNG)

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/size2.PNG)

in size DataFrame we can see slight different in Medium size bin, if we compare overal passing in PyCitySchools is 90.62 and in PyCitySchools_challenge is 90.55 .

#### - Scores by school type

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/type1.PNG)

![name-of-you-image](https://github.com/samiramghd/School_District_Analysis/blob/main/Resources/type2.PNG)

in type DataFrame we can see slight different in charter bin, if we compare overal passing in PyCitySchools is 90.43 and in PyCitySchools_challenge is 90.39 .

### Summary: Summarize four changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.

- The overall passing rate for Thomas High School droped from 91% to 65%
- Thomas High School before change had the 2nd in top 5 but after change it dropped to 8th place.
- All data is showing "NaN" in reports for the 9th grade students at Thomas High School which is affecting on entire data results.
- In most results we compared the overall passing rate, the campus math and reading averages and passing percentages all been affected too. 
