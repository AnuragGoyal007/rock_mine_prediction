# Rock vs Mine Prediction using Logistic Regression

This project demonstrates a machine learning model built using Logistic Regression to classify sonar signals as either a "Rock" or a "Mine". The dataset used contains 60 features representing the sonar signal and a target variable indicating whether the object is a rock or a mine.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Dependencies](#dependencies)
- [Project Structure](#project-structure)
- [How to Run](#how-to-run)
- [Model Performance](#model-performance)
- [Contributing](#contributing)

## Project Overview

The goal of this project is to accurately distinguish between rocks and mines based on sonar data. A Logistic Regression model is trained on a pre-processed dataset, and its performance is evaluated using accuracy scores on both training and test sets. The project also includes a simple predictive system to demonstrate how the trained model can be used to classify new, unseen data.

## Dataset

The dataset, `sonar.csv`, consists of 208 entries, each with 60 numerical features and a target label.

- **Features (Columns 0-59):** These represent various characteristics extracted from the sonar signals.
- **Target (Column 60):** This column contains the labels 'R' (Rock) or 'M' (Mine).

### Data Distribution

- Mines (M): 111 instances
- Rocks (R): 97 instances

## Dependencies

To run this notebook, you will need the following Python libraries:

- `numpy`
- `pandas`
- `scikit-learn`

You can install them using pip:

```bash
pip install numpy pandas scikit-learn
```

## Project Structure

- `Rock vs Mine Prediction.ipynb`: The main Jupyter Notebook containing the data loading, preprocessing, model training, evaluation, and prediction logic.
- `sonar.csv`: The dataset used for training and testing the model.

## How to Run

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AnuragGoyal007/rock_mine_prediction
   cd rock_mine_prediction
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   Alternatively, install them manually as listed in the [Dependencies](#dependencies) section.

3. **Open the Jupyter Notebook:**
   ```bash
   jupyter notebook "Rock vs Mine Prediction.ipynb"
   ```

4. **Run all cells** in the notebook to see the data processing, model training, and evaluation results.

## Model Performance

The Logistic Regression model achieved the following accuracy scores:

- **Accuracy on Training Data:** ~83.42%
- **Accuracy on Test Data:** ~76.19%

## Contributing

Feel free to fork this repository, make improvements, and submit pull requests. Any contributions are welcome!