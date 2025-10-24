# 🎓 Jamboree Admission Prediction — Data-Driven Insights for Graduate Admissions

### 🧠 Predictive Modeling | Data Analytics | Linear & Ridge Regression

---

## 📘 Project Overview

This project predicts students’ **chances of admission** to graduate programs using the **Jamboree Education Dataset**.  

By applying **Linear and Ridge Regression**, the analysis identifies which academic and qualitative factors (CGPA, GRE, TOEFL, SOP, LOR, Research experience) most influence a student’s likelihood of admission.  

The project demonstrates how **data-driven insights** can guide students and education consultants in improving admission outcomes.

---

## 🎯 Business Objective

To empower **students and academic counselors** with actionable insights into the key drivers of admission success, enabling **personalized improvement strategies** and informed decision-making.

---

## 🧩 Dataset Details

| Feature | Description |
|---------|-------------|
| **GRE_Score** | Graduate Record Exam score |
| **TOEFL_Score** | Test of English as a Foreign Language score |
| **University_Rating** | Rating of the university (1–5) |
| **SOP** | Statement of Purpose strength (1–5) |
| **LOR** | Letter of Recommendation strength (1–5) |
| **CGPA** | Cumulative Grade Point Average |
| **Research** | Research experience (0 = No, 1 = Yes) |
| **Chance_of_Admit** | Target variable (0–1) |

📊 **Rows:** 500  
🎯 **Target Variable:** `Chance_of_Admit`

---

## ⚙️ Methodology

1.  **EDA (Exploratory Data Analysis)** 
     - Understanding feature distribution and skewness to fit in model 
     -  Outlier Handling

2. **Data Preprocessing**  
   - Handled missing values and standardized numerical features  
   - verify assumption of linearity
   - Train-test split (80/20)

3. **Modeling**  
   - Baseline **Linear Regression** model  
   - Regularized **Ridge & Lasso Regression** for stability  
   - Optimal `alpha` selected via `RidgeCV` & `LassoCV`

4. **Evaluation**  
   - Metrics: **R² Score** , **MAE** , **RMSE**, residual diagnostics  
   - Visual validation using:  
     - Actual vs Predicted Plot  
     - Residual Distribution Plot  
     - Feature Importance Barchart  

---

## 🧮 Model Results

| Model | R² Score |MAE| RMSE | Remarks |
|-------|:--------:|:---:|:----:|---------|
| Linear Regression | 0.8315 |0.02429| 0.03441| Strong baseline model |
| Ridge Regression | 0.8314 | 0.02426 | 0.03428|Improved stability and generalization |

---

## 📈 Feature Importance (Ridge Model)

| Feature | Influence (%) |
|---------|---------------|
| CGPA | 49.6 |
| GRE Score | 13.8 |
| TOEFL Score | 11.5 |
| LOR | 10.8 |
| Research | 7.2 |
| SOP | 4.7 |
| University Rating | 2.5 |

📊 **Insight:** CGPA is the most influential factor, followed by GRE and TOEFL.

---

## 🖼️ Visualization Summary

| Visualization | Description |
|---------------|------------|
| 🎯 **Actual vs Predicted Plot** | Evaluates how closely predictions match actual values |
| 📉 **Residual Plot** | Checks error distribution and model assumptions |
| 📊 **Feature Importance Bar Chart** | Shows relative influence of each feature |

> Visuals can be found in the `/images` folder of this repository.

---

## 💡 Insights & Recommendations

### 🎓 For Students
- Focus on **CGPA** — the strongest predictor of admission.  
- Prepare strategically for **GRE** and **TOEFL**.  
- Secure strong **LORs** and engage in **Research** projects.  
- Craft a compelling **SOP** to differentiate profiles.

### 🏫 For Education Counselors
- Prioritize training modules that improve academic performance and test preparation. 
- Offer personalized admission strategy sessions focusing on key predictors. 
- Integrate predictive modeling into student dashboards for real-time guidance.

---

## 🧾 Conclusion

Academic consistency (**CGPA**) and test performance (**GRE, TOEFL**) are the primary drivers of admission.  
Qualitative factors (**Research, LOR, SOP**) strengthen profiles but cannot replace strong academics.  

This project demonstrates how **machine learning and data analytics** can enhance educational guidance.

---

## 🔮 Future Enhancements
 
- Explore **non-linear models** (Random Forest, XGBoost).  
- Apply **SHAP analysis** for interpretability.  


---

## 🧰 Tech Stack

**Language:** Python  
**Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  
**Environment:** Jupyter Notebook  
**Version Control:** Git & GitHub  

---

## 👨‍💻 Author

**Manish Nandi**  
Data Analyst | Machine Learning Enthusiast  
📍 Open to opportunities in Data Analytics & Machine Learning  
🔗 [LinkedIn Profile](https://www.linkedin.com/public-profile/settings?trk=d_flagship3_profile_self_view_public_profile&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3BOGf5iXBeSluHw2JT14mUhQ%3D%3D) • [Gmail]()

---

## 📂 Repository Structure
```
Jamboree_Admission_Prediction/
│
├── data/
│ └── jamboree_dataset.csv
├── notebooks/
│ └── Jamboree_Admission_Prediction.ipynb
├── images/
│ ├── actual_vs_predicted.png
│ ├── residual_plot.png
│ └── feature_importance.png
├── Business_Report.pdf
├── README.md
└── requirements.txt
```

---

## ⭐ Project Highlights

- End-to-end **data science workflow**  
- Clear **business insights** from predictive modeling  
- Professional **visual storytelling**  
- Recruiter-ready presentation
