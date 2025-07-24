# 🧑‍💼 Employee Salary Prediction App

A Streamlit-based web application that predicts whether an employee's annual income is **<=50K** or **>50K** based on demographic and work-related details. This project uses a trained machine learning model on the classic Adult Income dataset from the UCI repository.

---

## 🚀 Features

- ✅ Interactive web UI with Streamlit
- ✅ Predict salary category based on user inputs
- ✅ Uses a trained machine learning pipeline (`RandomForestClassifier`, `ColumnTransformer`, etc.)
- ✅ Encodes categorical data and preserves feature ordering
- ✅ Displays intuitive predictions (`<=50K` or `>50K`)
- ✅ Handles model loading with caching and error handling

---

## 📂 Project Structure
├── app.py # Streamlit app script (main file)
├── train_and_save_model.py # Script to train model and save .pkl files
├── salary_prediction_model.pkl # Trained model pipeline (joblib)
├── label_encoder.pkl # Label encoder for target classes
├── categorical_options.pkl # Dictionary of options for dropdowns
├── requirements.txt # Python dependencies
└── README.md # Project documentation

---

## 🛠️ Installation

### 🔧 1. Clone the repository

```bash
git clone https://github.com/your-username/employee-salary-predictor.git
cd employee-salary-predictor

📦 2. Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
📥 3. Install dependencies
pip install -r requirements.txt
🧠 4. Train the model (if not already available)
python train_and_save_model.py
This will generate the following files:

salary_prediction_model.pkl

label_encoder.pkl

categorical_options.pkl

⚠️ These files are necessary to run the app.
▶️ Usage
Launch the Streamlit app:
streamlit run app.py

🧾 Inputs Collected
Field	Type
Age	Number
Workclass	Dropdown
Education	Dropdown
Education Num	Number
Marital Status	Dropdown
Occupation	Dropdown
Relationship	Dropdown
Race	Dropdown
Gender	Dropdown
Capital Gain	Number
Capital Loss	Number
Hours per Week	Number
Native Country	Dropdown

📊 Example Output
🎯 The predicted annual income is: >50K
ℹ️ The predicted annual income is: <=50K

🧠 Model Info
Trained on the UCI Adult Income Dataset

Uses scikit-learn pipeline with preprocessing

Includes a label encoder and categorical field mappings

📦 Dependencies
All dependencies are in requirements.txt. Main libraries:

streamlit

pandas

numpy

scikit-learn

joblib

🌐 Deployment
You can deploy the app on:

Streamlit Community Cloud

Hugging Face Spaces (with Gradio/Streamlit)

Render or Heroku

🧩 To-Do / Future Enhancements
Add explainability with SHAP

Log user predictions

Support CSV batch predictions

Add unit testing

📜 License
MIT License – feel free to use and modify.


