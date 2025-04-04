User Manual
Project Title: 97_CSM_241009
Project Type: Machine Learning Web Application (Streamlit)
________________________________________
📌 Purpose of the Project
This web-based application allows users to:
•	Upload and preprocess datasets
•	Visualize data using various plots
•	Apply machine learning models
•	View performance metrics
•	Download processed data
It provides a simple GUI for beginners and practitioners to explore ML workflows without writing any code.
________________________________________
💻 How to Run the Application
1.	Install Required Libraries
Open your terminal/command prompt and run:
bash
CopyEdit
pip install streamlit pandas numpy scikit-learn seaborn matplotlib
2.	Run the Application
bash
CopyEdit
streamlit run 97_CSM_241009.py
3.	The app will open in your browser (typically at http://localhost:8501/).
________________________________________





🧭 Application Sections
1. Upload Dataset
•	Navigate to the left sidebar.
•	Upload a .csv dataset file using the file uploader.
•	The dataset will be displayed in the main area for review.
________________________________________
2. Handle Missing Values
•	Choose a method from:
None, Mean, Median, or Mode.
•	Select one or more columns where missing values should be filled.
•	Numeric methods (Mean, Median) work on numeric columns only.
________________________________________
3. Scaling
•	Select a scaling method:
None, Standard Scaling, or Min-Max Scaling.
•	Choose numeric columns to apply the selected scaling method.
________________________________________
4. View Processed Dataset
•	After preprocessing, the modified dataset is displayed.
•	This version will be used for visualization and modelling.
________________________________________
5. Visualize Dataset
Choose from the following plots:
•	Histogram: Distribution of one variable
•	Boxplot: Visualize outliers and spread
•	Scatter Plot: Compare two numeric variables
•	Line Plot: Show trend over index or time
•	Heatmap: Correlation matrix of numeric variables
You'll be prompted to select relevant columns depending on the plot.
________________________________________
6. Apply Machine Learning Model
•	The app automatically selects the last column of the dataset as the target variable.
•	Choose a model:
o	Logistic Regression
o	Decision Tree
o	Random Forest
o	K-Nearest Neighbours (KNN)
o	Support Vector Machine (SVM)
•	On clicking Run Model, it:
o	Encodes categorical variables
o	Splits data into training/testing
o	Trains and evaluates the model
o	Shows:
	Accuracy
	Classification Report
	Confusion Matrix (with heatmap)
________________________________________
7. Download Processed Dataset
•	Use the button in the sidebar to download the cleaned and pre-processed dataset as a CSV file.
________________________________________
📂 Input File Format
Your input should be a CSV file with:
•	A header row (column names)
•	At least one feature column and one target column
•	The target column should be the last column in the dataset
________________________________________
🔧 Dependencies
Package	Purpose
streamlit	Web app interface
pandas	Data manipulation
numpy	Numerical processing
matplotlib	Plotting (basic)
seaborn	Enhanced visualizations
scikit-learn	Preprocessing & ML models
________________________________________
💡 Tips & Best Practices
•	Always review your dataset before applying ML models.
•	Use Mean/Median only on numeric columns.
•	Heatmaps give quick insight into correlated features.
•	Make sure the last column is your target variable.
•	Download the processed dataset if you want to use it outside the app.
________________________________________
📞 Contact
For issues, suggestions, or contributions:
Maintainer: DEBASIS MAJI
Mobile No: 9800319882
Email: debasismaji1999@gmail.com
GitHub: https://github.com/Coding-Debasis/97_CSM_241009_Streamlit
