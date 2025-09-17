# Iris Classification with Decision Tree & Perceptron

This project performs **data exploration and classification** on the classic
[Iris dataset](https://raw.githubusercontent.com/jbrownlee/Datasets/master/iris.csv)  
using Python, pandas, scikit-learn, seaborn, and matplotlib.

## 📋 Overview
- Loads and cleans the Iris dataset
- Performs quick EDA (summary statistics & pairplot visualization)
- Splits the data into training and testing sets
- Trains and evaluates:
  - **Decision Tree Classifier**
  - **Perceptron Classifier**
- Displays confusion matrices for model comparison
- Saves both trained models as `.pkl` files using `joblib`

## 🛠 Requirements
Install dependencies (Python 3.8+ recommended):
```bash
pip install pandas seaborn matplotlib scikit-learn joblib

▶️ How to Run

Clone the repository:

git clone https://github.com/<your-username>/iris-insight-notebook.git
cd iris-insight-notebook


Run the notebook or script:

python iris_classification.py


or open the .ipynb notebook in Jupyter and execute cells.

📊 Key Steps in Code

EDA: sns.pairplot visualizes relationships across features.

Model Training:

dt_model = DecisionTreeClassifier()
perc_model = Perceptron(max_iter=1000, tol=1e-3, random_state=42)
perc_model.fit(X_train, y_train)
dt_model.fit(X_train, y_train)


Evaluation:

accuracy_score(y_test, y_pred)
ConfusionMatrixDisplay.from_predictions(y_test, y_pred)


Saving Models:

joblib.dump(dt_model, 'decision_tree_model.pkl')
joblib.dump(perc_model, 'perceptron_model.pkl')

📈 Results

Typical accuracies:

Decision Tree: ~95%+

Perceptron: ~90%+
(Results may vary slightly due to random splits.)

🗂 Project Structure
.
├─ DATA1.ipynb            # Jupyter notebook with full workflow
├─ decision_tree_model.pkl
├─ perceptron_model.pkl
└─ README.md


Author: Shumani Marvellous Raludzingana
Feel free to fork or contribute!


---

### Tips
- Replace `<your-username>` with your actual GitHub username.
- If your main file is still `DATA1.ipynb`, keep that name in the structure section or rename it to som
