
# ✈️ British Airways Reviews Data Analysis with Tableau by Shubham Pawar

*[My LinkedIn Profile.](https://www.linkedin.com/in/mjshubham21/)*

---

## 🌐 Project Links

- **Live Tableau Dashboard:** [View on Tableau Public](https://public.tableau.com/app/profile/shubham.pawar4669/viz/Airlines_Review_PROJECT/Dashboard?publish=yes)

---

## 📌 Overview

This project leverages **Tableau** to analyze customer reviews of British Airways, uncovering actionable insights about passenger satisfaction, service quality, and experience across different routes and cabin classes.

The primary objective is to help airline decision-makers:
- Understand overall customer satisfaction and recommendation trends.
- Identify areas—routes, cabins, and services—driving high and low ratings.
- Discover key service and experience factors influencing customer endorsements.

---

## 📁 Project Files

- `/dataset/ba_reviews.csv` – British Airways customer reviews dataset. [Link to main dataset](https://github.com/mjshubham21/BritishAirways_Tableau_Project/blob/main/dataset/ba_reviews.csv)
- `/dataset/Countries.csv` – Country mapping file (if applicable). [Link to Countries dataset](https://github.com/mjshubham21/BritishAirways_Tableau_Project/blob/main/dataset/Countries.csv)
- `/images/dashboard.png` – Main dashboard screenshot.
- `Airlines_Review_PROJECT.twbx` – Tableau packaged workbook for full interactivity.

---

## 🧩 Interactive Parameters & Calculated Fields

To enable dynamic filtering and flexible analysis, this dashboard includes:
- **Parameter:** `"Pick a Metric"` — allows users to select a metric (e.g., Overall Rating, Cabin Staff Service, Entertainment, etc.) for focused analysis.
- **Calculated Field:** `"Selected Parameter"` — returns the value of the selected metric for interactive dashboard filtering.
```
CASE [Pick a Metric]
WHEN 'Overall Rating' THEN [Rating]
WHEN 'Cabin Staff Service' THEN [Cabin Staff Service]
WHEN 'Entertainment' THEN [Entertainment]
WHEN 'Food' THEN [Food Beverages]
WHEN 'Ground Service' THEN [Ground Service]
WHEN 'Seat Comfort' THEN [Seat Comfort]
WHEN 'Value' THEN [Value For Money]
END
```

These fields are used for filters and comparisons in the dashboard. On the left side of the dashboard, users can easily choose which review aspect to explore using this parameter and calculated field setup.

---

## 📊 Key Metrics (KPIs)

1. **Total Reviews:** 1,324
2. **Average Rating:** 3.12 (out of 5)
3. **Recommendation Rate:** 41.6%
4. **Trip Verified Rate:** 57.3%

**Average Ratings by Cabin Class:**

| Cabin            | Avg. Rating |
|------------------|-------------|
| Economy          | 2.81        |
| Premium Economy  | 3.18        |
| Business         | 3.39        |
| First            | 3.71        |

**Top 5 Routes by Avg. Rating (Min 15 Reviews):**
- London Heathrow (LHR) – JFK: 3.9
- LHR – Los Angeles (LAX): 3.7
- LHR – Singapore (SIN): 3.6
- LHR – Hong Kong (HKG): 3.6
- LHR – Dubai (DXB): 3.5

**Bottom 5 Routes by Avg. Rating (Min 15 Reviews):**
- LHR – Rome (FCO): 2.4
- LHR – Paris (CDG): 2.5
- LHR – Barcelona (BCN): 2.6
- LHR – Madrid (MAD): 2.6
- LHR – Amsterdam (AMS): 2.7

**12-Month Trends:**
- Overall rating improved from approximately 2.9 to 3.3 (+0.4).
- Recommendation rate increased by 5.2 percentage points.

---

## 📈 Key Insights

- **Drivers of Satisfaction:**  
  - Key factors correlating with recommendation rates: **seat comfort** (≈ 0.52), **cabin staff service** (≈ 0.57), and **value for money** (≈ 0.49).
  - Entertainment and food/beverages play a weaker but still visible role in overall experience.

- **Positive Themes:**  
  - Passengers praised punctuality on short-haul routes, attentive cabin crews on well-staffed flights, and newer interiors on A350/787 aircraft.

- **Areas for Improvement:**  
  - Inconsistent food/catering quality on certain routes.
  - Older cabin products (especially on some aircraft types) need upgrading.
  - Reliability issues with inflight entertainment, particularly on A380s.

---

## ✅ Recommendations

### Short-Term Actions
- Enhance crew service, especially on short-haul and economy flights.
- Address quick fixes for inflight entertainment reliability on older fleet.
- Standardize catering quality, focusing on lower-rated European routes (e.g., Rome, Paris, Barcelona, Madrid).

### Medium-Term Strategies
- Invest in seat comfort improvements in Economy cabins; upgrade older seats with added support where possible.
- Emphasize value-for-money perks in customer communications (e.g., inclusive baggage, transfer protection vs low-cost competitors).

### Ongoing Measurement
- Monitor monthly trends in ratings and recommendation rates for each cabin and route.
- Take proactive action if the 3-month average rating drops by more than 0.3 points or recommendation rate falls more than 5 percentage points.

---

## 📷 Visuals

- **Dashboard Overview**  
  ![Dashboard](https://github.com/mjshubham21/BritishAirways_Tableau_Project/blob/main/images/dashboard.png)

---

## 🛠️ Tools & Technologies

- **Tableau Desktop / Tableau Public** – Data visualization and storytelling.
- **Datasets:** Provided in the `/dataset/` folder of this repository.
- **VS Code & GitHub** – Development environment and version control.

---

## 🚀 How to Use

1. Download or clone this repository.
2. Open the `Airlines_Review_PROJECT.twbx` file in Tableau Desktop or Tableau Public.
3. Use the interactive "Pick a Metric" parameter and filters to explore detailed insights by aspect, date, route, cabin class, and more.

---

## 📌 Future Enhancements

- Add sentiment analysis of review text for deeper qualitative insights.
- Analyze additional airlines for competitive benchmarking.
- Integrate real-time social media feedback and new data sources.

---

**Note:This project is for *educational and portfolio purposes* only.**

---