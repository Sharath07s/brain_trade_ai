# 🧠 BrainTrade AI

> An AI-powered trading intelligence platform that combines real-time market data, financial news, and sentiment analysis to provide explainable stock insights and market predictions.

![React](https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi)
![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=for-the-badge&logo=python)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-38BDF8?style=for-the-badge&logo=tailwind-css)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase)
![License](https://img.shields.io/badge/License-MIT-success?style=for-the-badge)

---

# 📈 Overview

BrainTrade AI is an intelligent financial analytics platform that helps investors understand market behavior using Artificial Intelligence, real-time stock data, financial news, and sentiment analysis.

Rather than only predicting price movements, BrainTrade AI focuses on **Explainable AI**, allowing users to understand *why* a prediction was made through feature importance and model reasoning.

The platform integrates market intelligence into a modern dashboard, making complex financial analysis easier to interpret for traders, investors, and researchers.

---

# 🎯 Problem Statement

Financial markets generate enormous volumes of data every second.

Investors often struggle to:

- Monitor multiple stocks simultaneously
- Understand the impact of breaking news
- Measure market sentiment
- Interpret AI-generated predictions
- Make informed trading decisions quickly

BrainTrade AI addresses these challenges by combining multiple intelligence sources into a single explainable platform.

---

# ✨ Features

## 📊 Real-Time Stock Dashboard

- Live stock monitoring
- Historical price visualization
- Interactive charts
- Stock performance metrics
- Quick symbol search

---

## 🤖 AI Prediction Engine

Generate AI-assisted market predictions based on historical trends and financial indicators.

Features include:

- Price trend estimation
- Market movement prediction
- Confidence scoring
- AI-generated insights

---

## 🧠 Explainable AI (XAI)

Unlike traditional black-box prediction systems, BrainTrade AI explains every prediction.

Includes:

- Feature importance
- SHAP-style explanations
- Confidence indicators
- Human-readable reasoning

---

## 📰 Financial News Intelligence

Analyze market-moving news articles.

Capabilities:

- News aggregation
- Headline analysis
- Market impact estimation
- Sentiment extraction

---

## 💬 Sentiment Analysis

Aggregates market sentiment from multiple sources.

Provides:

- Bullish sentiment
- Bearish sentiment
- Neutral sentiment
- Overall Market Mood

---

## 📈 Historical Market Analysis

- Historical stock prices
- Trend visualization
- Moving averages
- Performance comparisons

---

## 🎨 Premium User Experience

- Glassmorphism-inspired interface
- Responsive layout
- Smooth animations using Framer Motion
- Mobile-friendly design
- Interactive dashboards

---

# 🏗️ System Architecture

```
                    +-----------------------------+
                    |     React + Vite Frontend   |
                    +--------------+--------------+
                                   |
                           REST API Requests
                                   |
                    +--------------+--------------+
                    |        FastAPI Backend      |
                    +------+-----------+----------+
                           |           |
                           |           |
                    yFinance API   News Services
                           |           |
                           +-----+-----+
                                 |
                          AI Analytics Layer
                                 |
                   Sentiment + Prediction Engine
                                 |
                           Supabase Database
```

---

# 🛠️ Tech Stack

## Frontend

- React
- Vite
- TypeScript
- Tailwind CSS v3
- Framer Motion
- Recharts / Chart.js *(depending on implementation)*

---

## Backend

- FastAPI
- Python
- REST APIs

---

## AI & Machine Learning

- Scikit-learn
- Pandas
- NumPy
- SHAP-style Explainability
- Sentiment Analysis

---

## Market Data

- yfinance

---

## Database

- Supabase
- PostgreSQL

---

## APIs

- Yahoo Finance
- News APIs *(if configured)*

---

# 📂 Project Structure

```
BrainTrade_AI/
│
├── backend/
│   ├── database/
│   ├── routers/
│   ├── services/
│   ├── main.py
│   ├── requirements.txt
│   └── .env
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── services/
│   │   ├── assets/
│   │   ├── pages/
│   │   └── App.tsx
│   ├── package.json
│   └── vite.config.ts
│
├── schema.sql
│
└── README.md
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/yourusername/brain_trade_ai.git

cd brain_trade_ai
```

---

# Database Setup

Create a Supabase project.

Run the SQL script:

```
schema.sql
```

Configure your backend `.env` file.

Example:

```env
SUPABASE_URL=

SUPABASE_KEY=

NEWS_API_KEY=
```

---

# Backend Setup

```bash
cd backend

python -m venv venv

source venv/bin/activate
```

Windows

```bash
venv\Scripts\activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the server

```bash
uvicorn main:app --reload --port 8000
```

---

# Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

Visit

```
http://localhost:5173
```

Search for symbols such as:

- AAPL
- TSLA
- NVDA
- MSFT
- GOOGL

---

# ⚙️ Application Workflow

```
User Searches Stock
          │
          ▼
Fetch Market Data
          │
          ▼
Retrieve Financial News
          │
          ▼
Sentiment Analysis
          │
          ▼
AI Prediction
          │
          ▼
Explainability Engine
          │
          ▼
Interactive Dashboard
```

---

# 📊 Core Modules

- Real-time Stock Monitoring
- Historical Price Analysis
- AI Prediction Engine
- Explainable AI
- Financial News Analysis
- Sentiment Aggregation
- Interactive Charts
- Market Intelligence Dashboard

---

# 📸 Screenshots

Add application screenshots here.

```
screenshots/

├── dashboard.png
<img width="1280" height="832" alt="PHOTO-2026-08-05-19-21-09" src="https://github.com/user-attachments/assets/5159d973-a77d-4b3f-8fc3-b4e8a8d5c190" />

├── prediction.png
<img width="1280" height="832" alt="PHOTO-2026-08-05-19-21-45" src="https://github.com/user-attachments/assets/44599802-9ad9-44de-9327-552f44060f16" />

├── sentiment.png
<img width="1280" height="832" alt="PHOTO-2026-08-05-19-23-09" src="https://github.com/user-attachments/assets/dfe8aa70-718d-4bcd-980a-483d91bdff6f" />

├── explainability.png
<img width="1280" height="832" alt="PHOTO-2026-08-05-19-25-09" src="https://github.com/user-attachments/assets/b57e56a0-8fd1-47d6-b5fc-de0e3557383b" />

---

# 🚀 Deployment

## Frontend

Deploy using **Vercel**.

```bash
npm run build
```

---

## Backend

Deploy using **Render** or any FastAPI-compatible hosting platform.

Startup command:

```bash
uvicorn main:app --host 0.0.0.0 --port $PORT
```

---

# 🔒 Security

- Environment variable management
- API key protection
- Secure backend communication
- Server-side data processing
- Input validation

---

# 🤝 Contributing

Contributions are welcome.

1. Fork the repository
2. Create a feature branch

```bash
git checkout -b feature/new-feature
```

3. Commit changes

```bash
git commit -m "Add new feature"
```

4. Push

```bash
git push origin feature/new-feature
```

5. Open a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

---

# 👨‍💻 Team

**BrainTrade AI**

Developed as a hackathon project demonstrating the application of AI, explainable machine learning, and financial analytics in modern investment intelligence systems.

---

# ⭐ Support

If you found this project interesting, consider giving it a ⭐ on GitHub!

It helps others discover the project and supports future development.
