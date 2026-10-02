## Business Understanding

### Context
Diabetes screening is costly, and clinics can only test a limited number of
patients. This project uses a Kaggle diabetes risk dataset to explore how a
clinic network could prioritize who to screen first.
(Note: the clinic scenario is a hypothetical use case for this analysis.)

### Stakeholders and Decisions
- **Clinic screening team:** decides which patients to screen first
- **Health education team:** decides which lifestyle habits to promote

### Business Questions
1. **Descriptive:** What share of patients in each age group and BMI
   category has high diabetes risk?
2. **Predictive:** Which patients are most likely to be high risk, so
   they can be prioritized for follow-up testing?
3. **Prescriptive:** Which modifiable lifestyle factors (activity, sleep,
   stress, smoking) show the largest difference in high-risk rates after
   controlling for age and BMI?

### Success Criteria
- Identify the age/BMI groups with the highest risk rates
- Build a model that catches high-risk patients (target: strong recall)
- Provide clear, data-backed lifestyle recommendations

### Scope and Limitations
- The data is a snapshot (no follow-up), so it shows current risk, not
  future diagnosis
- No data on diet sugar intake or on any screening program's effect
- Findings show association, not causation
- fasting_blood_sugar and hba1c_level closely define diabetes, so their
  use is handled carefully to avoid data leakage

### Data Source
Kaggle: 'diabetes_risk.csv' [https://www.kaggle.com/datasets/mansiaggarwal88/diabetes-risk-prediction']