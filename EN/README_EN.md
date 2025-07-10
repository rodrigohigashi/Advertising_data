
Advertising_data
Logistic Regression Project
Description
This project implements a logistic regression model using a dataset. The goal is to predict the probability of a specific event occurring based on independent variables, using logistic regression techniques. The model was evaluated using metrics such as Accuracy, Precision, Recall, and F1-Score.

Features
Data loading and preparation.
Logistic regression model creation.
Model training with train-test split.
Model evaluation using performance metrics.
Graphical visualizations for result analysis.
Requirements
To run this project, you need to have installed:

Python 3.12.8
Libraries:
pandas
numpy
scikit-learn
scipy
seaborn
matplotlib
Installation
Clone the repository:

git clone https://github.com/your-username/your-repository.git
Create a virtual environment:

python -m venv venv
Activate the virtual environment:

On Windows:

venv\Scripts\activate
On Linux/macOS:

source venv/bin/activate
Install dependencies:

pip install -r requirements.txt
How to Use
Data Preparation: Load the dataset, adjust the variables, and separate dependent and independent variables.
Model Creation and Training: Use the LogisticRegression function from scikit-learn to create and train the model using the training dataset.
Model Evaluation: Assess model performance using metrics such as Accuracy, Precision, Recall, and F1-Score.
Visualization: Generate plots such as ROC curves, scatter plots, and other visualizations to facilitate result interpretation.
Examples
Here is an example of how to run the model:

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LogisticRegression
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score

# Assuming 'data' is the loaded DataFrame
X = data.drop('target', axis=1)  # Independent variables
y = data['target']  # Dependent variable

# Split the data into training and testing sets
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=42)

# Create the model
model = LogisticRegression()

# Train the model
model.fit(X_train, y_train)

# Predictions
y_pred = model.predict(X_test)

# Model evaluation
print(f'Accuracy: {accuracy_score(y_test, y_pred)}')
print(f'Precision: {precision_score(y_test, y_pred)}')
print(f'Recall: {recall_score(y_test, y_pred)}')
print(f'F1-Score: {f1_score(y_test, y_pred)}')
Contribution
Fork this repository.
Create a branch for your feature (git checkout -b feature/MyFeature).
Make the necessary changes and commit (git commit -am 'Adding new feature').
Push the changes to your fork (git push origin feature/MyFeature).
Open a pull request.
License
This project is licensed under the MIT License - see the LICENSE file for details.
=======
# Online Advertising - Click Prediction with Logistic Regression 📊💻

## Project Overview

This project applies **logistic regression** to predict the probability of a user clicking on an online ad, based on features such as age, time spent on the site, area income, and internet usage.

The analysis includes **cross-validation**, **confusion matrix**, and classification metrics like **accuracy**, **precision**, **recall**, and **F1-score**, in order to evaluate the model’s performance across different data splits.

---

## Project Goals

- Predict ad click likelihood based on user attributes.  
- Evaluate classification performance through multiple metrics.  
- Apply cross-validation to ensure model robustness.  
- Explore threshold adjustment to balance precision and recall.

---

## Dataset

The dataset is located in `data/advertising.csv` and includes:

- `Age`: User age  
- `Daily Time Spent on Site`: Time spent on the website  
- `Area Income`: Average income of the user's area  
- `Daily Internet Usage`: Daily internet usage in minutes  
- `Clicked on Ad`: Target variable (1 = clicked, 0 = not clicked)

---

## Tools and Technologies

- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn

---

## How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/rodrigohigashi/Advertising_data.git
cd Advertising_data

2. Create Virtual Environment (optional)

python -m venv venv
Activate the environment:

Windows: venv\Scripts\activate

Linux/macOS: source venv/bin/activate

3. Install Dependencies

pip install -r requirements.txt

4. Run the Notebook

Open in Jupyter Notebook or VS Code:

cd EN
jupyter notebook logistic-regression.ipynb

Project Structure

Advertising_data/
├── data/
│   └── advertising.csv
├── EN/
│   └── logistic-regression.ipynb
│   └── README_EN.md
├── PT/
│   └── projeto-de-regressao-logistica.ipynb
│   └── README_PT.md
├── requirements.txt
└── README.md

Results & Metrics

Average Accuracy: 97.0%
Average Precision: 98.2%
Average Recall: 95.8%
Average F1-score: 96.9%

These metrics were obtained using 5-fold cross-validation, showing strong and consistent model performance for predicting ad clicks.

License
This project is licensed under the MIT License.


