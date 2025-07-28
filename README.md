# 🧠 SkinLens

SkinLens is an AI-powered web platform for skin disease detection and dermatological reporting. It enables users to upload images, receive predictions using a deep learning model, and manage cases through separate dashboards for patients and dermatologists.

---

## 🚀 Features

- 📷 **Image Upload**: Submit skin condition images for analysis  
- 🧠 **AI Diagnosis**: Predict skin diseases using a trained model  
- 💬 **Chat Interface**: Interactive support and education  
- 👤 **Patient Dashboard**: Review past diagnoses and results  
- 🩺 **Dermatologist Dashboard**: Manage and review patient cases  
- 📄 **Report Generator**: Download PDF or view results online  

---

## 🩻 Classification Categories

SkinLens is trained to recognize the following 21 skin conditions:

1. Acne  
2. Actinic keratoses and Bowen's disease  
3. Allergic contact dermatitis  
4. Basal cell carcinoma  
5. Benign keratosis-like lesions  
6. Eczema  
7. Folliculitis  
8. Lichen planus  
9. Lupus erythematosus  
10. Melanocytic nevi  
11. Melanoma  
12. Neutrophilic dermatoses  
13. Photodermatoses  
14. Pityriasis rosea  
15. Pityriasis rubra pilaris  
16. Psoriasis  
17. Sarcoidosis  
18. Scabies  
19. Scleroderma  
20. Squamous cell carcinoma  
21. Urticaria  

---

## 🗂️ Project Structure

```
SkinLens/
├── frontend/             # React-based frontend
│   └── src/
│       └── pages/        # UploadPage, ResultPage, etc.
├── flask-server/         # Flask API backend
│   └── app.py            # Main prediction endpoint
├── models/               # Keras model files
├── README.md             # Project description and usage
└── .gitignore
```

---

## 🛠️ Getting Started

### ⚙️ Backend Setup (Flask + TensorFlow)

```bash
cd flask-server
pip install -r requirements.txt
python app.py
```

> Make sure Python 3.8+ and TensorFlow are installed.

### 💻 Frontend Setup (React)

```bash
cd frontend
npm install
npm start
```

> Runs at `http://localhost:3000`

---

## 📡 API Usage Example

**Endpoint:** `POST /predict`

**Request JSON:**
```json
{
  "imageUrl": "https://example.com/image.jpg"
}
```

**Response JSON:**
```json
{
  "prediction": "Melanoma"
}
```

---

## 🧬 Model Info

- Format: `.keras` model  
- Input size: `224x224x3`  
- Output: 21-class softmax prediction  
- Trained using image folders labeled by condition name

---

## 📄 License

This project is for educational/research purposes only.  
Based on original work from [`htmw/2024F-Biased`](https://github.com/htmw/2024F-Biased) under MIT license.

---

## 🙌 Credits

Developed and maintained by [Sorafune/SkinLens](https://github.com/Sorafune/SkinLens).  
Uses open-source tools: React, Flask, TensorFlow, and more.
