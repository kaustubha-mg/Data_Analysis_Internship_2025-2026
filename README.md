# Titanic Mini Visualization Dashboard — Task 4

## Dataset
**Titanic passenger dataset** (891 rows, 12 columns), sourced from the classic Kaggle
Titanic competition. A copy is included at `data/titanic.csv` so the notebook runs
without any extra downloads.

Columns include `PassengerId`, `Survived`, `Pclass`, `Name`, `Sex`, `Age`, `SibSp`,
`Parch`, `Ticket`, `Fare`, `Cabin`, `Embarked`.

## What's inside the notebook
`Titanic_Dashboard_Task4.ipynb` is organized into six Markdown-headed sections:

1. **Overview** — dataset intro and shape/missing-value check
2. **Cleaning** — median-fill `Age`, mode-fill `Embarked`, drop `Cabin`
3. **Features** — `FamilySize` (SibSp + Parch + 1) and `AgeGroup` (binned Age)
4. **Visualizations** — 5 required chart types + 1 bonus facet grid:
   - Histogram — Age distribution
   - Bar chart — Survival rate by Sex and by Class
   - Boxplot — Fare distribution by Class
   - Scatterplot — Age vs Fare, colored by Survival
   - Heatmap — Correlation of numeric features
   - *Bonus:* Facet grid — Survival by Class, split by Sex
5. **Insights** — a 5-point summary of the key patterns
6. **Conclusion** — takeaways and a suggested next step (simple classification model)

Every chart is followed by 1–2 sentences of interpretation, as required.

## How to run
1. Make sure `pandas`, `numpy`, `seaborn`, and `matplotlib` are installed:
   ```bash
   pip install pandas numpy seaborn matplotlib
   ```
2. Keep `data/titanic.csv` in a `data/` folder next to the notebook (already set up).
3. Open `Titanic_Dashboard_Task4.ipynb` in Jupyter Notebook, JupyterLab, or Google
   Colab and run all cells top to bottom.
4. Rendered charts are also exported as `.png` files into the `images/` folder for
   reuse outside the notebook.

## Folder structure
```
.
├── Titanic_Dashboard_Task4.ipynb
├── README.md
├── data/
│   └── titanic.csv
└── images/
    ├── 01_age_histogram.png
    ├── 02_survival_by_sex_class.png
    ├── 03_fare_boxplot.png
    ├── 04_age_vs_fare_scatter.png
    ├── 05_correlation_heatmap.png
    └── 06_facet_survival_class_sex.png
```
