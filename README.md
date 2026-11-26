# Predictive Maintenance Analysis

Analysis of industrial sensor data to understand and predict machine failures.
Work in progress: data understanding and feature engineering are complete;
modeling and SQL analysis are planned.

## Data Source
AI4I 2020 Predictive Maintenance Dataset, UCI Machine Learning Repository
(https://doi.org/10.24432/C5HS5C). Licensed under CC BY 4.0.
The dataset is synthetic: it was generated to reflect real predictive maintenance
data encountered in industry, so results do not transfer directly to real machines.

## Progress
- [x] 01 Data understanding and quality checks
- [x] 02 Feature engineering (temperature difference, power, wear x torque)
- [ ] 03 Modeling and evaluation
- [ ] SQL analysis

## Key Findings So Far
- Failures are rare (339 of 10,000 records, 3.39%), so accuracy alone would be misleading.
- Three engineered features reproduce the documented failure rules (HDF, PWF, OSF) exactly on this data.
- These rules explain 287 of the 339 failures; most of the rest are tool wear failures, which occur at a random time.
- Some failure-mode records in the file do not match the official description (noted in the notebooks).
