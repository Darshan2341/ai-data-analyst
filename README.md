# 📄 AI Resume Analyzer

A conversational AI app that analyzes your resume and gives instant feedback — powered by LangChain, Groq (LLaMA 3), and Streamlit.

---

## 🚀 Features

- Upload your PDF resume
- Get an **overall score out of 10**
- Identifies **strengths and weaknesses**
- Suggests **specific improvements**
- **ATS (Applicant Tracking System)** score
- Match your resume against a **job description**
- Suggests **best suited roles** for your profile

---

## 🛠 Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.10+ | Core language |
| Streamlit | Web UI |
| LangChain | AI orchestration |
| Groq (LLaMA 3) | Language model |
| PyPDF2 | PDF text extraction |

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/Darshan2341/ai-resume-analysis.git
cd ai-resume-analysis
```

### 2. Create a virtual environment

```bash
python -m venv venv

# On Windows:
venv\Scripts\activate

# On Mac/Linux:
source venv/bin/activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Set up your API key

```bash
cp .env.example .env
```

Open `.env` and replace `your_groq_api_key_here` with your actual **Groq API key**.

### 5. Run the app

```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`

---

## 📸 How to Use

1. Open the app in your browser
2. Choose **General Analysis** or **Match with Job Description** from the sidebar
3. If matching, paste the job description in the text box
4. Upload your PDF resume
5. Click **Analyze Resume 🚀**
6. Get instant AI-powered feedback!

---

## 📁 Project Structure

```
ai-resume-analyzer/
├── app.py              # Main application logic
├── requirements.txt    # Python dependencies
├── .env.example        # API key template
├── .env                # Your actual keys (not committed)
├── .gitignore
└── README.md
```

---

## 💡 How It Works

1. **Text Extraction** — PyPDF2 reads the raw text from your resume PDF
2. **Prompt Engineering** — A detailed prompt is built asking the AI to analyze specific aspects
3. **AI Analysis** — Groq's LLaMA 3 model reads the resume and generates structured feedback
4. **Job Matching** — If a job description is provided, the AI compares it against your resume and finds missing keywords
5. **ATS Scoring** — The AI estimates how well your resume will pass Applicant Tracking Systems

---

## 🔐 Security Notes

- Never commit your `.env` file — it's in `.gitignore` for this reason
- Keep your Groq API key private
- For production, consider adding authentication

---

## 🙋 Author

**Darshan Pokale**
[www.linkedin.com/in/darshan-pokale-b1834334b](#) | [](#)

---

## 📄 License

MIT License — free to use and modify.
