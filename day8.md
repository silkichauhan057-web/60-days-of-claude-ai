# Day 8 — Personal Environmental Health Analyzer

## Task
Built a fully interactive HTML dashboard using Claude that analyzes AQI and water-quality data across multiple cities, generates a personal environmental health report, and gives personalized recommendations.

## Data Note (Important)
This session's environment did **not** have live web-search access, so I could not pull real-time AQI/water-quality data automatically. Instead, Claude used a **representative, illustrative dataset** of 12 major Indian cities (Delhi, Mumbai, Bengaluru, Chennai, Kolkata, Hyderabad, Pune, Ahmedabad, Jaipur, Lucknow, Patna, Shimla) with directionally realistic values. The dashboard clearly discloses this in a header badge and footer note, and points to live sources:
- CPCB National Air Quality Index — app.cpcb.gov.in
- AQICN — aqicn.org
- IQAir — iqair.com

**Selected city for personal analysis:** Delhi

## What the Dashboard Includes
- **Key Metrics:** Average AQI, highest/lowest AQI city, cities analyzed, personal environmental health score
- **Breathing AQI Gauge:** Animated radial gauge that pulses faster for worse air quality (signature visual element)
- **Charts:** AQI comparison, city ranking (best→worst), PM2.5 comparison, PM10 comparison, AQI distribution donut — all Chart.js powered and filter-responsive
- **Interactive Filters:** AQI range slider, pollutant selector (AQI/PM2.5/PM10), health-risk category chips, comparison mode (select up to 3 cities)
- **City Detail Cards:** Click any card to set it as your analyzed city — shows AQI, PM2.5, PM10, category badge, water score, health score
- **Environmental Health Analysis:** Dynamic, per-city breakdown of air quality impact (lungs, sleep, energy, exercise, long-term health) and water quality impact (hair fall, dryness, scalp, skin dryness, acne, sensitivity) — each with 🟢🟡🔴 risk tags
- **Personal Report Card:** 0-100 overall score with Air/Water/Hair/Skin grades (A-F)
- **Insights Panel:** Top 3 cleanest/most polluted cities, biggest anomaly, most surprising observation
- **Personalized Recommendations:** Tabbed sections for daily actions, indoor air, outdoor activity, hair care, skin care, water-quality improvement — all adapt automatically to the selected city's severity level

## Analysis Results (from the dataset used)
- **Average AQI:** 190 (Poor)
- **Most polluted city:** Patna (AQI 345)
- **Cleanest city:** Shimla (AQI 42)
- **Cities analyzed:** 12
- **Biggest anomaly:** Kolkata and Ahmedabad show similar AQI (~215-224) despite very different geography — suggesting local industrial/traffic sources matter more than regional climate.
- **Most surprising observation:** Shimla's AQI is ~8x lower than Patna's despite both being in North India — altitude and lower vehicle density make a dramatic difference.

## Screenshots
- [ ] Add screenshot of hero section (breathing gauge + metrics)
- [ ] Add screenshot of charts section
- [ ] Add screenshot of city cards + filters in action
- [ ] Add screenshot of health analysis + report card
- [ ] Add screenshot of recommendations tabs

## Files in This Folder
- `index.html` — the complete, self-contained interactive dashboard (open directly in any browser)
- `day8.md` — this documentation file

## Key Learnings
- Without live data access, transparency matters most — clearly labeling data as "representative/illustrative" (rather than presenting it as real-time) keeps the tool honest and still useful as a demo.
- Tying visual design to the subject matter (a "breathing" gauge that pulses faster for worse air) makes a dashboard memorable, not just functional.
- Deriving all downstream values (grades, risk tags, recommendations) from a small set of core numbers (AQI, PM2.5, PM10, water score) keeps the dashboard consistent and easy to extend to more cities later.
- Interactive filters + click-to-select city cards make a single dashboard feel personalized without needing separate pages per city.
- A single self-contained HTML file (no build step, all CSS/JS inline, charts via CDN) is the easiest possible format to share, screenshot, and upload to GitHub.
