# CareLoop Clinics – No-Show Guard
**GitHub Repository:** https://github.com/muskansirohi06-afk/CareLoop-No-Show-Guard

## Project Overview

This project aims to identify the reasons behind missed clinic appointments and predict patients who are at risk of missing their appointments using Python, SQL, Machine Learning and Generative AI.

## Key Findings

- **Part 1 – Data Cleaning:** The cleaned dataset contains 990 appointments, 16 columns and 218 no-shows.
- **Part 2 – SQL Analysis:** The overall no-show rate across 8 clinics was 22.02%.
- **Part 3 – Machine Learning:** Logistic Regression was selected as the final model, achieving a test ROC-AUC of 0.7889.
- **Part 4 – Generative AI:** Gemini analysed 10 follow-up notes, producing 9 valid responses and correctly skipping 1 blank note. Eight of the nine non-blank classifications matched the expected categories.

## Final Model

- Selected model: Logistic Regression
- Test ROC-AUC: 0.7889
- Selected risk threshold: 0.35
- Precision: 57.14%
- Recall: 57.14%
- High-risk appointments identified: 49

## Business Recommendations

CareLoop Clinics should introduce targeted appointment reminders because 218 out of 990 appointments were missed, representing a no-show rate of 22.02%.

The Logistic Regression model, with a ROC-AUC of 0.7889 and a risk threshold of 0.35, can help identify high-risk appointments for additional follow-up.

Among the analysed notes, 3 were classified as forgetting or not receiving reminders, 2 as transportation problems and 2 as work or scheduling problems. Clinics should improve reminder delivery, provide flexible scheduling and offer transportation guidance where possible.

## Generative AI Findings

The detailed CRAFT prompt produced more valid classifications than the simple prompt in the two-note comparison. Both intentionally invalid examples were correctly rejected by Pydantic. The final session recorded 15 API calls.

## Limitations

1. Only 10 follow-up notes were analysed, which may not represent all patients.
2. The relationship between reminders and missed appointments does not establish causation.
3. A random train-test split may not fully represent future appointment patterns.

## Tools and Technologies

- Python and Pandas
- Google Colab
- SQLite
- Scikit-learn
- Google Gemini API
- Pydantic
- GitHub

## Conclusion

The project demonstrates how data analysis, machine learning and Generative AI can support clinics in identifying high-risk appointments, understanding patient difficulties and improving appointment management.
