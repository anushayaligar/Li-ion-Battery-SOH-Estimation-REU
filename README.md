
# Estimation of State of Health (SoH) of Li-ion Battery

This repository contains my **Research Experience for Undergraduates (REU)** project focused on
estimating the **State of Health (SoH)** of Li-ion batteries for Electric Vehicle (EV) applications.

---

## Problem Statement
State of Health (SoH) is a critical indicator of battery aging and performance, but it is **not directly measurable**
from experimental data. The available datasets contain only **voltage, current, time, and temperature**
measurements. The challenge was to estimate SoH **indirectly** using a data-driven approach.

---

## Methodology
The project follows a structured, step-by-step workflow:

1. Imported HPPC battery datasets under different operating conditions into MATLAB  
2. Performed data cleaning and normalization to improve consistency and stability  
3. Extracted internal battery parameters (R0, R1, R2, C1, C2) using an **Equivalent Circuit Model (ECM)**  
4. Calculated State of Health (SoH) using resistance-based mathematical formulations  
5. Developed and trained a **Backpropagation Feedforward Neural Network**  
6. Evaluated model performance using training convergence and prediction accuracy analysis  

---

## Neural Network Modeling
- Three neural network models were implemented with increasing input complexity:
  - Model 1: R0-based inputs  
  - Model 2: R0 + R1-based inputs  
  - Model 3: R0 + R1 + R2-based inputs  
- Training was performed for **500 epochs**
- **Mean Squared Error (MSE)** was used as the performance metric

---

## Results
The detailed results, including:
- Training convergence plots  
- Actual vs predicted SoH comparisons  
- Impact of input parameters on prediction accuracy  

are documented in the **REU_Report.pdf** available in the `Results/` section.

The results demonstrate stable convergence, close alignment between predicted and calculated SoH values,
and improved accuracy with richer parameter inputs.

---

## Tools & Technologies
- MATLAB  
- Neural Network Toolbox  
- Excel (HPPC datasets)

---

## Conclusion
This project demonstrates that combining **ECM-based feature extraction** with
**neural network modeling** provides an effective and reliable approach for estimating
the State of Health of Li-ion batteries under varying operating conditions.

---

## Repository Structure
- `Data/` – HPPC experimental datasets  
- `MATLAB_Code/` – MATLAB scripts and models  
- `Results/` – Project report and result summary  
- `PPT_and_Report/` – Project presentation files  

---

## Acknowledgment
The datasets used in this project were sourced from publicly available battery datasets
provided for academic and research purposes.

