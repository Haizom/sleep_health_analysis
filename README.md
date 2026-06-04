# SleepScope Sleep Health Analysis

This project analyzes anonymized sleep and lifestyle survey data for **SleepInc**, using Python to explore relationships between sleep quality, occupation, BMI category, physical activity, stress, and sleep disorders.

The analysis is contained in the Jupyter notebook `notebook(3).ipynb` and uses the dataset `sleep_health_data.csv`.

## Project Overview

SleepInc provided sleep and lifestyle metrics for 374 individuals collected through its SleepScope tracking app. The goal of this analysis is to identify patterns that may help explain differences in sleep duration, sleep quality, and insomnia risk across different demographic and lifestyle groups.

The notebook performs exploratory data analysis and answers questions such as:

- Which occupations have the lowest average sleep duration?
- Which occupations have the lowest average quality of sleep?
- Is the occupation with the lowest sleep duration also the occupation with the lowest sleep quality?
- How does insomnia prevalence vary by BMI category?
- What relationships exist among numerical features such as sleep duration, quality of sleep, activity level, stress level, heart rate, and daily steps?

## Dataset

The project expects a CSV file named:

```text
sleep_health_data.csv
```

The dataset contains 374 rows and 13 columns:

| Column | Description |
|---|---|
| `Person ID` | Unique identifier for each individual |
| `Gender` | Gender of the person |
| `Age` | Age in years |
| `Occupation` | Occupation or profession |
| `Sleep Duration` | Average hours of sleep per day |
| `Quality of Sleep` | Sleep quality rating on a 1–10 scale |
| `Physical Activity Level` | Daily physical activity in minutes |
| `Stress Level` | Stress rating on a 1–10 scale |
| `BMI Category` | BMI category such as Normal, Overweight, or Obese |
| `Blood Pressure` | Blood pressure reading |
| `Heart Rate` | Resting heart rate in beats per minute |
| `Daily Steps` | Average daily steps |
| `Sleep Disorder` | Sleep disorder status: None, Insomnia, or Sleep Apnea |

## Key Findings

The notebook identifies several notable patterns:

- **Sales Representatives** have the lowest average sleep duration, at approximately **5.9 hours**.
- **Sales Representatives** also have the lowest average sleep quality, with an average score of **4.0**.
- The occupation with the lowest sleep duration is the same as the occupation with the lowest sleep quality.
- Insomnia ratios by BMI category are:
  - **Normal:** 0.04
  - **Overweight:** 0.43
  - **Obese:** 0.40
- People categorized as Overweight or Obese show much higher insomnia ratios than people in the Normal BMI category.

## Visualizations

The notebook includes the following exploratory visualizations:

1. Distribution of sleep duration
2. Count of sleep disorder categories
3. Correlation heatmap of numerical features

These charts help summarize sleep patterns and relationships between lifestyle and health metrics.

## Requirements

Install the following Python libraries before running the notebook:

```bash
pip install pandas matplotlib seaborn jupyter
```

## How to Run

1. Clone or download this project.
2. Place `sleep_health_data.csv` in the same directory as the notebook.
3. Open the notebook:

```bash
jupyter notebook "notebook.ipynb"
```

4. Run the cells from top to bottom.

## Project Files

```text
.
├── notebook.ipynb          # Main analysis notebook
├── sleep_health_data.csv      # Sleep and lifestyle dataset
├── insomnia.jpg               # Optional image used in the notebook
└── README.md                  # Project documentation
```

## Notes

- The CSV file must be available locally for the notebook to run successfully.
- The image `insomnia.jpg` is referenced in the first markdown cell, but it is only used for display and is not required for the data analysis.
- The analysis is exploratory and should be interpreted as descriptive, not causal.

## License

No license has been specified. Add a license before sharing or publishing this project publicly.
