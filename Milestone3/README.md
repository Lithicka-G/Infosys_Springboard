# TextMorph: Text Summarization and Paraphrasing Platform

## Project Overview
TextMorph is an NLP-powered web application designed for text summarization, paraphrasing, and readability analysis.  
Developed using Streamlit, it enables users to transform and understand text through intelligent summarization and complexity-based paraphrasing — all within a secure and intuitive interface.

---

## Key Features

### User Authentication & Security
- Secure JWT-based authentication system  
- Role-based access with user profiles  
- Reading preferences and content type management  
- Encrypted login and registration interface  

### Readability Analysis Dashboard
- Real-time readability scoring using multiple indices:
  - Flesch-Kincaid Readability Score  
  - Gunning Fog Index  
  - SMOG Index  
- Color-coded complexity visualization  
- Drag-and-drop file upload  
- Comprehensive text metrics display  

### Multi-Level Summarization
- Integrated models: PEGASUS, BART, and FLAN-T5  
- Adjustable summary lengths: Short, Medium, Long  
- Side-by-side comparison of original and summarized text  
- Summary quality evaluation using ROUGE metrics  
- Word count tracking and compression ratio calculation  

### Complexity-Based Paraphrasing
- Multiple complexity levels: Beginner, Intermediate, Advanced  
- Readability grade-level control  
- Style-based paraphrasing options  
- Original vs paraphrased text comparison  

---

## Technical Implementation

### Models and Tools
- PEGASUS – Abstractive summarization  
- BART – Sequence-to-sequence text generation  
- FLAN-T5 – Versatile text-to-text transformer  
- NLTK – Readability analysis and text preprocessing  

### Security and Deployment
- JWT for secure session management  
- Ngrok for tunneling and public access  
- Streamlit-based responsive web interface  
- Secure file upload and session handling  

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

| **Name**             | **Contribution**                                                                                                                               |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| **Lithicka**      | Implemented readability analysis using NLTK indices, developed visual complexity indicators, and created real-time scoring and metrics display |
| **Aakanksha Jadhav**  | Implemented JWT-based authentication, user profiles, and session management                                                                    |
| **Kushagra Hada**     | Designed and developed the UI/UX, dashboard layout, and navigation                                                                             |
| **Sherwin Jonathan** | Integrated summarization and paraphrasing models, optimized performance                                                                        |

---

## Installation and Setup
To set up TextMorph locally, follow these steps:

First, clone the repository from GitHub to your local machine.  
Next, install all the required dependencies mentioned in the `requirements.txt` file using pip.  
Ensure that you have Python version 3.8 or higher installed on your system before proceeding.  

After installation, configure the necessary environment variables.  
Set up a JWT secret key for authentication token generation and add your Ngrok authentication token for secure tunneling and public access.  
These environment variables are important for maintaining the application’s security and functionality.  

Once the configuration is complete, launch the Streamlit application to start the local development server.  
The application will automatically open in your web browser, allowing you to access TextMorph locally.  

Finally, navigate to the localhost address provided by Streamlit in your browser, register a new account, or log in to begin using all the features of TextMorph.

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

