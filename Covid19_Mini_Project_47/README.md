# COVID-19 India Data Analysis 🇮🇳

An exploratory data analysis (EDA) project on COVID-19 cases and vaccination progress in India, built with Python, Pandas, Matplotlib, and Seaborn.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)

---

## 📌 Project Overview

This project analyzes the spread, impact, and recovery from COVID-19 across Indian states and union territories, along with the national vaccination rollout. It covers data cleaning, aggregation, statistical summaries, and a series of visualizations that answer key questions such as:

- How did confirmed cases, recoveries, and deaths evolve over time?
- Which states were the most and least affected?
- How do recovery and death rates compare across states?
- How did vaccination progress from 2021 onward?

## 📊 Dataset

The analysis uses two publicly available datasets (loaded directly from their sources in the script):

| Dataset | Source | Description |
| --- | --- | --- |
| **COVID-19 India Cases** | [imdevskp/covid-19-india-data](https://github.com/imdevskp/covid-19-india-data) | State-wise daily cumulative confirmed, death, and recovery counts |
| **Vaccination Data** | [OWID COVID-19 Data](https://github.com/owid/covid-19-data) | Daily vaccination doses administered in India |

## 🛠️ Tech Stack

- **Python 3.8+**
- **Pandas** — data loading, cleaning, transformation
- **NumPy** — numerical operations
- **Matplotlib** & **Seaborn** — data visualization

## 📁 Project Structure

```javascript
covid-19-india-analysis/
│
├── tut1.py                     # Main analysis script (notebook-style)
├── cleaned_covid_india.csv     # Cleaned dataset (generated after running)
├── README.md
└── requirements.txt
```

## ⚙️ Setup & Usage

1. **Clone the repository**

```bash
git clone https://github.com/<your-username>/covid-19-india-analysis.git
cd covid-19-india-analysis
```

2. **Install dependencies**

```bash
pip install -r requirements.txt
```

3. **Run the analysis**

```bash
python tut1.py
```

The script fetches the datasets from the web, cleans them, prints summary statistics, generates all plots, and exports `cleaned_covid_india.csv`.

## 🧹 Data Cleaning Steps

- Renamed columns to clean `snake_case`
- Converted `date` to datetime and coerced invalid numeric values
- Standardized inconsistent state/UT names (e.g. `Telangana***` → `Telangana`)
- Removed duplicate `(date, state)` rows
- Derived an `active cases` column: `confirmed - deaths - cured`

## 📈 Analysis & Visualizations

The script produces the following outputs:

1. Cumulative confirmed, recovered, and death cases over time
2. Daily new confirmed cases (national)
3. Top 10 states by total confirmed cases
4. Recovery rate (%) of the top 10 worst-hit states
5. Confirmed cases over time — top 5 states
6. Share of total cases by state (pie chart)
7. National recovery rate trend
8. Recovery rate vs death rate scatter plot (bubble = case count)
9. Correlation heatmap of national COVID metrics
10. Monthly box plot of daily new cases
11. Vaccination progress (total doses vs fully vaccinated)
12. 10 least-affected states/UTs

## 📦 Output

- **`cleaned_covid_india.csv`** — the cleaned, analysis-ready dataset

## 🤝 Contributing

Contributions are welcome! Feel free to fork the repo and submit a pull request.

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [imdevskp](https://github.com/imdevskp) for the India COVID-19 dataset
- [Our World in Data](https://ourworldindata.org/coronavirus) for vaccination data# COVID-19 India Data Analysis 🇮🇳

An exploratory data analysis (EDA) project on COVID-19 cases and vaccination progress in India, built with Python, Pandas, Matplotlib, and Seaborn.

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green)
