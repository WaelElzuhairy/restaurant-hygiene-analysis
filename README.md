# Restaurant Hygiene Analysis

A data mining project that uses NLP and fuzzy logic to evaluate and categorize how clean restaurants are based on Google Places reviews.

## Overview

This project scrapes Google Places data from chicken restaurants, isolates English-language reviews mentioning hygiene-related terms (such as clean, dirty, fresh, and bacteria), then applies fuzzy logic to generate a cleanliness score (0–1) for each restaurant. The results are presented through a Power BI dashboard.

## Key Findings

- A moderate **0.36 correlation** was found between hygiene sentiment and Google star ratings
- The analysis flagged **7 poorly-rated** and **6 well-rated** restaurants based on hygiene scores
- Hygiene sentiment and overall star ratings don't always agree

## Project Structure

```
├── notebooks/
│   └── restaurant_hygiene_analysis.ipynb   # Core analysis (NLP + fuzzy logic)
├── data/
│   ├── google_places_reviews.csv           # Raw review data from Google Places
│   └── google_places_stars.csv             # Restaurant star rating data
├── results/
│   └── powerbi_dashboard.pbix.zip          # Exported Power BI dashboard
├── report/
│   └── report.pdf                          # Complete project report
├── slides/
│   └── project_poster.pdf                  # Project poster
├── docs/
│   └── code_reference_sheet.pdf            # Code reference documentation
├── README.md
└── .gitignore
```

## Methodology

1. **Data Collection** — Gathered restaurant reviews via the Google Places API
2. **Preprocessing** — Applied tokenization, lemmatization, and stopword removal
3. **Hygiene Keyword Filtering** — Isolated reviews containing hygiene-relevant terms
4. **Fuzzy Logic Scoring** — Assigned each restaurant a cleanliness score on a 0–1 scale
5. **Visualization** — Built a Power BI dashboard for business intelligence reporting

## Tech Stack

- Python (Pandas, NLTK, scikit-fuzzy)
- Power BI
- Google Places API
