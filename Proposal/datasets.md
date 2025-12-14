# Dataset Notes for Research Task 9: Pothole Risk

## Primary Dataset:
- **311 Service Requests (Cityline)**
  - URL: https://data.syr.gov/dataset/Cityline-Service-Requests
  - Use: Filter by Category = "Pothole"
  - Fields: request_type, request_date, lat, lng, status, response_time
  - Frequency: Updated monthly

## Optional Enrichment:
- Snow removal or plow data (if available)
- Weather overlays from NOAA (via API)
- Syracuse neighborhood boundary files (GeoJSON)