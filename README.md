# social-media-dashboard

# Social Media Performance Dashboard (LinkedIn)

## Overview
This project analyzes LinkedIn post performance to understand what drives reach, engagement, and virality. The dashboard is designed for decision-makers to quickly identify the best-performing content formats, topics, and posting times.

---

## Dataset
**Table:** social_media_performance  
**Columns:**
- post_id
- content_type
- topic
- language
- region
- post_datetime
- hashtags
- sentiment_score
- views
- likes
- comments
- shares
- engagement_rate (recalculated in DAX)
- is_viral

---

## Tools Used
- **Power BI Desktop**
- **Power Query** (data cleaning & feature extraction)
- **DAX** (measures and KPIs)
- **GitHub** (project hosting)

---

## Data Preparation (Power Query)
- Corrected data types (date/time, numeric fields)
- Removed unnecessary fields (single platform)
- Created time intelligence columns from `post_datetime`:
  - Year, Month, Month Name, Day Name, Hour
- Created `total_engagement` (likes + comments + shares)

---

## Key Measures (DAX)
- **Total Views**
- **Total Engagement**
- **Engagement Rate** = Total Engagement / Total Views
- **Total Posts**
- **Viral Rate** (share of posts marked viral)

---

## Key Insights
- **Video dominates reach and volume**, generating the highest total views and total engagement.
- **Feed posts are the most efficient**, delivering the highest engagement rate.
- **Posting time matters:** engagement peaks around **20:00 (8 PM)**.
- **Viral posts outperform non-viral posts** significantly in total engagement.
- **Topics drive performance:** **Entertainment** leads in average engagement, while **Entertainment and Sports** show top viral potential.

---

## Recommendations
- Use **Video** content for maximum reach and awareness.
- Focus content strategy around **Entertainment** and **Sports** themes.
- Build a balanced content mix: **Video for scale** + **Feed for efficiency/virality**.

---

## Files
- `*.pbix` — Power BI dashboard file (download and open in Power BI Desktop)
- Screenshots — preview of dashboard pages for quick viewing

---

## How to View
GitHub cannot preview `.pbix` files directly.
1. Download the `.pbix` file from this repository
2. Open using **Power BI Desktop**
