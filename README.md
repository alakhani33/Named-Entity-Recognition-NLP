
# Named Entity Recognition (NER) on Public Health Article

This project demonstrates the use of **Named Entity Recognition (NER)** to extract entities such as persons, organizations, locations, and other named elements from a text article about public health. Built with **spaCy**, the project includes text preprocessing, entity extraction, visualization, and an entity glossary for interpretation.

## 📂 Project Overview

1. **Dependencies and Setup**
   - Utilizes the `spacy` library and its `en_core_web_sm` model.
   - Uses `displacy` for rendering entity visualization within the notebook.

2. **Data Source**
   - The input text is read from a `public_health.txt` file.
   - The text discusses public health topics (modifiable for any text input).

3. **Named Entity Recognition Workflow**
   - Load and parse the text using spaCy’s NLP pipeline.
   - Identify entities within the text.
   - Visualize entities inline with `displacy.render()`.
   - List and count entities by type.

4. **Entity Glossary**
   The notebook includes a reference table explaining common NER labels like `PERSON`, `ORG`, `GPE`, `NORP`, etc.

---

## 🧰 Dependencies

Install required packages:

```bash
pip install spacy pandas nltk
python -m spacy download en_core_web_sm
```

---

## 🚀 How to Run

1. Place your input text in a file named `public_health.txt` in the same directory as the notebook.
2. Open the notebook in **Jupyter Notebook** or **JupyterLab**.
3. Run all cells sequentially to:
   - Load the text
   - Process with spaCy
   - View inline entity visualization
   - Review entity glossary and counts

---

## 📊 Example Entity Output

Sample detected entities:

| Entity Text      | Label   |
| ---------------- | ------- |
| "John Doe"        | PERSON  |
| "World Health Organization" | ORG     |
| "New York"       | GPE     |


---

## 📝 Notes

- You can replace `public_health.txt` with any plain-text file to analyze different content.
- The notebook can be extended with custom entity filtering, CSV export, or interactive dashboards.
