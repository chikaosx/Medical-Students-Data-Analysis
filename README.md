# Medical-Students-Data-Analysis


# Introduction
This task focus on the insightful analysis of the Medical Students Data, focusing on key parameters and statistics to better understand the health profile of medical students at Chika's University.

# Activity
Using the provided data, we are required to create Pivot Tables displaying the average values for various health metrics, as well as other relevant statistics, categorized by gender and medical conditions. Below are the necessary tasks we required to perform for this project:

1. Average Values for Male and Female Students:
   - Age: The average age for male and female students was calculated separately.
   - BMI (Body Mass Index): Average BMI for male and female students.
   - Temperature: Average body temperature for male and female students.
   - Heart Rate: Average heart rate for male and female students.
   - Blood Pressure: Average blood pressure for male and female students.
   - Cholesterol: Average cholesterol level for male and female students.

2. Average Height and Weight for both Genders:
   - Average Height: The average height of male and female students (rounded to two decimal places).
   - Average Weight: The average weight of male and female students (rounded to two decimal places).

3. Number of Students across Different Blood Groups:
   - The distribution of students across various blood groups is presented, providing an overview of the blood group distribution within the cohort.

4. Number of Students Who Smoke and Those Who Don't:
   - The count of students who smoke and those who don't, allowing us to understand the prevalence of smoking habits among the students.

5. Number of Students Who Have Diabetes and Those Who Don't:
   - The count of students with diabetes and those without, enabling us to assess the incidence of diabetes in the student population.

# Skill Demonstrated
1. Data Cleaning
2. Data Manipulation
3. Pivot tables

# Raw Data
The Medical Student Dataset, comprises 13 essential columns and an impressive 200,000 records. The dataset encompasses crucial parameters, providing invaluable insights into the health profile of our medical student population.

The dataset includes the following columns:

1. Student ID: A unique identifier for each medical student in the dataset.
2. Age: The age of each student at the time of data collection.
3. Height: The height of each student, providing anthropometric information.
4. Weight: The weight of each student, essential for assessing body mass characteristics.
5. Body Temperature: The recorded body temperature of each student, helping gauge health status.
6. Diabetes: A binary attribute indicating whether a student has diabetes (Yes) or not (No).
7. Cholesterol: Cholesterol levels of each student, a key indicator of cardiovascular health.
8. Blood Type: The blood type of each student A, B, AB, O, aiding in blood group distribution analysis.
9. Blood Pressure: The recorded blood pressure values for each student, essential for cardiovascular assessment.
10. Gender: The gender classification of each student as male or female.
11. BMI (Body Mass Index): Calculated BMI values for each student, a measure of body composition.
12. Smoking: A binary attribute indicating whether a student smokes (Yes) or not (No).
    
![](dataset.PNG)


# Data Cleaning
To clean the dataset, I first conducted a thorough assessment of missing values in each column. It was observed that approximately 20,000 records were missing in each column, accounting for about 10% of the data, which is below the acceptable threshold of 40%. Hence, I opted to use the imputation method for data cleaning.

As the dataset consists of both numerical and categorical data, they required distinct imputation approaches. For the numerical columns, which include age, height, weight, temperature, heart rate, blood pressure, and cholesterol, I decided to impute the missing values with the average value of each respective column. By doing so, we ensure minimal disruption to the overall statistical distribution.

However, for the BMI column, we employed a slightly different approach. To obtain the missing values, we performed data manipulation using the height and weight columns. As BMI is calculated using the formula BMI = kg/m^2, we first converted the height column from centimeters to meters. Subsequently, we applied the mathematical calculation as follows: BMI = weight / (Height(M) * Height(M)). This enabled us to derive accurate BMI values for the affected records.

Moving on to the categorical columns, such as gender, diabetes, blood type, and smoking, we utilized the Mode imputation technique. The Mode refers to the value that appears most frequently in each column. To determine the Mode, we obtained the unique values in each categorical column and used the =COUNTIF() function with a value in the column as a criteria. This process ensured that we assigned the most common value to the missing records, thereby preserving the integrity of the categorical distribution.

# Data Manipulation

# Pivot tables

# Conclusion
