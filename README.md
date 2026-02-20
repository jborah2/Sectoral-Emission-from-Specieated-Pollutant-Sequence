# Sectoral-Emission-from-Specieated-Pollutant-Sequence

# STL–ML Hybrid Time-Series Prediction Framework

## Overview
This repository implements a hybrid STL decomposition + machine learning framework for time-series forecasting.

The framework:
- Performs STL decomposition (Trend, Seasonal, Residual)
- Builds lag & rolling features
- Uses component-specific model banks (LGBM, XGBoost, RF)
- Applies strict temporal holdout validation
- Recombines component predictions
- Exports final and component-level predictions

## Features
- Sheet selection from Excel
- Timestamp recovery in outputs
- Strict end-of-series test holdout
- Configurable test length
- NaN-safe metric computation
- Component-level prediction export

## Methodology

1. STL decomposition
2. Feature engineering (lags + rolling stats)
3. Component-wise model training
4. Ensemble weighting
5. Recombination of STL components
6. Evaluation on unseen temporal horizon

## Usage

Edit in `main.py`:
