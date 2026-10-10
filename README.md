<div align="center">

# 🔋 Machine Learning: Course Materials (2026)

**Lectures, hands-on Jupyter tutorials and battery datasets for an introductory, project-driven machine learning course**

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebooks-F37626?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-F7931E?logo=scikitlearn&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-Neural%20Nets-EE4C2C?logo=pytorch&logoColor=white)

</div>

---

## 📖 About

This repository has all the teaching material for the course: lecture slides, Jupyter notebooks to work through alongside each lecture, setup guides and a set of **lithium-ion battery datasets** for the course project.

The course starts with the Python data stack (NumPy, pandas) and covers **regression, feature engineering, classification, clustering and neural networks**. Students then apply these methods to real battery problems such as estimating **State of Charge (SOC)**, **State of Health (SOH)** and **Remaining Useful Life (RUL)**.

> 💡 **Tip:** GitHub renders every `.ipynb` notebook in the browser. Click a **Colab** badge to run a notebook in the cloud without installing anything.

---

## 🗂️ Table of Contents

- [Getting Started](#-getting-started)
- [Course Modules](#-course-modules)
  - [0. Setup](#0--setup)
  - [1. Kick-off & Python Foundations](#1--kick-off--python-foundations)
  - [2. Classification](#2--classification)
  - [3. Clustering](#3--clustering)
  - [4. Artificial Neural Networks](#4--artificial-neural-networks)
  - [5. Linear Regression, Feature Selection & PCA](#5--linear-regression-feature-selection--pca)
- [Battery Datasets & Project](#-battery-datasets--project)
- [Repository Structure](#-repository-structure)

---

## 🚀 Getting Started

```bash
# 1. Clone the repository
git clone https://github.com/sourasb05/1DT11561204-2026.git
cd 1DT11561204-2026

# 2. (Recommended) create a virtual environment
python -m venv .venv
source .venv/bin/activate          # Windows: .venv\Scripts\activate

# 3. Install the libraries used in the notebooks
pip install numpy pandas matplotlib seaborn scikit-learn torch scipy jupyter

# 4. Launch Jupyter
jupyter notebook
```

New to Jupyter or VS Code? Start with the [setup guides](#0--setup).

---

## 📚 Course Modules

### 0 · Setup

| Resource | Description |
|---|---|
| 📄 [Install Jupyter Notebook Guide](setup/Install_Jupyter_Notebook_Guide.docx) | Step-by-step install of Python and Jupyter Notebook |
| 📄 [VS Code Setup for Jupyter & ML](setup/VS_Code_Setup_Jupyter_ML.docx) | Configure VS Code with the Python and Jupyter extensions for ML work |

---

### 1 · Kick-off & Python Foundations

An overview of the course, the project and the tools, followed by two hands-on tutorials on the core Python data libraries.

| Type | Resource | Description | Run |
|---|---|---|---|
| 🎞️ Lecture | [Kick-off Tutorial](ML-Kickoff/Kick-off-tutorial.pptx) | Course overview, ML workflow, project introduction | |
| 📓 Tutorial | [NumPy Tutorial](Tutorial/numpy_tutotial.ipynb) | Arrays, indexing, broadcasting, linear algebra: the basics for ML | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Tutorial/numpy_tutotial.ipynb) |
| 📓 Tutorial | [pandas Tutorial](Tutorial/pandas_tutorial.ipynb) | DataFrames, selection, cleaning, grouping and aggregation | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Tutorial/pandas_tutorial.ipynb) |

---

### 2 · Classification

Supervised classification on the classic **Iris** dataset: exploring the data, splitting train/test, training models and evaluating them with accuracy, confusion matrices and classification reports.

| Type | Resource | Description | Run |
|---|---|---|---|
| 🎞️ Lecture | [Lecture 2: Classification](Classification/Lecture2_classification.pptx) | Classification concepts, decision boundaries, evaluation metrics | |
| 📓 Tutorial | [Classification Walk-through](Classification/notebooks/Lecture2_classification.ipynb) | End-to-end classification pipeline on Iris | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Classification/notebooks/Lecture2_classification.ipynb) |
| 📓 Tutorial | [k-Nearest Neighbours](Classification/notebooks/KNN%20Classifier.ipynb) | KNN classifier and the effect of *k* | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Classification/notebooks/KNN%20Classifier.ipynb) |
| 📓 Tutorial | [Random Forest](Classification/notebooks/RandomForest%20Classifier.ipynb) | Ensemble of decision trees, feature importance | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Classification/notebooks/RandomForest%20Classifier.ipynb) |

---

### 3 · Clustering

Unsupervised learning: grouping data without labels. The notebook covers **K-means**, **K-means++** and **DBSCAN**, choosing *k* with the elbow method, estimating `eps`/`MinPts`, visualising clusters with PCA and comparing methods with the silhouette score. It uses Iris and an **EV battery charging** dataset.

| Type | Resource | Description | Run |
|---|---|---|---|
| 🎞️ Lecture | [Lecture 3: Clustering](clustering/Lecture-3%20Clustering_new.pptx) | Partitional and density-based clustering, cluster validation | |
| 📓 Tutorial | [Clustering: K-means, K-means++, DBSCAN](clustering/notebooks/Clustering_2025_SB_RUL_EV.ipynb) | Elbow method, silhouette score, DBSCAN tuning, EV battery application | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/clustering/notebooks/Clustering_2025_SB_RUL_EV.ipynb) |

---

### 4 · Artificial Neural Networks

From the perceptron to multi-layer networks. The tutorial builds, trains and evaluates a feed-forward neural network in **PyTorch**, using scikit-learn for preprocessing.

| Type | Resource | Description | Run |
|---|---|---|---|
| 🎞️ Lecture | [Lecture 4: Artificial Neural Networks](neural%20network/Lecture-4-ANN.pptx) | Neurons, activation functions, back-propagation, training | |
| 📓 Tutorial | [ANN with PyTorch](neural%20network/tutorial/Lecture%207%20-%20ANN.ipynb) | Build and train an MLP classifier on Iris | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/neural%20network/tutorial/Lecture%207%20-%20ANN.ipynb) |

---

### 5 · Linear Regression, Feature Selection & PCA

Predicting continuous values and engineering better inputs: linear regression with gradient descent, feature transformation and encoding, feature selection and dimensionality reduction with PCA.

| Type | Resource | Description | Run |
|---|---|---|---|
| 🎞️ Lecture | [Linear Regression & Feature Selection](Feature%20Selection%20and%20regression/linear_regression_feature_selection.pptx) | Regression, loss functions, gradient descent, feature engineering | |
| 📓 Tutorial | [Linear Regression](Feature%20Selection%20and%20regression/Tutorials/Linear_regression.ipynb) | Gradient descent from scratch on the **Auto MPG** dataset, epoch-wise loss | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Feature%20Selection%20and%20regression/Tutorials/Linear_regression.ipynb) |
| 📓 Tutorial | [Feature Transformation](Feature%20Selection%20and%20regression/Tutorials/Feature_transformation.ipynb) | Polynomial features, the household power consumption dataset, categorical encoding | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Feature%20Selection%20and%20regression/Tutorials/Feature_transformation.ipynb) |
| 📓 Tutorial | [Feature Selection](Feature%20Selection%20and%20regression/Tutorials/Feature_selection.ipynb) | How selecting features affects classification and regression performance | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Feature%20Selection%20and%20regression/Tutorials/Feature_selection.ipynb) |
| 📓 Tutorial | [Principal Component Analysis](Feature%20Selection%20and%20regression/Tutorials/PCA.ipynb) | Explained variance and how PCA affects model accuracy | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Feature%20Selection%20and%20regression/Tutorials/PCA.ipynb) |

#### 📌 Recommended material for understanding regression

| Type | Resource | Description |
|---|---|---|
| 📄 Lecture notes | [Modern Regression, Lecture 13 (C. Shalizi, CMU)](https://www.stat.cmu.edu/~cshalizi/mreg/15/lectures/13/lecture-13.pdf) | Lecture notes from Carnegie Mellon's *Modern Regression* course that explain the theory behind linear regression in depth |
| 🎥 Video playlist | [Regression video series (YouTube)](https://www.youtube.com/playlist?list=PLblh5JKOoLUIzaEkCLIUxQFjPIlapw8nU) | Short visual videos that build intuition for regression step by step |
| 💻 Code example | [Battery State-of-Charge Estimation (GitHub)](https://github.com/sautee/battery-state-of-charge-estimation) | An open-source project that treats battery SOC estimation as a regression problem, a useful reference for the course project |

---

## 🔋 Battery Datasets & Project

The course project applies the methods above to **lithium-ion battery data**. Suggested research questions are in
📄 [Research Questions and Datasets for Battery Technology & Clustering](research%20questions%20/Research%20Questions%20and%20Datasets%20for%20Battery%20Technology%20%26%20Clustering.pdf).

| Resource | Description | Run |
|---|---|---|
| 📄 [Battery Dataset Guide](Baterry%20datasets/battery%20dataset.docx) | Descriptions of each dataset and the applications they suit | |
| 📓 [Battery Data Analysis](Baterry%20datasets/data_analysis.ipynb) | Loading NASA battery data, feature descriptions, transient response and SOH analysis | [![Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/sourasb05/1DT11561204-2026/blob/main/Baterry%20datasets/data_analysis.ipynb) |

> ⚠️ **The raw dataset archives are not stored in this repository.** They are too large for GitHub (about 470 MB in total). Download them from the sources below and put them in the `Baterry datasets/` folder.

### Main datasets

| Dataset | What it contains | Suggested tasks | Download |
|---|---|---|---|
| **NASA PCoE Battery Aging** (`5. Battery Data Set`, ~200 MB) | Run-to-failure cycling of 18650 Li-ion cells: CC-CV charging, several discharge profiles, voltage/current/temperature, reference capacity and EIS impedance | SOH · SOC · RUL | [NASA PCoE Repository](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/) |
| **CALCE Battery Data** (Univ. of Maryland) | Several chemistries (LiCoO₂, LiFePO₄) and form factors; calendar aging and dynamic drive cycles (DST, FUDS) over a range of SOC windows and temperatures | SOH · SOC · RUL | [calce.umd.edu](https://calce.umd.edu/battery-data) |
| **Panasonic 18650PF** (`Panasonic_18650PF.zip`, ~270 MB) | 2.9 Ah cell tested at 25 °C, 10 °C, 0 °C, −10 °C and −20 °C under US06, HWFET, UDDS and LA92 drive cycles scaled to an electric Ford F-150 | SOC estimation | Course Canvas page |
| **NASA Randomized Battery Usage (RW9–RW12)** | Random-walk charge/discharge between −4.5 A and +4.5 A, updated every 5 min, with periodic reference cycles to track health | Dynamic SOC · RUL | [Kaggle](https://www.kaggle.com/datasets/patrickfleith/nasa-randomized-battery-usage-dataset) |

### More datasets to explore

- [Li-S Battery Thermal Failure Dataset (Kaggle)](https://www.kaggle.com/datasets/ziya07/li-s-battery-thermal-failure-dataset)
- [eVTOL Battery Dataset (CMU KiltHub)](https://kilthub.cmu.edu/articles/dataset/eVTOL_Battery_Dataset/14226830)
- [Time-Series Data of a Battery Energy Storage System (IEEE DataPort)](https://ieee-dataport.org/documents/time-series-data-battery-energy-storage-system)
- [Battery dataset on Zenodo (record 7244939)](https://zenodo.org/records/7244939)
- [NASA Randomized & Recommissioned Battery Dataset](https://data.nasa.gov/dataset/randomized-and-recommissioned-battery-dataset/resource/cdea0a46-2c8d-4192-bbe7-8fbebfcfdb31)
- [NREL Battery Failure Databank](https://www.nrel.gov/transportation/battery-failure)

### Other data used in the tutorials

Most tutorials load small datasets straight from scikit-learn (`load_iris`, `load_wine`, `load_diabetes`, `load_digits`) or from a URL. A few expect a local file next to the notebook:

| File | Used in | Source |
|---|---|---|
| `Iris.csv` | Classification, Clustering, ANN | [Kaggle: Iris Species](https://www.kaggle.com/datasets/uciml/iris) |
| `ev_battery_charging_data.csv` | Clustering | Course Canvas page |
| `household_power_consumption.txt` | Feature Transformation | [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption) |
| `CMaps/train_FD001.txt` | Clustering (RUL) | [NASA PCoE Repository: Turbofan Engine Degradation (C-MAPSS)](https://www.nasa.gov/intelligent-systems-division/discovery-and-systems-health/pcoe/pcoe-data-set-repository/) |

---

## 🌳 Repository Structure

```
1DT11561204-2026/
├── setup/                              # Installation guides (Jupyter, VS Code)
├── ML-Kickoff/                         # Course kick-off slides
├── Tutorial/                           # NumPy & pandas tutorials
├── Classification/
│   ├── Lecture2_classification.pptx
│   └── notebooks/                      # Classification walk-through, KNN, Random Forest
├── clustering/
│   ├── Lecture-3 Clustering_new.pptx
│   └── notebooks/                      # K-means, K-means++, DBSCAN
├── neural network/
│   ├── Lecture-4-ANN.pptx
│   └── tutorial/                       # ANN with PyTorch
├── Feature Selection and regression/
│   ├── linear_regression_feature_selection.pptx
│   └── Tutorials/                      # Linear regression, feature transformation/selection, PCA
├── Baterry datasets/                   # Dataset guide + analysis notebook (raw zips excluded)
└── research questions /                # Project research questions (PDF)
```

---

<div align="center">

**Happy learning! 🚀** If you find a mistake or have a question, please open an [issue](https://github.com/sourasb05/1DT11561204-2026/issues).

</div>
