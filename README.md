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
## Project Structure

```text
Crop-Recommendation-System/
│
├── app.py                  # Flask backend
├── crop_model.pkl          # Saved ML model
├── crop_data.csv           # Dataset
├── train_model.py          # Model training script
├── Procfile                # Deployment instruction
├── requirements.txt        # Dependencies
├── screenshot.png          # Webpage screenshot
├── README.md
│
├── templates/
│   └── index.html          # Frontend UI
│
└── static/
    ├── style.css           # Styling
    └── script.js           # Frontend logic
```

 
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

## Deployment on Render

1. Push your code to GitHub.

2. Go to Render → New → Web Service.

3. Connect your GitHub repository.

4. Make sure the project contains:

```text
requirements.txt   # Lists all dependencies
Procfile           # Tells Render how to run the app
```

5. Add the following inside `Procfile`:

```text
web: gunicorn app:app
```

6. Choose Python 3.10+ in Render.

7. Click Deploy.

8. Render will generate a live deployment URL 🎉

---

## 📊 Example Input

| Parameter | Value |
|-----------|-------|
| Nitrogen (N) | 90 |
| Phosphorus (P) | 42 |
| Potassium (K) | 43 |
| Temperature | 20.87°C |
| Humidity | 82.00% |
| pH | 6.5 |
| Rainfall | 202.93 mm |
## ✅ Example Output
🌾 Recommended Crop: rice


