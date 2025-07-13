# The Unemployed Guide to Living Forever: A Lifestyle Data Analysis

# 🧠 Mind & Body: A Holistic Health Analysis

## 📌 Introduction

In today's culture, where mental and physical health are heavily emphasized, we, *The Unemployed*, aim to better understand how lifestyle, socioeconomic factors, and biological indicators contribute to overall quality of life. This project explores the complex interplay between well-being, cognitive ability, and physical health, using a wide set of variables to assess how education, income, and lifestyle habits influence both emotional and physical outcomes.

Societal expectations often pressure individuals to pursue higher education and high-paying careers under the assumption that these paths lead to healthier, happier lives. But do they really? Our analysis will challenge this narrative and investigate whether external success markers actually lead to greater well-being.

---

## 🎯 Objectives

- Evaluate whether **education** and **income level** contribute significantly to **mental and physical health outcomes**.
- Determine the relationships between **cognitive function** and physical health indicators such as **bone density**, **vision**, and **blood glucose**.
- Explore how **lifestyle choices** impact **predicted vs actual age**, particularly in the context of appearance and perceived health.

---

## 🧪 Data & Variables

We analyze a dataset with a mix of **categorical** and **quantitative** health and lifestyle indicators.

### Categorical Variables
- Gender  
- Education Level  
- Smoking Status  
- Alcohol Consumption  
- Physical Activity Level  
- Family History  
- Chronic Disease Presence  
- Mental Health Status  

### Quantitative Variables
- Income Level  
- Cognitive Function  
- Stress Levels  
- Diet Score  
- Bone Density (g/cm²)  
- Hearing Ability  
- Vision Sharpness  
- Blood Glucose Levels (mg/dL)  
- Blood Pressure (Systolic/Diastolic mmHg)  
- Cholesterol Levels (mg/dL)  
- BMI  
- Pollution Exposure  
- Age (years)  
- Weight (kg)  

---

## ❓ Research Questions

### Question 1: Is the brain dependent on a healthy body?
We explore whether there is a measurable link between **cognitive function** and physical health metrics such as **vision clarity**, **bone density**, **blood glucose**, and **age**. Are individuals with healthier physical markers more cognitively sharp, or do external factors play a more significant role?

### Question 2: What is the impact of lifestyle on age prediction?
We examine how **physical activity**, **smoking**, and **alcohol use** influence **age appearance and prediction**. Our goal is to identify lifestyle indicators that correlate with how old someone looks or seems, based on health behaviors and external appearance.

---

## 🔬 Hypotheses

- **H1**: Physical health metrics (vision sharpness, bone density, blood glucose, age) do not have a significant relationship with cognitive function.
- **H2**: Lifestyle choices (smoking, alcohol consumption, physical activity) do not correlate with age prediction accuracy.

---

## 🧠 Results: Physical Health & Cognitive Function

To test our first hypothesis, we performed a detailed regression analysis to assess associations between physical health metrics and cognitive function.

Our findings reveal **two significant predictors** of lower cognitive function:

- **Age**
- **Hearing Ability**

### 📉 Key Findings
- As **age increases**, **cognitive function decreases**, consistent with general aging research.
- Interestingly, as **hearing ability** scores increased, **cognitive function** decreased. This unexpected result may suggest that individuals with excellent hearing rely less on cognitive effort during communication, potentially reducing cognitive stimulation or engagement in our dataset.

### 🧐 Surprising Results
Contrary to expectations:
- **Vision Sharpness** — despite being a known barrier to information intake — showed no significant link to cognition.
- **Blood Glucose Levels**, the brain’s primary energy source, also lacked a significant relationship with cognitive function.

### 🔍 Model Selection
Using **stepwise regression**, our best-fitting model identified only **Age** and **Hearing Ability** as meaningful predictors. This implies that other important variables affecting cognitive function may not have been included in the dataset, such as sleep quality or neurological health.

---

## 📈 Results: Lifestyle and Age Prediction

The aim of our model was to explore whether **lifestyle choices** significantly affect **age prediction**. Using a linear regression framework, we found a **meaningful connection**, with **smoking status** standing out as a strong predictor.

To address non-normality in the features, we applied an **Empirical CDF (ECDF) transformation**, which helped normalize distributions. However, this also **reduced our model's R²**, suggesting an increase in unexplained variability.

### Key Takeaways
- **Smoking status** showed the most substantial effect on predicted age.
- **ECDF transformation** improved statistical assumptions but lowered model explanatory power.
- Several important variables, like **sleep duration** and **diet quality**, were missing from the dataset and may enhance future models.

### Future Improvements
- Add new lifestyle features such as **sleep hours**, **hydration**, and **nutrition** data.
- Test **nonlinear models** (e.g., Random Forest, XGBoost) to better capture interactions.
- Expand dataset for better generalizability and stronger statistical inference.

---

## 📄 Dataset Information

- **Dataset Title**: *Human Age Prediction Synthetic Dataset*  
- **Authors**: M Abdullah and Shahzaib Yaqoob  
- **Published**: August 2024  
- **Platform**: [Kaggle](https://www.kaggle.com/datasets/abdullah0a/human-age-prediction-synthetic-dataset)  
- **Retrieved on**: October 24, 2024  

> This dataset includes synthetic data with variables related to physical health, lifestyle, and demographic factors designed for machine learning-based age prediction.

---

## 🧠 Team

**The Unemployed**  
- Richard Zhang  
- Randy Van Waes  
- Vincent Agrella  



