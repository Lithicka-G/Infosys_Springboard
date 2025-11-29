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

## 📑 Table of Contents
- [About The Project](#AboutTheProject)
- [Problem Statement & Motivation](#ProblemStatement&Motivation)
- [Key Features](#KeyFeatures)
- [Architecture](#Architecture)
- [Tech Stack](#TechStack)
- [Models Used](#ModelsUsed)
- [Project Structure](#ProjectStructure)
- [Installation & Setup](#Installation&Setup)
- [Usage Guide](#UsageGuide)
- [Admin Controls](#Admincontrols)
- [Dataset & Evaluation](#Dataset&Evaluation)
- [Screenshots](#Screenshots)
- [Team](#Team)
- [License](#License)

---

## 📘 About The Project


---

## Technical Challenges and Solutions

| Area | Challenge | Solution |
|------|------------|-----------|
| Authentication | Token expiration and session management | Implemented JWT refresh and secure session state in Streamlit |
| Model Integration | High memory usage from PEGASUS and BART | Added model caching and selective loading mechanisms |
| Performance | Slow inference on CPU | Optimized batch processing and added progress indicators |
| Ngrok Stability | Tunnel drops and port conflicts | Implemented auto-reconnect and dynamic port allocation |
| Readability Accuracy | Noise from special characters | Added robust text cleaning and normalization |
| UI/UX Layout | Streamlit’s limited layout control | Utilized columns, expanders, and custom CSS for structure |

---

## Contributors

| Name | Contribution | GitHub |
|------|---------------|--------|
| Aakanksha Jadhav | Implemented JWT-based authentication, user profiles, and session management | [GitHub](https://github.com/aakankshajadav) |
| Kushgra Hada | Designed and developed the UI/UX, dashboard layout, and navigation | [GitHub](https://github.com/Kushagra92004) |
| Sherwin Jonathan | Integrated summarization and paraphrasing models, optimized performance | [GitHub](https://github.com/sherwinjonathan) |

---

## Installation and Setup

1. **Clone the Repository**  
   Clone the TextMorph repository from GitHub to your local machine.

2. **Install Dependencies**  
   Install all required Python packages using pip. Ensure your system has **Python 3.8 or higher** before installing.

3. **Configure Environment Variables**  
   Set up the following environment variables:  
   - `JWT_SECRET_KEY` – for authentication token generation  
   - `NGROK_AUTH_TOKEN` – for secure tunneling and public access  
   These are essential for the application’s security and proper functionality.

4. **Launch the Application**  
   Start the Streamlit application to run the local development server. The app will open in your web browser, allowing you to access TextMorph.

5. **Register or Log In**  
   Create a new account or log in to start using all the features of TextMorph.

---

## Usage
1. Register or log in to access all features.  
2. Upload or paste text directly into the interface.  
3. View real-time readability scores and metrics.  
4. Generate concise summaries using the integrated models.  
5. Paraphrase text to adjust style and complexity levels.  

---

## Technology Stack
- **Frontend:** Streamlit  
- **Authentication:** JWT Tokens  
- **NLP Models:** PEGASUS, BART, FLAN-T5  
- **Text Analysis:** NLTK  
- **Security and Access:** Ngrok  
- **Deployment:** Streamlit Cloud / Local  

---
## Team 1
TextMorph was developed by a collaborative team of AI and software enthusiasts committed to building an intuitive and secure NLP platform.  
The team combined expertise in **NLP modeling, web development, UI/UX design, and security** to create a seamless experience for text summarization and paraphrasing.

