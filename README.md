# Hospital-Visitation-Report
![Capture](https://github.com/noshiobec/Hospital-Visitation-Report/assets/96450822/6a5b6f83-ab21-4757-9c6a-7faf269346ad)


## [View Report](https://app.powerbi.com/view?r=eyJrIjoiNGYyMTU1NGYtZDFhMS00YzVkLTgzMjgtOWJmMWUzYTY2NjA4IiwidCI6Ijg2ZDhlM2ViLTQ4YzYtNDdlZC05Nzk0LTdiZmZmNWE2ZTUyNCJ9)

### Overview
This project provides a comprehensive analysis of hospital patient visit data, including demographics, satisfaction scores, wait times, and department referrals. Using Power BI, a dashboard was created to visualize the data, ensuring accuracy through data cleaning and transformation. Key insights and trends are explored to inform recommendations for enhancing patient satisfaction and optimizing hospital operations.

### Data Description
The dataset consists of the following columns:
- Date: Date and time of patient visit
- Patient ID: Unique identifier for each patient
- Patient Gender: The gender of the patient
- Patient Age: Age of the patient in years
- Patient SAT Score: Patient satisfaction score (out of 10)
- Patient First Initial: First initial of the patient's first name
- Patient Last Name: Patient's last name
- Patient Race: Race or ethnicity of the patient
- Patient Admin Flag: Indicating whether the patient was admitted (TRUE) or not (FALSE)
- Patient Wait Time: Time the patient waited for treatment (in minutes)
- Department Referral: The department to which the patient was referred (if any)

### Data Cleaning and Preparation
Before analyzing the data, I performed several cleaning and transformation steps:
- **Data Quality Checks**: Ensured that the data had no significant missing values or anomalies.
- **Standardization of Formats**: Converted date and time formats to a consistent structure for accurate temporal analysis.
- **Data Type Conversions**: Ensured correct data types for each column (e.g., integers, strings, dates).
- **Duplicate Removal**: Removed any duplicate records based on unique identifiers.
- **Data Transformation**: Combined "Patient First Initial" and "Patient Last Name" to create a new "Patient Name" column.

### Calculated Columns
Calculated columns are custom columns derived from existing data to facilitate deeper analysis. The following calculated columns were created:
- **Age Group**: A column that categorizes patients into age groups (e.g., 0-10, 11-20, 21-30, etc.). This allows for age-based segmentation and analysis.
- **Day of the Week**: A column that extracts the day of the week from the "Date" column, providing insights into patient visits by weekday.
- **Time of Day**: A column that categorizes visits into morning, afternoon, evening, or night based on the "Date" column's time component.

### Quick Measures
Quick measures are predefined calculations in Power BI used to generate metrics based on existing data. Here are some of the quick measures created for this analysis:
- **Percentage Admitted**: The proportion of patients who were admitted (TRUE) versus the total number of patients.
- **Percentage Male/Female**: The proportion of male and female patients, respectively.
- **Percentage Non-Categorized**: The proportion of patients who did not specify a gender.
- **Percentage Not Admitted**: The proportion of patients who were not admitted (FALSE).
- **Average Satisfaction**: The average patient satisfaction score across all records.
- **Average Wait Time**: The average wait time across all patients.
- **Department Referral Percentage**: The proportion of patients referred to a specific department versus the total number of patients.
- **Non-Department Referral Percentage**: The proportion of patients not referred to any department.
- **Admitted Male/Female Percentage**: The proportion of male and female patients who were admitted.


## Key Insights

The following key insights were observed:

### 1. Demographics
- **Total Number of Patient Visits**: 9,216 recorded visits.
- **Gender Distribution**: 48.7% female, 51.1% male, and 0.3% not categorized.
- **Age Group Distribution**:
  - Highest visits from young adults.
  - Followed by older adults, mid-adults, mid-childhood groups, teenagers, and infants.
- **Race Distribution**: Various patient races were recorded, contributing to the diverse demographic analysis.

### 2. Admission and Referrals
- **Admission Rates**: 50.04% of patients were admitted, while 49.96% were not.
- **Department Referrals**:
  - 41.41% of patients were referred to a department.
  - 58.59% of patients were not referred to any department.
- **Department Referrals Breakdown**:
  - General Practice: 1,840 referrals
  - Orthopedics: 995 referrals
  - Other departments: Physiotherapy, Cardiology, Neurology, Gastroenterology, and Renal (fewest referrals).

### 3. Patient Experience
- **Satisfaction Scores**: The average satisfaction score was 5.47.
- **Service Rating**: 75.1% of the services were not rated by patients.

### 4. Wait Times
- **Average Wait Time**: 35.26 minutes.
- **Correlation with Satisfaction**: Longer wait times were generally associated with lower satisfaction scores.

### 5. Other Analysis
- **Visits by Year**: Data covers 2019 and 2020.
- **Visits by Day of the Week**: Highest on Tuesday.
- **Visits by Month**: Highest in August and lowest in February.
- **Time of Day Analysis**: Evening had the highest number of visits.

## Recommendations

Based on the insights derived from the data analysis, the following recommendations are made:

1. **Reduce Wait Times**: Implement strategies to streamline patient processing, such as increasing staff during peak hours or optimizing scheduling systems. Shorter wait times are likely to improve patient satisfaction scores, which currently average 5.47.

2. **Improve Service Rating**: Encourage patients to rate their service experience by simplifying the feedback process and emphasizing its importance. With 75.1% of services not rated, there is a lack of comprehensive feedback to guide service improvements.

3. **Develop Age-Specific Services**: Create age-specific programs or services tailored to the needs of the highest visiting age groups, particularly young and older adults. Customized care can address specific health concerns of different age groups, improving satisfaction and health outcomes.

4. **Enhance Evening Services**: Strengthen staffing and resources during evening hours, which see the highest number of visits. Ensuring adequate support during peak evening times can help maintain service quality and reduce patient wait times.

5. **Increase Feedback Awareness**: Promote the importance of patient feedback through various channels, such as signage in the hospital, staff reminders, and digital platforms. Increased feedback will provide more data to identify areas for improvement and enhance patient satisfaction.

