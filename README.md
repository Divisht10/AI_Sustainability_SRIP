# AI for Sustainability: Delhi Airshed Land-Use analysis (SRIP 2026)

**Author:** Divisht 
---

## Project Overview
This repository contains a complete Earth Observation data pipeline commissioned for the Ministry of Environment. The goal is to audit the Delhi Airshed to identify land-use patterns using Sentinel-2 RGB satellite imagery and ESA WorldCover 2021 raster data.

The pipeline handles data filtering from .geojson files, label extraction from raster files, and trains a CNN model (based on cpu usage) to classify land-use categories.

## 📁 Repository Structure
```text
├── data/
│   ├── rgb/                     # Sentinel-2 128x128 image patches (.png)
│   ├── land_cover.tif           # ESA WorldCover 2021 raster
│   └── delhi_ncr_region.geojson # .geojson files
│   └── delhi_airshed.geojson     
├── notebooks/
│   ├── q1_spatial.ipynb         # Q1: Spatial Reasoning & Data Filtering
│   ├── q2_labels.ipynb          # Q2: Label Construction & Data Splits
│   └── q3_model.ipynb           # Q3: CNN Training & Evaluation
├── train_data.csv               # Generated training split (60%)
├── test_data.csv                # Generated testing split (40%)
├── requirements.txt             # Python dependencies
└── README.md                    # Project documentation

Note: 
I acknowledge some use of AI and chatgpt.com for this project especially in creating a custom CNN model.
