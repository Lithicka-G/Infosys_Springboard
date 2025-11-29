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
- [About The Project](#AboutTheProject)
- [Problem Statement](#ProblemStatement)
- [Key Features](#KeyFeatures)
- [Architecture](#Architecture)
- [Tech Stack](#TechStack)
- [Models Used](#ModelsUsed)
- [Project Structure](#ProjectStructure)
- [Installation & Setup](#Installation&Setup)
- [Usage Guide](#UsageGuide)
- [Admin Controls](#Admincontrols)
- [Dataset & Evaluation](#Dataset&Evaluation)
- [Technical Challenges and Solutions](#Technical-Challenges-and-Solutions)
- [Screenshots](#Screenshots)
- [Team](#Team)
- [License](#License)

---
## 📘 About The Project
TextMorph transforms complex, lengthy text into clear summaries and readable paraphrases using adaptive AI models. It supports specialized domains like academic, medical, and legal content, and delivers accurate results through an intuitive interface—no machine learning background required. Optimized for both CPU and CUDA, it’s built for research, education, and enterprise use.

📌 Built as part of Infosys Springboard Internship Final Project
 📌 Target users: Students, educators, researchers, bloggers, media professionals
 
---
## 🎯 Problem Statement
 Millions of students, researchers, and professionals struggle with lengthy, technical, or poorly structured documents. Manually summarizing or paraphrasing complex content is time-consuming and requires strong linguistic skills.

TextMorph uses advanced AI to automatically:
🔹 Improve readability while preserving key information
🔹 Condense long documents into clear, concise summaries
🔹 Rewrite content in simpler or more professional language
🔹 Help users learn and understand complex material faster

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
📌 Database ER Model

---
## 🛠 Tech Stack


- **Frontend:** Streamlit  
- **Authentication:** JWT Tokens  
- **NLP Models:** PEGASUS, BART, FLAN-T5  
- **Text Analysis:** NLTK  
- **Security and Access:** Ngrok  
- **Deployment:** Docker 



---
## 🤖 Models Used

| Model | Purpose | Framework |
|-------|---------|-----------|
| Pegasus | High-quality abstractive summarization | 🤗 Transformers |
| BART | Balanced summarization & rewriting | 🤗 Transformers |
| FLAN-T5 | Paraphrasing & complexity control | 🤗 Transformers |
| NLTK Metrics | Readability scoring | NLTK Toolkit |

**Supports model versioning:** custom

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
   
Screenshots included below 👇

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
| [Full Name] | Project lead & architecture design | [@username] |
| [Full Name] | ML models & fine-tuning | [@username] |
| [Full Name] | Backend API & database | [@username] |
| [Full Name] | Frontend & UI/UX | [@username] |
| [Full Name] | Deployment & DevOps | [@username] |

---
## 📜 License
This project is open source and freely available under the MIT License, allowing anyone to use, modify, distribute, and share the software for any purpose, with proper attribution to the original authors.
