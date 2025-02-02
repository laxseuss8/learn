# Analyzing-a-dataset-using-SQL

## Overview
This project explores the mental health of international students studying at a Japanese university, focusing on factors like social connectedness, acculturative stress, and length of stay. The analysis aims to determine whether studying abroad impacts mental health and identifies potential correlations between stay duration and mental health metrics.

## Key Features
- **SQL Analysis**: Uses PostgreSQL to group data by length of stay and compute average depression, social connectedness, and stress scores.
- **Jupyter Notebook**: Combines markdown explanations, data visualizations, and SQL queries for a comprehensive workflow.
- **Findings**: Investigates trends such as how mental health metrics evolve with longer stays abroad.

## Dataset Description
The dataset contains survey responses from students, including the following key columns:
- `inter_dom`: Student type (international/domestic)
- `japanese_cate`/`english_cate`: Language proficiency levels
- `stay`: Length of stay in years
- `todep`: Depression score (PHQ-9 test)
- `tosc`: Social connectedness score (SCS test)
- `toas`: Acculturative stress score (ASISS test)
- 
## Key Findings (Preview)
- International students with shorter stays (1-2 years) show higher average depression scores (`todep`) compared to those with longer stays.
- Social connectedness (`tosc`) tends to improve slightly with longer stays.
- Acculturative stress (`toas`) peaks in the middle years of stays (e.g., 3-4 years).
