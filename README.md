# Arsenic Contamination Detection in Water Distribution Networks

## Project Overview

This project presents a machine learning-based approach for detecting arsenic contamination in a water distribution network using only **flow** and **chlorine** sensor measurements. Since direct arsenic sensors are expensive and are not commonly installed, the proposed method uses existing sensor data to identify contamination events.

The **Hanoi Water Distribution Network** was simulated using **EPANET-MSX** through the **EPYT-Flow** framework. A total of **100 random arsenic contamination scenarios** were generated to create the dataset. A **Random Forest** classifier was trained using sliding time windows to detect contamination events.

---

## Features

* Hanoi Water Distribution Network simulation
* EPANET-MSX water quality simulation
* EPYT-Flow framework
* 100 randomly generated arsenic contamination scenarios
* Sliding time window approach (4, 8, 12, and 24)
* Random Forest classifier
* Performance evaluation using:

  * Accuracy
  * Precision
  * Recall
  * F1 Score
* Analysis based on contamination size
* Analysis based on injection location

---

## Technologies Used

* Python
* JupyterLab
* EPANET-MSX
* EPYT-Flow
* Scikit-learn
* NumPy
* Pandas
* Matplotlib

---

## Project Workflow

1. Simulate the Hanoi Water Distribution Network.
2. Generate 100 random arsenic contamination scenarios.
3. Collect flow and chlorine sensor measurements.
4. Generate the dataset.
5. Apply sliding time windows.
6. Train a Random Forest classifier.
7. Evaluate model performance.

---

## Results

The model was evaluated using four sliding window sizes (4, 8, 12, and 24). The best performance was achieved with the **24-sample sliding window**.

| Metric    |      Value |
| --------- | ---------: |
| Accuracy  | **98.12%** |
| Precision | **96.55%** |
| Recall    | **80.87%** |
| F1 Score  | **88.02%** |

The model was also evaluated for different contamination sizes and injection locations, demonstrating reliable performance under different contamination conditions.

---

## Repository Structure

```text
.
├── Arsenic_Contamination_Detection
├── Hanoi.inp
├── chlorine_arsenic.msx
├── README.md
├── data
├── notebooks
└── results/
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Hamzanaeem00/Arsenic-Contamination-Detection.git
```


Open the notebook:

```bash
jupyter lab
```

or

```bash
jupyter notebook
```

Run the notebook to reproduce the experiments.

---

## References

* Rossman, L. A. *EPANET 2 Users Manual*, U.S. Environmental Protection Agency, 2000.
* Artelt, A., et al. *EPyT-Flow: A Toolkit for Generating Water Distribution Network Data*, Journal of Open Source Software, 2024.
* Breiman, L. *Random Forests*, Machine Learning, 2001.
* Lučin, I., et al. *Machine-learning Classification of a Number of Contaminant Sources in an Urban Water Network*, Sensors, 2021.

---

## Author

**Hamza Naeem**

Master's Student – AI Engineer
