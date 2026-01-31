# 🗳️ Comp2laintBox (AI-Powered Feedback System)

![Python](https://img.shields.io/badge/python-3.x-blue?style=flat&logo=python)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange?style=flat)
![Interface](https://img.shields.io/badge/Interface-Gradio-yellow?style=flat)
![Status](https://img.shields.io/badge/Status-Model%20Showcase-lightgrey?style=flat)

**Comp2laintBox** is an intelligent internal tool designed to modernize the traditional "Complaint Box" concept. It uses Natural Language Processing (NLP) to analyze, categorize, and report on employee feedback collected via Google Forms.

This repository serves as a **technical showcase** for the serialized machine learning model (`.pkl`). Due to strict corporate data privacy policies and the inclusion of proprietary datasets, the full source code and training data are not publicly available.

---

## 🤖 System Architecture

The system acts as a bridge between raw employee feedback and HR management, transforming unstructured text into actionable data.

### 🔄 Data Pipeline
1.  **Input Source:** Feedback (Complaints, Suggestions, Comments) is collected through **Google Forms**.
2.  **Data Processing:** **Pandas** is used to clean, structure, and preprocess the raw text data.
3.  **AI Analysis:** The core model (built with **Scikit-learn**) processes the text to:
    * **Analyze Sentiment:** Detects whether the feedback is positive, negative, or neutral.
    * **Categorize Topics:** Automatically tags issues (e.g., "IT Support," "Cafeteria," "Management," "Working Hours").
4.  **User Interface:** A conversational **Gradio** interface allows managers to query the database naturally.

---

## 🔐 Security Features

* **Corporate Authentication:** Access to the chatbot is restricted. The system validates users against a whitelist of company email domains, ensuring that sensitive internal data remains secure.
* **Privacy Compliance:** The public version of this repository does not contain any Personally Identifiable Information (PII) or real employee data.

---

## 🧠 Tech Stack

* **Python 3:** Primary development language.
* **Scikit-learn:** Utilized for training the classification and sentiment analysis algorithms.
* **Pandas:** For dataframe manipulation and data cleaning.
* **Joblib:** For efficient model serialization (saving/loading the state).
* **Gradio:** For building the interactive, web-based chatbot UI.

---

## 💬 Use Cases (Turkish Language Support)

The model is specifically trained on **Turkish** corporate datasets and handles queries such as:

* *"Yemekhane ile ilgili kaç şikayet var?"* (How many complaints are there regarding the cafeteria?)
* *"En çok hangi departman hakkında öneri geldi?"* (Which department received the most suggestions?)
* *"Geçen ayki olumsuz yorumların özetini ver."* (Summarize the negative comments from last month.)

---

## ⚠️ Portfolio Note

This repository contains the `model.pkl` file to demonstrate the project's existence and architecture. It is **not intended for public deployment** as it requires a specific server environment and private vectorizer vocabularies to function correctly.

---

## 👨‍💻 Author

**Ozan Arda Özçelik**

- **GitHub:** [@ozanardaozcelik](https://github.com/ozanardaozcelik)
- **LinkedIn:** [Ozan Arda Özçelik](https://www.linkedin.com/in/ozanardaozcelik/)
