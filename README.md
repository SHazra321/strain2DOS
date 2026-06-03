# strain2DOS
## Machine Learning Assisted Reconstruction of Local Electronic Structure of Non-Uniformly Strained MoS₂

**Paper**: arXiv:2603.29298 | DOI: [10.48550/arXiv.2603.29298](https://doi.org/10.48550/arXiv.2603.29298)

## Overview

This repository contains code and datasets for reproducing the results from our paper on Machine Learning assisted reconstruction of local electronic structure of Non-Uniformly Strained MoS2.

## What's Included

- **1 Jupyter Notebooks**:
  - `/Training_Prediction_DOS.ipynb` — Train and prediction by the neural network model on DFT data
  - `/PostProcessing_DOS_map.ipynb` — Prediction from the trained model
- **2 Dataset Files**:
  - `data/training_data.csv` — Training dataset (strain maps + band gap from DFT)
  - `data/test_data.csv` — Test dataset for validation
- **Dependencies**: `requirements.txt` — Python packages needed

## How to Download All Files

### Option 1: Download as ZIP (Recommended)

1. Click the green **`Code`** button at the top right of this page
2. Select **`Download ZIP`**
3. Extract the ZIP file to your computer

### Option 2: Download Individual Files

Click each file below to download:

- [train_model.ipynb](notebooks/train_model.ipynb)
- [evaluate_model.ipynb](notebooks/evaluate_model.ipynb)
- [training_data.csv](data/training_data.csv)
- [test_data.csv](data/test_data.csv)
- [requirements.txt](requirements.txt)

## Setup Instructions

### Step 1: Install Python

Make sure you have **Python 3.8 or higher** installed. Check by running:

```bash
python --version
```

### Step 2: Install Required Packages

Open a terminal/command prompt in the extracted folder and run:

```bash
pip install -r requirements.txt
```

### Step 3: Install Jupyter (if not already installed)

```bash
pip install jupyter
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

This will open Jupyter in your web browser. Navigate to the `notebooks/` folder and open `train_model.ipynb`.

## Running the Code

1. **Open `train_model.ipynb`**
2. Click **`Kernel` → `Restart & Run All`** (or press `Ctrl+Shift+Enter`)
3. Wait for training to complete (approximately 10–30 minutes depending on your system)
4. **Open `evaluate_model.ipynb`**
5. Run all cells to see test results and validation plots

## Expected Output

After running the notebooks, you should see:

- Training loss curves
- Band gap prediction plots
- Spatial band gap reconstruction maps
- Comparison with experimental PL data

## System Requirements

| Requirement | Minimum |
|-------------|---------|
| Python | 3.8+ |
| RAM | 8 GB |
| CPU | Multi-core recommended |
| GPU | Optional (for faster training) |

## Dependencies
