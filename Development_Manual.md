🛠️ Development Manual
📘 Project Title: 97_CSM_241009
________________________________________
🎯 Purpose
This manual is intended for developers who want to understand, modify, or extend the functionality of the Streamlit ML App. It outlines the internal architecture, file structure, key components, and guidelines for future enhancements.
________________________________________
🗂️ Project Structure
bash
CopyEdit
97_CSM_241009/
│
├── app.py                   # Main Streamlit application
├── requirements.txt         # List of dependencies
├── datasets/                # Optional directory to keep test datasets
├── README.md                # Project overview and usage instructions
├── user_manual.pdf          # End-user documentation
└── dev_manual.pdf           # This document
________________________________________
🧠 Key Modules in 97_CSM_241009.py
Section	Description
Upload Dataset	Handles CSV file upload using Streamlit's sidebar
Handle Missing Values	Fills NaNs using user-selected method and columns
Scaling	Applies StandardScaler or MinMaxScaler to numeric columns
Visualize Dataset	Plots (hist, boxplot, scatter, line, heatmap) based on user selection
Apply ML Models	Runs selected ML algorithm on preprocessed data (auto-selects target)
Download CSV	Downloads the transformed dataset
________________________________________
💡 Important Design Decisions
•	Last Column as Target: Automatically treats the last column in the CSV as the target for ML.
•	Encoding: Uses pd.get_dummies for feature encoding and pd.factorize for target encoding.
•	Exception Handling: Simple try/except blocks around model logic to catch common errors.
•	Separation of Concerns: Data preprocessing, visualization, and modeling are clearly separated in logic.
________________________________________
🔧 Technologies Used
•	Streamlit for web UI
•	Pandas / NumPy for data handling
•	Seaborn / Matplotlib for visualizations
•	Scikit-learn for preprocessing and machine learning
________________________________________
🚀 Suggestions for Future Development
1.	Add Regression Model Support
2.	Model Comparison Dashboard
3.	Hyperparameter Tuning (GridSearchCV)
4.	Export Trained Models (joblib/pickle)
5.	Authentication System (for multi-user setup)
6.	Cloud Deployment (Streamlit Cloud, Heroku, etc.)
7.	Log System for tracking model results
________________________________________
