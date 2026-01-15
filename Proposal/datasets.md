# 📦 Datasets Used – Syracuse Pothole Risk Project

This document describes all raw datasets used in this project and how they contribute to the pothole risk prediction model.

---

## 1. Potholes Filled (2018)
- **Source**: https://data.syr.gov/dataset/77e2864358274649bda42b059028029d_0
- **Downloaded**: Jan 1, 2026
- **Fields**: `date_fixed`, `latitude`, `longitude`, `address`, `repair_type`
- **Use**: Primary label source — locations where potholes were actually filled (positive cases)

---

## 2. Road Ratings (2015)
- **Source**: https://data.syr.gov/dataset/road-ratings-2015
- **Fields**: `segment_id`, `street_name`, `overall_score`, `geometry`
- **Use**: Infrastructure quality snapshot (pre-pothole). Used as model feature.

---

## 3. Road Ratings (2017)
- **Source**: https://data.syr.gov/dataset/road-ratings-2017
- **Fields**: Same as 2015
- **Use**: Detect changes/improvements in infrastructure over time. Feature engineering: score delta.

---

## 4. Water Main Breaks (2004–2019)
- **Source**: https://data.syr.gov/dataset/water-main-breaks
- **Fields**: `break_date`, `latitude`, `longitude`, `location_desc`
- **Use**: Environmental risk proxy — higher break frequency may indicate aging infrastructure = pothole risk.

---

## Notes:
- All datasets downloaded manually and stored in `data/raw/`
- Initial processing and joins will be done in `notebooks/01_eda_pothole_prediction.ipynb`