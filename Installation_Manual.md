🧰 Installation Manual
🛠️ For Project: 97_CSM_241009
________________________________________
📋 Requirements
•	Python 3.8+
•	Pip (Python package installer)
•	Internet connection to install dependencies
________________________________________
📦 Installation Steps
1. Clone or Download the Project
bash
CopyEdit
git clone https://github.com/ Coding-Debasis/97_CSM_241009_Streamlit /97_CSM_241009.git
cd 97_CSM_241009
Or download the ZIP and extract.
________________________________________
2. Create a Virtual Environment (Recommended)
bash
CopyEdit
python -m venv venv
source venv/bin/activate     # For Linux/Mac
venv\Scripts\activate        # For Windows
________________________________________
3. Install Dependencies
Make sure you're inside the project folder, then run:
bash
CopyEdit
pip install -r requirements.txt
If requirements.txt doesn't exist yet, create it using:
bash
CopyEdit
pip freeze > requirements.txt
________________________________________
4. Run the Application
bash
CopyEdit
streamlit run 97_CSM_241009.py
Then open the URL shown in your terminal (usually http://localhost:8501/).
________________________________________
5. Test with Sample Dataset (Optional)
Place a sample .csv dataset inside a /datasets folder or upload one using the app UI.
________________________________________
🧪 Troubleshooting
Issue	Solution
Module not found	Run pip install <module> manually
streamlit command not found	Ensure virtual environment is activated
App crashes on model execution	Check for NaNs, non-numeric types in dataset
Port already in use	Add --server.port 8502 to run on a different port
________________________________________
