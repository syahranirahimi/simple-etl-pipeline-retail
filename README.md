# Simple ETL Pipeline for Fashion Retail Data

An automated Data Engineering project designed to implement a clean, modular ETL (Extract, Transform, Load) pipeline using Python. Developed as an academic milestone for the Dicoding Coding Camp 2026, this project focuses on processing fashion retail datasets to transform raw transaction records into structured, analytics-ready data.

## 📌 Project Overview
In a retail business environment, raw transaction logs often contain inconsistencies, missing values, or unstructured formats that prevent efficient business intelligence analysis. This pipeline automates the lifecycle of that data:
1. **Extract**: Retrieves raw products and transaction records from unstructured/flat file formats (`.csv`).
2. **Transform**: Cleanses data constraints, handles missing fields, and standardizes data models using modular Python transformation logic.
3. **Load**: Saves the structured, high-quality output into a designated analytical storage format.

## 🛠️ Tech Stack & Key Concepts
* **Language**: Python 3.x
* **Core Packages**: `pandas` (or native Python utilities), `pytest` (for pipeline unit testing)
* **Architecture**: Modular Software Engineering (Separation of Concerns via independent scripts)
* **Testing**: Automated test scripts to validate the integrity of each ETL phase.

---

## 📂 Project Structure
The repository is organized following clean development standards to separate core logic from configuration and tests:

```text
├── tests/
│   ├── test_extract.py     # Unit tests for data extraction logic
│   ├── test_transform.py   # Unit tests for data cleaning transformations
│   └── test_load.py        # Unit tests for storage loading operations
├── utils/
│   ├── extract.py          # Extraction script handles raw files reading
│   ├── transform.py        # Business logic, data cleansing, and mapping
│   └── load.py             # Handles writing structured data into targets
├── main.py                 # Core entry point to trigger the whole automation pipeline
├── requirements.txt        # Project dependencies and environment libraries
├── products.csv            # Sample dataset utilized for processing
└── submission.txt          # Step-by-step user guide and project documentation
