# SOM_Sentinel2_field_scale  

High-resolution field-scale mapping of Soil Organic Matter (SOM) using multi-temporal Sentinel-2 data and machine learning approaches.  


---

## 📂 Repository Structure  
```
SOM_Sentinel2_field_scale/
│
├── scripts/ # R scripts for data processing and modeling
│ ├── 01_feature_selection.R # RF-Embedded feature selection
│ ├── 02_RF_model.R # Random Forest model training & prediction
│ ├── 03_XGBoost_model.R # XGBoost model training & prediction
│ ├── 04_uncertainty_analysis.R # LOOCV-based uncertainty analysis
│ └── 05_SHAP_interpretability.R # SHAP value analysis (interpretability)
│
├── RS_data/ # Remote sensing raw/processed data
│ └── Sentinel2/
│ └── Selected features raster_files
│ └── Selected features + SOM data Excel_fileraster_files
│
└── README.md # Project documentation
```

---

## 🛰 Remote Sensing Data  

- **Sentinel-2 folder**: Multi-temporal optical data  
- **Spectral bands**: Blue, Green, Red, NIR, SWIR  
- **Vegetation indices**: NDVI, SAVI, EVI, etc.  

---

## ⚙️ Requirements  

- **R version**: 4.3.1  
- **Required R packages**:  
  - `ranger`  
  - `xgboost`  
  - `caret`  
  - `terra`  
  - `raster`  
  - `tidyverse`  
  - `fastshap`  

---

## 🚀 Usage  

1. Clone the repository  
2. Install the required R packages.
3. Run scripts in numerical order (01_feature_selection.R → 05_SHAP_interpretability.R).
4. Results (metrics, predictions, maps) will be generated in the respective output directories.

---

## 📖 Citation

Paper under review

---
## 📧 Contact
For questions or collaboration: yassine.bouslihim@gmail.com
