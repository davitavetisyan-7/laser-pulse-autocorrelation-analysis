# Laser Pulse Autocorrelation Analysis 🔬

A robust Python tool designed for analyzing experimental laser pulse autocorrelation data, performing precise Gaussian curve fitting, and extracting real laser pulse durations ($\tau_p$).

## Features 🚀
- **Automated Data Parsing:** Seamlessly reads autocorrelator export files, skips header metadata, and extracts the target `[Data]` section containing mirror positions and power values.
- **Gaussian Curve Fitting:** Utilizes `scipy.optimize.curve_fit` with optimized initial guesses (`p0`) to fit theoretical Gaussian models to experimental data points.
- **Physical Conversions & Deconvolution:** 
  - Converts stage positionto time delay using the speed of light .
  - Applies Gaussian pulse deconvolution factor  to calculate the true pulse duration[cite: 1].
- **Professional Visualization:** Generates clean, publication-ready plots combining experimental scatter data and fitted theoretical curves using `matplotlib`.

## Requirements 📦
Make sure you have the following Python libraries installed:
```bash
pip install numpy pandas matplotlib scipy
