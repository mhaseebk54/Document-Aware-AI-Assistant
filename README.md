# 📄 Document-Aware AI Assistant (Using Free Open-Source LLM)

## 📌 Project Overview

This project implements a **Document-Aware AI Assistant** that reads a single text document and answers user questions **strictly based on the document content** using a **free and open-source Large Language Model (LLM)**.

The assistant does **not use any paid APIs** and runs entirely on **CPU**, making it suitable for local execution and academic use.

---

## 🎯 Problem Statement

Build a Gen-AI based assistant that:
- Reads a text document
- Accepts a user question
- Generates an answer using only the document content
- Avoids hallucination or external knowledge
- Uses a free open-source LLM via HuggingFace

---

## 🧠 Model Used

- **Model Name:** `google/flan-t5-base`
- **Framework:** HuggingFace Transformers
- **Pipeline Used:** `text2text-generation`
- **Execution:** CPU only

This model is lightweight, fast, and ideal for academic and exam use.

---

## 📂 Dataset / Input

- A **single text document (`.txt`)**
- Example content:
  - Course notes
  - Company policy document
  - Product description
  - Short research article

The assistant answers questions **only from this document**.

---

## ⚙️ Features

- Reads and cleans a `.txt` document
- Uses prompt engineering to restrict answers to document content
- Returns a fallback message if the answer is not found
- Fully offline and free to use
- Simple and easy-to-understand implementation

---

## 🛠️ Installation

Install required libraries:

```bash

pip install transformers torch

▶️ How to Run

Place your document in the project folder as document.txt

Run the Python script:

python app.py


Enter your question when prompted

🧪 Example

Document Content:

Artificial Intelligence is used in healthcare, education, and automation.


Question:

Where is AI used?


Answer:

AI is used in healthcare, education, and automation.

❌ Hallucination Control

If the answer is not present in the document, the assistant responds with:

Answer not found in the document.


This ensures reliable and document-grounded responses.

📁 Project Structure
├── document.txt
├── app.py
├── README.md

📌 Use Cases

Academic assignments

Exam demonstrations

Document-based Q&A systems

Beginner Gen-AI projectspip install transformers torch

