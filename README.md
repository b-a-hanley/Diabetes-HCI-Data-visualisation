# Diabetes HCI & Data Visualisation

---

## 1. Abstract  
Diabetes affects approximately **5.8 million people in the UK** [1], posing severe risks to the cardiovascular system, blood vessels, and organs [2].  
This report explores a comprehensive dataset comprised of medical, genetic, and lifestyle-related variables associated with different diabetes-related conditions.  

Sourced from hospitals, clinical studies, and public health repositories, the dataset supports an in-depth analysis of key risk factors and diagnostic indicators.  

Drawing on established data visualisation methods used in medical and epidemiology, this report will explore techniques to visually present this data, with the goal of enhancing understanding and early detection of diabetes-related conditions.  

---

## 2. Description of the Dataset  

### 2.1 Dataset: Diabetes Dataset  
[Diabetes Dataset – Kaggle](https://www.kaggle.com/datasets/ankitbatra1210/diabetes-dataset?resource=download)  

- **70,000 patients**  
- **34 features** (numerical + categorical)  
- Sourced from hospitals, clinical studies, and public health databases.  

This diversity and scale make it suitable for exploratory and predictive analysis of diabetes and its subtypes.  

### 2.2 Diabetes-related classifications  
Target label includes:  
- Cystic Fibrosis-Related Diabetes  
- Type 2 Diabetes  
- Type 3c Diabetes (Pancreatogenic)  
- Wolcott-Rallison Syndrome  
- Wolfram Disease  
- Gestational Diabetes  
- Latent Autoimmune Diabetes (LADA)  
- Maturity-Onset Diabetes (MODY)  
- Neonatal Diabetes Mellitus  
- Prediabetic  
- Secondary Diseases  
- Steroid-Induced Diabetes  
- Type 1 Diabetes  

### 2.3 Categorical features  
- **Dietary Habits**: Healthy, Unhealthy  
- **Smoking Status**: Smoker, Non-Smoker  
- **Alcohol Consumption**: Low, Moderate, High  
- **Ethnicity**: Low Risk, High Risk  
- **Socioeconomic Factors**: Low, Medium, High  

These variables evaluate external risk factors and potential health disparities.  

### 2.4 Numerical features  

| Feature                | Description |
|-------------------------|-------------|
| **Age** [3]             | Patient age in years |
| **BMI** [3]             | Body Mass Index (weight / height) |
| **Insulin Levels** [3]  | Fasting insulin in blood (µU/mL) |
| **Blood Glucose** [3]   | Fasting glucose in blood (mmol/L) |
| **Cholesterol Levels** [4] | Cholesterol measured in blood (mmol/L) |
| **Blood Pressure** [4]  | Force of blood against artery walls (mmHg) |
| **Digestive Enzyme Levels** [4] | Amylase in blood (U/L) |
| **Pancreatic Health** [4] | Lipase in blood (U/L) |
| **Pulmonary Function** [4] | Forced Expiratory Volume (FEV) |

These features give insight into clinical health, critical for diagnosis and management.  

---

## 3. Current State of the Art  

### 3.1 NHS Digital Visualisations [5]  
- Interactive dashboards using Power BI.  
- Bar charts + stacked bar charts for **age distribution** and **demographics**.  
- Issues: cluttered data, poor comparative clarity.  

**Radar plots** (e.g., young adult Type 1 diabetes audits) lack accurate percentage representation. A **geographic heatmap** would be more effective.  

### 3.2 World Mapper Expenditure for Diabetes [6]  
- **Non-Contiguous Cartogram** resizing countries by diabetes expenditure.  
- Reflects disparity between nations.  
- Limitation: distortion reduces recognisability.  

### 3.3 DiabetesAtlas [7]  
- **Interactive heat maps** showing diabetes cases worldwide.  
- Proportionate colour coding aids readability.  
- Limitation: Colour-blind accessibility concerns.  

---

## 4. Innovation  

### 4.1 Lifestyle & Social Context Categories (Radar Plot)  
- Radar plots compare multiple groups of information.  
- Customisable colour overlays + filters.  
- Unique approach: overlaying diabetes classifications on lifestyle/social categories.  

### 4.2 Diabetes Conditions as a Line Graph  
- Overlay diabetes classifications.  
- Dropdown selection for clinical measures.  
- Highly interpretable + interactive.  

### 4.3 Interactive Diabetes Density Plot  
- Shows distribution of continuous variables.  
- Identifies age groups with higher prevalence (e.g., ages 40–50 for blood pressure).  
- Animated density plots could represent **age progression** (3s = 1 year).  

### 4.4 3D Visualisation Graph  
- VR interaction with 3D datasets.  
- Haptic feedback gloves or sound cues to indicate density.  
- Limitation: high cost + possible sensory overload.  

### 4.5 Predictive Diagnostic Stacked Bar Chart  
- **ML-driven model** to predict diabetes risk.  
- Users input medical data → bar chart shows **likelihood of conditions**.  
- Colour coded + percentage-labelled.  
- Could reduce waiting times and improve early intervention.  

---

## 5. Conclusion  
This report explored the diabetes dataset, reviewed existing visualisations, and identified gaps.  

Proposed **interactive and innovative visualisation prototypes** aim to:  
- Detect anomalies → potential scientific breakthroughs.  
- Improve diagnosis speed → reduce clinical waiting times.  
- Decrease doctor workload → focus on treatment.  
- Provide clearer comparative insights into diabetes data.  

**Future Work:**  
- User testing.  
- Time-assessment tasks to evaluate speed of information comprehension.  

---

## 6. References  

[1] Roglic, G. (2016). *WHO Global report on diabetes: A summary*. International Journal of Noncommunicable Diseases, 1(1), p.3. doi:[10.4103/24688827.184853](https://doi.org/10.4103/24688827.184853).  

[2] Diabetes UK. (n.d.). *How many people in the UK have diabetes?* [Link](https://www.diabetes.org.uk/aboutus/about-the-charity/ourstrategy/statistics).  

[3] Fazakis, N., Kocsis, O., Dritsas, E., Alexiou, S., Fakotakis, N. & Moustakas, K. (2021). *Machine Learning Tools for Long-Term Type 2 Diabetes Risk Prediction*. IEEE Access, 9, 103737–103757. doi:[10.1109/access.2021.3098691](https://doi.org/10.1109/access.2021.3098691).  

[4] BelHadj, S., Hentati, O., Elfeki, A. & Hamden, K. (2013). *Inhibitory activities of Ulva lactuca polysaccharides on digestive enzymes related to diabetes and obesity*. Archives of Physiology and Biochemistry, 119(2), 81–87. doi:[10.3109/13813455.2013.775159](https://doi.org/10.3109/13813455.2013.775159).  

[5] NHS Digital. (n.d.). *Clinical audits and registries*. [Link](https://digital.nhs.uk/data-and-information/clinical-audits-and-registries).  

[6] Worldmapper. (2019). *Expenditure for patients with Diabetes*. [Link](https://worldmapper.org/maps/healthdiabetesexpenditure-2017/) (Accessed 13 May 2025).  

[7] International Diabetes Federation. (2021). *Diabetes around the World in 2021*. [Link](https://diabetesatlas.org/).  

[8] Saary, M.J. (2008). *Radar plots: a useful way for presenting multivariate health care data*. Journal of Clinical Epidemiology, 61(4), 311–317. doi:[10.1016/j.jclinepi.2007.04.021](https://doi.org/10.1016/j.jclinepi.2007.04.021).  

[9] Thompson, P. (2010). *Learning by Doing*. ScienceDirect. [Link](https://www.sciencedirect.com/science/article/abs/pii/S0169721810010105).  
