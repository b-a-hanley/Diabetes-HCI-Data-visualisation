# Diabetes HCI & Data visualisation 

---

## 1. Abstract  
Diabetes affects approximately 5.8 million people in the UK [1], posing severe risks to the cardiovascular system, blood vessels, and organs [2]. This report explores a comprehensive dataset comprised of medical, genetic and lifestyle related variables associated with different diabetes-related conditions.  

Sourced from hospitals, clinical studies, and public health repositories, the dataset supports an in-depth analysis of key risk factors and diagnostic indicators. Drawing on established data visualisation methods used in medical and epidemiology, this report will explore techniques to visually present this data, with the goal of enhancing understanding and early detection of diabetes-related conditions.  

---

## 2. Description of the Dataset  

### 2.1 Dataset: Diabetes Dataset  
<https://www.kaggle.com/datasets/ankitbatra1210/diabetes-dataset?resource=download>  

This study uses the Diabetes Dataset sourced from Kaggle (available in the link above). It contains clinical records of 70,000 patients, each with a diabetes-related diagnosis. The dataset comprises 34 features, both numerical and categorical, collected from hospitals, clinical studies, and public health databases.  

The diversity and scale of the data make it suitable for exploratory and predictive analysis of diabetes and its subtypes.  

### 2.2 Diabetes-related classifications  
The dataset includes the following diabetes related classifications under the target label:  

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

These classifications allow for the analysis across different diabetes related conditions.  

### 2.3 Categorical features  
The dataset consists of categorical lifestyle and social context variables:  

- Dietary Habits: Healthy, Unhealthy  
- Smoking Status: Smoker, Non-Smoker  
- Alcohol Consumption: Low, Moderate, High  
- Ethnicity: Low Risk, High Risk  
- Socioeconomic Factors: Low, Medium, High  

These variables are critical for evaluating external risk factors and potential health disparities.  

### 2.4 Numerical features  

Key clinical characteristics are represented as continuous variables.  

| Feature | Description |
|---------|-------------|
| **Age [3]** | Patient age in years |
| **BMI [3]** | Body Mass index, Weight / height |
| **Insulin Levels [3]** | Insulin measured in the patient's blood while fasting (µU/mL). |
| **Blood glucose levels [3]** | Glucose measured in the blood while fasting (mmol/L) |
| **Cholesterol Levels [4]** | Cholesterol measured in blood while fasting (mmol/L) |
| **Blood Pressure [4]** | Force of blood against artery walls (mmGH) |
| **Digestive enzyme levels [4]** | Amylase produced in blood (U/L) |
| **Pancreatic Health [4]** | Lipase produced in blood (U/L) |
| **Pulmonary Function [4]** | Forced Expiratory Volume (FEV) |

These features offer insight into specific clinical health, which is critical in the diagnosis and management of diabetes.  

---

## 3. Current State of the Art  

### 3.1 NHS Digital Visualisations [5]  
The NHS have several interactive dashboards displaying data of the institutional care for diabetes patients utilising Googles Power BI.  

Figure 1 contains a table breakdown of age distribution for each care board. It then describes this data in bar charts however the information is cluttered with too many care boards, making value insights offered across ages less distinguishable.  

<img width="532" height="287" alt="image" src="https://github.com/user-attachments/assets/21d06719-42a0-4795-ae0b-57a21aad9699" />
**Figure 1a** Age band of people with type 1 diabetes by Care Board  
It allows users to click on a bar chart for the percent of a given care board and age but doesn’t represent this comparatively.  

<img width="532" height="286" alt="image" src="https://github.com/user-attachments/assets/8082dca5-e0ee-47e6-961a-45f3ed70c548" />
**Figure 1b** Age band of people with type 1 diabetes by Care Board with selected detail.  

The NHS Digital. Uses stacked bar charts representing distribution of Type 2 Diabetes by demographics. This visually describes the breakdown well, being labelled with percentages to give quantitative values.  

<img width="532" height="282" alt="image" src="https://github.com/user-attachments/assets/7e70fdf3-ad8f-4a52-b489-dc1b0bd62236" />
**Figure 2** Type 2 Diabetes breakdown stacked bar charts.  

<img width="532" height="290" alt="image" src="https://github.com/user-attachments/assets/1f44739e-b8a6-4587-b08f-99fce32119cc" />
**Figure 3** Young adult Type 1 Diabetes audit within care boards  
Figure 3 is a radar plot that describes the number of young persons with type 2 diabetes in each region. This graph however doesn’t have clear indication of percentage on the radar: 48.5% of young people in London have type 2 diabetes, but the graph seemingly presents this data to suggest 26%. The radar plot is a great way of describing the influence of each attribute effect a condition, but I feel this would have been better represented by a heat map of geographical locations.  

<img width="532" height="290" alt="image" src="https://github.com/user-attachments/assets/a0fb175b-b105-46c9-a6c3-99dec224713b" />
**Figure 4** Young adult Type 1 Diabetes audit demographic graphs  
Figure 4 Represents breakdown of age, sex, ethnicity and deprivation by bar charts. The graph allows for filtering by audit year, country and region, two improvements of this graph would be smaller axis intervals making the results more interpretable, the graph seemingly describes a prevalence within the white ethnicity, this distribution however doesn’t describe the prevalence of the white ethnicity within the region which can lead to misinterpretation.  

### 3.2 World Mapper Expenditure for patients with diabetes [6]  
This Non-Contiguous Cartogram represents the expenditure for patients with diabetes across different countries. Each region is resized based on the amount the country has spent. Countries are placed approximately to their actual location.  

This graph reflects the disparity between different countries in expenditure to tackle the disease. A difficulty with this approach is the distortion of a country may end up making it unrecognisable which impacts readability of most significant changes.  

<img width="513" height="257" alt="image" src="https://github.com/user-attachments/assets/ee4bc882-f649-4983-8852-2306173b5251" />
**Figure 5** A non-contiguous Cartogram of Country diabetes expenditure.  

### 3.3 DiabetesAtlas Diabetes cases  

<img width="489" height="331" alt="image" src="https://github.com/user-attachments/assets/aac56bce-1333-413b-bdab-e62e954d1cbe" />
**Figure 6** An interactive world heat map which displays country diabetes cases.  

This interactive world map helps users process geospatial context, helping in form decisions based on location rather than economic factors. The map displays data about the number of cases. It allows for general comparison of countries through proportionate colour coding allowing easy readability however colour-blind users, may misinterpret this graph without customisation. DiabetesAtlas as organisation has covered many of the areas of geographical representation of diabetes data sufficiently covering our dataset including age, blood glucose, health expenditure, glucose tolerance and hyperglycaemia.  

---

## 4. Innovation  

### 4.1 Lifestyle and social context categories  
Given the categorical and Boolean nature of the demographic variables in the dataset the number of ways to represent this data is limited. Health care researchers have not described multivariate data through graphical presentation [8].  

It is best to try and describe as much information as possible in the simplest manner. The use of radar plot is great to describe characteristic nature of features. A radar plot is form of radial graphing, best for comparing multiple groups of information such as the diabetes classifications.  

It is possible to overlay the different diabetes classifications with individual colours. To aid interpretability a filter should be added to ensure ease of comparison by applying relevant classifications. A legend should describe the colour coding and allow for customisation based on user preferences. Based on my finding the use of a customisable coloured radar plot with filtered obesity classifications is unique.  
<img width="542" height="376" alt="image" src="https://github.com/user-attachments/assets/7467f474-a106-4a0c-8c6a-96e39c33610c" />
**Figure 7** Lifestyle and Social factors of diabetes conditions radar plot  

### 4.2 Diabetes conditions as a line graph  

<img width="537" height="295" alt="image" src="https://github.com/user-attachments/assets/712ca24a-5b28-444f-a2bf-c9e7eae649dd" />
**Figure 8** Lifestyle and Social factors of diabetes conditions radar plot  

Line graphs are highly interpretable describing two variables and their effect on each other. The classifications can be overlaid with a legend describing a customisable colour scheme. They can filter classifications for ease of use. This interaction allows for dropdown methods for each of the available clinical measures. By a user interacting with the graph and seeing the implications their memory of the event is greatly improved. Currently there is no dataset in which you can overlay diabetes classifications with the ability to select different data axis.  

### 4.3 Interactive Diabetes density plot  
A density plot is used to show the distribution of continuous variables and helps users to understand where values are most concentrated.  

<img width="532" height="345" alt="image" src="https://github.com/user-attachments/assets/e5038dcb-3285-48d8-a68f-20ccbae0c693" />
**Figure 9** Prototype Blood Pressure and Age Density plot  

In the graph above a line of best fit can be determined but further still information about their being a prominence of the condition at ages 40-50 can be easily interpreted. Density plots also describe unique elements lost in averages such as the prevalence in the graph above of some 60-year-olds having less high blood pressure. Understanding small deviating patterns can lead to breakthroughs.  

Being a dynamic graph there is an ability to change colours as well as the value which represents density, meaning more anomalies can be removed if the user is overwhelmed by results. A further improvement of this graph is for it to be animated thus a third variable perhaps best chosen would-be age, would be displayed with the duration of 3 seconds representing 1 year. This helps describe even more information to a user helping them process even more data.  

### 4.4 3D visualisation graph  
Many computers are limited in displaying data in 2d dimensions but to best replicate data, having three dimensions would preferable. Users interacting with Virtual reality can explore more axis. Being in an immersive graph helps bring a level of depth to analysis.  

It is possible to explore using gloves, which might have haptic feedback that vibrate or through sound with higher frequencies indicating interactions with a high density point. However, some users may find an immersive experience overwhelming and the there would be a significant cost overhead.  

### 4.5 Predictive Diagnostic stacked bar chart  

<img width="532" height="376" alt="image" src="https://github.com/user-attachments/assets/7e4899f3-9d96-4b35-af46-8c4ab8f2f317" />
**Figure 10** Predictive Diabetes Diagnostic Stacked Bar chart  

This graph is most unique, the user can put in relevant medical measurements, and a stacked bar chart is generated by supervised machine learning model trained by the dataset. The predictive diagnostic stacked bar chart helps individuals quickly assess their diabetes risk without waiting for clinical tests, offering faster intervention. Without need of a waiting list.  

Which will mean Doctors can treat their patients more effectively and efficiently in other areas. The Stacked bar chart is colour coded based on the different diabetes conditions and is labelled with the percent of likelihood of the condition.  

---

## 5. Conclusion  
In this report, we have explored the diabetes dataset, detailing the available data and its types. We reviewed the current state of diabetes visualizations, focusing on interpretations from leading institutions such as the NHS and the International Diabetes Federation.  

Through this review, we identified gaps in the visual representation of diabetes data and proposed innovative prototypes for highly interactive graphs. These proposed visualizations aim to provide valuable insights, including the detection of frequent anomalies that could lead to scientific breakthroughs, improved diagnosis processes that may reduce waiting times, and a decreased workload for doctors.  

By offering clearer comparative views of diabetes data, these visualizations can facilitate research categorization and deepen understanding.  

Moving forward, these prototypes should undergo user testing to assess their usability. Tasks should be time-assessed to measure the speed at which users comprehend the information, as this aspect has not been fully quantified.  

---

## 6. References  

[1] Roglic, G. (2016). WHO Global report on diabetes: A summary. International Journal of Noncommunicable Diseases, [online] 1(1), p.3. doi:<https://doi.org/10.4103/24688827.184853>.  

[2] Diabetes UK. (n.d.). How many people in the UK have diabetes? Available at: <https://www.diabetes.org.uk/aboutus/about-the-charity/ourstrategy/statistics>  

[3] Fazakis, N., Kocsis, O., Dritsas, E., Alexiou, S., Fakotakis, N. and Moustakas, K. (2021). Machine Learning Tools for Long-Term Type 2 Diabetes Risk Prediction. IEEE Access, 9, pp.103737–103757. doi:<https://doi.org/10.1109/access.2021.3098691>.  

[4] BelHadj, S., Hentati, O., Elfeki, A. and Hamden, K. (2013). Inhibitory activities ofUlva lactucapolysaccharides on digestive enzymes related to diabetes and obesity. Archives of Physiology and Biochemistry, 119(2), pp.81–87. doi:<https://doi.org/10.3109/13813455.2013.775159>.  

[5] NHS Digital. (n.d.). Clinical audits and registries. [online] Available at: <https://digital.nhs.uk/data-andinformation/clinical-audits-andregistries>.  

[6] Worldmapper. (2019). Expenditure for patients with Diabetes. [online] Available at: <https://worldmapper.org/maps/healthdiabetesexpenditure-2017/> [Accessed 13 May 2025].  

[7] International Diabetes Federation (2021). Diabetes around the World in 2021. [online] IDF Diabetes Atlas. Available at: <https://diabetesatlas.org/>.  

[8] Saary, M.J. (2008). Radar plots: a useful way for presenting multivariate health care data. Journal of Clinical Epidemiology, [online] 61(4), pp.311317. doi:<https://doi.org/10.1016/j.jclinepi.2007.04.021>. 

[9] Thompson, P. (2010). Chapter 10 - Learning by Doing. [online] ScienceDirect. Available at: <https://www.sciencedirect.com/science/article/abs/pii/S0169721810010105>.  
