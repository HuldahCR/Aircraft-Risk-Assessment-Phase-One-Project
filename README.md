# ✈️ Aviation Accident Risk Assessment  - Phase One Data Science Project

## 📁 1. Project Overview

This project analyzes global aircraft accident data to support **Huru Capital Investments Group** in identifying **safe and high-performing aircraft manufacturers** as the company diversifies into the aviation sector.

The project follows the **CRISP-DM methodology** and leverages **prescriptive analytics** to guide strategic investment decisions by analyzing accident causes, occurrence of fatal accidents, and risk distribution across aircraft makes, models, and conditions.

---

## 🧠 2. Business Understanding

- **Client**: Huru Capital Investments Group – a US investment firm expanding into aviation.
- **Stakeholder**: The head of the new Aviation Division at Huru Capital Investments Group
- **Objective**: Identify the types of aircraft with the lowest historical risk profile to guide purchasing and operational decisions
- **Problem Statement**: Aircraft accidents can result in major. financial and reputational losses
- **Metrics of success**:
  - At least **three** clear evidence based recommendations are provided to guide aircraft acquisition
  - Develop an interactive dashboard for decision-making
  - Key safety patterns are clearly visualised


---

## 📊 3. Data Understanding

- **Source**: [Kaggle - Aviation Accident Database and Synopses (up to 2023)*] (https://www.kaggle.com/datasets/khsamaha/aviation-accident-database-synopses)
- **Description**
- Contains civil aviation accident data from 1962 to 2023.
- Records include variables such as Make, Model, Location, Weather Conditions, Aircraft Damage, Injury Severity, and more.

---

## 📊 4. Data Cleaning and Preparation

  - Imputation of missing values (e.g. Model, Make)
  - Standardisation of data (e.g change of Event_Date datatype to Datetime)
  - Feature engineering: 
	- Total_Aboard = sum of all aboard categories 
	- Fatality_Rate(%)= (Total Fatal Injuries / Total Aboard) * 100
	- Fatal_Accident = 1 if fatal injury occurred, 0 otherwise
  - Removal of outliers where necessary

- **Key Fields Used**:  
  Make, Model, Aircraft_Category, Injury_Severity, Weather_Condition, Aircraft_Damage, Fatal_Accident,Total_Fatal_Injuries, Total_Aboard, Year, etc.

---

## 🧪 5. Methodology: CRISP-DM

1. **Business Understanding**: Define investment-oriented goals
2. **Data Understanding**: Explore structure, completeness, and patterns
3. **Data Preparation**: Clean and engineer key features
4. **EDA**:
   - Univariate, Bivariate, and Multivariate analyses
   - Trend analysis and fatality distribution
5. **Modeling** *(Planned in Phase 2)*
6. **Evaluation**: Actionable findings and recommendations

---

## 📊 6. Visualizations

### Injury Severity Distribution
- Majority of records are fatal injuries, indicating high safety concern.

### Aircraft Category vs. Fatality Rate
- Rocket and Gyrocraft aircraft have the highest fatality proportions.

> Visuals are available in the Jupyter Notebook, Presentation and Tableau dashboard.

---

## 📈 7. Key Findings

- **Majority of accidents are fatal**, particularly among certain light aircraft types
- **Amateur-built aircraft** have significantly higher fatality rates
- Aircraft with **multiple engines** tend to be safer, especially under poor weather (IMC)
- Certain makes (e.g., **Boeing, Grumman, Hughes**) have exceptionally **low fatality rates**
- Top fatality-prone models include the **Piper PA25**, **Robinson R66**, and **Beech V35**

---

## 💡 8. Prescriptive Recommendations

1. Prioritize investment in low-fatality makes like Boeing, Grumman and Hughes
2. Avoid or inspect high-risk aircraft models thoroughly
3. Exclude amateur-built aircraft from commercial operations
4. Favor multi-engine aircraft for flights in poor weather conditions

---

## 📊 9. Deliverables

- ✅ **Jupyter Notebook** with full EDA and code
- ✅ **Interactive Tableau Dashboard** (link below)
- ✅ **Presentation slides** for stakeholders
- ✅ **Cleaned dataset** (CSV)
- ✅ **README** (this file)

---

## 📎 10. Repository Structure

```bash
aviation-accident-analysis/
│
├── data/
│
├── notebooks/
│   └── Final_Aviation_Risk_Assessment.ipynb # Main Jupyter Notebook
│
├── presentation/
│   └── presentation.pdf # Stakeholder presentation
│
├── dashboard/
│   └── AircraftRiskAssessment.twb # Packaged Tableau Workbook
│
├── README.md
├── .gitignore
```

---

## 📊 11. Tableau Dashboard

👉 [View Interactive Dashboard (Tableau Public)](https://public.tableau.com/app/profile/huldah.rotich/viz/AircraftRiskAssessment_17513009300660/AircraftSafetyDashboard)  
*Features filters by Aircraft Make, Category, Weather Condition, Amateur Status, Year Range*

---

## 🛠 12. Tools & Technologies

- Python (Pandas, NumPy, Seaborn, Matplotlib)
- Tableau Public
- Jupyter Notebook
- CRISP-DM methodology
- [Google Slides](https://docs.google.com/presentation/d/1OYWchi1UZz2onbjavMrelPrbgvtNmTdx_nWjE7XSbeE/edit?slide=id.g36b7c59c46c_1_213#slide=id.g36b7c59c46c_1_213)

---

## 👤 13. Author

**Huldah Chepkoech Rotich**  
Data Science Student | Moringa School  
*This project is part of Phase 1 Presentation for Moringa’s Data Science Program.*

---

## 📬 14. Contact

For feedback or questions, please email: rotichhuldah@gmail.com  
Or connect via [LinkedIn](https://www.linkedin.com/in/huldah-rotich-339797181/)

---

## 📝 License

This project is for educational purposes and not intended for production-grade use or regulatory decision-making.
