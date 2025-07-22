
# lEHERBOT- ANNUAL SALARY PREDICTOR


The project features a **React-based frontend** styled with a custom neon theme and background, and a **FastAPI backend** powered by a trained **TensorFlow regression model**. It also provides intuitive charts and visualizations to interpret model performance.

---

## 🚀 Key Features

- 📥 Easy-to-use form to input employee data
- 📈 Real-time salary prediction using a TensorFlow model
- 🎨 Visually appealing UI with custom background and stylish fonts
- 📊 Dynamic plots of:
  - R² Score, MAE, RMSE
  - Prediction vs Actual Salaries
  - Residual Histograms and Scatterplots
  - Boxplots and Error Distributions

---

## 🏗️ Tech Stack

| Layer     | Tech                         |
|-----------|------------------------------|
| Frontend  | React, Tailwind CSS, Chart.js |
| Backend   | FastAPI, Uvicorn             |
| ML Model  | TensorFlow (.h5)             |
| Styling   | Dancing Script Font + Neon Theme |

---

## 📁 Project Structure

```
wagewizard/
├── backend/
│   ├── main.py
│   ├── model_utils.py
│   ├── wagewizard_model.h5
│   └── static/
│       └── (generated visualizations)
├── frontend/
│   ├── public/
│   │   └── background.png
│   └── src/
│       ├── components/
│       │   ├── EmployeeForm.jsx
│       │   ├── ChartsDisplay.js
│       │   └── ModelInsights.jsx
│       ├── App.jsx
│       └── index.js
└── README.md
```

---

## ⚙️ How to Run the Project

### 1. 🔧 Backend Setup

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

Ensure the trained TensorFlow model file `wagewizard_model.h5` is present in the backend folder.

### 2. 🎨 Frontend Setup

```bash
cd frontend
npm install
npm start
```

Your React frontend will launch on `http://localhost:3000` and communicate with the FastAPI backend running on `http://localhost:8000`.

---

## 📊 Sample Model Metrics

| Metric       | Value    |
|--------------|----------|
| R² Score     | 0.9099   |
| MAE          | 989.98   |
| RMSE         | 1324.18  |


## 📝 Acknowledgments

- [TensorFlow](https://www.tensorflow.org/)
- [FastAPI](https://fastapi.tiangolo.com/)
- [React](https://reactjs.org/)
- [Chart.js](https://www.chartjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
