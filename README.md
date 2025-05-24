# ⚙️ BlazeEdge – GenAI-Powered Competitive Product Analyzer

**BlazeEdge** is an intelligent web-based tool engineered to help manufacturers make their products more competitive in the market using **Generative AI**, **web scraping**, and **automated PDF analysis**.


https://github.com/user-attachments/assets/5b4c32a7-9197-4b2c-a600-ce7c6caf96c2


---

## 🚀 Overview

BlazeEdge enables manufacturers to:

- Upload product specification PDFs
- Analyze product competitiveness using market data
- Compare features, pricing, and specs with current market leaders
- Receive suggestions on features to add/remove
- Interact with a GenAI chatbot for clarity and explanation

---

## 🧠 Key Functionalities

### 🔍 Product Competitiveness Analyzer
- **PDF Upload**: User uploads their product spec sheet.
- **Price Range Input**: Define upper and lower bounds to focus analysis.
- **Competitive Score**: View current and improved competitiveness score.
- **Feature Analysis**:
  - Strengths & Weaknesses
  - Features to Add/Remove
- **Market Ranking**: Compares product ranking among competitors.
- **Downloadable PDF Report**: Summary of all insights for offline use.

### 💬 ClarityBot – GenAI-Powered Assistant
- Upload multiple reports (product, analysis, consolidated).
- Ask questions and get natural language explanations of:
  - Product scores
  - Suggested improvements
  - Market position and reasoning

---

## 🛠️ Technology Stack

| Layer         | Tech Used                    |
|---------------|------------------------------|
| Frontend      | HTML, CSS, JavaScript        |
| Backend       | Python (Flask)               |
| AI Engine     | OpenAI GPT-3.5 Turbo         |
| Scraping      | Scrapy (Flipkart data)       |
| NLP Analysis  | Custom PDF parser + GenAI    |
| Storage       | JSON-based intermediate store|

---

## 🧩 System Workflow

1. User uploads a PDF of product specs.
2. Web scraper collects competing products from Flipkart based on price.
3. Cleaned and structured data is extracted from product pages.
4. Features and reviews are parsed and cleaned.
5. GPT-3.5 analyzes user product against competitors.
6. Recommendations are generated:
   - Add/remove features
   - Improvement areas
   - Competitive ranking
7. Final consolidated PDF report is produced.
8. Users can query the system using ClarityBot for clarification.

---

## 🗃️ Main Modules

- `flipkart_scrapy1.py`: Scrapes products by price range.
- `Data_cleaning2.py`: Cleans scraped data.
- `flipkart_specs3.py`: Extracts detailed specs.
- `specs_cleaning4.py`: Formats and sanitizes specs.
- `flipkart_reviews5.py`: Gathers reviews and star ratings.
- `reviews_cleaning6.py`: Normalizes review data.
- `data_combination7.py`: Combines all product data.
- `GEN_AI.py`: Performs GPT-powered competitive analysis.
- `main.py`: Handles dashboard logic and PDF rendering.
- `claritybot.py`: Responds to user queries from PDF reports.

---

## 📊 Sample Use Case

A smartphone manufacturer uploads their product PDF and enters a price range of ₹15,000–₹20,000. BlazeEdge:
- Scrapes Flipkart for similar phones
- Identifies missing key features (e.g., NFC, IP rating)
- Highlights excessive features driving up cost
- Suggests optimal changes to improve ranking
- Generates a full market ranking and downloadable report

---

## 🔮 Future Enhancements

- User account and dashboard history
- Integration with other e-commerce sites (Amazon, Croma)
- Real-time competitor tracking
- Manufacturer-specific benchmarking
- API access for enterprise clients

---

> “BlazeEdge gives your product a strategic edge – not just data, but AI based decisions.”

---


