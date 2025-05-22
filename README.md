# Utilizing SQL-driven descriptive and diagnostic analytics to explore demographic profiles, environmental factors, and lesion characteristics.

# Project Overview
This project presents an in-depth analysis of a skin cancer dataset using SQL queries executed on a PostgreSQL database. The aim is to uncover
trends, patterns, and key insights related to skin cancer diagnoses, treatments, demographics, and outcomes to support data-driven decision-making 
in healthcare.
Disclaimer⚠️: All datasets and reports do not contain real proprietary, confidential, or sensitive information from any company, institution, or individual. All info are dummy and design to demonstrate my capabilities of using SQL to perform descriptive and diagnostic analytics.




# Understanding DermAI Diagnostics
Skin cancer remains one of the most prevalent and potentially life-threatening diseases; however, early detection greatly increases the chances of
successful treatment. DermAI Diagnostics harnesses the power of machine learning and clinical dermatology research to advance early diagnosis and
intervention. By analyzing patient demographics, environmental influences, and lesion characteristics, actionable insights are generated to support
dermatologists in identifying skin cancer at its earliest stages.

AI-powered diagnostic tools are integrated with real-world clinical data and SQL-based analytics to close the gap between healthcare professionals and
intelligent skin lesion classification systems. Through the provision of structured datasets and digital solutions, contribution is made to medical
research, epidemiological analysis, and AI-enhanced skin cancer detection—ultimately aiming to improve outcomes and advance public health.

# Data Description
The dataset consist of two tables namely Patient_info and Lesion_info respectively. Each table includes anonymized records of patients with suspected or confirmed skin cancer cases. These tables are linked by a common identifier (patient_id) and together provide a comprehensive view of skin cancer cases, including patient demographics and lesion-specific clinical data.


# Project Workflow
The analysis of the skin cancer dataset followed a structured, step-by-step workflow to ensure data integrity, analytical clarity, and meaningful insights:

1. Data Import & Setup
Loaded the patient_info and lesion_info tables into a PostgreSQL database.

Established relationships via patient_id as a foreign key.

Verified data types and cleaned missing or inconsistent values.

2. Data Exploration & Profiling
Conducted initial SQL queries to:

Understand the distribution of demographic variables.

Explore lesion types, locations, and sizes.

Identify outliers and missing data.

3. Descriptive Analytics
Aggregated data to summarize key trends:

Frequency of cancer types by age, gender, and region.

Distribution of UV exposure levels and skin types.

Lesion sizes by location and biopsy results.

4. Diagnostic Analytics
Cross-tabulated variables to uncover deeper patterns:

Relationship between lesion type and treatment outcomes.

Correlation between exposure levels and cancer incidence.

Family history vs. likelihood of malignant diagnosis.

5. Insight Generation
Highlighted key findings:

Most affected demographics.

Most effective treatments per cancer type.

Regions with higher prevalence of malignant lesions.

6. Reporting & Documentation
Documented SQL queries in the /queries folder.

Summarized insights and visualizations in the /insights or /reports folder.

# Some Key Analytical questions Addressed.
A number of queries were 
1. What are the most common types of skin cancer in the dataset?

2. How many lesions were biopsied?

3. Which gender has the highest proportion of biopsied lesions?

4. What body part(s) has the most lesion?

# Summary of Insights
This dataset presents a multi-dimensional view of skin cancer, categorized by demographics, environmental exposure, and lesion characteristics to 
different types of skin cancer. The skin cancer dataset shows that certain signs like bleeding, growing, and painful skin lesions are strong reasons
why doctors decide to perform a biopsy. The size and where the lesion appear on the body also play a big role, especially if the lesion is large or
in a visible area. Analysis of the dataset showed that most lesions are commonly found on the face, chest, back, and forearm, these are areas often
exposed to the sun. However, doctors are more likely to biopsy lesions found on the lips, nose, ears, and neck. 
Other factors like age, family history, exposure to harmful chemicals like pesticides, and lack of clean water or sanitation also increase the
chances of needing a biopsy. Altogether, this information helps researchers and doctors understand skin cancer better and also helps build smarter AI
tools by using clean, well-organized data that combines personal, medical, and environmental risks.

# Limitations

While the dataset provides valuable insights, several limitations affect the depth and generalizability of findings. The sample size of 1,088
lesions may not represent broader or more diverse populations.Only 458 out of 1,088 cases were biopsy-confirmed, and of those, just 441 were
medically relevant to this study i.e. MEL, SCC, ACK, BCC (cancerous), the remaining 17 cases i.e. SEK and NEV are benign. This means a significant
portion of the cancer-labelled data lacks clinical validation.
Additionally, the use of binary variables (e.g., TRUE/FALSE for symptoms or exposures) simplifies complex clinical and environmental realities,
limiting analytical details. A major data gap is seen in demographic completeness—over 583 out of 1,088 patients have Unknown or UNK parental ethnic
backgrounds, which weakens the dataset’s suitability for predictive modeling and machine learning. 
Lastly, potential data collection biases, such as underreporting of symptoms or missing socioeconomic context, may skew results and reduce the
reliability of interpretations.



# Recommendations

Based on the insights drawn from the patient info and lesion info datasets, here are some data-driven recommendations to help determine the accuracy
of lesion info provided by patients to enhance dermatological research by providing a well-organized dataset for epidemiological studies and AI
model training:

More biopsy needs to be performed as a standard in this medical research to make our data more relevant and accurate for machine learning studies or
correct analysis.

Other factors like age, family history, exposure to harmful chemicals like pesticides, and lack of clean water or sanitation also increase the
chances of needing a biopsy.

The problem statement says there are a total of 1,089 cases but after running diagnostic analysis, it shows there are 1,088 cases. I recommend use
of up to date records and proper database management systems.

By applying these recommendations, DermAI will be able to manage patient data properly and have accurate records for AI model training.

