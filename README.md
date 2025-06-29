Here is your complete `README.md` file **with step-by-step numbering (Step 1, Step 2, etc.)** clearly included in the **Setup Guide** and relevant sections for better clarity.

---

```markdown
# 🛡️ InsuranceSaathi - Your Claim Assistant

InsuranceSaathi is a powerful AI-driven Streamlit application that helps users file, understand, and manage their **insurance claims** in three major categories: **Vehicle**, **Health**, and **Home**. It combines the capabilities of Large Language Models (LLMs), intelligent document and image processing, multilingual translation, and cost estimation to simplify the complex insurance process.

---

## ✨ Key Features

- 📸 **Image Damage Analysis**  
  Upload vehicle/home images to assess severity using OpenCV-based edge density and image quality metrics.

- 🧾 **PDF Health Report Analysis**  
  Upload health-related documents (PDFs) and detect flags like duplicate bills, expired documents, or missing data.

- 🗣️ **LLM Chatbot for Insurance Queries**  
  Chat with a multilingual (English/Hindi) AI assistant. Choose from HuggingFace, Gemini, Groq, or Ollama for responses.

- 🌍 **Multilingual Support**  
  Dynamic translation of content and responses via Google Translate API (Hindi and English supported).

- 💸 **Smart Repair Cost Estimation**  
  Intelligent cost prediction for repair/damage based on the type of insurance claim and severity of analysis.

- 📋 **Quick Action Buttons**  
  Get instant answers for required documents, claim timelines, and what steps to take next.

- 🌙 **Modern Dark UI**  
  Beautiful Streamlit app styled with custom dark mode using HTML/CSS.

---

## 🔧 Tech Stack

| Area                | Technologies Used                                      |
|---------------------|--------------------------------------------------------|
| Frontend & UI       | Streamlit, HTML/CSS                                    |
| Image Processing    | OpenCV, NumPy, PIL (Pillow)                            |
| PDF Processing      | PyMuPDF (fitz)                                         |
| Multilingual Support| googletrans (Google Translate)                         |
| LLMs Integration    | HuggingFace, Gemini (Google), Groq, Ollama             |
| Environment Config  | python-dotenv                                          |
| Chat Interface      | streamlit-chat                                         |
| Cost Estimation     | Custom logic + insurance type base ranges              |

---

## 📁 Folder Structure

```

InsuranceSaathi/
├── app.py                # Main application script
├── .env                  # API keys (not committed to GitHub)
├── requirements.txt      # Python dependencies
└── README.md             # You’re here

````

---

## ⚙️ Setup Guide

### ✅ Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/InsuranceSaathi.git
cd InsuranceSaathi
````

---

### ✅ Step 2: (Optional) Create and Activate Virtual Environment

```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```

---

### ✅ Step 3: Install Required Python Packages

```bash
pip install -r requirements.txt
```

---

### ✅ Step 4: Create and Configure `.env` File

Create a `.env` file in the project root directory and add your API keys:

```env
HUGGINGFACEHUB_API_TOKEN=your_huggingface_api_key
GEMINI_API_KEY=your_gemini_api_key
GROQ_API_KEY=your_groq_api_key
OLLAMA_API_URL=http://localhost:11434
```

---

### ✅ Step 5: (Optional) Run Ollama Locally

If using Ollama, ensure it's installed and the model is downloaded:

```bash
ollama run phi3
```

> ⚠️ Ollama must be running on port `11434` if used as a provider.

---

### ✅ Step 6: Run the Streamlit App

```bash
streamlit run app.py
```

Visit `http://localhost:8501` in your browser to start using the app.

---

## 💬 How It Works

### ▶️ Step 1: Select Configuration

* Choose **Language**, **AI Provider**, and **Claim Type** (Vehicle, Health, Home)

### ▶️ Step 2: Upload Supporting Files (Optional)

* **Upload images** for damage analysis
* **Upload PDFs** for health claim document checks

### ▶️ Step 3: Analyze and Chat

* View AI-powered analysis of uploaded content
* Chat with InsuranceSaathi using LLMs
* Use Quick Action Buttons for instant info

---

## 🧠 LLM Providers

You can choose from these supported LLMs:

| Provider    | Model Name / Endpoint         |
| ----------- | ----------------------------- |
| HuggingFace | Mistral 7B                    |
| Gemini      | Gemini Pro API                |
| Groq        | Mixtral-8x7b                  |
| Ollama      | Local `phi3` model via Ollama |

---

## 📦 Sample `.env` Template

```env
HUGGINGFACEHUB_API_TOKEN=hf_abc123...
GEMINI_API_KEY=AIzaSyA...
GROQ_API_KEY=groq_xyz456...
OLLAMA_API_URL=http://localhost:11434
```

---

## 🚀 Future Improvements

* ✅ Audio input for queries (speech-to-text integration)
* ✅ Claim form auto-filling from uploaded documents
* ✅ SMS or Email notifications for updates
* ✅ Expanded language support (Marathi, Tamil, etc.)
* ✅ Cloud deployment (Streamlit Sharing / HuggingFace Spaces)

---

## 📜 License

This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute it with attribution.

---

## 📬 Contact

For queries, suggestions, or collaboration:

* 💻 GitHub: [your-username](https://github.com/thatChiragiscoding)
* ✉️ Email: [your.email@example.com](chiragas2005@gmail.com)
* 📱 LinkedIn: [your-linkedin-profile](https://www.linkedin.com/in/chiragsawant05/)

---


