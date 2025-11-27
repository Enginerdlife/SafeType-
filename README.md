#  SafeType+  AI-Powered Text & Image Risk Scanner

SafeType+ is a multi-modal AI security tool designed to detect and prevent the accidental sharing of sensitive information.  
It analyzes **text** and **images (via OCR)** to identify:

- Personally Identifiable Information (PII)
- Sensitive keywords
- Risky URLs
- Phishing intent & social engineering patterns
- Image-embedded text (OCR)
- And computes a final **risk score + classification (Low / Medium / High)**

Built with **FastAPI + spaCy + Regex + Transformers + Tesseract OCR** and a modern **React + Tailwind** dashboard.

---

##  Features

### Text Risk Scanner
- Email / phone / credit card / Aadhaar-pattern detection  
- Sensitive PII extraction using spaCy NER  
- URL analysis + shortened link detection  
- Phishing intent scoring via ML + heuristics  
- Automatic highlighting of risky text  

###  Image Risk Scanner
- OCR with Tesseract  
- Preprocessing with OpenCV (grayscale, thresholding)  
- Automatic extraction + scanning of hidden text  

###  Risk Scoring Engine
Outputs:
- `pii_hits`
- `risk_factors`
- `phishing_score (0–100)`
- `classification (LOW / MEDIUM / HIGH)`
- `highlighted_text`
- `ocr_text (optional)`

### Modern React Dashboard
- Text scanner panel  
- Image upload and preview panel  
- Combined mode  
- Tailwind UI components  
- Toasts, badges, risk score bars, dark mode  

---

##  Project Structure

```bash
SafeTypePlus/
│
├── backend/                  # FastAPI server
│   ├── app.py
│   ├── routers/
│   ├── services/
│   ├── core/
│   ├── models/
│   └── tests/
│
└── frontend/                 # React + Vite + Tailwind UI
    ├── src/
    ├── public/
    └── package.json
