# FinancialReportsAnalysis
# Financial Report Sentiment Analysis 🧾📈

This project analyzes the sentiment of different sections in 10-K filings using FinBERT, a BERT-based language model fine-tuned for financial text. The goal is to quantify and compare how sentiment in financial disclosures changes across time and companies.

We manually downloaded 10-K filings from the SEC EDGAR database. An EDGAR crawler was then used to extract individual sections (typically 16 items) from each filing. Sentiment scoring was applied **section-wise**, and the yearly sentiment was calculated by averaging scores across all sections for that year.

---

## 📁 Project Files

- **`1company_data.ipynb`**  
  - Extracts all sections from each 10-K filing of a single company  
  - Applies FinBERT sentiment scoring (scale of 1 to 5) per section  
  - Aggregates and visualizes average sentiment per year

- **`n_companies_comparison.ipynb`**  
  - Repeats the same analysis across multiple companies  
  - Compares yearly average sentiment trends  
  - Visualizes inter-company sentiment comparisons

---

## ⚙️ Tools & Technologies

- **Python**
- **FinBERT** (via Hugging Face Transformers)
- **EDGAR Crawler** (for section-wise extraction of 10-K filings)
- **Pandas, Matplotlib, Seaborn** (for data analysis and visualization)
- **Jupyter Notebooks**


