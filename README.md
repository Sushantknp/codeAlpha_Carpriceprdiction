# Car-price-prdiction
Car Price Prediction with Machine Learning 🚗
A machine learning project that estimates the resale price of a used car in Indian rupees (₹ lakhs). It includes exploratory data analysis, feature engineering, model training and evaluation, plus a Streamlit web app for interactive predictions.
Features
- Explore car-price data with visualizations and correlation analysis.
- Engineer features such as car age, brand, and kilometers driven per year.
- Preprocess numeric and categorical data for regression models.
- Compare Ridge Regression, Random Forest, and Gradient Boosting.
- Tune model hyperparameters with cross-validation.
- Evaluate predictions using R², MAE, RMSE, residual plots, and feature importance.
- Enter car details in a Streamlit app to get an estimated resale price.
Model Results
The project README's reported results are shown below. Results depend on the dataset and train/test split.
Metric	Reported value
Cross-validation R² (tuned Ridge Regression)	0.96
Test R²	0.91
Test MAE	0.82 lakhs


These are project-reported results, not a guarantee of performance on every car or in real-world transactions.

Project Structure
car-price-prediction/
├── app.py                       # Streamlit prediction app
├── car_price_model.joblib       # Saved trained model
├── requirements.txt             # Python dependencies
├── data/
│   └── car_data.csv             # Dataset
├── notebooks/
│   └── car_price.ipynb          # Analysis and model training
├── images/
│   ├── eda.png                  # Exploratory data analysis
│   ├── evaluation.png           # Model evaluation
│   └── importance.png            # Feature importance
├── .gitignore
└── README.md
Getting Started
1. Clone the repository
Replace YOUR-USERNAME with your GitHub username:
git clone [https://github.com/Sushantknp/car-price-prediction.git](https://github.com/Sushantknp/Car-price-prdiction/blob/main/car-price-prediction.zip)
cd car-price-prediction
2. Create and activate a virtual environment (recommended)
Windows
python -m venv .venv
.venv\Scripts\activate
macOS / Linux
python3 -m venv .venv
source .venv/bin/activate
3. Install dependencies
python -m pip install --upgrade pip
pip install -r requirements.txt
Run the Streamlit App
From the project root directory, run:
streamlit run app.py
Open the local URL shown in the terminal (usually [http://localhost:8501](http://localhost:8501/)). Enter the car details and select Predict to see the estimated selling price in lakhs.
Run the Notebook
To explore the analysis and training workflow:
jupyter notebook notebooks/car_price.ipynb
You can also open the notebook directly on GitHub without running it locally.
Workflow
1. Exploratory data analysis: inspect distributions, correlations, and outliers.
2. Feature engineering: derive car age, brand, and distance-driven features.
3. Preprocessing: encode categorical variables and transform/scale features as implemented in the notebook.
4. Model comparison: evaluate Ridge Regression, Random Forest, and Gradient Boosting using cross-validation.
5. Hyperparameter tuning: use GridSearchCV to tune the selected model.
6. Evaluation: review R², MAE, RMSE, residuals, and permutation feature importance.
Visualizations
Model evaluation

Feature importance

Exploratory data analysis

Dataset
The project dataset is stored at data/car_data.csv. Review the notebook for the data fields, cleaning steps, and transformations used during training.
Limitations
- The dataset is relatively small (approximately 300 rows), so predictions may not generalize to every market or vehicle.
- Important variables such as engine condition, accident history, service records, and detailed specifications may not be represented.
- Rare models and luxury vehicles may be predicted less accurately.
- The output is an estimate for learning/demo purposes, not a formal valuation or guaranteed sale price.
Tech Stack
- Python
- Pandas and NumPy
- Scikit-learn
- Matplotlib and Seaborn
- Joblib
- Streamlit
- Jupyter Notebook
Contributing
Contributions and suggestions are welcome. For a change:
1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Open a pull request describing the improvement.
License
No license is specified yet. Add a LICENSE file before presenting this project as open source, and choose a license appropriate for your intended use.
