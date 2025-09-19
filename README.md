# AutoEDA + AutoML + Feature Visualization + Local GPT4All Q&A

![Project Banner](https://img.shields.io/badge/Streamlit-EDA%20Dashboard-blue)
![Python](https://img.shields.io/badge/Python-3.12-green)
![License](https://img.shields.io/badge/License-MIT-yellow)

## 📌 Project Overview

This project is a **fully local, interactive Streamlit app** that provides:

1. **Automated EDA (AutoEDA)** using `ydata-profiling`  
   - Reports missing values, correlations, distributions, duplicates, and interactions.  
   - Generates an interactive, downloadable HTML report.  

2. **Feature Visualization**  
   - Select any two numeric columns and generate interactive scatter plots using Plotly.  

3. **AutoML & Prediction**  
   - Uses `dabl` and `scikit-learn` to automatically train multiple models.  
   - Selects the best model based on performance (accuracy/F1-score).  
   - Provides metrics and allows predictions on new datasets.  

4. **Local GPT4All Chatbot Q&A**  
   - Fully local natural language query about the dataset.  
   - Example questions:  
     - “When was this unit last repaired?”  
     - “Which parts were used in the repair?”  
     - “Will this repair be required soon?”  
   - Does **not require internet**. GPT4All model file is downloaded once and stored locally.  

---

## 🛠️ Installation

1. **Clone the repository**

```
git clone https://github.com/your-username/autoeda-automl-gpt4all.git
cd autoeda-automl-gpt4all
```

Create and activate a virtual environment
```
python -m venv venv
# Windows
venv\Scripts\activate
# Mac/Linux
source venv/bin/activate
```
Install dependencies

```
pip install -r requirements.txt
```
requirements.txt should include:
```ىشس
``` streamlit
pandas
plotly
ydata-profiling
streamlit-pandas-profiling
dabl
scikit-learn
gpt4all
openpyxl
```

🚀 Running the App
```
streamlit run app.py
```
Open your browser at the local host link (usually http://localhost:8501).

Upload your CSV or Excel dataset to start the analysis.

📂 App Usage

1️⃣ AutoEDA Tab
Displays a full automated EDA report with missing values, correlations, distributions, duplicates, and interactions.

Report is interactive and downloadable as HTML.

2️⃣ Feature Visualization Tab
Select any two numeric columns to generate interactive scatter plots.

Helps explore relationships visually.

3️⃣ AutoML & Prediction Tab
Choose the target column for prediction.

dabl automatically trains multiple models and selects the best one.

Displays model metrics (Precision, Recall, F1-score).

Allows uploading new datasets for predictions.

4️⃣ Local GPT4All Chatbot Q&A Tab
Ask natural language questions about the dataset.

Fully local, no internet required.

Requires GPT4All model file downloaded once (~1GB).

💡 Benefits
Fully local: data never leaves your computer.

Interactive exploration + visualization + predictive modeling + Q&A in one app.

Reduces manual EDA effort and speeds up insights.

Easy for non-technical users.

🧰 Technologies
Python 3.12

Streamlit – interactive web interface

ydata-profiling – automated EDA report

Plotly – interactive visualizations

dabl & scikit-learn – AutoML & predictive modeling

GPT4All – local Chatbot Q&A

pandas – data manipulation

⚖️ License
MIT License

📌 Notes
GPT4All model file must be downloaded locally and can be large (~1GB).

AutoEDA may take longer on very large datasets.

Predictions require datasets with the same structure as the training data.

Chatbot answers are based on the uploaded dataset only.

yaml
Copy code
