# KARE_bot - Faculty Meet Assistant

**KARE_bot** is a Streamlit-based web application that allows students at KL University to find available time slots to meet faculty members. The app uses Natural Language Processing (powered by Gemini 2.0 Flash) to answer queries like _“Is Dr. Smith free tomorrow afternoon?”_ by parsing and storing faculty timetable PDFs.

Only faculty can upload timetables (admin access), while students (with `@klu.ac.in` email) can query for availability using a simple chat interface.

---

## 🚀 Features

- 🔐 **Secure Authentication** – Role-based login for faculty (admin) and students  
- 📄 **Timetable Upload & Processing** – Admins can upload PDF timetables which are parsed and stored  
- 💬 **NLP Chat Interface** – Ask natural language questions like “When is Prof. Ravi free?”  
- 🔎 **LLM + RAG-based Querying** – Uses Gemini 2.0 Flash and SQL query structuring to return contextual responses  
- 📚 **RAG-Enabled** – ChromaDB used for few-shot learning + LangChain-based logic for better query structuring  

---

## 🧰 Prerequisites

- Python 3.8+  
- MySQL Server  
- `pip` (Python package manager)  
- Google Gemini API Key  
---
## 🧑‍💼 How to Use

### 🔐 Admin Access

- **Upload Timetables:** Navigate to the "Upload Timetable" section
- **Supported Format:** Only well-formatted PDFs

### 🎓 Student Access

- **Sign Up:** Use your `@klu.ac.in` email
- **Login and Use Chat Interface**
  - Try queries like:
    - “Is Dr. Arjun available on Wednesday morning?”
    - “Can I meet Prof. Meena tomorrow?”
    - “When is Dr. Priya free next week?”

---

## 📁 Project Structure

```bash
├── kare_bot.py           # Main app file
├── utils.py              # Utility functions and LLM interaction
├── config.yaml           # Authentication config
├── requirements.txt      # Python dependencies
├── few_shot_db/          # Few-shot examples database
├── temp.pdf              # Uploaded temporary PDF file
```

---

## 🧪 Tech Stack

- **Frontend**: Streamlit  
- **Backend**: Python, MySQL, LangChain  
- **LLM**: Google Gemini 2.0 Flash  
- **PDF Parser**: PDFPlumber  
- **Auth**: Streamlit Authenticator  
- **Data**: SQLAlchemy, ChromaDB  
- **NLP Logic**: RAG (Retrieval-Augmented Generation)  

---

## 📜 License

This project is licensed under the Apache License 2.0 – see [LICENSE](LICENSE) file for full details.

---

## 🤝 Contributing

Have suggestions or fixes?  
Feel free to fork the repo and submit a pull request!

---

## ✉️ Contact

For issues or queries, feel free to reach out to the project creator:  
📧 `bharathinukurthi1@gmail.com`
