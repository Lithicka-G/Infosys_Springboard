# ✨TextMorph: Text Summarization and Paraphrasing Platform

## Project Overview
TextMorph is an advanced AI-driven platform that transforms complex text into clear, accessible content through intelligent summarization and paraphrasing. Built with cutting-edge transformer models and secure authentication, it serves students, researchers, and professionals seeking to enhance text comprehension and communication.

---
## 🔗 Quick Links

| Category | Details |
|----------|---------|
| **📽️ Demo Video** | Coming Soon |
| **🧩 Source Code** | [This Repository](link-to-your-repo) |
| **🐳 Docker Support** | Yes |
| **🧠 AI Models** | Pegasus · BART · FLAN-T5 |

---
## 📑 Table of Contents

- About The Project <a id="AboutTheProject"></a>
- Problem Statement <a id="ProblemStatement"></a>
- Key Features <a id="KeyFeatures"></a>
- Architecture <a id="Architecture"></a>
- Models Used <a id="ModelsUsed"></a>
- Tech Stack <a id="TechStack"></a>
- Project Structure <a id="ProjectStructure"></a>
- Installation & Setup <a id="InstallationSetup"></a>
- Usage Guide <a id="UsageGuide"></a>
- Datasets & Evaluation <a id="DatasetEvaluation"></a>
- Technical Challenges and Solutions <a id="TechnicalChallengesSolutions"></a>
- Screenshots <a id="Screenshots"></a>
- Team <a id="Team"></a>
- License <a id="License"></a>

---
## 📘 About The Project
TextMorph transforms complex, lengthy text into clear summaries and readable paraphrases using adaptive AI models. It supports specialized domains like academic, medical, and legal content, and delivers accurate results through an intuitive interface—no machine learning background required. Optimized for both CPU and CUDA, it’s built for research, education, and enterprise use.
- Built as part of Infosys Springboard Internship Final Project
- Target users: Students, educators, researchers, bloggers, media professionals

#### Key Statistics:
- 86% of students already use AI in their studies.
- In the 2024 Global AI Student Survey (3,839 students, 16 countries), 86% said they use AI tools for coursework. Among the most common use-cases:
- 33% use AI to summarize documents
- 28% use AI to paraphrase a document

---
## 🎯 Problem Statement
 Millions of students, researchers, and professionals struggle with lengthy, technical, or poorly structured documents. Manually summarizing or paraphrasing complex content is time-consuming and requires strong linguistic skills.

TextMorph uses advanced AI to automatically:
- Improve readability while preserving key information
- Condense long documents into clear, concise summaries
- Rewrite content in simpler or more professional language
- Help users learn and understand complex material faster

---
## 🚀 Key Features

1)👤 User Features:

| Feature | Description |
|---------|-------------|
| Secure Login | JWT-based authentication with OTP recovery |
| Easy Input | Paste text or upload documents (PDF/txt) |
| Summarization | Adjustable length: Short/Medium/Long |
| Paraphrasing | Simple, Neutral, and Advanced tones |
| Readability Analysis | Real-time scoring with detailed metrics |
| Side-by-Side Compare | Original vs generated text view |
| Automatic History | Save and access previous operations |
| Feedback System | Rate results and provide comments |
| Document Support | PDF and text extraction for long documents |
| Custom Models | Fine-tuned models for specific domains |
| Data Augmentation | Expand training data for improved accuracy |
| Profile Management | Change password with security validation |

2)👨‍💼 Admin-only Features:

| Feature | Description |
|---------|-------------|
| Admin Limits | Strict limit of two super-admin accounts |
| Admin Access | Manage user accounts (add, remove, promote) |
| Usage Analytics | Charts and real-time insights on platform usage |
| Feedback Monitoring | Track model performance and user ratings |
| Global History | Full access with advanced search filters |
| Audit Logging | Track all critical user and system actions |
| Full Audit View | Complete input/output visibility across all operations |
| Workflow Monitoring | Track workflow patterns and platform performance |

---
## 🧩 Architecture
📌 Architecture Diagram
![Architecture Diagram](https://github.com/user-attachments/assets/ab796282-3ce1-4933-a393-d01f57cdeee1)

📌ER Model Diagram
<img width="6468" height="3489" alt="er diagram" src="https://github.com/user-attachments/assets/e9155251-1d81-460a-9b7c-30c2998de01f" />

---

## 🤖 Models Used

| Model | Purpose | Purpose |
|-------|---------|-----------|
| Pegasus | High-quality abstractive summarization |	Summarization & ParaphrasingT |
| BART | Balanced summarization & rewriting | Summarization & Paraphrasing |
| FLAN-T5 | Paraphrasing & complexity control | Summarization & Paraphrasing |
| Custom Model FLAN-T5 | Domian-Specific NLP tasks | Data Augmentation & Model Tuning |

**Supports model versioning:** custom

---
## 🛠 Tech Stack
<img width="1536" height="1024" alt="Tech Stack" src="https://github.com/user-attachments/assets/37c7b29d-c19e-4b16-b81b-27f530dfc56d" />

---
## 📂 Project Structure





---
## ⚙️ Installation & Setup






---
## 📝 Usage Guide

1. **Register/Login** – Secure JWT authentication
2. **Input Text** – Paste or upload documents (PDF/txt)
3. **Select Task** – Choose summarization or paraphrasing style
4. **Generate & Compare** – View side-by-side results instantly
5. **Save & Rate** – Store in history and provide feedback
   
---
## 📊 Datasets & Evaluation

Evaluation Datasets:

| Dataset | Domain |
|---------|--------|
| ArXiv | Scientific writing |
| CNN/DailyMail | Journalistic content |
| PubMed | Medical literature |
| BillSum | Legal documents |

Evaluation Metrics:

| Metric | Purpose |
|--------|---------|
| ROUGE | Summary quality vs reference |
| BLEU | Output accuracy measurement |
| Lexical Diversity | Vocabulary richness analysis |
| Readability Metrics | Clarity and comprehension scoring |

---
## 🔧 Technical Challenges and Solutions

| Area | Challenge | Solution |
|------|------------|-----------|
| Authentication | Token expiration and session management | Implemented JWT refresh and secure session state in Streamlit |
| Model Integration | High memory usage from PEGASUS and BART | Added model caching and selective loading mechanisms |
| Performance | Slow inference on CPU | Optimized batch processing and added progress indicators |
| Ngrok Stability | Tunnel drops and port conflicts | Implemented auto-reconnect and dynamic port allocation |
| Readability Accuracy | Noise from special characters | Added robust text cleaning and normalization |
| UI/UX Layout | Streamlit’s limited layout control | Utilized columns, expanders, and custom CSS for structure |

---
## 📸 Screenshots



---
## 👥 Team

| Name | Contribution | GitHub |
|------|--------------|--------|
| Lithicka G | Login part, Authentication, Admin dashboard (Global activity), History in User Login| https://github.com/Lithicka-G |
| Vijendra Cherupally | User Login (Data Augmentation and Model Testing part), Docker, Readme | https://github.com/vijayendracherupally |
| Immadisetti Tejo Thoshani | User Login (Paraphrasing), User Profile | https://github.com/Thoshani |
| Jaagruthi Musinada | User Login( Summarization), User Feedback and PPT | https://github.com/Jaagruthi-Musinada |
| Aakanksha Sainath Jadhav | Admin Dashboard ( User Management, Analytics and Insights) | https://github.com/aakankshajadhav412-alt |

---
## 📜 License
This project is open source and freely available under the MIT License, allowing anyone to use, modify, distribute, and share the software for any purpose, with proper attribution to the original authors.
