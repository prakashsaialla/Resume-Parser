
# 📄 Resume Parser

This project is an **NLP-based Resume Parsing Tool** that extracts meaningful information such as **name, contact details, skills, education, and experience** from resumes. The aim is to automate resume screening and make candidate shortlisting faster and more efficient.

## 🚀 Features

* Tokenizes resumes using **NLTK**
* Removes stopwords for cleaner text processing
* Extracts structured fields such as:

  * 📛 Name
  * 📧 Email
  * 📞 Phone Number
  * 🎓 Education
  * 💼 Experience
  * 🛠 Skills
* Supports parsing resumes in **text and document formats**

## 🛠️ Tech Stack

* **Python 3.x**
* **NLTK** – Natural Language Processing (tokenization, stopwords removal)
* **Regex** – pattern matching for emails, phone numbers, etc.
* **libarchive / pydot** – handling compressed resume archives and visualization
* **Cartopy** – optional geographic info extraction (if location parsing is added)

## 📂 Workflow

1. **Load Resumes** – input resumes in `.txt` / `.pdf` / `.docx` formats
2. **Preprocess Text** – tokenize words, remove stopwords
3. **Entity Extraction** – use regex + NLP to extract key fields
4. **Skill Extraction** – match against predefined list of skills
5. **Output** – structured JSON or CSV file with parsed details

## ▶️ How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/prakashsaialla/resume-parser.git
   cd resume-parser
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook Resume-Parser.ipynb
   ```

4. Load resumes and parse them into structured data.

## 📊 Example Output

```json
{
  "Name": "John Doe",
  "Email": "johndoe@email.com",
  "Phone": "+1-202-555-0143",
  "Education": ["B.Sc. Computer Science, XYZ University"],
  "Experience": ["Software Engineer at ABC Corp"],
  "Skills": ["Python", "Machine Learning", "SQL"]
}
```

## 📌 Future Improvements

* Integrate with a **web app** for uploading resumes
* Use **spaCy / Transformers** for advanced Named Entity Recognition
* Expand to multilingual resume parsing
* Add ranking system for resumes based on job description

## 📜 License

This project is licensed under the MIT License – feel free to use and improve.

---

