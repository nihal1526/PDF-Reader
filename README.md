# 📄 Universal PDF Reader & AI Data Extractor

This project is an automated workflow built with n8n that reads any type of PDF sent via Telegram, extracts useful information using AI, and converts it into structured data for API usage.

---

## 🚀 Features

- Upload any PDF via Telegram bot
- Extract text from PDF automatically
- AI-powered data extraction (dynamic & customizable)
- Supports multiple document types:
  - Bank statements
  - Invoices
  - Receipts
  - Reports
  - Forms
- Converts unstructured text → structured JSON
- Sends data to API via HTTP POST
- Telegram response with processed output

---

## 🧠 How It Works

1. User sends a PDF file to the Telegram bot
2. The workflow downloads the file
3. Text is extracted from the PDF
4. AI analyzes the content
5. Extracts relevant structured data based on prompt rules
6. Data is formatted into JSON
7. JSON is sent to an API endpoint
8. Response is returned to the user

---

## 📦 Example Output

> Output depends on the document type and AI prompt configuration

```json
{
  "field1": "value",
  "field2": "value",
  "field3": "value"
}

