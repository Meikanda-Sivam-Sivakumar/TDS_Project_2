# Data Analyst Agent — Your AI-Powered Data Companion

> Smarter, faster, and more intuitive analysis of your datasets using **Generative AI and Python.**
> Repository: *Insert your GitHub repository link here*

---

## Overview

**Data Analyst Agent 1.0** is an AI-driven assistant designed to simplify data analysis.
Upload your dataset and queries to instantly receive:

* Visual reports
* AI-generated insights
* Automated workflows

Ideal for:

* Analysts
* Researchers
* Startups and businesses
* Anyone interested in turning raw data into actionable insights

---

## Key Features

| Feature                 | Description                                                        |
| ----------------------- | ------------------------------------------------------------------ |
| AI-Powered Insights     | Utilizes Google’s Generative AI to interpret your data and queries |
| Rich Visualizations     | Automatically generates plots using Seaborn and Matplotlib         |
| Web Scraper Mode        | Enables real-time data extraction from URLs                        |
| Multi-Format Support    | Accepts CSV, Excel, JSON, Parquet, and TXT files                   |
| Batch Query Processing  | Supports multiple questions in a single run                        |
| User-Friendly Interface | Designed for ease of use, no technical expertise required          |
| High-Speed Performance  | Optimized for fast execution and real-time results                 |

---

## Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/data-analyst-agent.git  
cd data-analyst-agent  
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt  
```

### 3. Configure API Keys

Create a `.env` file in the root directory:

```env
GEMINI_API_KEY=your_google_api_key  
LLM_TIMEOUT_SECONDS=240  
```

### 4. Launch the Application

```bash
python -m uvicorn app:app --reload  
```

Visit [http://localhost:8000/](http://localhost:8000/) in your browser to begin.

---

## How It Works

1. **Create Your Questions**
   Write your data-related questions in a plain text file. Examples:

   * What is the revenue growth month-over-month?
   * Find the correlation between Age and Income
   * Show the most profitable products

2. **Upload Your Dataset and Questions File**

   * Dataset (optional): CSV, Excel, JSON, Parquet, or TXT
   * Questions file (required): Plain text

3. **Generate Results**

   * The AI processes your queries
   * Insights and summaries are generated
   * Visualizations are automatically created

---

## Technology Stack

### Backend

* **FastAPI** – High-performance asynchronous web server
* **LangChain** – Orchestrates large language model interactions
* **Google Generative AI** – Powers core AI features
* **Pandas & NumPy** – Efficient data manipulation and analysis
* **Seaborn & Matplotlib** – For professional-grade data visualizations

### Frontend

* HTML5, CSS, JavaScript
* Clean, responsive interface using a Bootstrap-inspired layout

---

## API Endpoints

| Method | Endpoint   | Description                       |
| ------ | ---------- | --------------------------------- |
| `GET`  | `/`        | Loads the web application         |
| `POST` | `/api`     | Submit dataset and question file  |
| `GET`  | `/summary` | Returns diagnostics and summaries |

---

## Supported File Formats

| Type    | Extensions      |
| ------- | --------------- |
| CSV     | `.csv`          |
| Excel   | `.xlsx`, `.xls` |
| JSON    | `.json`         |
| Parquet | `.parquet`      |
| Text    | `.txt`          |

---

## Use Cases

* **Business Intelligence** – Analyze sales trends, KPIs, and forecasting
* **Academic Research** – Explore datasets and validate hypotheses
* **Data Science** – Perform exploratory data analysis and anomaly detection
* **Automated Reporting** – Generate dashboards and executive summaries

---

## Security

* All processing is done locally; no cloud storage is used
* API keys are securely stored via `.env` configuration
* CORS policy can be customized for production environments

---

## License

This project is licensed under the **MIT License** – free to use for personal and commercial purposes.

