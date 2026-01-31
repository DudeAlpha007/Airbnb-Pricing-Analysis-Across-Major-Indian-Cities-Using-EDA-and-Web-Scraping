# Airbnb Pricing Analysis Across Indian Metro Cities  
### Web Scraping • Exploratory Data Analysis • Hypothesis Testing • Business Insights

---

## 📌 Project Overview

Airbnb pricing often appears inconsistent and confusing to users. Listings with similar size, amenities, and ratings can differ drastically in price — even within the same city.

This project aims to **decode Airbnb pricing behavior across major Indian metro cities** using:
- Web-scraped real-world Airbnb data
- Structured Exploratory Data Analysis (EDA)
- Statistical hypothesis testing
- Business-oriented interpretation

The analysis focuses on answering **whether price differences are driven by location, timing, amenities, capacity, or trust signals**, and how users can make better booking decisions.

---

## 🎯 Problem Context

A working professional planning a short stay in cities like Mumbai or Hyderabad faces:
- Hundreds of Airbnb listings
- Large price variation for seemingly similar properties
- No clear explanation of what actually drives price

At the same time, hosts struggle with:
- Competitive pricing
- Understanding which features genuinely increase value

This project addresses **both guest and host perspectives**.

---

## ❓ Business Questions

- Is paying more on Airbnb actually worth it?
- Does location significantly impact pricing?
- Do weekends always cost more than weekdays?
- Do amenities and capacity justify higher prices?
- Are ratings and reviews strong pricing signals?
- How is the Airbnb market segmented?

---

## 📂 Dataset Description

- **Source:** Airbnb website (web scraped)
- **Cities Covered:**  
  - Bangalore  
  - Delhi  
  - Hyderabad  
  - Mumbai
- **Total Records:** 2,144 listings
- **Date Types:**  
  - Weekday (5-day stay normalized to per-night)  
  - Weekend (1-night stay)

### Key Columns
- `city`
- `date_type`
- `property_type`
- `price_per_night`
- `price_per_night_normalized`
- `amenities_count`
- `max_guests`
- `overall_rating`
- `review_count`
- Various pricing and data-quality flags

---

## 🛠️ Data Preprocessing

- Converted multi-day weekday prices into **normalized per-night prices**
- Handled structurally missing values (ratings, reviews)
- Identified and flagged:
  - Price outliers
  - High-amenity low-capacity listings
- Ensured **fair comparison between weekend and weekday prices**

---

## 📊 Exploratory Data Analysis (EDA)

### Univariate Analysis
- Price distribution (normalized)
- Right-skewed pricing with luxury outliers
- Median prices better represent typical bookings

### Bivariate Analysis
- Weekend vs Weekday pricing (city-wise)
- City vs Price
- Amenities vs Price
- Capacity vs Price
- Ratings vs Price

### Multivariate Analysis
- City-level market fingerprint using radar charts
- Value-for-money heatmap (amenities × capacity)
- Market segmentation into budget, mid-range, premium, and luxury

---

## 🧪 Hypothesis Testing

| Hypothesis | Test Used | Result |
|----------|---------|--------|
| Weekend vs Weekday Pricing | Two-sample t-test | Significant difference |
| City vs Price | One-way ANOVA | Significant difference |
| Amenities vs Price | Pearson Correlation | Weak but significant |
| Capacity vs Price | Pearson Correlation | Moderate, significant |
| Ratings vs Price | Pearson Correlation | Very weak, significant |

**Key Insight:**  
Statistical significance does not always imply practical importance. Effect sizes were carefully interpreted.

---

## 📈 Key Business Insights

- Airbnb pricing is **not random**
- **Location is the strongest pricing driver**
- Weekend effects are **city-specific**, not universal
- Mean prices are inflated by luxury listings
- Amenities and capacity have **diminishing returns**
- Ratings affect trust, not price
- Airbnb markets are clearly segmented

---

## 💡 Recommendations

### For Guests
- Focus on **median prices**, not averages
- Prefer weekdays when flexible
- Choose capacity based on actual need
- Avoid overpaying for marginal rating differences
- Watch out for over-amenitized, low-capacity listings

### For Hosts
- Apply **city-specific pricing strategies**
- Use competitive pricing for new listings
- Invest in capacity and property type over excess amenities
- Adopt dynamic pricing based on demand timing

---

## ⚠️ Challenges Faced

- Unstructured and inconsistent web data
- Structurally missing ratings and reviews
- Dynamic pricing behavior
- Presence of extreme outliers
- Limited location granularity
- Feature interaction effects
- Gap between statistical and practical significance

---

## 🧠 Conclusion

Airbnb pricing across Indian metro cities is influenced by a **combination of structural, geographic, and demand-based factors**.  
Location dominates pricing decisions, while amenities, ratings, and capacity contribute incrementally.  
Understanding these dynamics enables **better decision-making for both guests and hosts**.


