# Job-Change-of-Data-Scientists
### EDA and Predict who will move to a new job

### General information
A company which is active in Big Data and Data Science wants to hire data scientists among people who successfully pass some courses which conduct by the company. Many people signup for their training. Company wants to know which of these candidates are really wants to work for the company after training or looking for a new employment because it helps to reduce the cost and time as well as the quality of training or planning the courses and categorization of candidates. Information related to demographics, education, experience are in hands from candidates signup and enrollment.

This dataset designed to understand the factors that lead a person to leave current job for HR researches too. By model(s) that uses the current credentials,demographics,experience data you will predict the probability of a candidate to look for a new job or will work for the company, as well as interpreting affected factors on employee decision.

### Features and target

    - enrollee_id : Unique ID for candidate

    - city: City code

    - city_ development _index : Developement index of the city (scaled)

    - gender: Gender of candidate

    - relevent_experience: Relevant experience of candidate

    - enrolled_university: Type of University course enrolled if any

    - education_level: Education level of candidate

    - major_discipline :Education major discipline of candidate

    - experience: Candidate total experience in years

    - company_size: No of employees in current employer's company

    - company_type : Type of current employer

    - lastnewjob: Difference in years between previous job and current job

    - training_hours: training hours completed

    - target: 0 – Not looking for job change, 1 – Looking for a job change
    
### EDA limitation and conclusion 
    - The data contains 19158 Rows and 14 columns includes Target variable. This is a reasonable size and will allow me to work in Jupyter notebooks
    - The most of features dtype is 'object', its mean we work with categorical data.
    - There are many features contains missing values.
    - we should to make some transformations on the features like 'relevant_exprience' to change values to 'yes', or 'no', and 'Experience', and company size.
    - The distribution of training hours seems to be skewed right.
    - There are systematic algorithms that we can use to generate synthetic samples. The most popular of such algorithms is called SMOTE or the Synthetic Minority Over-sampling Technique
    - One way to remove the skewness is by doing the log transformation. As we take the log transformation, it does not affect the smaller values much, but reduces the larger values.
    - city_development index is highly correlated with target variable
    - some information: Most of the people whome participate in our courses are 'male' and they have a 'relevant experience' in the field and they graduates or complete the master degree.
    - STEM Students are more intersted in data science more than another discplines
### Modeling Phase
    KNeighborsClassifier
    LogisticRegression
    DecisionTreeClassifier
    XGBClassifier
    SVM

#### Hint:- The project is still in the progress 

