# Chiral Nanoparticle g-Factor Machine Learning Prediction

This project focuses on predicting the g-factor of chiral nanoparticles using various machine learning models and feature encoding strategies. The repository contains the complete workflow from data preprocessing and feature encoding to model training, validation, and visualization.

## KEncoding Strategies
Three different encoding approaches are implemented and compared:
1.Chemical Encoding (chemical_encoding/): Domain-specific feature representation for chiral nanoparticles using chemical descriptors and properties
2.One-Hot Encoding (onehot_encoding/): Categorical variable encoding for machine learning compatibility, creating binary columns for each category
3.Ordinal Encoding (ordinal_encoding/): Ordered categorical encoding preserving inherent relationships between values
Each encoding folder contains:
A processed_data.csv file with the encoded dataset
A complete analysis workflow in Jupyter notebooks (0-9)
## Installation
1. Create virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # Linux/Mac
.venv\Scripts\activate    # Windows
```

2. Install dependencies:
```bash
pip install numpy pandas scikit-learn matplotlib seaborn Joblib Tqdm
```
or:
```bash
uv add numpy pandas scikit-learn matplotlib seaborn Joblib Tqdm
```

## Project Structure
    ├── raw_data.csv                   # Original dataset (raw data)
    ├── chemical_encoding/             # Chemical feature encoding results and analysis
    │   ├── processed_data.csv         # Processed data after chemical encoding
    │   ├── 0_Dataset_Description.ipynb
    │   ├── 1_Scaling_and_Transforming.ipynb
    │   ├── 2_size_aug_model.ipynb
    │   ├── 3_augmentation.ipynb
    │   ├── 4_g_aug_model.ipynb
    │   ├── 5_Corelation.ipynb
    │   ├── 6_Single_Output.ipynb
    │   ├── 7_k-fold_cross_validation.ipynb
    │   ├── 8_PCA.ipynb
    │   └── 9_Plot.ipynb
    ├── onehot_encoding/               # One-hot encoding results and analysis
    │   ├── processed_data.csv         # Processed data after one-hot encoding
    │   ├── 0_Dataset_Description.ipynb
    │   ├── 1_Scaling_and_Transforming.ipynb
    │   ├── ... (same notebook structure as above)
    │   └── 9_Plot.ipynb
    ├── ordinal_encoding/              # Ordinal encoding results and analysis
    │   ├── processed_data.csv         # Processed data after ordinal encoding
    │   ├── 0_Dataset_Description.ipynb
    │   ├── ... (same notebook structure as above)
    │   └── 9_Plot.ipynb
    └── README.md                      # This file



## Usage
raw_data.csv
    │
    ├── chemical_encoding/ → processed_data.csv → Analysis (0-9 notebooks)
    ├── onehot_encoding/   → processed_data.csv → Analysis (0-9 notebooks)
    └── ordinal_encoding/  → processed_data.csv → Analysis (0-9 notebooks)

