# Restaurant Hygiene Analysis

A data mining project that analyzes Google Places reviews to assess and classify restaurant cleanliness using NLP and fuzzy logic scoring.

## Overview

This project crawls Google Places data for chicken restaurants, filters English-language reviews for hygiene-related keywords (clean, dirty, fresh, bacteria, etc.), and applies fuzzy logic to produce a hygiene score (0–1) per restaurant. Results are visualized in a Power BI dashboard.

## Key Findings

- Moderate **0.36 correlation** between hygiene sentiment and Google star ratings
- Identified **7 poorly-rated** and **6 well-rated** restaurants by hygiene score
- Hygiene sentiment does not always align with overall star ratings

## Project Structure

```
restaurant_hygiene_analysis.ipynb   # Main analysis notebook (NLP + fuzzy logic)
google_places_reviews.csv           # Raw Google Places review data
google_places_stars.csv             # Restaurant star rating data
powerbi_dashboard.pbix.zip          # Power BI dashboard file
report.pdf                          # Full project report
project_poster.pdf                  # Project poster
code_reference_sheet.pdf            # Code reference sheet
```

## Methodology

1. **Data Collection** — Google Places API crawl for restaurant reviews
2. **Preprocessing** — Tokenization, lemmatization, stopword removal
3. **Hygiene Keyword Filtering** — Extract hygiene-relevant reviews
4. **Fuzzy Logic Scoring** — Score each restaurant on a 0–1 hygiene scale
5. **Visualization** — Power BI dashboard for business intelligence reporting

## Tech Stack

- Python (Pandas, NLTK, scikit-fuzzy)
- Power BI
- Google Places API
