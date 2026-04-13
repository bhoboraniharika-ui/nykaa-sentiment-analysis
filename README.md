# nykaa-sentiment-analysis
Analysis of 5,000+ Google Play Store reviews for the Nykaa app (Feb–Mar 2026)
to identify the root causes of negative sentiment and surface actionable
product recommendations.

## Overview

- Data source: Google Play Store (via `google-play-scraper`)
- Reviews scraped: 5,000 (Feb 8 – Mar 22, 2026)
- **Negative reviews analysed:** 1,055
- **Overall app rating (period):** 3.96 / 5.0

## Key Findings

1. Delivery is the #1 complaint — 379 of 685 categorised negative reviews
   (55.3%) are about delivery failures, making it the dominant retention risk.

2. ETA promises are broken — High-upvote reviews (👍122, 👍104, 👍98)
   cite same-day delivery shown at checkout but not honoured.

3. No delivery partner visibility — Users cannot see which logistics
   partner (e.g. Xpressbees) is handling their order, forcing all escalations
   to Nykaa's customer support.

## Charts

![Complaint Categories](images/nykaa_complaint_categories.png)
![Complaints Excluding Noise](images/nykaa_complaints_clean.png)
![Rating Trend](images/nykaa_rating_trend.png)

## How to Run

1. Open `Nykaa_Reviews.ipynb` in Google Colab or Jupyter
2. Run all cells — the first cell installs `google-play-scraper`
3. The notebook will scrape fresh reviews and regenerate all charts

## Dependencies

- `google-play-scraper`
- `pandas`
- `matplotlib`
