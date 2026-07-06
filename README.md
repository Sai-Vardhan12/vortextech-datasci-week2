# Week 2 — Student Performance EDA

## Overview
This project performs exploratory data analysis (EDA) on a student performance dataset, examining how factors like study hours, attendance, sleep, and internet usage relate to exam scores and placement outcomes.

## Dataset
The dataset (`dataset.csv`) contains the following columns:

| Column | Description |
|---|---|
| `study_hours` | Number of hours a student studies |
| `attendance` | Attendance percentage |
| `sleep_hours` | Average hours of sleep |
| `internet_usage` | Hours of internet usage |
| `assignments_completed` | Number of assignments completed |
| `previous_score` | Score from a previous exam/assessment |
| `exam_score` | Final exam score |
| `placement_status` | Placement outcome (e.g., `Placed`, `Not Placed`) |

## Analysis Performed
1. **Data loading & inspection** — loaded the CSV with pandas and previewed the data using `df.head()` and `df.tail()`.
2. **Correlation heatmap** — visualized correlations between all numeric features using a Seaborn heatmap.
3. **Study hours vs. exam score** — scatter plot to explore the relationship between the two.
4. **Grouped averages** — average exam score grouped by `study_hours` and by `placement_status`.
5. **Exam score by placement status** — boxplot comparing score distributions for placed vs. not-placed students.
6. **Distribution of study hours** — histogram (with KDE) showing how study hours are spread across students.

## Key Insights
These are the insights captured directly in the notebook's analysis:

- **Study hours strongly predict exam performance.** There is a clear positive relationship between study hours and exam scores — students who study longer tend to score better, making study hours one of the strongest predictors of academic performance.

- **Exam score is linked to placement outcome.** Students who passed (were placed) consistently achieved higher exam scores than those who were not, indicating a strong association between exam score and final placement outcome.

- **Most students study a moderate amount.** The distribution of study hours shows that the majority of students study around **4–8 hours**, with only a few studying for very short or very long durations.

## Requirements
- Python 3
- pandas
- numpy
- matplotlib
- seaborn

## Usage
1. Place `dataset.csv` in the project directory (update the file path in the notebook to match your local setup).
2. Open `week-2.ipynb` in Jupyter Notebook / JupyterLab.
3. Run all cells to reproduce the visualizations and insights.
