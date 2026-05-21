<<<<<<< HEAD
# 🌱 Smart Crop Recommendation System

A **machine learning powered web application** that recommends the most suitable crop to grow based on soil nutrients and environmental conditions.

---

## 🚀 Features
- **Machine Learning Model (Random Forest)** trained on agricultural dataset.
- Predicts the best crop based on:
  - Nitrogen (N)
  - Phosphorus (P)
  - Potassium (K)
  - Temperature (°C)
  - Humidity (%)
  - pH
  - Rainfall (mm)
- **Modern Web UI** with glassmorphism design (Bootstrap + custom CSS).
- **Flask Backend API** serving ML predictions.
- **Interactive Frontend** with loading spinner and styled result card.

---

## 🛠️ Tech Stack
- **Python 3.10+**
- **Flask** (backend web framework)
- **Scikit-learn** (ML model training)
- **Pandas** (data preprocessing)
- **HTML / CSS / Bootstrap** (frontend)
- **JavaScript (Fetch API)** (AJAX requests)

---

 ## 📂 Project Structure
Crop-Recommendation-System/
│── app.py               # Flask backend
│── crop_model.pkl       # Saved ML model
│── crop_data.csv        # Dataset
│── train_model.py       # Model training script
│── Procfile             # Deployment instruction
│── requirements.txt     # Dependencies
│── screenshot.png       # Webpage Sereenshot
├── templates/
│   └── index.html       # Frontend UI
│
├── static/
│   ├── style.css        # Styling
│   └── script.js        # Frontend logic
│
└── README.md
## ⚙️ Local Setup (Run on Your PC)
1. Clone the Repository
git clone https://github.com/your-username/Crop-Recommendation-System.git
cd Crop-Recommendation-System
2. Create Virtual Environment (optional but recommended)
python -m venv venv
venv\Scripts\activate       # Windows
source venv/bin/activate    # Linux/Mac
3. Install Dependencies
pip install -r requirements.txt
4. Train the Model (optional)
python train_model.py
5. Run the Application
python app.py
Now visit 👉 http://127.0.0.1:5000/

 ## 🌍 Deployment on Render
Push your code to GitHub.
Go to Render → New → Web Service.
Connect your repo.
Make sure you have:
requirements.txt → lists dependencies
Procfile → tells Render how to run app:
web: gunicorn app:app
Choose Python 3.10+ in Render.
Deploy → Render gives you a live URL 🎉.
 ## 📊 Example Input
Feature	Example Value
Nitrogen (N)	45
Phosphorus(P)	41
Potassium (K)	54
Temperature	27
Humidity	65
pH	6
Rainfall	146
✅ Example Output
🌾 Recommended Crop: rice
