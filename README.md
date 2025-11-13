

# **T&C Analyzer – Chrome Extension + FastAPI Backend**

T&C Analyzer is a smart Chrome extension designed to **summarize Terms & Conditions (T&C)** and highlight **potential risks** using AI.
It helps users quickly understand long legal documents using a clean UI and an intelligent backend.

---

## 🚀 **Features**

* 🔍 **AI-powered summarization** of long Terms & Conditions
* ⚠️ **Risk tagging** (risky clauses, data collection points, hidden rules, etc.)
* 📌 **Clean Chrome extension UI** for easy copy-paste or auto-capture
* ⚡ **FastAPI backend** for fast processing
* 🤖 **Transformer-based ML model** for summarization & classification
* 🔐 Secure communication between extension & backend
* 📄 Supports long T&C text inputs

---

## 🏗️ **Project Architecture**

```
Chrome Extension  →  FastAPI Backend  →  AI/ML Model
```

**Frontend (Extension):**

* Popup.html for UI
* Popup.js for sending text to backend
* Manifest v3

**Backend:**

* FastAPI REST APIs
* Transformer model for summarization
* Risk classification module
* CORS enabled for Chrome Extension

---

## 📂 **Folder Structure**

```
/tandc-analyzer
│── chrome-extension
│   ├── manifest.json
│   ├── popup.html
│   ├── popup.js
│   └── styles.css
│
│── backend
│   ├── main.py
│   ├── model.py
│   ├── requirements.txt
│   └── utils/
│
└── README.md
```

---

## ⚙️ **Tech Stack**

### **Frontend**

* HTML, CSS, JavaScript
* Chrome Extension (Manifest V3)

### **Backend**

* Python
* FastAPI
* HuggingFace Transformers
* Pydantic
* Uvicorn

---

## 🚀 **How to Run**

### **Backend**

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### **Chrome Extension**

1. Go to `chrome://extensions/`
2. Enable **Developer Mode**
3. Click **Load Unpacked**
4. Select your **chrome-extension** folder

---

## 🧪 **API Endpoints**

### **POST /summarize**

Input T&C text → returns short summary

### **POST /risk-analysis**

Returns risk tags and explanations

---

## 📌 **Future Enhancements**

* Automatic webpage scraping
* Downloadable PDF summary
* Chrome right-click menu for instant analysis
* User dashboard & analytics

---

## 🧑‍💻 **Author**

**Rakesh Gowda**
Final-year Information Science Engineering
Passionate about **AI, Cloud, DevOps, and full-stack development**.


