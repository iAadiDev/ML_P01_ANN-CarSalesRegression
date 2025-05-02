# Car Purchase Amount Predictions Using ANNs

## About

This repository contains a machine learning project that uses an Artificial Neural Network (ANN) to predict the dollar amount customers will spend on car purchases based on their demographic and financial attributes. Built with Python, Pandas, scikit-learn, and TensorFlow/Keras, the model learns from historical customer data (age, annual salary, credit card debt, net worth) to perform a regression task and estimate purchase amounts.

> **Tech Stack:** Python 3.x, Jupyter Notebook, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, TensorFlow & Keras.

## Table of Contents

* [Project Structure](#project-structure)
* [Prerequisites](#prerequisites)
* [Setup](#setup)

  * [Clone the Repository](#clone-the-repository)
  * [Create a Virtual Environment](#create-a-virtual-environment)
  * [Activate the Virtual Environment](#activate-the-virtual-environment)
  * [Install Dependencies](#install-dependencies)
* [Data](#data)
* [Running the Project](#running-the-project)
* [Results & Visualization](#results--visualization)
* [Contributing](#contributing)
* [License](#license)

## Project Structure

```
ML_P01_ANN-CarSalesRegression/
├── Car_Purchasing_Data.csv      # Dataset: customer attributes & purchase amount
├── P1 - Car Purchase Amount Predictions Using ANNs.ipynb  # Jupyter notebook with end-to-end code
├── requirements.txt             # Python dependencies
└── .ipynb_checkpoints/          # Jupyter notebook checkpoints
```

## Prerequisites

* Python 3.8 or higher
* Git
* (Optional) Anaconda or Miniconda

## Setup

### Clone the Repository

```bash
git clone https://github.com/<iAadiDev>/ML_P01_ANN-CarSalesRegression.git
cd ML_P01_ANN-CarSalesRegression
```

### Create a Virtual Environment

Using `venv` (built‑in):

```bash
python3 -m venv venv
```

Or using Conda:

```bash
conda create --name ann-car-sales python=3.9
```

### Activate the Virtual Environment

* On macOS/Linux:

  ```bash
  source venv/bin/activate
  ```
* On Windows:

  ```powershell
  venv\\Scripts\\activate
  ```
* For Conda:

  ```bash
  conda activate ann-car-sales
  ```

### Install Dependencies

Make sure you have a `requirements.txt` file in the root. If not, create one with the following:

```
pandas
numpy
matplotlib
seaborn
scikit-learn
tensorflow
keras
jupyter
```

Then install:

```bash
pip install -r requirements.txt
```

## Data

The dataset `Car_Purchasing_Data.csv` contains the following columns:

* **Customer Name**, **Customer e-mail**, **Country** (dropped during preprocessing)
* **Gender**, **Age**, **Annual Salary**, **Credit Card Debt**, **Net Worth**
* **Car Purchase Amount** (target variable)

Place the CSV file in the project root (it is already included in this repo).

## Running the Project

1. Launch Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
2. Open `P1 - Car Purchase Amount Predictions Using ANNs.ipynb`.
3. Follow the notebook cells in order:

   * **Step 0:** Import libraries
   * **Step 1:** Load and inspect data
   * **Step 2:** Data preprocessing (drop unused columns, scaling)
   * **Step 3:** Train/test split
   * **Step 4:** Build and compile the ANN model
   * **Step 5:** Train the model and monitor loss
   * **Step 6:** Evaluate performance and make predictions

## Results & Visualization

<!-- TODO: Add plots of training vs. validation loss -->

![Loss Curve](images/loss_curve_placeholder.png)

<!-- TODO: Add scatter plot of actual vs. predicted purchase amounts -->

![Actual vs Predicted](images/actual_vs_predicted_placeholder.png)

## Contributing

1. Fork this repository.
2. Create a new branch: `git checkout -b feature/YourFeatureName`
3. Make your changes and commit: `git commit -m "Add some feature"`
4. Push to your branch: `git push origin feature/YourFeatureName`
5. Open a Pull Request on the original repo.

Please ensure code is well-documented and follows PEP8 style.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
