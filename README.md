# Skin-Disorder-Prediction
A Machine Learning Project
## Problem Statement:
### 1)Prepare a complete data analysis report on the given data.
### 2) Create a predictive model using machine learning techniques to predictthe various classes of skin disease.
### 3) Suggestions to the Doctors to identify the skin diseases of the patient atthe earliest.
## Steps Involved:
### 1) Importing Neccessary libraries and dataset:
i) numpy 

ii) pandas 

iii) matplotlib.pyplot

iv) seaborn

### 2) Basic Checks and Data Cleaning:
i) Checking for the top and bottom entries to get general idea about the dataset. 

ii) Checking for the duplicates. 

iii) Checking for the null values. 

iv) Checking for the data types for all features. 

v) It is observed that the 'Age' feature has data type as object but 'Age' must be numeric, so finding the non-numeric entries from the 'Age' feature. 

vi) Coverting the 'Age' feature tu numeric which converts the all non-numeric entries into NaN. 

vii) Drpoing the NaN entries. 

### 3) EDA:
i) Finding the Descriptive Statistics for the data. 

ii) Calculating the mode during Univariate Analysis. 

iii) In Bivariate Analysis Ploting the countplot of every feature of the disease to see the presennce of that feature in the patients of various types of skin diseases. 

iv) In Multivariate Analysis checking the correlation between the different features of the data using the Heatmap plot of seaborn library. 

### 4) Data Preprocessing and Feature Engineering:
i) PCA, which involves the dimenssion reduction.  

ii) Feature selection, which involves selecting only those principle components who explains the 90% of variance in the data. 

### 5) Model Implementation:
i) Logistic Regression 

ii) Decision Tree 

iii) Random Forests 

iv) KNN 

v) SVM 

vi) XGBoost 

### 6) Saving the Best Model 

## Key Findings:
### 1) Logistic Regression:
Perfect classification for classes 1, 5, and 6, with precision, recall, and F1-score = 1.00.
Class 4 has slightly lower precision & recall (87% & 93%), meaning occasional misclassification.
Macro & weighted averages (~97%) confirm consistent performance across all classes.
The model shows strong generalization with high recall, ensuring most classes are correctly identified.
### 2) Decision Tree:
Perfect classification for classes 1 and 3, with precision, recall, and F1-score = 1.00.
Class 2 has high recall (100%), meaning it correctly identifies all instances of this class.
Class 4 has a lower recall (71%), indicating some misclassifications.
Class 6 has lower precision (71%), meaning some instances are misclassified into this class.
Macro and weighted averages (~93-94%) show consistent overall performance across all classes.
### 3) Random Forests:
Perfect classification for classes 1, 3, 5, and 6 (precision, recall, and F1-score = 1.00), meaning these classes are predicted flawlessly.
Class 2 has 100% recall, meaning all instances of class 2 were correctly identified.
Class 4 has a slightly lower recall (79%), suggesting a few misclassifications.
Macro and weighted averages (~97%) confirm consistent performance across all classes.
### 4) KNN:
High precision (94%) for Class 1, meaning very few false positives.
Class 2 struggles (70% precision & 67% recall), suggesting misclassification.
Class 4 has lower precision (50%), implying significant misclassification.
Class 5 has low recall (65%), meaning some instances were missed.
Macro and weighted averages (~82-85%) indicate overall reasonable performance, but not as strong as other models.
### 5) SVM:
Perfect classification for classes 1, 3, 5, and 6, achieving 100% precision, recall, and F1-score.
Class 2 has high recall (100%), ensuring all instances are correctly classified.
Class 4 has slightly lower recall (86%), suggesting a few misclassifications.
Macro and weighted averages (~98%) confirm strong generalization across all classes.
### 6) XGBoost:
Some classes, like 0, 2, 4, and 5, are classified perfectly with 100% precision, recall, and F1-score.
Class 1 and 3 have slight variations, but still maintain a strong performance.
Class 3’s recall (0.79) indicates a few misclassifications, but overall, the model is highly effective.
### 7) Best Model:
SVM stands out as the strongest candidate, delivering perfect classification for multiple classes, maintaining high recall across all, and having the highest overall consistency.
### 8) Suggestions to the Doctors:
Most of the patients have class 1 disease, which is Psoriasis. Therefore, prioritize checking for this disease. The most commonly observed symptoms are erythema, scaling, definite borders, itching, acanthosis, parakeratosis, and inflammatory mononuclear infiltrate at levels 1 and 2, which are the early stages. So, check for these symptoms first.
