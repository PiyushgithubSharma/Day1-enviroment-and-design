# Day 1: Environment Setup and ML Problem Design

## Project Overview

This repository contains the deliverables for **Day 1** of the Machine Learning project setup.

The project focuses on:

- Setting up a Machine Learning development environment.
- Creating a standard ML project structure.
- Configuring Git and GitHub.
- Creating a complete Machine Learning Problem Framework.
- Designing a Credit Card Fraud Detection System.

---

## Repository Structure

```
day1-environment-and-design/
|
├──data/
│   ├── raw/
│   └── processed/
│
├── models/
│
├── notebooks/
│
├── reports/
│   └── figures/
│
├── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   └── utils/
│
├── tests/
│
├── README.md
├── requirements.txt
├── .gitignore
└── fraud_detection_design.md
```

---

## Project Objective

Design a Machine Learning solution for detecting fraudulent credit card transactions.

### Problem Statement

- Process approximately **10 million transactions per day**
- Fraud rate: **0.1%**
- Real-time prediction required (**<100 ms**)
- Missing fraud costs **$100**
- False positive costs **$5**

The goal is to build an ML problem framework and design a production-ready fraud detection system.

---

## ML Problem Framework

The project follows the standard four-step ML problem framing process.

### Step 1: Understand the Business Problem

- Identify business objectives
- Understand the cost of prediction errors
- Define prediction timing
- Analyze available data

### Step 2: Frame as an ML Problem

- Binary Classification
- Target Variable
- Feature Selection
- Success Metrics

### Step 3: Design the Solution

- Data Pipeline
- Feature Engineering
- Model Selection
- Evaluation Strategy

### Step 4: Identify Pitfalls

- Data Leakage
- Class Imbalance
- Deployment Challenges
- Monitoring Strategy

---

## Technologies Used

- Python 3.x
- Git
- GitHub
- Visual Studio Code

---

## Environment Setup

### Clone the Repository

```bash
git clone https://github.com/PiyushgithubSharma/day1-environment-and-design.git
```

### Navigate to the Project

```bash
cd day1-environment-and-design
```

### Create a Virtual Environment

```bash
python -m venv venv
```

### Activate the Virtual Environment

**Windows**

```bash
venv\Scripts\activate
```

**Linux / macOS**

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Git Workflow

Check repository status:

```bash
git status
```

Stage files:

```bash
git add .
```

Commit changes:

```bash
git commit -m "Your commit message"
```

Push changes:

```bash
git push origin main
```

---

## Evaluation Metrics

Since fraud detection is a highly imbalanced classification problem, the primary evaluation metrics are:

- Recall
- Precision
- F1 Score
- Precision-Recall AUC (PR-AUC)

Accuracy is **not** used as the primary metric because the dataset contains only **0.1% fraudulent transactions**.

---

## Author

**Piyush Sharma**

GitHub: https://github.com/PiyushgithubSharma

---

## License

This project is created for educational and learning purposes.