# A-pipeline-to-enhance-animal-vehicle-collision-analysis-in-crash-report-dataset

This repository contains the code and resources for the research paper:

**"A Pipeline to Enhance Animal Vehicle Collision Analysis in Crash Report Dataset"**  
Authors: Boshra Besharatian, Sattar Dorafshan  
Department of Civil Engineering, University of North Dakota  

## Overview

This project introduces a comprehensive pipeline for analyzing crash report datasets related to animal-vehicle collisions (AVCs). The pipeline includes steps for:

1. **Data Cleaning**: Removing outliers, duplicates, irrelevant features, and addressing missing values.
2. **Data Quality Control**: Ensuring temporal and spatial consistency within the dataset.
3. **Feature Selection**: Identifying statistically significant features using variance thresholds, Theil's U association index, and Chi-square tests.
4. **Contributing Factor Analysis**: Highlighting features crucial for predictive modeling.

The pipeline was applied to North Dakota crash report data, improving dataset integrity, runtime efficiency, and predictive analysis reliability.

---

## Features

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
├── code/                  # Contains the Python code for the pipeline
├── data/                  # Sample data (optional; anonymized if included)
├── figures/               # Visualizations and figures from the analysis
├── README.md              # Project overview (this file)
└── LICENSE                # Licensing information
```

---

## Requirements

### Python Packages

The following Python packages are required to run the pipeline:

- `pandas`
- `numpy`
- `tqdm`
- `matplotlib`
- `sklearn` (scikit-learn)
- `dython`
- `openpyxl`

Install them using:

```bash
pip install pandas numpy tqdm matplotlib scikit-learn dython openpyxl
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

The dataset used in this study includes crash reports from North Dakota (2005–2023). Ensure that your dataset aligns with the preprocessing requirements outlined in the code.

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

## License

This project is licensed under the [MIT License](LICENSE).
