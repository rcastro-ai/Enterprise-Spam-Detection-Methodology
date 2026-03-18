# Enterprise Spam Detection Methodology
This is the solution to the Final Assignment in course "Data Science Methodology" from the IBM Data Science Professional Certificate program

**Stakeholder:** Chief Information Officer (CIO)

**Framework:** CRISP-DM (Cross-Industry Standard Process for Data Mining)

**Objective:** Reduce corporate risk by classifying malicious emails (Spam/Phishing) using Machine Learning.

## Executive Summary

This project outlines a comprehensive 6-stage data science methodology to address the rising threat of phishing and scam emails in a large corporate environment. By moving from **Business Understanding** to **Deployment**, this framework ensures that the technical solution directly impacts the company’s bottom line by reducing data breach risks and increasing employee productivity.

## The 6-Stage Methodology

<img src="CRISP-DM_Process_Diagram.png" width="500">

### 1. Business Understanding
   
* **Goal:** Improve cybersecurity and reduce employees' manual filtering time.

* **Approach:** Binary Classification (Predicting "Legitimate" vs "Illegitimate" emails).

* **Success Metric:** Decrease in successful phishing incidents reported to IT department.

### 2. Data Understanding

* **Data Sources:** IP Reputation services, Domain lists, and 3 years of historical labeled email archives.

* **Quality Check:** Verified header integrity and addressed class imbalance in spam/phishing samples.

### 3. Data Preparation

* **Text Pre-processing:** HTML stripping, lowercase conversion, and punctuation removal.

* **Feature Engineering:** Tokenization and removal of stop words (e.g., "the", "and", "is").

* **Data Splitting:** 80/20 Train/Test split for model validation.

### 4. Modeling

* **Algorithm Selection:** Naïve Bayes and Logistic Regression.

* **Training:** Iterative hyperparameter tuning to optimize classification accuracy.

### 5. Evaluation

* **Metric:** Confusion Matrix analysis.

* **Optimization:** Threshold Tuning specifically to minimize "False Positives" (protecting client communications).

### 6. Deployment

* **Strategy:** Canary rollout (initial small user group) followed by full integration into the email gateway.

* **Maintenance:** Established a feedback loop via "Report Spam" and "Not Spam" buttons for continuous model retraining.






