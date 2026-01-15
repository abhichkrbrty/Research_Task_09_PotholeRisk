# 🔁 Proposal Update – Phase 2 Data Strategy

## Why the update?
The original proposal aimed to use recent 311 complaint data for potholes in Syracuse. However, real-time complaint data was not accessible in the expected format from data.syr.gov.

## New Plan:
We pivoted to using the following verified public datasets:
- Potholes Filled (2018) — acts as our “label” dataset
- Road Ratings (2015 and 2017) — infrastructure condition before/after
- Water Main Breaks (2004–2019) — aging infrastructure risk proxy

This new approach allows us to:
- Train a supervised classification model to predict pothole risk
- Use structured ground-truth data instead of unstructured complaint logs
- Deliver more actionable insights to the city based on validated repairs

## Impact on Deliverables:
No change. The end goal remains an interactive predictive risk map for potholes in Syracuse, trained on multiple civic infrastructure layers.

This pivot strengthens the technical integrity and makes the model easier to validate and explain to city officials.