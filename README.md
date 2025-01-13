# Animal-Vehicle Collision (AVC) Analysis Pipeline

This repository contains the code and resources for the research paper:

**"A Pipeline to Enhance Animal Vehicle Collision Analysis in Crash Report Dataset"**  
Authors: Boshra Besharatian, Sattar Dorafshan  
Department of Civil Engineering, University of North Dakota  

## Overview

Animal-vehicle collisions (AVCs) represent a significant challenge globally, leading to road safety concerns, ecological disruptions, and substantial property damage. Police crash reports are a primary data source for studying AVCs, but these datasets are often plagued by inconsistencies, missing information, and poor-quality data due to variations in reporting policies, especially in rural areas. To address these issues, this repository provides a robust pipeline that:

1. **Prepares and Cleans Data**: Outlier detection, duplicate removal, and skewed sample proportion adjustments ensure the dataset’s reliability.
2. **Ensures Data Quality**: Implements temporal and spatial checks to identify inconsistencies stemming from reporting policy changes or other factors.
3. **Selects Features Strategically**: Uses advanced statistical tools like Theil’s U association index, Chi-square tests, and variance thresholding to retain only the most informative features.
4. **Analyzes Contributing Factors**: Identifies and ranks the most significant factors impacting AVCs, such as light conditions, speed limits, and temporal patterns.

This pipeline was applied to crash report data from North Dakota, where AVCs are particularly prevalent due to the region's diverse wildlife and extensive rural road networks. The pipeline achieved:

- A 3.95% reduction in sample size and an 88.9% reduction in feature size.
- Improved runtime efficiency for association analysis by 92.46%.
- Enhanced integrity and spatiotemporal alignment of the dataset, enabling more accurate predictive modeling and analysis.

---

## Pipeline

- **Data Preprocessing**:
  - Outlier detection and removal.
  - Duplicate sample and feature elimination.
  - Handling skewed proportion samples.
  - Imputation of missing values.
- **Statistical Analysis**:
  - Variance Thresholding.
  - Theil’s U Association Index.
  - Chi-Square Tests (Independence, Homogeneity, Goodness-of-fit).
- **Visualization**:
  - Feature correlation heatmaps.
  - Temporal and spatial distribution analysis.
  - Feature importance ranking.
- **Optimized for Predictive Modeling**:
  - Spatiotemporal feature engineering.
  - Identification of high-impact features like light conditions, speed limits, and highways.

---

## Repository Structure

```plaintext
.
├── code/      # Contains the Python code for the pipeline
├── README.md  # Project overview (this file)
```

---

## Usage

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/avc-analysis-pipeline.git
   cd avc-analysis-pipeline
   ```

2. Run the main analysis notebook or script located in the `code/` directory.

3. Adjust file paths and parameters in the code to suit your dataset.

---

## Dataset

The dataset used in this study includes crash reports from North Dakota (2005–2023). These data are provided by the North Dakota Department of Transportation (NDDOT). The authors of this study do not have the right to publish or share the dataset publicly. Any use of similar data must adhere to the terms and conditions set by the NDDOT. Ensure that your dataset aligns with the preprocessing requirements outlined in the code.

---

## Results

- **Reduction in Sample Size**: 3.95% of samples removed.
- **Feature Reduction**: 22% of features dropped.
- **Runtime Improvement**: 92.46% decrease in association analysis runtime.
- **Key Features Identified**: Month, hour, light condition, county, highway, and speed limit.

---

## Citation

If you use this pipeline in your research, please cite:

```plaintext
Boshra Besharatian, Sattar Dorafshan, "A Pipeline to Enhance Animal Vehicle Collision Analysis in Crash Report Dataset", Journal of Safety Research, 2025.
```

---
