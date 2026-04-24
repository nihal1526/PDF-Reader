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

## 🖼️ Product Preview

<p align="center">
  <img src="PDF Reader.png" alt="PDF Reader Workflow" width="900"/>
</p>

<p align="center">
  <b>End-to-end automation:</b> Capture → Process → Store → Respond ⚡
</p>

---

## 🔄 Workflow Diagram

```mermaid
flowchart LR
    A[Telegram User] --> B[Upload PDF]
    B --> C[n8n Workflow]
    C --> D[Extract Text from PDF]
    D --> E[AI Processing]
    E --> F[Structured JSON Output]
    F --> G[HTTP API Request]
    G --> H[Telegram Response]
