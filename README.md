
#  House Price Prediction

##  Business Problem
Pricing properties accurately is crucial for real estate.  
- **Overpricing** → Long listing times, reduced buyer interest.  
- **Underpricing** → Loss of potential profit.  
**Goal:** Build a predictive model that estimates house sale prices based on property characteristics.

---

##  Approach
- **Dataset:** Ames Housing Dataset (numeric features used for simplicity)  
- **Preprocessing:**  
  - Dropped highly missing columns  
  - Removed rows with missing numeric values  
- **Models Used:**  
  1. Linear Regression (Baseline)  
  2. Random Forest Regressor  
  3. XGBoost Regressor  

---

##  Results
| Model               | RMSE      | R² Score |
|---------------------|-----------|----------|
| Linear Regression   | ~37,384   | 0.79     |
| Random Forest       | ~27,554   | 0.89     |
| **XGBoost**         | **~25,936** | **0.90** |

 **XGBoost performed the best** with the highest R² and lowest RMSE.

---

##  Recommendations
- **For Sellers:**  
  - Invest in quality improvements (materials, finishes) for better returns  
  - Garage and basement upgrades increase value  

- **For Buyers:**  
  - Use predicted price vs listing price to avoid overpaying  
  - Quality matters more than size alone  

- **For Agents & Banks:**  
  - Use model outputs for realistic listing prices  
  - Reduce lending risk with model-backed property valuations  

---

##  Executive Summary
> XGBoost model predicts house prices with **90% accuracy (R² = 0.90)** and an average error of **~$25,936**.  
> Key factors influencing price are overall quality, above-ground living area, garage size, basement size, and construction year.  
> Sellers can focus on quality upgrades; buyers can avoid overpriced properties; agents and banks can make more informed decisions.

---

##  Project Flow
```mermaid
graph TD
A[Data Collection] --> B[Data Preprocessing]
B --> C[Model Training]
C --> D[Model Evaluation]
D --> E[Model Comparison]
E --> F[Recommendations & Insights]
