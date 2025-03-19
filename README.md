## Principal Component Analysis (PCA) on Swiss Banknote Data

## Project Overview
This project applies **Principal Component Analysis (PCA)** to a dataset of Swiss banknotes to analyze variance, identify key features, and distinguish genuine from counterfeit banknotes. The project follows a structured approach that includes data standardization, covariance matrix calculations, eigen decomposition, and principal component interpretation.

## Project Structure
- **Section 1: PCA on Raw Data**
  - Load and visualize the dataset.
  - Compute the mean and variance of each variable.
  - Calculate the covariance matrix and eigenvalues/eigenvectors.
  - Identify principal components and their variance contribution.
  - Scatter plots to visualize separation between genuine and counterfeit banknotes.

- **Section 2: PCA on Scaled Data (Centimeters)**
  - Convert key features to centimeters.
  - Repeat PCA computations and analyze differences from Section 1.
  - Evaluate the impact of unit conversion on variance and principal components.

- **Section 3: PCA on Standardized Data (Normalized Principal Components - NPC)**
  - Standardize variables to have zero mean and unit variance.
  - Compute the correlation matrix instead of the covariance matrix.
  - Analyze eigenvalues, eigenvectors, and their impact on component interpretation.
  - Compare results with previous sections to highlight the effect of normalization.

## Installation
Ensure you have the following dependencies installed before running the project:
```bash
pip install numpy pandas matplotlib
```

## Usage
Run the main script to execute PCA on the dataset:
```bash
python pca_analysis.py
```

## Key Findings
- **Raw Data PCA:** Principal components are heavily influenced by variables with larger scales, such as length and diagonal measurements.
- **Unit Conversion (cm):** Changes variance magnitude but retains data structure.
- **Standardized PCA:** Balances variable contributions, making the analysis independent of original scales.

## Conclusion
PCA is sensitive to data scaling, and standardization ensures that all variables contribute equally. This approach is essential when analyzing datasets with mixed units or varying magnitudes of measurement.
