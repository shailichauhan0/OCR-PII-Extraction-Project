# OCR + PII Extraction Pipeline for Handwritten Documents

## Author: Shaili Chauhan

## 🚀 Project Overview

This project implements a complete **OCR (Optical Character
Recognition) + PII (Personally Identifiable Information) Extraction
pipeline** for handwritten JPEG documents. It extracts text, detects
sensitive information, and generates an optional redacted image.

## 🧠 Key Features

-   Works with handwritten images
-   Handles tilted images
-   OCR using EasyOCR
-   Text cleaning
-   PII detection (Regex + NLP)
-   Optional redaction
-   Streamlit UI + FastAPI backend included

## 🏗️ System Architecture

    Input JPEG → Preprocessing → OCR → Text Cleaning → PII Detection → (Optional) Redaction

## 📦 Folder Structure

    ocr_pii_project/
    ├── src/
    ├── ui/
    ├── docs/
    └── samples/

## 🖥️ Sample Output

### Extracted PII JSON:

{ "name": "Rahul Verma", "age": "32", "phone": "9876543210", "email":
null, "address": "Rajpur Road, Dehradun" }

## ⚙️ How to Run

pip install -r requirements.txt python src/main.py streamlit run
ui/app_streamlit.py uvicorn ui.api_fastapi:app --reload

## 🎯 Use Cases

-   Clinic/doctor notes scanning
-   Form digitization
-   Sensitive info redaction

## 🌐 Author

Shaili Chauhan
