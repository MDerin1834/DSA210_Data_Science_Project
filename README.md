# DSA210_Data_Science_Project

[Mustafa Derin 32272]

## Project Proposal: Colorectal Cancer Prediction Using Global Data

### 1. Project Overview
   
This project aims to analyze a large global dataset on colorectal cancer (CRC) with the goal of developing a machine learning model that can predict survival outcomes based on various factors. The public dataset contains 26 parameters across over 160,000 records, including demographic and medical data related to colorectal cancer patients from various countries taken from kaggle website https://www.kaggle.com/datasets/ankushpanday2/colorectal-cancer-global-dataset-and-predictions. Given the size and complexity of the dataset, the project will focus on a manageable subset of 20,000 records for analysis. Additionally, the project will incorporate augmented data from external sources, such as age distribution scores and cancer mortality rates (ASR) by country, to enhance the model's predictive performance. This combination of clinical data and contextual country-based information is expected to provide more accurate and insightful predictions.

### 2. Motivation
   
Colorectal cancer is one of the leading causes of cancer-related deaths worldwide. Its incidence and mortality rates vary significantly across different regions due to factors such as healthcare access, lifestyle, diet, and genetics. By analyzing a global dataset, My aim is to identify patterns that can inform early detection and survival prediction strategies. The motivation for this project stems from the need to better understand how factors like age, geographical location, physical features, alcohol or tobacco consupmtion and other demographic information impact colorectal cancer survival rates, thus enabling more tailored healthcare strategies for different regions.

### 3. Project Goals and Objectives
   
The main goal of this project is to understand the most crucial factors leading to death from colorectal cancer. Specific objectives include:
My hypothesis is that it is more likely to have less survival ratios among colorectal cancer patients in American continents rather than the other continents due to relatively less developed health care systems or less healthy lifestyle in American countries, which may be the strong hinderances in one's survival. Also, by further analysis and enhancing the data, the leading causes of deaths from colorectal cancer and crucial factors that may give rise to colorectal cancer will be detailly investigated.

Augmenting the dataset with two additional parameters:
Age distribution score: Calculated using data from the United Nations, this score categorizes the global population into age groups, which will be assigned to corresponding patients in the dataset. The estimated distrubution of the new cases of colorectal cancer with respect to age is the following: 150 cases among 0 to 19 years old, 6,880 cases among 20 to 44 years old, 138,722 cases among 45 to 69 years old, and 195,667 cases 70+ years old. I standardize these numbers and age distribution scores (ADS) are listed in corresponding order: 0.00044 (age: 0-19), 0.02015 (age: 20-44), 0.40631(age: 45-69), 0.57310 (Age: 70+).
Source: https://encr.eu/sites/default/files/inline-files/Colorectal_cancer_factsheet_March_2021.pdf [ENCR] 

Death rates by country (ASR): This score, based on country-specific mortality rates, will enhance the model's ability to account for the impact of healthcare systems and country-level factors on colorectal cancer survival. I plan to used these scores and implement them in my data using reported country information for each student, which I believe will play a significant role in decision-making performance of the ML model. Sources: Wang, C. C., Sung, W. W., Yan, P. Y., Ko, P. Y., & Tsai, M. C. (2021). Favorable colorectal cancer mortality-to-incidence ratios in countries with high expenditures on health and development index: A study based on GLOBOCAN database. Medicine, 100(41), e27414. https://doi.org/10.1097/MD.0000000000027414 (1) https://www.wcrf.org/preventing-cancer/cancer-statistics/colorectal-cancer-statistics/ [WCRF] (2)

### 4. Data Description
   
The project will use the following datasets:

Colorectal Cancer Dataset:
This dataset contains 21 parameters (e.g., age, gender, stage of cancer, country, survival outcome) across over 160,000 records of colorectal cancer patients.
The parameters are a mix of categorical and numerical variables that describe clinical, demographic, and medical factors influencing colorectal cancer prognosis.
External Data Sources:
UN Age Distribution Data: This data includes global population age distribution statistics, which will be used to calculate age scores and assign these scores to colorectal cancer patients based on their reported age.
ASR Data: The death rate by country data will be sourced from global health reports (e.g., World Health Organization, UN). The ASR data reflects the age-adjusted death rates caused by colorectal cancer in various countries. These country-specific values will help contextualize survival outcomes based on national factors.

The project aims to drive insightful information by analyzing and elaborating on colorectal cancer data and various statistics. Since colorectal cancer accounted for
12.7% of all new cancer diagnoses and 12.4% of all deaths due to cancer (ENCR, 2021), I believe this project will be helpful breakpoint to spread more awereness about colorectal cancer. 
