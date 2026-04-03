🏠 House Price Prediction App (India)A streamlined Machine Learning web application built with Streamlit that predicts residential property prices in India based on key architectural and geographic features.🚀 OverviewThis project provides an interactive interface for users to estimate house prices. It leverages a pre-trained regression model, accounting for modern factors like property age (calculated up to the year 2026) and regional postal codes.🛠️ Tech StackFrontend: StreamlitMachine Learning: Scikit-learnData Processing: NumPyModel Persistence: Joblib📋 FeaturesInteractive Sliders: Adjust parameters like number of bedrooms, postal code, and year of construction.Real-time Feature Engineering: Automatically calculates House Age based on the input Built Year.Preprocessing Pipeline: Integrates a pre-fitted StandardScaler to ensure input data matches the model's training distribution.Indian Currency Formatting: Displays predictions in Rupees (₹) with localized comma formatting.📁 Project StructurePlaintext├── app.py                # Main Streamlit application script
├── house_price_model.pkl # Pickled dictionary containing the model and scaler
├── requirements.txt      # List of dependencies
└── README.md             # Project documentation
⚙️ Installation & UsageClone the repository:Bashgit clone https://github.com/your-username/house-price-prediction-india.git
cd house-price-prediction-india
Install dependencies:Bashpip install streamlit numpy joblib scikit-learn
Run the app:Bashstreamlit run app.py
💡 How it WorksThe application loads a model_dict which contains both the trained regressor and the scaler.Note: The house_age is dynamically calculated as:$$House\ Age = 2026 - Built\ Year$$This ensures the model remains relevant for near-future projections.
