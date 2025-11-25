## 📌 Overview

Difference_Check is a Python-based tool deployed on Streamlit designed to compare datasets, detect duplicates, and generate categorized difference reports.

It is especially useful for data analysts, QA teams, auditors, and engineers who frequently compare dataset versions.

---

## 🚀 Features
- Detect duplicate rows

- Compare two datasets (CSV/XLSX)

- Find Added, Removed, and Modified rows

- Column-level difference detection

- Summary document generation (PDF/Docx)

- Clean CSV/Excel output

- Easily scriptable and lightweight
---

## 🛠 Tech Stack

- Python 3.x

- ```diff_check.py``` (main script)

- Dependencies in ```requirements.txt```

- Uses ```pandas``` for data handling

## 📥 Installation
```
git clone https://github.com/chandan-00/Difference_check.git
cd Difference_check

python3 -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows

pip install -r requirements.txt
```
---
## ▶️ Usage
Basic comparison
```
python diff_check.py \
  --input1 old_data.csv \
  --input2 new_data.csv \
  --key-columns id,name \
  --output-path output_folder
  ```

With duplicate detection
```
python diff_check.py \
  --input1 dataset_v1.xlsx \
  --input2 dataset_v2.xlsx \
  --key-columns rec_id \
  --output-path ./reports \
  --duplicates true \
  --format docx
  ```
---
## 📄 Input & Output Formats
### Input:

- CSV or Excel files

- Two datasets (old vs new)

- Key columns to match records

### Output:

- Difference report (CSV/Excel)

- Categorized changes

- Duplicate summary (optional)

- Summary document (PDF/Docx)

---

## ⚙️ Script Parameters
| Parameter | Description |	Example |
|---|---|---|
|--input1 |	Baseline dataset |	old.csv
|--input2 |	New dataset |	new.csv |
|--key-columns |	Columns used to match rows |	id,email |
|--output-path	 | Directory to store generated reports	| ./diff_output |
|--duplicates | Enable duplicate detection | true
| --format | Summary format (pdf, docx)	| pdf

---

## 📁 Folder Structure
```
Difference_check/
├── .devcontainer/
├── .gitattributes
├── diff_check.py
├── requirements.txt
└── README.md
```

## 🔍 How It Works

- Loads two datasets

- Optional: performs duplicate detection

- Compares datasets using key columns

- Identifies added, removed, and modified rows

- Generates difference reports

- Builds a summary document

## 🤝 Contribution

- Fork the repo

- Create a feature branch

- Commit your changes

- Submit a pull request

## 📃 License

License not specified (you may add MIT/Apache 2.0/etc.)

## 📬 Support

Open an issue in the GitHub repository for bugs or feature requests.