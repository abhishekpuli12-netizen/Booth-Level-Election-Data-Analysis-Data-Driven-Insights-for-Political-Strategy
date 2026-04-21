# 🗳️ Booth-Level Electoral Analysis — Warangal West
### BJP Performance Analysis | Telangana Assembly Elections 2023

> Built a complete data pipeline from scratch — extracted real polling station data from scanned PDF images, converted to structured CSV, preprocessed, and performed in-depth EDA to uncover booth-level electoral patterns and strategic insights.

<br>

![Python](https://img.shields.io/badge/Python-3.10-blue?logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2.0-darkblue?logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange?logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical-teal)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)

---

## 🌟 What Makes This Project Unique

Unlike most EDA projects that use ready-made datasets, this project was built **entirely from scratch**:

- 📄 **No dataset was available** — data existed only as a scanned PDF image of official polling records
- 🔍 **Manually extracted** booth-level vote counts from the PDF using Python
- 🧹 **Preprocessed raw messy data** into a clean, structured CSV
- 📊 **Performed full EDA** on 250+ polling stations with actionable insights
- 💡 **Generated real strategic recommendations** for booth-level campaign planning

---

## 📌 Project Overview

This project presents a comprehensive **Exploratory Data Analysis (EDA)** of booth-level voting patterns in the **Warangal West Assembly Constituency**, Telangana. The analysis focuses on BJP's electoral performance, party-wise comparisons, historical trends (2018 vs 2023), and identification of high-opportunity zones across all polling stations.

---

## 🔢 Key Numbers at a Glance

| Metric | Value |
|--------|-------|
| 📍 Constituency | Warangal West, Telangana |
| 🗳️ Polling Stations Analyzed | 250+ |
| 📅 Election Years Compared | 2018 vs 2023 |
| 🏆 INC Vote Share (2023) | 43.78% — Leads |
| 🔵 BRS Vote Share (2023) | 35.72% — Declining |
| 🟠 BJP Vote Share (2023) | 18.87% — Fast Growing |
| 📈 BJP Growth Rate | **+415.7% (2018 → 2023)** |
| 💪 BJP Strongest Booth | Krishna Colony — 289 votes |
| ⚠️ BJP Weakest Booth | Peddamma Gadda — 19 votes |
| 🚨 Highest NOTA Booth | Vishnupuri Somidi — 879 votes |

---

## 🔄 Data Pipeline — Built From Scratch

```
Scanned PDF Image
      ↓
PDF Data Extraction (Python)
      ↓
Raw CSV (unstructured)
      ↓
Data Preprocessing & Cleaning
      ↓
Structured Clean Dataset
      ↓
Exploratory Data Analysis
      ↓
Insights & Visualizations
```

### Step 1 — PDF Image to CSV
- Official polling data existed only as a **scanned PDF image**
- Extracted tabular vote counts for all parties across every booth
- Converted unstructured text into a raw CSV file

### Step 2 — Preprocessing
- Standardized column names (BJP, INC, BRS, BSP, NOTA)
- Handled missing values and inconsistencies
- Removed duplicates and validated vote totals
- Added derived columns (vote share %, party rankings per booth)

### Step 3 — EDA & Analysis
- Booth-level statistical analysis for all parties
- Performance segmentation (High / Medium / Low)
- Historical comparison (2018 vs 2023)
- Opportunity zone identification

---

## 📊 Analysis Performed

### Vote Share Analysis
- Party-wise percentage distribution across the full constituency
- INC leads with 43.78%, BRS second at 35.72%, BJP emerging at 18.87%

### Booth-Level Party Analysis
- BJP, INC, BRS, BSP individual booth performance mapped
- Strongest and weakest booths identified for each party
- Vote range and distribution pattern analysis

### BJP Deep Dive
- Top 20 highest performing BJP booths
- Top 30 lowest performing BJP booths
- Middle-tier booths with swing potential
- Strategic opportunity zones

### NOTA Analysis
- Unusually high NOTA at Vishnupuri Somidi (879 votes) — protest voting signal
- High NOTA booths = conversion opportunities for BJP

### Historical Trend (2018 vs 2023)

| Party | 2018 Votes | 2023 Votes | Change |
|-------|-----------|-----------|--------|
| BJP | 5,979 | 30,826 | **+415.7%** |
| INC | 44,555 | 72,649 | +63.1% |
| BRS | 81,006 | 57,318 | -29.2% |
| BSP | 865 | 808 | -6.6% |
| NOTA | 3,075 | 2,426 | -21.2% |

---

## 📈 Visualizations Included

- Party-wise vote share bar chart
- BJP votes by polling station (line plot with highest/lowest markers)
- INC votes by polling station
- BRS votes by polling station
- NOTA votes by polling station (with outlier spike)
- Top 20 high-performing BJP booths (horizontal bar chart)
- Top 30 low-performing BJP booths (horizontal bar chart)
- 2018 vs 2023 vote comparison (multi-line trend)
- Percentage change chart across all parties

---

## 💡 Key Insights

1. **BJP is the fastest-growing party** — 415% vote increase in 5 years
2. **INC is the current leader** — consistent across most high-population booths
3. **BRS is rapidly declining** — lost nearly 24,000 votes since 2018
4. **Voter consolidation is happening** — smaller parties and NOTA shrinking
5. **BJP has strong urban pockets** — Ramannapet, Krishna Colony, Hanumannagar
6. **Critical weak zones for BJP** — Peddamma Gadda (19), Kakatiya Colony (20), Lashkar Singaram (23)
7. **Mid-level booths are high opportunity** — improving 30–40 votes per booth can change overall results
8. **Constituency is becoming bipolar** — heading toward INC vs BJP two-party contest

---

## 🛠️ Tech Stack

```
Python 3.10        — Core programming language
Pandas             — Data extraction, cleaning, analysis
Matplotlib         — Charts and visualizations
Seaborn            — Statistical plots
Jupyter Notebook   — Interactive development environment
NumPy              — Numerical operations
```

---

## 📁 Project Structure

```
election-eda-warangal-west/
│
├── data/
│   ├── raw/
│   │   └── polling_data_scanned.pdf      ← original scanned PDF
│   ├── extracted/
│   │   └── polling_data_raw.csv          ← after PDF → CSV extraction
│   └── processed/
│       └── polling_data_clean.csv        ← after preprocessing
│
├── notebooks/
│   ├── 01_data_extraction.ipynb          ← PDF to CSV conversion
│   ├── 02_preprocessing.ipynb            ← data cleaning pipeline
│   └── 03_eda_analysis.ipynb             ← full EDA and insights
│
├── plots/
│   ├── vote_share_percentage.png
│   ├── bjp_votes_by_booth.png
│   ├── inc_votes_by_booth.png
│   ├── brs_votes_by_booth.png
│   ├── nota_analysis.png
│   ├── top20_high_bjp_booths.png
│   ├── top30_low_bjp_booths.png
│   └── 2018_vs_2023_trend.png
│
├── report/
│   └── election_eda_report.pdf           ← full analysis report
│
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/abhishekpuli12-netizen/election-eda-warangal-west.git
cd election-eda-warangal-west

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run notebooks in order
jupyter notebook notebooks/01_data_extraction.ipynb
jupyter notebook notebooks/02_preprocessing.ipynb
jupyter notebook notebooks/03_eda_analysis.ipynb
```

---

## 📦 Requirements

```
pandas>=2.0
matplotlib>=3.7
seaborn>=0.12
jupyter
numpy>=1.24
```

```bash
pip install pandas matplotlib seaborn jupyter numpy
```

---

## 🎯 Skills Demonstrated

| Skill | How It Was Applied |
|-------|-------------------|
| **Data Extraction** | Extracted real data from scanned PDF images |
| **Data Wrangling** | Cleaned and structured raw messy data |
| **EDA** | Full exploratory analysis on 250+ booths |
| **Data Visualization** | 9+ custom charts and plots |
| **Statistical Analysis** | Vote share, distributions, trend analysis |
| **Domain Understanding** | Electoral data interpretation and strategy |
| **End-to-End Pipeline** | PDF → CSV → Clean Data → Insights |

---

## 👤 Author

**Puli Abhishek**
*Aspiring Data Scientist | Python | Machine Learning | EDA*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/puli-abhishek-05914a264)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black?logo=github)](https://github.com/abhishekpuli12-netizen)
[![Email](https://img.shields.io/badge/Email-Contact-red?logo=gmail)](mailto:abhishekpuli12@gmail.com)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

⭐ **Star this repo if you found it useful!**

*"Data tells the story that words cannot."*

</div>
