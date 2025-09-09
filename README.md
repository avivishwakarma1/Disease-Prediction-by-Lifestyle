🩺 Disease Prediction by Lifestyle
A Machine Learning project for predicting multiple diseases based on lifestyle habits and health indicators using Multi-Output Classification.

📌 Features
- 🧹 Data Preprocessing – Missing value handling, categorical encoding, feature scaling
- 🧠 Feature Engineering – BMI calculation and health metric transformations
- 🌐 Multi-Target Prediction – Random Forest Classifier for simultaneous disease prediction
- 📊 Model Evaluation – Accuracy, F1-score, and Hamming Loss metrics
- 🧾 User Input Interface – Real-time predictions based on lifestyle data
- 💾 Model Persistence – Saved .pkl files for reuse and deployment

🗂 Project Structure
├── disease_prediction.py              # Training & prediction script  
├── health_activity_data_25diseases.csv # Dataset  
├── multi_target_disease_model.pkl     # Trained Random Forest model  
├── scaler.pkl                         # StandardScaler for input features  
├── label_encoder.pkl                  # Encoder for categorical variables  
└── README.md                          # Project Documentation  



📂 Dataset
- Input File: health_activity_data_25diseases.csv
- Attributes Include:
- Age, Gender, Height, Weight, BMI
- Daily Steps, Calories Intake, Hours of Sleep, Exercise Hours
- Heart Rate, Blood Pressure
- Smoker Status, Diet Quality
- Target Labels: 25 disease conditions (multi-label format)

⚙️ Installation & Setup
- Clone the repository
git clone https://github.com/your-username/disease-prediction-by-lifestyle.git  
cd disease-prediction-by-lifestyle  
- Install dependencies
pip install -r requirements.txt  
- Run the training script
python disease_prediction.py  



▶️ Usage
Upload dataset in Colab:
from google.colab import files  
uploaded = files.upload()  


Enter user input for prediction:
--- Disease Prediction ---
Enter Age: 25  
Enter Gender: Male  
Enter Height_cm: 175  
Enter Weight_kg: 70  
Enter BMI: 22.9  
Enter Daily_Steps: 8000  
Enter Calories_Intake: 2200  
Enter Hours_of_Sleep: 7  
Enter Heart_Rate: 72  
Enter Systolic_Pressure: 120  
Enter Diastolic_Pressure: 80  
Enter Exercise_Hours_per_Week: 5  
Enter Smoker: No  
Enter Diet: Healthy  


Get predictions:
--- Predicted Diseases ---
Diabetes: No  
Hypertension: Yes  
Obesity: No  
...



📊 Model Performance
- ✅ Accuracy Score: ~0.85
- ❌ Hamming Loss: ~0.12
- 📋 Detailed performance metrics available per disease label

🛠️ Tech Stack
- Language: Python 🐍
- Libraries:
- pandas, numpy – Data handling
- matplotlib, seaborn – Visualization
- scikit-learn – Machine Learning
- joblib – Model saving

🚀 Future Improvements
- 🌐 Deploy with Streamlit or Flask for interactive web access
- 📈 Expand dataset with real-world health records
- 🧬 Experiment with advanced models (XGBoost, Neural Networks)

👨‍💻 Author
Abhitesh
B.Tech in Artificial Intelligence & Data Science
