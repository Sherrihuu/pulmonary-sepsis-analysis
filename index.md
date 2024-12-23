# Pulmonary and Sepsis Analysis

## Objective
This exploratory data analysis (EDA) investigates the prevalence, co-occurrence, mortality, and length of stay (LOS) among patients with pulmonary conditions and sepsis. Two patient-identification methods—free-text admission diagnoses versus ICD-9 codes—are compared and evaluated.

---

## Key Findings

### Overall Patient Counts
- **Pulmonary Patients**  
  - *Admission Diagnosis*: 5,311  
  - *ICD-9 Codes*: 15,505  

- **Sepsis Patients**  
  - *Admission Diagnosis*: 1,831  
  - *ICD-9 Codes*: 5,325  

- **Both Pulmonary and Sepsis**  
  - *Admission Diagnosis*: 94  
  - *ICD-9 Codes*: 2,366  

**Interpretation**  
The ICD-9–based approach yields higher patient counts, indicating broader capture of clinical conditions. By contrast, the admission-diagnosis approach, which relies on free-text data, may omit less explicit or secondary diagnoses.

---

## Explanation of Methods

1. **Admission Diagnosis Method**  
   - Flags pulmonary or sepsis cases using keyword searches in the free-text admission diagnosis field.  
   - Offers a quick overview but may miss ambiguous or secondary terms.

2. **ICD-9 Codes Method**  
   - Identifies pulmonary or sepsis cases via standardized diagnostic codes.  
   - More comprehensive but reliant on accurate and consistent coding practices.

Using both approaches provides a more robust understanding of the patient population.

---

## Contingency Table

|                   | ICD-9 Codes | Admission Diagnosis |
|-------------------|------------:|--------------------:|
| Neither           |       40,512|              51,928 |
| Pulmonary Only    |       13,139|               5,217 |
| Sepsis Only       |        2,959|               1,737 |
| Pulmonary + Sepsis|        2,366|                  94 |

---

## Proportional Analysis

- **Pulmonary Patients Developing Sepsis**  
  - *ICD-9 Codes*: 15.26%  
  - *Admission Diagnosis*: 1.77%

- **Sepsis Patients Developing Pulmonary Conditions**  
  - *ICD-9 Codes*: 44.43%  
  - *Admission Diagnosis*: 5.13%

These percentages underscore the variations in capture rates between methods.

---

## Mortality Analysis (ICD-9 Codes)

### In-Hospital Mortality
- **Pulmonary Group**: 15.11% vs. **Non-Pulmonary Group**: 8.92%  
- **Sepsis Group**: 32.66% vs. **Non-Sepsis Group**: 8.21%

### Category-Wise Mortality
- **Neither**: 7.16%  
- **Pulmonary Only**: 11.33%  
- **Sepsis Only**: 31.18%  
- **Pulmonary + Sepsis**: 34.45%

Patients diagnosed with both pulmonary conditions and sepsis show the highest mortality rates.

---

## Length of Stay (ICD-9 Codes)

- **Pulmonary Group**: 5.9 days vs. **Non-Pulmonary Group**: 4.6 days  
- **Sepsis Group**: 7.2 days vs. **Non-Sepsis Group**: 4.7 days

### Category-Wise LOS
- **Neither**: 4.2 days  
- **Pulmonary Only**: 5.1 days  
- **Sepsis Only**: 8.8 days  
- **Pulmonary + Sepsis**: 5.6 days  

Patients with sepsis generally have extended hospital stays, while pulmonary diagnoses also contribute to increased LOS.

---

## Visualizations

1. **Contingency Table Heatmap**  
2. **Proportional Analysis**  
3. **Category Distribution (Bar and Pie Charts)**  
4. **Mortality Analysis (by Pulmonary Group, Sepsis Group, and Combined Categories)**  
5. **Length of Stay (by Pulmonary Group, Sepsis Group, and Combined Categories)**  

*(Figures omitted for brevity.)*

---

## Recommendations

1. **Use Both Methods**  
   - Combine free-text admission diagnoses with ICD-9 data for a more complete patient population.

2. **Prioritize High-Risk Patients**  
   - Focus on those with both sepsis and pulmonary diagnoses, given their high mortality and LOS.

3. **Improve Data Quality**  
   - Strengthen coding practices to ensure reliable ICD-9 documentation and accurate analyses.

4. **Optimize Resource Allocation**  
   - Target interventions to reduce LOS and improve outcomes for high-risk groups, especially sepsis patients.

5. **Expand Research**  
   - Explore clinical factors contributing to high co-occurrence and adverse outcomes in pulmonary/sepsis patients.

---

© 2024 Tongxun Hu. All Rights Reserved.