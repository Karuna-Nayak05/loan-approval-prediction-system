# Credit Pulse: AI-Powered Loan Approval Prediction System 🚀

Credit Pulse is a modern, full-stack machine learning web application designed to predict whether a loan application should be approved or rejected. It helps financial institutions reduce manual decision-making errors, speed up loan processing, and assess risk efficiently.

## 🌟 Key Features
- **AI-Powered Predictions:** Uses a trained Machine Learning model (Random Forest) to evaluate applicants based on income, dependents, education, and credit history.
- **Smart CIBIL Score Override:** The system intelligently factors in CIBIL scores. An exceptionally high score (750+) can override an otherwise borderline rejection, while a very poor score (<600) can override an approval.
- **Dynamic & Encouraging UI:** Features a sleek, modern, permanent dark-mode interface with glassmorphism elements. The system provides supportive, encouraging feedback to applicants even when a loan is rejected.
- **Fast & Scalable:** Powered by a lightning-fast Python API and a highly responsive React frontend.

## 🛠️ Technology Stack
- **Machine Learning:** Python, Pandas, NumPy, Scikit-learn
- **Backend API:** FastAPI, Uvicorn, Pydantic
- **Frontend:** React (Vite), Tailwind CSS (v4), Lucide React (Icons)

## 📁 Project Structure
```text
├── backend/          # FastAPI server logic and endpoint routing
├── frontend/         # React + Vite web application 
├── ml/               # Machine Learning training scripts and saved models
└── README.md         # Project documentation
```

## 🚀 How to Run the Project Locally

To run this application, you need to start both the Python Backend and the React Frontend simultaneously in two separate terminal windows.

### 1. Start the Backend API (Terminal 1)
Open your terminal, navigate to the project folder, and run:
```bash
# Navigate to the backend directory
cd backend

# Install dependencies (if you haven't already)
pip install -r requirements.txt

# Start the FastAPI server
uvicorn main:app --reload
```
*The backend will run on `http://localhost:8000`*

### 2. Start the Frontend Web App (Terminal 2)
Open a **new** terminal window, navigate to the project folder, and run:
```bash
# Navigate to the frontend directory
cd frontend

# Install dependencies (if you haven't already)
npm install

# Start the Vite development server
npm run dev
```
*The frontend will run on `http://localhost:5173`*

### 3. View the App
Hold `Ctrl` (or `Cmd` on Mac) and click the `http://localhost:5173` link in your second terminal to open Credit Pulse in your browser!

## 🧪 Testing Scenarios
You can test the application's intelligence using these sample profiles:

1. **The Ideal Candidate (Standard Approval):** High income, good credit history, Urban property.
2. **The High-Risk Candidate (Standard Rejection):** Low income, high loan request, poor credit history.
---
