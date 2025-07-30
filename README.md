#🎓 Nexyug Classes Project

This project explores student performance data to identify trends and insights using Python and data science tools. It's ideal for beginners looking to understand how to clean
, transform, and analyze data in a structured way.


# Project Overview

The goal of this notebook is to analyze a dataset called StudentsPerformance.csv which contains information about students' demographics, their participation in test preparation
courses, and their scores in math, reading, and writing. Using this data, we aim to:

###1.Clean and prepare the dataset.

###2.Perform basic statistical analysis.

###3.Apply label encoding to categorical variables.

###4.Visualize and interpret performance trends.

---

##🧠 What You'll Learn

###1.Loading and previewing CSV data with pandas

###2.Checking and handling missing data

###3.Encoding categorical variables using LabelEncoder

###4.Visualizing data distributions and correlations

###5.Understanding how different factors (like parental education, gender, lunch types, etc.) influence student performance

---

##📦 Dependencies

To run this notebook smoothly, make sure you have the following libraries installed:

pip install pandas numpy matplotlib seaborn scikit-learn


---

##🧾 Dataset Description

The dataset contains the following columns:

Column Name	Description

gender	Gender of the student (male/female)
race/ethnicity	Ethnic group the student belongs to
parental level of education	Highest education level of the parents
lunch	Type of lunch (standard or free/reduced)
test preparation course	Whether the student completed a test prep course
math score	Score in math (0–100)
reading score	Score in reading (0–100)
writing score	Score in writing (0–100)


##🛠 Key Steps

###1. Load and View Data

Har = pd.read_csv("StudentsPerformance (1).csv")
Har.head()

###2. Data Cleaning

Check for missing values:

Har.isnull().sum()

###3. Encode Categorical Columns

Label encoding is used to convert text categories into numeric labels for ML models.

###4. Data Analysis

#### Plotted the score distributions using Histograms 
#### Compared the average values by gender , lunch type and test preparation
#### Created the correlation heatmap
#### Have used the boxplots and barplots for the insights

###5.Features Enginerring 

#### Created a new column average_score
#### Created a new column result which consist of :
     1. "Pass" if average score ≥ 50
     2. else "Fail"
#### Converted the result to binary labels(0 and 1) , by using LabelEncoder 

-----

## Used Machine Learning Models

### 1. Prediction 

       Used the following models to predict "Pass" or "Fail":
       #### 1. Logistic Regression
       #### 2. K-Nearest Neighbors (KNN)

        Also checked the following things : 
        #### 1.Accuracy Score
        #### 2.Classification Report
        #### 3.Confusion Matrix


##2. Clustering 

            Use K-Means Clustering to group students based on performance patterns
            Cluster by math score, reading score, and writing score
            Visualize clusters using 2D plots



---

##📊 Sample Output Preview

gender	race	education	lunch	prep course	math	reading	writing

Female	B	Bachelor	Standard	None	72	72	74
Male	C	Some College	Reduced	Completed	47	57	44


After label encoding:

Gender becomes 0 (female) or 1 (male)

Lunch becomes 0 or 1

Other categories are also numerically mapped



---

🧩 Conclusion

By the end of this project, you'll be able to:

Handle and clean real-world datasets

Apply preprocessing steps like encoding

Analyze trends in educational data

Build visual representations to support findings

