<h1 align="center">LegalEase AI</h1>

<p align="center">
  AI-Powered Legal Document Simplification and Analysis
</p>

<p align="center">
  <img src="https://img.shields.io/github/last-commit/hannahjan06/Legal_docs" alt="last commit">
  <img src="https://img.shields.io/github/languages/top/hannahjan06/Legal_docs?color=1b4b9c&label=top%20language" alt="Python">
  <img src="https://img.shields.io/github/languages/count/hannahjan06/Legal_docs?label=languages" alt="languages">
</p>

<p align="center">
  Built using:
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Hugging%20Face-FFCC00?style=for-the-badge&logo=huggingface&logoColor=black">
  <img src="https://img.shields.io/badge/Python-3572A5?style=for-the-badge&logo=python&logoColor=white">
  <img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white">
  <img src="https://img.shields.io/badge/Gemini%20API-000000?style=for-the-badge&logo=google&logoColor=white">
</p>

## Overview

LegalEase AI is a web platform designed to simplify complex legal documents using structured AI agents. Users can upload agreements, policies, contracts, and other legal files, and the system automatically generates simplified summaries, risk assessments, and visual flowcharts for faster understanding. The project demonstrates the practical use of generative AI for legal assistance, clarity, and accessibility.

---

## Core Features

* **User Authentication**
  Secure signup and login with a modern UI.

* **Document Upload Support**
  PDF upload with OCR processing for scanned files.

* **AI Agent Pipeline**

  * PDF Reader Agent (OCR + text extraction)
  * Summarization Agent (section-level simplification)
  * Structuring Agent (risk and clause analysis)
  * Flowchart Agent (visual representation of key relationships)

* **Interactive Chat Interface**
  Users can ask clarifying questions about the uploaded document.

* **Modern UI Design**
  Clean, minimal interface prioritizing readability and structure.

---

## How It Works

1. The user authenticates and uploads a legal document.
2. The document is stored in Google Cloud Storage.
3. The PDF Reader agent extracts and preprocesses text.
4. The Summarization and Structuring agents analyze the content.
5. The Flowchart agent produces a visual logic diagram of key clauses.
6. Users view results through a dashboard and chatbot interface.

---

## Tech Stack

| Layer         | Technologies                     |
| ------------- | -------------------------------- |
| Frontend      | Next.js, React, TailwindCSS      |
| Backend       | FastAPI or Flask                 |
| AI Processing | Google Gemini API, Python agents |
| OCR           | pytesseract, pdf2image           |
| Cloud         | Google Cloud Storage, Vertex AI  |
| Deployment    | GCP services                     |

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/legalease.git
cd legalease
```

### 2. Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### 3. Backend Setup

```bash
cd backend
pip install -r requirements.txt
uvicorn app:main --reload
```

---

## Project Structure

```bash
/frontend
   /components        # UI components including chatbot and upload interface
   /pages             # login, signup, dashboard screens
   /styles            # Tailwind configuration

/backend
   /agents            # PDF Reader, Summarizer, Structurer, Flowchart logic
   /utils             # Cloud storage helpers and error handling
   app.py             # FastAPI entry point
```

---

## Workflow

1. User logs in.
2. PDF document is uploaded and stored.
3. OCR extracts text where necessary.
4. AI agents analyze and structure document content.
5. Flowchart and simplified summary are generated.
6. Processed results are delivered through the dashboard and chatbot.

---

## Roadmap

* Multi-language support
* Clause comparison between similar contract types
* Exportable simplified reports
* Versioning for document history
* Fine-tuned legal language models for more accuracy

---

## Contributing

Contributions are welcome in interface refinement, AI pipeline improvements, dataset expansion, or document parsing. Submit a pull request with clear documentation.

---

## Acknowledgements

* Google Cloud Platform for compute, storage, and generative AI services
* Open-source OCR frameworks supporting document accessibility
* Legal research datasets used for testing and benchmarking
