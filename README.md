# SNR_power

## **Sample Size vs. SNR in Multivariable Regression**

This repository contains Python code to simulate and visualize the relationship between **signal-to-noise ratio (SNR)**, **sample size**, and **statistical power** in the context of multivariable regression. The code is particularly useful for understanding how noise in data affects the required sample size to achieve a specified power level, which is critical for designing genetic studies and other research involving complex datasets.

---

## **Key Features**
- **Power Analysis**: Calculates the required sample size for a given SNR, power level, and significance threshold using the `statsmodels` library.
- **Visualization**: Plots the relationship between SNR and required sample size for different power levels (e.g., 0.4, 0.6, 0.8, 0.99) on a log scale.
- **Smoothing**: Uses cubic spline interpolation to generate smooth curves, avoiding abrupt jumps caused by numerical instabilities.
- **Customizable Inputs**: Allows users to specify SNR range, power levels, and significance thresholds.

---

## **Use Cases**
- **Psychiatric Genetics**: Understand how noise in phenotypic or genotypic data impacts the sample size needed to detect genetic associations.
- **Experimental Design**: Plan studies by estimating the required sample size for a given effect size and desired statistical power.
- **Data Quality Assessment**: Evaluate the impact of data quality (noise level) on study feasibility and power.

---

## **Code Overview**
- **`calculate_sample_size`**: Computes the required sample size for a given SNR, power, and significance level.
- **Spline Interpolation**: Smooths the curve to eliminate numerical artifacts, especially for high power levels.
- **Plotting**: Visualizes the relationship between SNR and sample size for multiple power levels.

---

## **Usage**
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/sample-size-snr.git
   cd sample-size-snr
   ```
2. Install dependencies:
   ```bash
   pip install numpy matplotlib statsmodels scipy
   ```
3. Run the script:
   ```bash
   python sample_size_vs_snr.py
   ```
4. Customize the inputs (e.g., SNR range, power levels) in the script to suit your needs.

---

## **Example Output**
The script generates a plot showing the required sample size (y-axis, log scale) against the signal-to-noise ratio (x-axis) for different power levels. The plot highlights how noise in the data dramatically increases the sample size needed to achieve a desired power level.

---

## **Dependencies**
- Python 3.x
- `numpy`
- `matplotlib`
- `statsmodels`
- `scipy`

---

## **Contributing**
Contributions are welcome! If you have suggestions for improvements or new features, please open an issue or submit a pull request.

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Acknowledgments**
- The code leverages the `statsmodels` library for power analysis.

---
