# Kodagu Coffee Plantation – Data Science Project

## 1. Project Overview

**Project Name:** Kodagu Coffee Intelligence – A Data-Driven Study of Coffee Plantations

**Geographical Scope:** Kodagu (Coorg), Karnataka, India

**Study Regions:**
1. Madikeri
2. Virajpet
3. Ponnampet
4. Somwarpet
5. Kushalnagar

**Data Approach:** Publicly available datasets only.

### Background

Coffee cultivation is an important agricultural activity in Kodagu. Coffee production is influenced by several factors, including rainfall, temperature, soil conditions, geographical characteristics, cultivation practices and seasonal variations.

Changes in climatic conditions can affect coffee-growing conditions and potentially influence plantation productivity.

This project aims to explore publicly available agricultural, meteorological and satellite data to understand these relationships and develop data-driven insights that could benefit coffee growers.

## 2. Project Objectives

The project has two primary objectives.

**A. Farmer-oriented objective**

- Understand how weather patterns vary across coffee-growing regions.
- Study the relationship between weather conditions and coffee productivity.
- Identify unusual weather patterns that could create risks for coffee cultivation.
- Explore satellite-based indicators of plantation vegetation health.
- Develop insights that could support better plantation management decisions.

**B. Data Science Portfolio objective**

Demonstrate an end-to-end data science project involving:

- Data sourcing and collection.
- Data extraction and integration.
- Data cleaning and preprocessing.
- Exploratory Data Analysis (EDA).
- Feature engineering.
- Statistical analysis.
- Machine Learning.
- Model evaluation.
- Data visualisation.
- Dashboard development and deployment.

## 3. Business Problem

Can publicly available weather, geographical, agricultural and satellite data help us understand coffee-growing conditions and identify patterns that may influence coffee productivity across Kodagu?

The study will initially focus on five taluks and distinguish between Arabica and Robusta wherever the underlying data permits.

## 4. Data Sources

The project will initially explore the following public data sources.

| Data Category | Source | Purpose |
|---|---|---|
| Coffee production and productivity | Coffee Board of India | Historical agricultural statistics |
| Coffee cultivation area | Coffee Board / Government of Karnataka | Planted and bearing area |
| Rainfall | India Meteorological Department (IMD) | Historical rainfall patterns |
| Temperature | NASA POWER | Historical temperature observations |
| Satellite imagery | Copernicus Sentinel-2 | Vegetation and moisture indicators |
| Geographical boundaries | Survey of India | Taluk-level geographical reference |
| Soil characteristics | Government soil databases | Soil characteristics and suitability |

Only data that can be accessed through public sources will be used.

Actual data availability, geographical resolution, historical coverage and licensing will be verified before integration.

## 5. Geographical and Temporal Scope

The initial study will cover the five taluks of Kodagu.

The proposed common study period is 2016–2024, subject to data availability and compatibility across sources.

Different datasets may have different temporal and geographical resolutions.

For example:
- Rainfall may be available at daily and grid-cell levels.
- Temperature may be available at daily and grid-cell levels.
- Satellite observations may be available at individual pixel level.
- Coffee production statistics may only be available at district or grouped regional level.

Data will be aggregated to appropriate geographical and temporal levels without assuming that all sources have identical granularity.

## 6. Proposed Methodology

### Phase 1 – Data Acquisition

- Obtain taluk geographical boundaries.
- Download historical rainfall data.
- Extract historical temperature data.
- Obtain satellite imagery.
- Download historical coffee production and productivity statistics.
- Explore publicly available soil information.

### Phase 2 – Data Preparation

- Inspect individual datasets.
- Understand their structure and data types.
- Handle missing and inconsistent observations.
- Standardise geographical identifiers.
- Align time periods.
- Aggregate daily data into monthly and seasonal datasets.
- Integrate the datasets where geographical and temporal compatibility permits.

### Phase 3 – Exploratory Data Analysis

Explore:
- Rainfall trends across the five taluks.
- Seasonal temperature variations.
- Historical climate patterns.
- Arabica and Robusta cultivation patterns.
- Coffee production and productivity trends.
- Relationships between weather and available productivity statistics.
- Vegetation health indicators and their seasonal changes.

### Phase 4 – Feature Engineering

Potential features include:
- Monthly rainfall.
- Annual rainfall.
- Monsoon rainfall.
- Blossom-season rainfall.
- Number of consecutive dry days.
- Average maximum temperature.
- Average minimum temperature.
- Rainfall deviation from historical averages.
- Vegetation indices such as NDVI and NDMI.

Final features will be selected based on agricultural relevance and data availability.

### Phase 5 – Machine Learning

Potential modelling approaches:

1. Clustering – Group taluks or growing seasons based on similar weather patterns.
2. Anomaly Detection – Identify unusual weather and vegetation patterns.
3. Regression – Estimate coffee productivity if sufficient historical target observations are available.
4. Classification – Classify growing conditions into risk categories if suitable validated labels can be established.

The final algorithms will be selected after EDA and dataset validation.

### Phase 6 – Visualisation and Deployment

Develop an interactive Streamlit dashboard that allows users to:

- Select a taluk.
- Explore historical weather patterns.
- Compare seasonal variations.
- View vegetation indicators.
- Explore coffee production and productivity statistics.
- View model outputs where reliable predictions are possible.

## 7. Dataset Documentation Standards

Every dataset incorporated into the project will have its own documentation.

The following information will be recorded:

| Documentation Field | Description |
|---|---|
| Dataset Name | Name of the dataset |
| Source | Government department / organisation |
| Source URL | Original download or access link |
| Download Date | Date on which the dataset was accessed |
| Data Period | Historical period covered |
| Geographical Coverage | District, taluk, grid or pixel |
| File Format | CSV, Excel, GeoJSON, SHP, TIFF etc. |
| Original Granularity | Daily, monthly, annual etc. |
| Number of Records | Number of observations |
| Number of Variables | Number of columns |
| Missing Values | Missing or unavailable observations |
| Limitations | Known limitations and assumptions |
| Preprocessing | Transformations performed |

### Data Dictionary

Each dataset will have a separate data dictionary documenting:

- Variable name.
- Description.
- Data type.
- Unit of measurement.
- Example value.
- Source.
- Missing-value interpretation.

## 8. Important Project Principles

1. Use genuine, publicly available data.
2. Never fabricate missing observations.
3. Retain original downloaded datasets separately from processed datasets.
4. Document every transformation and assumption.
5. Maintain traceability between source data and final model features.
6. Distinguish correlation from causation.
7. Avoid making individual farm-level predictions using district-level statistics.
8. Validate model performance before presenting predictions.
9. Document the limitations of every model.

## 9. Expected Deliverables

1. Project documentation.
2. Source datasets and data dictionaries.
3. Cleaned and integrated analytical dataset.
4. Exploratory Data Analysis notebooks.
5. Machine learning notebooks.
6. Model evaluation reports.
7. Interactive Streamlit dashboard.
8. Final project presentation and findings.

## 10. Proposed Technology Stack

| Activity | Tools |
|---|---|
| Data collection | Python, APIs, public data portals |
| Data manipulation | Pandas, NumPy |
| Geospatial analysis | GeoPandas, Rasterio |
| Visualisation | Matplotlib, Seaborn, Plotly |
| Machine Learning | Scikit-learn |
| Satellite analysis | Google Earth Engine / Copernicus tools |
| Development | Jupyter Notebook |
| Dashboard | Streamlit |
| Documentation | Markdown, Excel |

---

**Project Status:** Initial planning and data discovery.

**Next Milestone:** Obtain the geographical boundaries of the five Kodagu taluks and begin documenting the first source dataset.

**Note:** This document is a working project charter. The methodology, features and modelling choices will be updated as we verify the actual datasets and discover their limitations.
