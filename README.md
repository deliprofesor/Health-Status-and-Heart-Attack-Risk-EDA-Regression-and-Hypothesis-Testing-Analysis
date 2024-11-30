# Health Status and Heart Attack Risk: EDA, Regression, and Hypothesis Testing Analysis

![health](https://github.com/user-attachments/assets/3c62c98f-a6f2-4591-9fe9-7a8894c418e7)


Veri setinin boyutu büyük olduğu için githuba eklenememiştir.
- **Veri seti: https://www.kaggle.com/datasets/tarekmuhammed/patients-data-for-medical-field/data**
- **Repo : https://www.kaggle.com/code/lknurylmaz/sa-l-k-durumu-ve-kalp-krizi-riski-eda-regresyon**

  
Veri seti aşağıdaki özellikleri içermektedir:

- **PatientID:** Unique identifier for each patient.
- **State:** Geographic state of residence.
- **Sex:** Gender of the patient.
- **GeneralHealth:** Self-reported health status.
- **AgeCategory:** Categorized age group of the patient.
- **HeightInMeters:** Height of the patient (in meters).
- **WeightInKilograms:** Weight of the patient (in kilograms).
- **BMI:** Body Mass Index, calculated from height and weight.
- **HadHeartAttack:** Indicator of whether the patient had a heart attack.
- **HadAngina:** Indicator of whether the patient experienced angina.
- **HadStroke:** Indicator of whether the patient had a stroke.
- **HadAsthma:** Indicator of whether the patient has asthma.
- **HadSkinCancer:** Indicator of whether the patient had skin cancer.
- **HadCOPD:** Indicator of whether the patient had chronic obstructive pulmonary disease (COPD).
- **HadDepressiveDisorder:** Indicator of whether the patient was diagnosed with a depressive disorder.
- **HadKidneyDisease:** Indicator of whether the patient had kidney disease.
- **HadArthritis:** Indicator of whether the patient had arthritis.
- **HadDiabetes:** Indicator of whether the patient had diabetes.
- **DeafOrHardOfHearing:** Indicator of hearing impairment.
- **BlindOrVisionDifficulty:** Indicator of vision impairment.
- **DifficultyConcentrating:** Indicator of concentration difficulties.
- **DifficultyWalking:** Indicator of walking difficulties.
- **DifficultyDressingBathing:** Indicator of difficulties in dressing or bathing.
- **DifficultyErrands:** Indicator of difficulties in running errands.
- **SmokerStatus:** Status of whether the patient is a smoker.
- **ECigaretteUsage:** Indicator of e-cigarette usage.
- **ChestScan:** Indicator of whether the patient had a chest scan.
- **RaceEthnicityCategory:** Race or ethnicity of the patient.
- **AlcoholDrinkers:** Status of whether the patient consumes alcohol.
- **HIVTesting:** Status of whether the patient was tested for HIV.
- **FluVaxLast12:** Status of whether the patient received a flu vaccine in the last 12 months.
- **PneumoVaxEver:** Status of whether the patient ever received a pneumococcal vaccine.
- **TetanusLast10Tdap:** Status of whether the patient received a tetanus vaccine in the last 10 years.
- **HighRiskLastYear:** Indicator of whether the patient was at high risk in the last year.
- **CovidPos:** Status of whether the patient tested positive for COVID-19.

This project focuses on analyzing a comprehensive dataset related to health status and heart attack risk, using Exploratory Data Analysis (EDA), hypothesis testing, and regression techniques. The dataset includes medical and demographic features such as BMI, heart attack history, lifestyle factors (e.g., smoking, alcohol consumption), and other health conditions. The main goal is to examine relationships between these variables, especially BMI, and heart attack risk, using statistical and machine learning methods.

## Objectives of the Project

## Data Cleaning and Preprocessing:

- **Handling missing data.**
- **Removing unnecessary columns.**
- **Converting non-numeric columns to numeric values.**
- **Ensuring that the data is clean for further analysis.**
  
## Exploratory Data Analysis (EDA):

Using statistical measures like means, medians, and distributions to analyze the data. Visualizing the data to understand the trends, patterns, and relationships between features.

- **Hypothesis Testing:** Testing the relationship between BMI and heart attack incidence using t-tests to check for significant differences between the two groups (those who had a heart attack vs. those who did not).
- **Regression Modeling:** Predicting heart attack risk based on the various factors such as BMI, age, lifestyle, and health conditions.


## 1. Data Loading and Preprocessing

The first step involves loading the dataset and addressing issues like missing values and irrelevant columns. Numerical data is converted into a format suitable for analysis, and categorical data is encoded to allow for regression analysis. The data is cleaned and prepared for further exploration.

## 2. Selecting Variables and Computing Correlation Matrix

We focus on numerical variables and compute a correlation matrix to understand the relationships between variables. Particularly, the relationship between BMI and heart attack history is analyzed. The correlation matrix helps in identifying strong and weak relationships among variables, which are essential for building predictive models.
-**Correlation Analysis:** A heatmap is used to visualize the correlation between features, showing how strongly each feature is related to others.

## 3. Exploratory Data Analysis (EDA)

EDA helps to understand the general distribution of the data and uncover insights. The distribution of various features (e.g., BMI, age, heart attack history) is analyzed using histograms and boxplots. Measures like mean, median, and mode are used to summarize the data. Distribution of heart attack cases and other key metrics are visualized to understand patterns.,

## 4. Hypothesis Testing: BMI and Heart Attack Risk

A hypothesis test is conducted to evaluate whether there is a significant difference between the BMI of people who had a heart attack and those who did not. This is done using a t-test, which compares the means of the two groups to see if any significant difference exists.

- **Null Hypothesis (H₀):** There is no significant difference in BMI between people who had a heart attack and those who did not.
- **Alternative Hypothesis (H₁):** There is a significant difference in BMI between the two groups.
- **Test:** A two-sample t-test is performed, and the p-value is computed to assess whether the difference is statistically significant.

## 5. Data Visualization

Various types of visualizations are used to explore the data. Boxplots are used to visualize the distribution of BMI for people who had a heart attack versus those who did not. This helps to understand the differences in BMI between the two groups. Show the distribution of BMI, heart attack cases, and other relevant features.

## 6. Regression Modeling

Regression models are used to predict the risk of heart attack based on the features available in the dataset:

- **Linear Regression:** A linear regression model is trained to predict heart attack risk based on various factors like BMI, age, and lifestyle choices.
- **Performance Metrics:** The model’s performance is evaluated using metrics like Mean Squared Error (MSE) and R² Score to measure the accuracy of predictions.

## Results Interpretation

Hypothesis Test Results: If the t-test shows a significant difference in BMI between the two groups (those who had a heart attack vs. those who did not), this could suggest that BMI is an important factor in determining heart attack risk. Boxplots and histograms show clear differences in BMI distributions between those who had a heart attack and those who did not.
Regression Results: The regression model provides predictions on heart attack risk, which can be used to guide health interventions and preventive measures.

## Conclusion

This project analyzes health data to predict heart attack risk by examining various health factors such as BMI, smoking status, and other medical conditions. By combining hypothesis testing, exploratory data analysis, and regression modeling, we gain valuable insights into how these factors contribute to heart attack risk. These findings can help healthcare providers in identifying high-risk individuals and providing targeted interventions.
