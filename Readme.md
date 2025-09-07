# 📊 AI-Driven Market Intelligence System

An **agentic RAG-powered** platform that automates market intelligence by combining data scraping, sentiment analysis, forecasting, translation, and report generation into a single production-ready system.  
Designed for **executives, investors, and analysts** who need **boardroom-ready insights** instead of raw data.

---

## 🚀 Features

- **Multi-Source Data Fetching**  
  Scrapes financial news, social media, and APIs (e.g., Yahoo Finance).

- **Sentiment Analysis**  
  Uses FinBERT + LLMs to classify news/events as bullish, bearish, or neutral.

- **Trend Forecasting**  
  Time-series predictions using Prophet / NeuralProphet.

- **Multi-Language Support**  
  Translation layer powered by Hugging Face (MarianMT / NLLB).

- **Automated Report Generation**  
  Creates concise PDF/HTML reports with sentiment scores, trends, and risk flags.

- **Interactive Dashboard**  
  Query-driven insights with charts, anomaly detection, and downloadable reports.

- **Agentic Workflow**  
  Powered by agents:
  - `DataFetcher` → Collects raw data  
  - `SentimentAnalyzer` → Classifies tone  
  - `TrendForecaster` → Predicts market movement  
  - `Translator` → Normalizes multilingual input  
  - `ReportGenerator` → Produces polished outputs  

---

## 🏗️ Architecture

The system follows a **highly modular, production-level structure** for scalability and maintainability:


---

## ⚙️ Tech Stack

- **Backend:** FastAPI (async-first, modular architecture)  
- **Data Models:** Pydantic  
- **Database:** PostgreSQL + Qdrant (vector DB)  
- **LLMs:** Google Gemini (free tier) + Hugging Face models (FinBERT, BGE embeddings, MarianMT)  
- **Forecasting:** Prophet / NeuralProphet / sktime  
- **Scraping:** RSS, Requests, BeautifulSoup  
- **Frontend (optional):** React + Next.js + Tailwind  
- **Reports:** WeasyPrint / ReportLab  

---

## 📂 Workflow Overview

1. **User Query** → e.g., "Summarize banking sector risks this week."  
2. **Data Fetcher Agent** → Collects news, stock data, social posts.  
3. **Translator Agent** → Normalizes multilingual inputs.  
4. **Sentiment Analyzer** → Assigns sentiment labels (bullish/bearish/neutral).  
5. **Trend Forecaster** → Predicts short-term market direction.  
6. **Report Generator** → Produces boardroom-ready insights.  
7. **Output** → PDF report, dashboard insights, or alerts.

---