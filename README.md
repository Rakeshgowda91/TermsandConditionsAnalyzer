

# **T&C Analyzer – AI-Based Terms & Conditions Insight Tool**

**T&C Analyzer** is a Chrome extension integrated with a FastAPI backend that helps users quickly understand lengthy Terms & Conditions documents.
The system uses transformer-based NLP models to generate meaningful summaries and flag clauses that may involve privacy concerns or user risks.

---

## **Highlights**

* Summarizes long legal documents into readable, short insights
* Identifies risk-related statements such as data sharing or hidden conditions
* Responsive Chrome extension interface designed for easy text input
* Backend powered by FastAPI for efficient API responses
* Advanced transformer model for summarization and risk evaluation
* Handles large and unstructured T&C text blocks
* Secure communication between extension and server

---

## **System Structure**

```
Chrome Extension → API Request → FastAPI Backend → NLP Model → Final Output
```

### **Extension Components**

* Popup UI built with HTML and CSS
* JavaScript logic to submit user text to backend
* Manifest V3 configuration

### **Backend Components**

* REST endpoints created with FastAPI
* Transformer model for text analysis
* Utility modules for text preprocessing
* CORS enabled for Chrome extension interaction

---

## **Project Directory**

```
tandc-analyzer/
│
├── chrome-extension/
│   ├── manifest.json
│   ├── popup.html
│   ├── popup.js
│   └── styles.css
│
├── backend/
│   ├── main.py
│   ├── model.py
│   ├── requirements.txt
│   └── utils/
│
└── README.md
```

---

## **Tech Stack Overview**

### **Frontend**

* HTML
* CSS
* JavaScript (MV3 Chrome Extension)

### **Backend**

* Python
* FastAPI
* Uvicorn
* Transformers
* Pydantic

---

## **Running the Project**

### **Backend Setup**

```bash
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### **Chrome Extension Setup**

1. Open `chrome://extensions/`
2. Turn on **Developer Mode**
3. Click **Load Unpacked**
4. Select the `chrome-extension` folder

---

## **Available API Routes**

### **POST /summarize**

Generates a simplified summary of the provided legal text.

### **POST /risk-analysis**

Returns risk indicators and context-based explanations.

---

## **Future Roadmap**

* Automatic extraction of T&C from website pages
* Button to download summary reports
* Right-click context menu for fast analysis
* Web dashboard for previous analyses and comparisons

---

## **Author**

**Rakesh Gowda P**
Information Science Engineering Student
Interested in **AI development, backend engineering, DevOps, and cloud-based applications**.

-
