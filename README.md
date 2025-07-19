# Rock vs Mine Prediction using Logistic Regression

This project demonstrates a machine learning model built using **Logistic Regression** to classify sonar signals as either a "Rock" or a "Mine". The dataset used contains 60 features representing the sonar signal and a target variable indicating whether the object is a rock or a mine.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Model Performance](#model-performance)
- [Contributing](#contributing)

---

## Project Overview

The goal of this project is to accurately distinguish between rocks and mines based on sonar data. A **Logistic Regression** model is trained on a pre-processed dataset, and its performance is evaluated using accuracy scores on both training and test sets. The project also includes a simple predictive system to demonstrate how the trained model can be used to classify new, unseen data.

---

## Dataset

The dataset, `sonar.csv`, consists of 208 entries, each with 60 numerical features and a target label.

- **Features (Columns 0-59):** These represent various characteristics extracted from the sonar signals.
- **Target (Column 60):** This column contains the labels `'R'` (Rock) or `'M'` (Mine).

### Data Distribution

- **Mines (M):** 111 instances  
- **Rocks (R):** 97 instances

---

## Dependencies

To run this notebook, you will need the following Python libraries:

- `numpy`
- `pandas`
- `scikit-learn`

Install them using pip:

```bash
pip install numpy pandas scikit-learn
