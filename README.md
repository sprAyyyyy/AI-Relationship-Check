# 🤖 AI Company Checker – CSV Batch Analyzer (Google Colab)

A Google Colab tool that batch-checks whether companies are AI-related based on public web data. It uses **SerpAPI** for live search results and **Gemini 1.5 Flash** for reasoning over structured company data.

> 📈 Upload a CSV file of company names → Get AI relevance tags, confidence scores, and explanations → Download results in CSV/Excel.

---

## 🚀 Try It Now

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](YOUR_COLAB_LINK_HERE)

---

## 🛠 Features

- 🔍 Search company profiles using SerpAPI
- 🤖 Analyze for AI relevance with Gemini 1.5 Flash
- 🧠 Output includes:
  - AI relevance (`is_ai`)
  - Confidence level
  - AI category (`Core AI`, `AI-Integrated`, etc.)
  - Explanation summary
  - Key AI-related terms
- 📁 CSV input with automatic column detection
- 📤 Exports results as `.csv` and `.xlsx`
- 📊 Prints summary stats (no visualization)
- 🧪 Includes sample CSV generator for testing

---

## 🔐 API Key Setup

Click the 🔑 icon in the **Colab sidebar** and add:

| Key Name         | Where to Get It                       |
|------------------|----------------------------------------|
| `GEMINI_API_KEY` | [Google AI Studio](https://makersuite.google.com/app/apikey) |
| `SERPAPI_API_KEY`| [SerpAPI](https://serpapi.com/manage-api-key) |

---

## 📁 Input Format

Upload a `.csv` file with one of the following column names:
- `Company`, `company_name`, `Company Name`, `Name`

Or let the script automatically detect the first column with names.

---

## ✅ Output Example

| company     | is_ai | confidence | category       | explanation                   |
|-------------|-------|------------|----------------|-------------------------------|
| OpenAI      | True  | High       | Core AI        | Known for developing GPT, etc |
| McDonald's  | False | Medium     | Non-AI         | Uses AI in ops, not core      |

Additional columns like `ai_aspects` and original CSV columns are preserved.

---

## 📊 Summary Output

