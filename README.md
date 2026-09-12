# 💰 FinPilot AI — Enterprise Financial Planning Agent

An AI-powered financial planning platform that helps individuals and 
businesses analyze budgets, forecast revenue, monitor expenses, detect 
anomalies, and receive strategic financial recommendations — all in one 
intelligent dashboard.

## 🎯 What It Does

- 📊 **Budget Analysis** — Track and analyze budgets by category with real-time insights
- 📈 **Revenue Forecasting** — Time-series ML models (ARIMA, Prophet, Moving Average) 
  predict future revenue with confidence intervals
- 🚨 **Anomaly Detection** — Isolation Forest & Z-Score algorithms flag unusual 
  expense patterns automatically
- 🤖 **AI Recommendations** — Google Gemini LLM generates personalized, actionable 
  financial advice based on your data
- 📉 **Interactive Dashboards** — Beautiful, responsive React UI with live charts 
  and KPIs

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Backend** | Python, FastAPI, SQLAlchemy, Pydantic |
| **Frontend** | React, Vite, TailwindCSS, Recharts |
| **Database** | SQLite (SQL) |
| **ML/AI** | scikit-learn, statsmodels, Prophet, Isolation Forest |
| **LLM** | Google Gemini API |
| **Auth** | JWT |

## 🏗️ Architecture

[React UI] → [FastAPI REST API] → [ML Services + Gemini] → [SQLite DB]

## 🚀 Features

- User authentication with JWT
- CRUD for budgets & transactions
- Category-wise expense breakdown
- Multi-model forecasting with accuracy metrics (MAE, RMSE, MAPE)
- Anomaly detection with severity levels
- AI-generated monthly financial reports
- Interactive charts & drill-down analytics
- Dark/Light theme
- Fully responsive design

## 📸 Screenshots

(Add your dashboard screenshots here)

## ⚡ Quick Start

(Setup instructions here)

## 📌 Status

Practice / Portfolio project — built to demonstrate full-stack + ML + LLM 
integration skills.

## 👨‍💻 Author

Your Name — [LinkedIn] | [Portfolio]


---

## 🛠️ Tech Stack

### Backend
| Technology | Purpose |
|-----------|---------|
| **Python 3.10+** | Core language |
| **FastAPI** | Web framework (async, auto-docs) |
| **Uvicorn** | ASGI server |
| **SQLAlchemy** | ORM for database |
| **Pydantic** | Data validation & schemas |
| **SQLite** | Lightweight relational DB |
| **python-jose** | JWT tokens |
| **passlib[bcrypt]** | Password hashing |
| **python-dotenv** | Environment variables |

### Machine Learning
| Library | Purpose |
|---------|---------|
| **pandas** | Data manipulation |
| **numpy** | Numerical computing |
| **scikit-learn** | Isolation Forest, metrics |
| **statsmodels** | ARIMA |
| **prophet** | Time-series forecasting |
| **joblib** | Model serialization |

### AI / LLM
| Service | Purpose |
|---------|---------|
| **Google Gemini API** | Recommendations, chat, explanations |

### Frontend
| Technology | Purpose |
|-----------|---------|
| **React 18** | UI library |
| **Vite** | Build tool (fast HMR) |
| **React Router v6** | Routing |
| **TailwindCSS** | Utility-first styling |
| **shadcn/ui** | Pre-built components |
| **Recharts** | Charts & graphs |
| **Axios** | HTTP client |
| **React Hook Form** | Form handling |
| **Zod** | Form validation |
| **Lucide React** | Icons |
| **react-hot-toast** | Notifications |
| **date-fns** | Date utilities |

### DevOps / Tooling
| Tool | Purpose |
|------|---------|
| **Git & GitHub** | Version control |
| **VS Code** | IDE |
| **Postman / Swagger** | API testing |
| **npm / pip** | Package managers |

---

## 📁 Project Structure



---

## ⚡ Quick Start

### Prerequisites

Make sure you have installed:

- **Python 3.10+** → [Download](https://python.org/downloads)
- **Node.js 18+** → [Download](https://nodejs.org)
- **Git** → [Download](https://git-scm.com)
- **Google Gemini API Key** → [Get Free Key](https://ai.google.dev)

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/finpilot-ai.git
cd finpilot-ai



cd backend

# Create virtual environment
python -m venv venv

# Activate it
# Windows:
venv\Scripts\activate
# macOS/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Setup environment variables
cp .env.example .env
# Edit .env and add your GEMINI_API_KEY

# Initialize database
python scripts/init_db.py

# Seed sample data (optional but recommended)
python scripts/seed_db.py

# Run the server
uvicorn main:app --reload --port 8000


# Open a new terminal
cd frontend

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env
# Edit .env if backend URL is different

# Run dev server
npm run dev