# ML Translation Pipeline

A modular Machine Learning pipeline for automatic text translation and evaluation, generated from a custom Cookiecutter template.

---

## 📌 Overview

This project implements a complete NLP pipeline that:

* loads textual data
* processes and prepares inputs
* translates text using a pre-trained model
* evaluates translation quality using standard metrics

The project is built with a modular architecture to ensure flexibility and scalability.

---

## 🧱 Project Structure

```text id="o1k3mj"
project/
├── src/
│   ├── loaders/        # Data loading
│   ├── processors/     # Preprocessing
│   ├── translators/    # Translation models
│   ├── evaluators/     # Evaluation metrics
│   └── orchestrator/   # Pipeline coordination
│
├── data/               # Input data
├── output/             # Generated results
├── tests/              # Unit tests
├── README.md
├── pyproject.toml
└── .gitignore
```

---

## ⚙️ Setup

```bash id="3h6d7n"
python -m venv .venv
.venv\Scripts\activate
pip install -U pip
pip install -r requirements.txt
```

---

## ▶️ Usage

Run tests:

```bash id="7b1jzo"
python -m pytest
```

Check formatting:

```bash id="c1mx0k"
black --check .
```

Run the pipeline (example):

```bash id="2xpw8u"
python src/orchestrator/pipeline.py
```

---

## 🧠 Pipeline Architecture

The pipeline is organized into independent components:

* **loaders** → load raw data
* **processors** → clean and transform data
* **translators** → apply NLP translation models
* **evaluators** → compute evaluation metrics (e.g., BLEU)
* **orchestrator** → manage the execution flow

This design allows each component to be extended or replaced independently.

---

## 🔁 Origin of the Project

This project was generated using a custom Cookiecutter template:

👉https://github.com/s123456-ops/COOKIECUTTER_ML_PROJECT.git

---

## 🎯 Academic Context

Developed as part of a Big Data and Machine Learning Infrastructure course.
The objective was to design a reusable project template and demonstrate its application through a complete ML pipeline.

---

## 👤 Author

Salma ALAOUI MRANI
Master Big Data, Analysis, Business Intelligence
Université Sorbonne Paris Nord
