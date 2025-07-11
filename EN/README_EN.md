# Online Advertising - Click Prediction with Logistic Regression 📊💻

## Project Overview

This project applies **logistic regression** to predict the probability of a user clicking on an online ad, based on variables such as age, time spent on the site, average regional income, and daily internet usage.

The analysis includes **cross-validation**, **confusion matrix**, and classification metrics such as **accuracy**, **precision**, **recall**, and **F1-score**, aiming to evaluate the model’s performance across different data splits.

---

## Project Objectives

- Predict ad click probability based on user attributes.  
- Evaluate classification performance through multiple metrics.  
- Apply cross-validation to ensure model robustness.  
- Explore decision threshold adjustment to balance precision and recall.

---

## Dataset

The dataset is located in `data/advertising.csv` and includes:

- `Age`: User age  
- `Daily Time Spent on Site`: Time spent on the site  
- `Area Income`: Average income of the user's region  
- `Daily Internet Usage`: Daily internet usage (minutes)  
- `Clicked on Ad`: Target variable (1 = clicked, 0 = did not click)

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

Windows:

venv\Scripts\activate
Linux/macOS:

source venv/bin/activate
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

Results and Metrics
Average Accuracy: 97.0%

Average Precision: 98.2%

Average Recall: 95.8%

Average F1-score: 96.9%

These metrics were obtained using 5-fold cross-validation, demonstrating strong and consistent model performance in predicting ad clicks.

Contribution
Fork this repository.

Create a branch for your feature:

git checkout -b feature/MyFeature
Make the necessary changes and commit:

git commit -am "Adding new feature"
Push to your fork:

git push origin feature/MyFeature
Open a pull request.

License
This project is licensed under the MIT License.
See the LICENSE file for more details.


