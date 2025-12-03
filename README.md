# 🌸 Breast Cancer Trends  
**CHIP 690–335: Milestone 2**  
**Helena Ford**  

---

## 📌 Project Overview  
This project uses Python and publicly available CDC datasets to explore several trends related to breast cancer in the United States. As an Operating Room nurse, I have noticed that many breast cancer patients seem to be diagnosed at younger ages.  

The analysis explores three main research questions:

1. **How have national breast cancer mortality rates changed over time?**  
2. **What is the relationship between state-level screening rates and mortality?**  
3. **How has the age distribution of breast cancer diagnoses changed over time?**

---

## 📁 Project Structure  

```
Breast_cancer_project/
│
├── breast_cancer_trends.ipynb    
├── requirements.txt               
├── README.md                      
│
└── data/
    ├── mortality.csv              
    ├── screening.csv              
    ├── state_mortality.csv       
    └── age_distribution.csv       
```

---

## 🧪 Methods Used  

### **Data Preparation**
- Loaded datasets using `pandas.read_csv`
- Renamed columns for readability
- Merged state-level datasets using `pd.merge` on `"State"`
- Converted age-incidence data into a pivot table

### **Tools & Libraries**
- **pandas** — data cleaning & manipulation  
- **matplotlib** — visualizations  
- **numpy** — created a simple trendline for scatterplot analysis  

### **Visualizations Generated**
- **National mortality trend line chart**  
-  **State-level screening vs mortality scatterplot**  
- **Age distribution line charts by age group**  

---

## 📊 Results Summary  

### **National Breast Cancer Mortality Trend**  
> The national age-adjusted breast cancer mortality rate shows a **steady decline from 1999 to the most recent available year**. This reflects improvements in early detection, treatment, and general cancer care.

---

### **Screening Rates vs Mortality (State-Level)**  
> The scatterplot shows a **weak negative relationship** between mammography screening and mortality. States with higher screening rates do *not* consistently show lower mortality.  
>
> This is expected, as mortality is influenced by many factors: treatment access, income, age distribution, stage at diagnosis, and other socioeconomic factors. Screening improves individual outcomes, but the relationship at the state level is not strongly linear.

---

### **Age Distribution of Diagnoses**  
> Most breast cancer diagnoses occur in women aged **45–74**, but younger age groups (especially **30–39**) show a **gradual increase** over time. This supports the observation that more younger women are being diagnosed than in previous decades.

---

## ▶️ How to Run This Project  

### **1. Install Required Packages**
```bash
pip install -r requirements.txt
```

### **2. Launch Jupyter Notebook**
```bash
python -m notebook
```

### **3. Open and Run the Notebook**
Open:

```
breast_cancer_trends.ipynb
```

Run all cells to load data, perform analysis, and generate charts.

---
Link to full notebook here: 
https://github.com/lenaford36/Breast_cancer_trends/blob/main/breast_cancer_trends.ipynb


## Sources
- Centers for Disease Control and Prevention (CDC) https://wonder.cdc.gov/cancer-v2020.html, https://wonder.cdc.gov/cancermort-v2021.html
  
- National Cancer Institute/NIH https://statecancerprofiles.cancer.gov/risk/index.php?topic=women&risk=v05&race=00&datatype=0&type=risk&sortVariableName=default&sortOrder=default#results
- Chat GPT: Chat GPT used to help with data collection, 

---
