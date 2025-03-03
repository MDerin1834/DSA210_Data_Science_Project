# DSA210_Data_Science_Project
[Mustafa Derin 32272]

Project Proposal: Colorectal Cancer Prediction Using Global Data

1. Project Overview
   
This project aims to analyze a large global dataset on colorectal cancer (CRC) with the goal of developing a machine learning model that can predict survival outcomes based on various factors. The dataset contains 21 parameters across over 160,000 records, including demographic and medical data related to colorectal cancer patients from various countries. Given the size and complexity of the dataset, the project will focus on a manageable subset of 20,000 records for analysis. Additionally, the project will incorporate augmented data from external sources, such as age distribution scores and cancer mortality rates (ASR) by country, to enhance the model's predictive performance. This combination of clinical data and contextual country-based information is expected to provide more accurate and insightful predictions.

2. Motivation
   
Colorectal cancer is one of the leading causes of cancer-related deaths worldwide. Its incidence and mortality rates vary significantly across different regions due to factors such as healthcare access, lifestyle, diet, and genetics. By analyzing a global dataset, My aim is to identify patterns that can inform early detection and survival prediction strategies. The motivation for this project stems from the need to better understand how factors like age, geographical location, physical features, alcohol or tobacco consupmtion and other demographic information impact colorectal cancer survival rates, thus enabling more tailored healthcare strategies for different regions.

3. Project Goals and Objectives
   
The main goal of this project is to build a machine learning model capable of predicting survival rates in colorectal cancer patients. Specific objectives include:

Analyzing the global colorectal cancer dataset, which includes 21 parameters and 160,000 records.
Selecting a representative subset of 20,000 records for analysis to ensure computational efficiency.
Augmenting the dataset with two additional parameters:
Age distribution score: Calculated using data from the United Nations, this score categorizes the global population into age groups, which will be assigned to corresponding patients in the dataset. Source: https://encr.eu/sites/default/files/inline-files/Colorectal_cancer_factsheet_March_2021.pdf [ENCR]
Age-standardized death rate (ASR): This score, based on country-specific mortality rates, will enhance the model's ability to account for the impact of healthcare systems and country-level factors on colorectal cancer survival. Sources: 
(1) Wang, C. C., Sung, W. W., Yan, P. Y., Ko, P. Y., & Tsai, M. C. (2021). Favorable colorectal cancer mortality-to-incidence ratios in countries with high expenditures on health and development index: A study based on GLOBOCAN database. Medicine, 100(41), e27414. https://doi.org/10.1097/MD.0000000000027414 
(2) https://www.wcrf.org/preventing-cancer/cancer-statistics/colorectal-cancer-statistics/ [WCRF]

5. Data Description
The project will use the following datasets:

Colorectal Cancer Dataset:
This dataset contains 21 parameters (e.g., age, gender, stage of cancer, treatment methods, survival outcome) across over 160,000 records of colorectal cancer patients.
The parameters are a mix of categorical and numerical variables that describe clinical, demographic, and medical factors influencing colorectal cancer prognosis.
External Data Sources:
UN Age Distribution Data: This data includes global population age distribution statistics, which will be used to calculate age scores and assign these scores to colorectal cancer patients based on their reported age.
ASR Data: The Age-Standardized Death Rate data will be sourced from global health reports (e.g., World Health Organization, UN). The ASR data reflects the age-adjusted death rates caused by colorectal cancer in various countries. These country-specific values will help contextualize survival outcomes based on national factors.
5. Data Collection Strategy
Colorectal Cancer Dataset:

The primary dataset will be sourced from a public health database or a research repository that specializes in cancer data, such as the Cancer Genome Atlas (TCGA) or a similar source.
Data will be filtered to focus on colorectal cancer cases, ensuring it aligns with the research objectives.
Due to the large size of the dataset (160,000+ records), a random sampling technique will be employed to select a manageable subset of 20,000 records.
External Data:

Age Distribution Data: The United Nations Population Division provides global population data, which includes age distribution by country. This data will be obtained from the UN’s website or related statistical sources.
ASR Data: The Age-Standardized Death Rate data will be sourced from international health organizations like the WHO or global cancer registries such as the Global Cancer Observatory (GCO).
6. Data Preprocessing and Augmentation
Data Cleaning:
Any missing or incomplete data in the colorectal cancer dataset will be handled by imputation or removal, depending on the extent of missing values.
Outliers will be identified and managed using standard statistical methods to prevent model skewing.
Data Augmentation:
Age Distribution Scores: After collecting age distribution data from the UN, an age score will be calculated by categorizing patients into different age groups. These scores will be assigned to corresponding records in the colorectal cancer dataset.
ASR Scores: The ASR data will be merged with the colorectal cancer dataset based on the country of each patient. This will provide a country-based adjustment to the survival prediction.
