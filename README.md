<h1 align="center">Premier League 2024-25: A Comprehensive Data Analysis & Data Science Project</h1>

<p align="center">
  <img src="image.jpg" alt="Premier League Analytics" width="600"/>
</p>

An end-to-end Data Science and Data Analysis project that performs a comprehensive analysis of the English Premier League 2024-25 season. This project transitions from descriptive **Data Analysis** (team/player performance) to inferential **Data Science** by applying hypothesis testing, explanatory regression modeling, and K-Means clustering to uncover deeper insights.

---

## 🚀 Table of Contents

- [✨ Features](#-features)
- [📊 Dataset Overview](#-dataset-overview)
- [🛠️ Installation](#️-installation)
- [▶️ Usage](#️-usage)
- [📈 Results & Performance](#-results--performance)
- [🔬 Technical Details & Methodology](#-technical-details--methodology)
- [📸 Visualizations](#-visualizations)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Features

- **Project Scope**: A full-cycle data science project covering data acquisition, cleaning, EDA, modeling, and reporting.
- **Dual Analysis**: In-depth analysis of both team dynamics (attacking, defensive, efficiency) and individual player performance (top scorers, positional analysis, goalkeeping).
- **Advanced Techniques**:
  - **Hypothesis Testing**: A statistical t-test to validate assumptions about top-performing teams.
  - **Explanatory Modeling**: Ordinary Least Squares (OLS) regression to determine the factors driving team points.
  - **Unsupervised Learning**: K-Means clustering to identify different profiles of attacking players.
- **Professional ML Engineering**:
  - Secure and automated data acquisition via the Kaggle API.
  - Robust data cleaning and feature engineering.
  - Comprehensive statistical evaluation and interpretation.
  - Interactive dashboards and professional-quality visualizations.
- **Technologies**: Python, Pandas, NumPy, Matplotlib, Seaborn, Plotly, SciPy, StatsModels, Scikit-learn.

---

## 📊 Dataset Overview

This analysis utilizes two high-quality, publicly available datasets from Kaggle:

| Dataset Type        | Description                                       | Source                   |
|---------------------|---------------------------------------------------|--------------------------|
| 🏟️ **Team Statistics**  | Team performance metrics, including Goals For (GF), Goals Against (GA), and Expected Goals (xG). | [Kaggle Dataset](https://www.kaggle.com/datasets/sattvikyadav/premier-league-2024-2025-team-statistics) |
| ⚽ **Player Statistics** | Detailed individual player stats, including goals, assists, tackles, and goalkeeper metrics.    | [Kaggle Dataset](https://www.kaggle.com/datasets/hubertsidorowicz/football-players-stats-2024-2025) |

**Key Metrics Analyzed**:
- **Team**: Points, Wins, Goals For/Against (GF/GA), Goal Difference (GD), Win Rate, Expected Goals (xG), Expected Goal Difference (xGD).
- **Player**: Goals, Assists, Goal Contributions, Tackles, Interceptions, Save Percentage, and various per-90-minute stats.

---

## 🛠️ Installation

### 1. Clone the repository
```bash
git clone https://github.com/X-XENDROME-X/Premier-League-Data-Science-Analysis.git
```

### 2. Set up your Kaggle API credentials using Google Colab Secrets (Secure Method - Recommended)

1. Go to your Kaggle account page and download your `kaggle.json` file
2. Open the downloaded file and note down the `username` and `key` values
3. In Google Colab:
   * Click the **🔑 key icon** in the left sidebar
4. Add two secrets:
   * **Name**: `KAGGLE_USERNAME` → **Value**: Your Kaggle username
   * **Name**: `KAGGLE_KEY` → **Value**: Your Kaggle API key
5. **Enable notebook access** for both secrets

---

### 3. Open the Notebook in Google Colab

* Upload `PremAnalytics.ipynb` to Google Colab

---

### 4. Install Dependencies

* If you're running the notebook in Google Colab, the first cell installs everything automatically
* If you're running it locally, use the following:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage

### 🔬 Complete Analysis Pipeline

Simply run the `PremAnalytics.ipynb` notebook from top to bottom in a Google Colab environment.

---

### ✅ Steps Overview

1. **Setup**
   The first cell installs all required packages.

2. **Data Acquisition**
   The notebook will automatically load your Kaggle credentials from Google Colab Secrets to securely download the datasets.
   ➤ **No manual file upload required.**

---

### 🔧 Setup Instructions

* Ensure you've added `KAGGLE_USERNAME` and `KAGGLE_KEY` to your Colab secrets.
* The notebook handles credential loading automatically.
* All datasets are downloaded securely from Kaggle via API.

---

### 🧩 First-Time Setup Instructions

If you haven't set up Colab secrets before, follow these steps:

1. Open your Google Colab notebook
2. Click the key icon (🔑) in the left panel
3. Add your Kaggle credentials as shown earlier
4. Run the credential loading cell in the notebook

---

### 📊 Analysis

The following tasks will run automatically:

* Data cleaning and feature engineering
* League table and team performance analysis
* Player performance and positional analysis
* Statistical modeling and clustering

---

### 👍🏼 Results

All findings, visualizations, and the interactive dashboard are generated inside the notebook.
Exported files are saved to your local directory.

---

## 📈 Results & Performance

### 🏆 Key Findings

| Category                 | Result                                                                     |
|--------------------------|----------------------------------------------------------------------------|
| **League Champion**      | 👑 Liverpool (84 Points)                                                    |
| **Best Attack**          | ⚽ Liverpool (86 Goals)                                                     |
| **Best Defense**         | 🛡️ Arsenal (34 Goals Conceded)                                              |
| **Top Scorer/Contributor**| 🎯 Mohamed Salah (Liverpool) - 29 Goals, 18 Assists                         |
| **Hypothesis Test Result** | ✅ Top 4 teams have a statistically significant higher Goal Difference (p < 0.05). |
| **Regression Model**     | 📊 Goals For/Against are strong predictors of final Points (R-squared: 0.942).|
| **Player Clustering**    | 🤖 Identified 3 distinct attacker archetypes using K-Means.                 |

### 🎯 Project Achievements

- ✅ **End-to-End Workflow**: Successfully demonstrated a complete data science pipeline.
- ✅ **Statistical Rigor**: Applied formal statistical methods to validate common football observations.
- ✅ **Machine Learning Application**: Used unsupervised learning to create data-driven player profiles.
- ✅ **Insightful Visualizations**: Created clear, interactive, and aesthetically pleasing charts and dashboards.

---

## 🔬 Technical Details & Methodology

### Data Science Techniques

- **Hypothesis Testing**: An independent two-sample t-test was used to compare the Goal Difference means between the Top 4 teams and the rest of the league. The rejection of the null hypothesis (p < 0.05) provides statistical evidence that a strong goal difference is a defining characteristic of elite teams.
- **Explanatory Regression**: An Ordinary Least Squares (OLS) model was built to explain the variance in `Points` using `GF`, `GA`, and `xGD` as predictors. The high R-squared value indicates a strong explanatory power, with `GF` and `GA` being the most significant coefficients.
- **K-Means Clustering**: Unsupervised clustering was applied to attacking players based on their `Goals_Per_90`, `Assists_Per_90`, and other creative/ball-progression metrics. This successfully segmented players into data-driven profiles like "Pure Finishers" and "Creative Forwards."

### Feature Engineering

New features were created to enable a more robust analysis:
- `Goals_Per_Game` / `Goals_Against_Per_Game`
- `Win_Rate` / `Points_Per_Game`
- `Goal_Contributions` (Goals + Assists)
- Per-90-minute metrics for fair player comparison.

---

## 📸 Visualizations

The project features a wide range of visualizations to tell a compelling data story:
- **League Standings**: Stacked bar charts and scatter plots showing team performance.
- **Team Performance**: Heatmaps comparing team ranks across various metrics (attacking, defensive, etc.).
- **Player Analysis**: Scatter plots for Goals vs. Assists and interactive radar charts for comparing top players.
- **Statistical Plots**: Histograms for performance distributions and correlation heatmaps.
- **Interactive Dashboard**: A final, interactive league table created with Plotly.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to fork the repository, make improvements, and open a pull request.

- **Areas for Contribution**:
  - Implement predictive models (e.g., forecasting match outcomes).
  - Add time-series analysis over multiple seasons.
  - Expand the data sources to include player wages or transfer fees.
  - Deploy the final insights into a web application (e.g., using Streamlit or Flask).

---

## 📚 Data Sources & Attributions

### Primary Data Sources
This analysis was made possible through the following high-quality, publicly available datasets from Kaggle. Full credit and acknowledgement are given to the dataset creators for their valuable contributions to the community.

#### Team Statistics:
- **Dataset:** Premier League 2024-2025 Team Statistics
- **Creator:** @sattvikyadav
- **Source URL:** [kaggle.com/datasets/sattvikyadav/premier-league-2024-2025-team-statistics](https://www.kaggle.com/datasets/sattvikyadav/premier-league-2024-2025-team-statistics)
- **License:** Open Data License
- **Usage:** Used for all team-level analysis, including league standings, performance metrics, and statistical modeling.

#### Player Statistics:
- **Dataset:** Football Players Stats 2024-2025 (Europe's Top 5 Leagues)
- **Creator:** @hubertsidorowicz
- **Source URL:** [kaggle.com/datasets/hubertsidorowicz/football-players-stats-2024-2025](https://www.kaggle.com/datasets/hubertsidorowicz/football-players-stats-2024-2025)
- **License:** Open Data License
- **Usage:** Used for all individual player analysis, including top performers, positional analysis, and clustering.

### Data Acknowledgements
- All underlying statistical data is originally sourced from **FBref.com**, a leading resource for football statistics provided by **Sports Reference**.
- Team and player performance metrics reflect the complete 2024-25 Premier League season.
- Advanced metrics such as Expected Goals (xG) are sourced from professional football analytics providers via FBref.

---

## 📄 License

This project is licensed under the **MIT License**. See the `LICENSE` file for details.

---
