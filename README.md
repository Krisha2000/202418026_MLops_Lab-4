# MLOps Lab 4 — CI/CD with DVC

This project demonstrates a simple **Machine Learning pipeline** (Linear Regression) integrated with **DVC** for data versioning and **GitHub Actions** for CI/CD automation.  


---
<img width="1374" height="891" alt="Screenshot From 2025-09-17 23-24-57" src="https://github.com/user-attachments/assets/422a0622-0b75-4121-94b4-2671d3d8a9be" />


##  How to Run Locally
```bash
# Clone the repository
git clone https://github.com/krisha2000/202418026_MLops_Lab-4.git
cd 202418026_MLops_Lab-4

# Install dependencies
pip install -r requirements.txt

# Initialize DVC (only first time)
dvc init

# Reproduce pipeline
dvc repro

# Show tracked metrics
dvc metrics show

202418035_MLops_Lab-4/
├─ data/
│   └─ raw/                  # Raw dataset (input data)
│
├─ src/
│   ├─ train.py              # Training script
│   └─ evaluate.py           # Evaluation script
│
├─ .dvc/                     # DVC internal files
├─ .dvcignore                # Ignore patterns for DVC
├─ .github/workflows/ci.yml  # GitHub Actions CI/CD pipeline
├─ dvc.yaml                  # DVC pipeline definition
├─ params.yaml               # Model hyperparameters
├─ requirements.txt          # Python dependencies
└─ README.md                 # Project documentation

