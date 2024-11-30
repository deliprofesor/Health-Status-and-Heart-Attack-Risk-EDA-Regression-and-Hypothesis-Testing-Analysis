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

This project focuses on analyzing the relationships between health conditions, lifestyle habits, and demographic factors on heart attack risk. By leveraging statistical methods and machine learning techniques, the study explores the impact of variables such as Body Mass Index (BMI), smoking, and alcohol consumption. Using a comprehensive dataset, the project aims to identify significant risk factors and provide actionable insights for mitigating heart attack risks.

- **Analyze the influence of lifestyle and health factors on heart attack risk.**
- **Evaluate BMI, smoking, and alcohol consumption as predictors of heart disease.**
- **Utilize statistical analyses and regression models to extract insights and make predictions.**


## Data Cleaning and Preprocessing

The dataset was processed to ensure accuracy and usability:

- **Missing Values:** Continuous variables were imputed using the median to maintain robustness against outliers.
- **Irrelevant Columns:** Non-contributory fields like individual IDs were removed.
- **Categorical Data:** Encoded into numeric values for analysis.
- **Duplicates:** Cleaned to enhance data integrity.
  
## Exploratory Data Analysis (EDA)

EDA was conducted to understand the dataset's structure and identify key patterns:

- **Descriptive Statistics:** Summarized variables using measures like mean, median, and mode.
- **Visual Analysis:** Histograms, boxplots, and heatmaps were used to assess distributions, detect outliers, and visualize correlations.
- **Correlation Matrix:** Highlighted relationships between variables, with a focus on BMI and heart attack history.
  
## Hypothesis Testing

Statistical tests were conducted to evaluate the relationship between BMI and heart attack risk:

- **Null Hypothesis (H₀):** No significant difference in BMI between individuals with and without heart attacks.
- **Alternative Hypothesis (H₁):** A significant difference exists.
- **Test:** A two-sample t-test was performed. Results confirmed a statistically significant difference (p < 0.05), indicating BMI’s impact on heart attack risk.
  
## Machine Learning Models

Regression models were used to predict heart attack risk based on lifestyle and health factors:

- **Linear Regression:** Served as a baseline model.
- **Ridge Regression:** Outperformed other models with low error rates and strong generalization capabilities.
- **Lasso Regression:** Highlighted important features but underperformed compared to Ridge Regression.
- **Model Evaluation:** Performance was assessed using Mean Squared Error (MSE) and R² scores.

## Results of Exploratory Data Analysis

- **Higher BMI levels were associated with increased heart attack risk.**
- **Smoking and alcohol consumption were more prevalent among individuals with a history of heart attacks.**
- **Visualizations revealed clear differences in BMI distributions between those with and without heart attacks.**

## Hypothesis Testing Outcomes

The t-test confirmed a statistically significant difference in BMI levels, validating its importance as a risk factor for heart attacks.

## Machine Learning Results
- **Ridge Regression** emerged as the best predictive model, offering:
- **Lowest Error Rates:** Demonstrated superior accuracy in predictions.
- **Generalization:** Effectively captured relationships in the dataset.

