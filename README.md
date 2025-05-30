# donor-prediction-sas
# Donor Response Prediction Using SAS Enterprise Miner

**Course:** ADTA 5230 – Data Analytics  
**University:** University of North Texas 
**Date:** May 2025  
**Collaborators:** Sathvik Chava, Sumanjali Banjara, Paulina Gomez Ibarra  
**Tool Used:** SAS Enterprise Miner  

##  Project Overview

This project aimed to support a non-profit organization by improving the cost-effectiveness of its direct marketing campaigns. Using historical donation data, we built two models:

- **Classification model** to predict if someone will donate.
- **Regression model** to predict how much a donor is likely to contribute.

By deploying these models, the non-profit can reduce mailing costs and focus on individuals most likely to respond.

##  Business Questions

1. Who is most likely to donate?  
2. How much will each donor likely donate?

##  Models Used

### Classification:
- Logistic Regression (standard and stepwise)
- Neural Network (default and with backpropagation)
- Gradient Boosting

**Best Model:** Neural Network (default settings) – Misclassification Rate: **9.2%**, Profit: **$10,181**

### Prediction:
- HP Forest
- AutoNeural (2 and 6 hidden units)
- Neural Network

**Best Model:** AutoNeural (6 hidden units) – Lowest ASE: **16.91**

##  Data & Preprocessing

- No missing values
- Binary & categorical variables encoded
- Train-validation split: 70-30
- Standardized variables

##  Deployment

The final scoring process created:
- `p_donr1`: Probability of donation  
- `p_damt`: Predicted donation amount

**Profit Formula:**
```math
Expected Profit = (p_donr1 × p_damt) - 2.00


### Strategy Comparison:
| Approach             | Individuals Targeted | Total Profit | Avg Profit |
|----------------------|----------------------|--------------|-------------|
| Mass Mailing         | 2,007                | $401.39      | $0.20       |
| Targeted Mailing     | 508                  | $3,129.60    | $6.16       |

##  Skills Used & Developed

###  Technical Skills
- Predictive modeling with **SAS Enterprise Miner**
- Classification & regression using logistic regression, neural networks, gradient boosting
- Data preprocessing, encoding, and standardization
- Model evaluation using validation metrics and profit analysis
- Scoring and deployment strategies for real-world use

###  Analytical & Business Skills
- Exploratory Data Analysis (EDA) for pattern detection
- Multicollinearity handling with clustering
- Business-centric model evaluation based on ROI
- Decision-making support through targeted marketing

###  Soft & Project Skills
- Collaborative teamwork and project execution
- Documentation and technical report writing
- Problem-solving in data-centric business contexts


## 🔖 Notes

This project was completed as part of a course "ADTA 5230 – Data Analytic" from University of North Texas. The work was collaborative. This repository reflects my version and includes proper credit to all team members.

